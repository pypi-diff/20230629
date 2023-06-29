# Comparing `tmp/qiskit_han-0.0.3.tar.gz` & `tmp/qiskit_han-0.0.4.tar.gz`

## Comparing `qiskit_han-0.0.3.tar` & `qiskit_han-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/Untitled.ipynb
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/qiskit_han/__init__.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/qiskit_han/backend.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/qiskit_han/job.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/qiskit_han/provider.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/qiskit_han/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/LICENSE
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 qiskit_han-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/Untitled.ipynb
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit.json
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/result.json
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit_han/__init__.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit_han/backend.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit_han/job.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit_han/provider.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/qiskit_han/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/LICENSE
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 qiskit_han-0.0.4/PKG-INFO
```

### Comparing `qiskit_han-0.0.3/Untitled.ipynb` & `qiskit_han-0.0.4/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `qiskit_han-0.0.3/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `qiskit_han-0.0.4/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `qiskit_han-0.0.3/qiskit_han/backend.py` & `qiskit_han-0.0.4/qiskit_han/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from qiskit.providers import BackendV2 as Backend
+from qiskit.providers import BackendV2
 from qiskit.transpiler import Target
 from qiskit.providers import Options
 from qiskit.circuit import Parameter, Measure
 from qiskit.circuit.library import PhaseGate, SXGate, UGate, CXGate, IGate
 from qiskit import assemble
 from qiskit_aer import AerSimulator
 from qiskit_han.job import MyJob
 import warnings
 import json
 
 
-class HanBackend(Backend):
+class HanBackend(BackendV2):
 
     def __init__(self):
         super().__init__()
         
         self.name = "Han"
         # Create Target
         self._target = Target("Target for My Backend")
```

### Comparing `qiskit_han-0.0.3/qiskit_han/provider.py` & `qiskit_han-0.0.4/qiskit_han/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_han-0.0.3/LICENSE` & `qiskit_han-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_han-0.0.3/pyproject.toml` & `qiskit_han-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "qiskit"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qiskit_han"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hangyul Son", email="hsn@example.com" },
 ]
 description = "qiskit provider han"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qiskit_han-0.0.3/PKG-INFO` & `qiskit_han-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_han
-Version: 0.0.3
+Version: 0.0.4
 Summary: qiskit provider han
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Hangyul Son <hsn@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

