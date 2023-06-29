# Comparing `tmp/jupyterhub-nomad-spawner-0.2.0.tar.gz` & `tmp/jupyterhub_nomad_spawner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-nomad-spawner-0.2.0.tar", max compression
+gzip compressed data, was "jupyterhub_nomad_spawner-0.2.1.tar", max compression
```

## Comparing `jupyterhub-nomad-spawner-0.2.0.tar` & `jupyterhub_nomad_spawner-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     3788 2023-06-29 20:19:18.872660 jupyterhub-nomad-spawner-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-06-29 20:20:11.780694 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/__init__.py
--rw-r--r--   0        0        0     1001 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/consul/consul_service.py
--rw-r--r--   0        0        0     1715 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_factory.py
--rw-r--r--   0        0        0      630 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_options_factory.py
--rw-r--r--   0        0        0        0 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/__init__.py
--rw-r--r--   0        0        0    61041 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_model.py
--rw-r--r--   0        0        0     4780 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_service.py
--rw-r--r--   0        0        0    20851 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/spawner.py
--rw-r--r--   0        0        0     2874 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/form.html.j2
--rw-r--r--   0        0        0     2045 2023-06-29 20:19:18.876660 jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/job.hcl.j2
--rw-r--r--   0        0        0     1435 2023-06-29 20:20:11.776694 jupyterhub-nomad-spawner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5112 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.2.0/setup.py
--rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 jupyterhub-nomad-spawner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3913 2023-06-29 20:24:32.085380 jupyterhub_nomad_spawner-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 20:24:56.881508 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/__init__.py
+-rw-r--r--   0        0        0     1001 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/consul/consul_service.py
+-rw-r--r--   0        0        0     1715 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/job_factory.py
+-rw-r--r--   0        0        0      630 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/job_options_factory.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/nomad/__init__.py
+-rw-r--r--   0        0        0    61041 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/nomad/nomad_model.py
+-rw-r--r--   0        0        0     4780 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/nomad/nomad_service.py
+-rw-r--r--   0        0        0    20851 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/spawner.py
+-rw-r--r--   0        0        0     2874 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/templates/form.html.j2
+-rw-r--r--   0        0        0     2045 2023-06-29 20:24:32.089380 jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/templates/job.hcl.j2
+-rw-r--r--   0        0        0     1435 2023-06-29 20:24:56.877508 jupyterhub_nomad_spawner-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 jupyterhub_nomad_spawner-0.2.1/PKG-INFO
```

### Comparing `jupyterhub-nomad-spawner-0.2.0/README.md` & `jupyterhub_nomad_spawner-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -173,7 +173,20 @@
 
         }
     }
 }
 
 
 ```
+
+
+## Development
+
+### Setup
+
+Get poetry: https://python-poetry.org/docs/#installation
+
+```sh
+poetry install
+```
+
+### Release
```

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/consul/consul_service.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/consul/consul_service.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_factory.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/job_factory.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/job_options_factory.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/job_options_factory.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_model.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/nomad/nomad_model.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/nomad/nomad_service.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/nomad/nomad_service.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/spawner.py` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/spawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/form.html.j2` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/templates/form.html.j2`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/jupyterhub_nomad_spawner/templates/job.hcl.j2` & `jupyterhub_nomad_spawner-0.2.1/jupyterhub_nomad_spawner/templates/job.hcl.j2`

 * *Files identical despite different names*

### Comparing `jupyterhub-nomad-spawner-0.2.0/pyproject.toml` & `jupyterhub_nomad_spawner-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jupyterhub-nomad-spawner"
-version = "0.2.0"
+version = "0.2.1"
 description = "A JupyterHub Spawner that launches isolated notebooks as job"
 authors = ["Max Fröhlich <maxbruchmann@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "jupyterhub_nomad_spawner" },
 ]
```

### Comparing `jupyterhub-nomad-spawner-0.2.0/PKG-INFO` & `jupyterhub_nomad_spawner-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-nomad-spawner
-Version: 0.2.0
+Version: 0.2.1
 Summary: A JupyterHub Spawner that launches isolated notebooks as job
 Author: Max Fröhlich
 Author-email: maxbruchmann@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
@@ -192,7 +192,20 @@
         }
     }
 }
 
 
 ```
 
+
+## Development
+
+### Setup
+
+Get poetry: https://python-poetry.org/docs/#installation
+
+```sh
+poetry install
+```
+
+### Release
+
```

