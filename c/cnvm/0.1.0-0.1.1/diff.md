# Comparing `tmp/cnvm-0.1.0.tar.gz` & `tmp/cnvm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnvm-0.1.0.tar", max compression
+gzip compressed data, was "cnvm-0.1.1.tar", max compression
```

## Comparing `cnvm-0.1.0.tar` & `cnvm-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-29 13:56:40.596892 cnvm-0.1.0/cnvm/__init__.py
--rw-r--r--   0        0        0     9576 2023-05-02 17:22:53.779313 cnvm-0.1.0/cnvm/collective_variables.py
--rw-r--r--   0        0        0    10290 2023-04-29 13:42:43.246793 cnvm-0.1.0/cnvm/model.py
--rw-r--r--   0        0        0     8552 2023-05-02 17:20:07.874030 cnvm-0.1.0/cnvm/network_generator.py
--rw-r--r--   0        0        0    10105 2023-04-29 13:42:43.213817 cnvm-0.1.0/cnvm/parameters.py
--rw-r--r--   0        0        0     6774 2023-05-02 17:20:07.903711 cnvm-0.1.0/cnvm/utils.py
--rw-r--r--   0        0        0    35823 2022-12-23 10:27:00.113337 cnvm-0.1.0/LICENSE
--rw-r--r--   0        0        0     1138 2023-04-30 06:37:31.053926 cnvm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5643 2023-05-02 17:28:23.540660 cnvm-0.1.0/README.md
--rw-r--r--   0        0        0     6543 1970-01-01 00:00:00.000000 cnvm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/__init__.py
+-rw-r--r--   0        0        0     9576 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/collective_variables.py
+-rw-r--r--   0        0        0    10290 2023-06-01 12:02:15.724243 cnvm-0.1.1/cnvm/model.py
+-rw-r--r--   0        0        0    10221 2023-06-29 14:27:54.206058 cnvm-0.1.1/cnvm/network_generator.py
+-rw-r--r--   0        0        0    10105 2023-06-01 12:02:15.725239 cnvm-0.1.1/cnvm/parameters.py
+-rw-r--r--   0        0        0     6774 2023-06-01 12:02:15.725239 cnvm-0.1.1/cnvm/utils.py
+-rw-r--r--   0        0        0    35823 2022-11-05 17:20:32.769485 cnvm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-29 15:23:06.929140 cnvm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5643 2023-06-01 12:02:15.723246 cnvm-0.1.1/README.md
+-rw-r--r--   0        0        0     6543 1970-01-01 00:00:00.000000 cnvm-0.1.1/PKG-INFO
```

### Comparing `cnvm-0.1.0/cnvm/collective_variables.py` & `cnvm-0.1.1/cnvm/collective_variables.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/cnvm/model.py` & `cnvm-0.1.1/cnvm/model.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/cnvm/network_generator.py` & `cnvm-0.1.1/cnvm/network_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Protocol
 import networkx as nx
 import numpy as np
+import time
 
 
 class NetworkGenerator(Protocol):
     num_agents: int
 
     def __call__(self) -> nx.Graph:
         """Generate a network."""
@@ -13,35 +14,45 @@
         """Return string representation of the generator."""
 
     def abrv(self) -> str:
         """Return short description for file names."""
 
 
 class ErdosRenyiGenerator:
-    def __init__(self, num_agents: int, p: float):
+    def __init__(self, num_agents: int, p: float, max_sample_time: float = 10):
         """
         Generate Erdös-Renyi (binomial) random graphs.
 
+        The random graph may contain isolated vertices, which is not allowed.
+        In that case, the Generator samples until a valid network is found,
+        or until max_sample_time seconds pass, in which case a RuntimeError is raised.
+
         Parameters
         ----------
         num_agents : int
         p : float
+        max_sample_time : float, optional
+            In seconds.
         """
         self.num_agents = num_agents
         self.p = p
+        self.max_sample_time = max_sample_time
 
     def __call__(self) -> nx.Graph:
         gnp_fun = nx.erdos_renyi_graph if self.p > 0.2 else nx.fast_gnp_random_graph
-        i = 0
-        while i < 10:
+        start = time.time()
+        while True:
             network = gnp_fun(self.num_agents, self.p)
-            if nx.is_connected(network):
+            if nx.number_of_isolates(network) == 0:
                 return network
-            i += 1
-        raise RuntimeError("Could not generate a connected graph.")
+
+            if time.time() - start > self.max_sample_time:
+                raise RuntimeError(
+                    "Timeout. Could not generate a graph without isolated vertices."
+                )
 
     def __repr__(self) -> str:
         return f"Erdos-Renyi random graph with p={self.p} on {self.num_agents} nodes"
 
     def abrv(self) -> str:
         return f"ER_p{int(self.p * 100)}_N{self.num_agents}"
 
@@ -118,25 +129,34 @@
         return f"Watts-Strogatz random graph on {self.num_agents} nodes"
 
     def abrv(self):
         return f"watts_k{self.num_neighbors}_p{int(self.p * 100)}_N{self.num_agents}"
 
 
 class StochasticBlockGenerator:
-    def __init__(self, num_agents: int, p_matrix: np.ndarray):
+    def __init__(
+        self, num_agents: int, p_matrix: np.ndarray, max_sample_time: float = 10
+    ):
         """
         Creates n stochastic blocks, block i is randomly connected to block j with edge density p_matrix[i, j].
 
+        The random graph may contain isolated vertices, which is not allowed.
+        In that case, the Generator samples until a valid network is found,
+        or until max_sample_time seconds pass, in which case a RuntimeError is raised.
+
         Parameters
         ----------
         num_agents : int
         p_matrix : np.ndarray
             (n x n) matrix of edge probabilities.
+        max_sample_time : float, optional
+            In seconds.
         """
         self.p_matrix = p_matrix
