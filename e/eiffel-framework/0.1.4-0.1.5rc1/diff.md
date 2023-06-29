# Comparing `tmp/eiffel_framework-0.1.4.tar.gz` & `tmp/eiffel_framework-0.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eiffel_framework-0.1.4.tar", max compression
+gzip compressed data, was "eiffel_framework-0.1.5rc1.tar", max compression
```

## Comparing `eiffel_framework-0.1.4.tar` & `eiffel_framework-0.1.5rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-23 15:27:52.569113 eiffel_framework-0.1.4/LICENSE
--rw-r--r--   0        0        0       77 2023-06-23 15:27:52.569233 eiffel_framework-0.1.4/README.md
--rw-r--r--   0        0        0      962 2023-06-23 15:30:11.612153 eiffel_framework-0.1.4/eiffel/__init__.py
--rw-r--r--   0        0        0      146 2023-06-23 15:30:11.612748 eiffel_framework-0.1.4/eiffel/__main__.py
--rw-r--r--   0        0        0      173 2023-06-27 22:05:43.538287 eiffel_framework-0.1.4/eiffel/module.py
--rw-r--r--   0        0        0     1332 2023-06-28 08:22:58.969581 eiffel_framework-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 eiffel_framework-0.1.4/setup.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 eiffel_framework-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-23 15:27:52.569113 eiffel_framework-0.1.5rc1/LICENSE
+-rw-r--r--   0        0        0       77 2023-06-23 15:27:52.569233 eiffel_framework-0.1.5rc1/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 15:33:31.839766 eiffel_framework-0.1.5rc1/eiffel/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-29 12:34:07.052904 eiffel_framework-0.1.5rc1/eiffel/__main__.py
+-rw-r--r--   0        0        0       41 2023-06-28 15:25:01.740170 eiffel_framework-0.1.5rc1/eiffel/eiffel.yaml
+-rw-r--r--   0        0        0      173 2023-06-27 22:05:43.538287 eiffel_framework-0.1.5rc1/eiffel/module.py
+-rw-r--r--   0        0        0     1488 2023-06-29 12:41:34.021348 eiffel_framework-0.1.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 eiffel_framework-0.1.5rc1/setup.py
+-rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 eiffel_framework-0.1.5rc1/PKG-INFO
```

### Comparing `eiffel_framework-0.1.4/LICENSE` & `eiffel_framework-0.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `eiffel_framework-0.1.4/pyproject.toml` & `eiffel_framework-0.1.5rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 [tool.poetry]
 name = "eiffel-framework"
-version = "0.1.4"
+version = "0.1.5-rc1"
 description = "Evaluation Framework for FL-based intrusion detection using Flower."
 authors = ["phdcybersec <82591009+phdcybersec@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "eiffel", from = "." }]
 
 [tool.poetry.dependencies]
-python = "~3.10"
-hydra-core = "^1.3.2"
-flwr = "^1.4.0"
-
+# GPU-related dependencies (installed with extras)
+# ------------------------------------------------
 # darwin
 tensorflow-metal = { platform = "darwin", version = "~0.6.0", optional = true }
 tensorflow-macos = { platform = "darwin", version = "~2.10.0", optional = true }
 grpcio = { platform = "darwin", version = ">=1.37.0,<2.0", optional = true }
 h5py = { platform = "darwin", version = ">=3.6.0,<3.7", optional = true }
 numpy = { platform = "darwin", version = ">=1.23.2,<1.23.3", optional = true }
 protobuf = { platform = "darwin", version = ">=3.19.1,<3.20", optional = true }
 
 # linux
 #tensorflow = { platform = "linux", version = "~2.10.0", optional = true }
 
+# Common dependencies
+# -------------------
+python = "~3.10"
+hydra-core = "^1.3.2"
+flwr = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 isort = "^5.12.0"
 autoflake = "^2.1.1"
 
 
 [tool.poetry.extras]
 darwin = ["tensorflow-metal", "tensorflow-macos", "grpcio", "h5py", "numpy", "protobuf"]
 linux = ["tensorflow"]
 
 
 [tool.poetry.scripts]
-# eiffel = "eiffel:main"
+eiffel = "eiffel.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eiffel_framework-0.1.4/setup.py` & `eiffel_framework-0.1.5rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 {'darwin:sys_platform == "darwin"': ['tensorflow-metal>=0.6.0,<0.7.0',
                                      'tensorflow-macos>=2.10.0,<2.11.0',
                                      'grpcio>=1.37.0,<2.0',
                                      'h5py>=3.6.0,<3.7',
                                      'numpy>=1.23.2,<1.23.3',
                                      'protobuf>=3.19.1,<3.20']}
 
+entry_points = \
+{'console_scripts': ['eiffel = eiffel.__main__:main']}
+
 setup_kwargs = {
     'name': 'eiffel-framework',
-    'version': '0.1.4',
+    'version': '0.1.5rc1',
     'description': 'Evaluation Framework for FL-based intrusion detection using Flower.',
     'long_description': '# eiffel\nEvaluation framework for FL-based intrusion detection using Flower.\n',
     'author': 'phdcybersec',
     'author_email': '82591009+phdcybersec@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `eiffel_framework-0.1.4/PKG-INFO` & `eiffel_framework-0.1.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eiffel-framework
-Version: 0.1.4
+Version: 0.1.5rc1
 Summary: Evaluation Framework for FL-based intrusion detection using Flower.
 License: MIT
 Author: phdcybersec
 Author-email: 82591009+phdcybersec@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