+        self.max_sample_time = max_sample_time
 
         self.num_blocks = p_matrix.shape[0]
         self.block_size = int(num_agents / self.num_blocks)
         self.num_agents = self.block_size * self.num_blocks
 
     def _sample_adj_matrix(self):
         adj_matrix = np.zeros((self.num_agents, self.num_agents))
@@ -153,22 +173,25 @@
 
         # only keep the lower triangle and symmetrize
         adj_matrix = np.tril(adj_matrix, -1)
         adj_matrix = adj_matrix + np.tril(adj_matrix).T
         return adj_matrix
 
     def __call__(self) -> nx.Graph:
-        i = 0
-        while i < 10:
+        start = time.time()
+        while True:
             adj_mat = self._sample_adj_matrix()
             network = nx.from_numpy_array(adj_mat)
-            if nx.is_connected(network):
+            if nx.number_of_isolates(network) == 0:
                 return network
-            i += 1
-        raise RuntimeError("Could not generate a connected graph.")
+
+            if time.time() - start > self.max_sample_time:
+                raise RuntimeError(
+                    "Timeout. Could not generate a graph without isolated vertices."
+                )
 
     def __repr__(self) -> str:
         return f"stochastic block model with {self.num_blocks} blocks and {self.num_agents} nodes."
 
     def abrv(self):
         return f"sbm_b{self.num_blocks}_N{self.num_agents}"
 
@@ -210,32 +233,45 @@
         if self.periodic:
             return f"lattice_{self.dim}D_periodic_N{self.num_agents}"
         else:
             return f"lattice_{self.dim}D_N{self.num_agents}"
 
 
 class BinomialWattsStrogatzGenerator:
-    def __init__(self, num_agents: int, num_neighbors: int, p_rewire: float):
+    def __init__(
+        self,
+        num_agents: int,
+        num_neighbors: int,
+        p_rewire: float,
+        max_sample_time: float = 10,
+    ):
         """
         Creates a ring where each node is connected to the num_neighbors nearest neighbors.
         (num_neighbors needs to be even!)
         Then iterate through each edge and rip it out with probability p_rewire.
         Then iterate through all the possible edges that are not present and insert with such a probability,
         that in expectation the resulting graph has the same number of edges again.
         For p=1, this yields the binomial Erdös-Renyi graph G(N, K/N).
 
+        The random graph may contain isolated vertices, which is not allowed.
+        In that case, the Generator samples until a valid network is found,
+        or until max_sample_time seconds pass, in which case a RuntimeError is raised.
+
         Parameters
         ----------
         num_agents : int
         num_neighbors : int
         p_rewire : float
+        max_sample_time : float, optional
+            In seconds.
         """
         self.num_agents = num_agents
         self.num_neighbors = num_neighbors
         self.p_rewire = p_rewire
+        self.max_sample_time = max_sample_time
 
         self.p_insert = (
             p_rewire * num_neighbors / (num_agents - 1 - (1 - p_rewire) * num_neighbors)
         )
         self.gnp_fun = (
             nx.erdos_renyi_graph if self.p_insert > 0.2 else nx.fast_gnp_random_graph
         )
@@ -250,20 +286,23 @@
 
         # insert edges
         network = self.gnp_fun(self.num_agents, self.p_insert)
         network.add_edges_from(edges)
         return network
 
     def __call__(self) -> nx.Graph:
-        i = 0
-        while i < 10:
+        start = time.time()
+        while True:
             network = self._sample_network()
-            if nx.is_connected(network):
+            if nx.number_of_isolates(network) == 0:
                 return network
-            i += 1
-        raise RuntimeError("Could not generate a connected graph.")
+
+            if time.time() - start > self.max_sample_time:
+                raise RuntimeError(
+                    "Timeout. Could not generate a graph without isolated vertices."
+                )
 
     def __repr__(self) -> str:
         return f"Binomial Watts-Strogatz graph on {self.num_agents} nodes with p_rewire={self.p_rewire}"
 
     def abrv(self):
         return f"binWS_k{self.num_neighbors}_p{int(self.p_rewire * 100)}_N{self.num_agents}"
```

### Comparing `cnvm-0.1.0/cnvm/parameters.py` & `cnvm-0.1.1/cnvm/parameters.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/cnvm/utils.py` & `cnvm-0.1.1/cnvm/utils.py`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/LICENSE` & `cnvm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/pyproject.toml` & `cnvm-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cnvm"
-version = "0.1.0"
+version = "0.1.1"
 description = "Continuous-time Noisy Voter Model (CNVM) of social dynamics."
 license = "GPL-3.0-or-later"
 authors = ["Marvin Lücke"]
 readme = "README.md"
 repository = "https://github.com/lueckem/cnvm"
 keywords = [
     "voter model",
@@ -40,12 +40,13 @@
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 ipykernel = "^6.22.0"
 matplotlib = "^3.7.1"
+jupyter = "^1.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cnvm-0.1.0/README.md` & `cnvm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cnvm-0.1.0/PKG-INFO` & `cnvm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnvm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Continuous-time Noisy Voter Model (CNVM) of social dynamics.
 Home-page: https://github.com/lueckem/cnvm
 License: GPL-3.0-or-later
 Keywords: voter model,social dynamics,opinion dynamics,statistical physics,agent-based model,epidemiology,interacting particle system
 Author: Marvin Lücke
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Science/Research
```

