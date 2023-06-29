# Comparing `tmp/openoligo-0.1.2.tar.gz` & `tmp/openoligo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.2.tar", max compression
+gzip compressed data, was "openoligo-0.1.3.tar", max compression
```

## Comparing `openoligo-0.1.2.tar` & `openoligo-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-06-23 09:08:17.765678 openoligo-0.1.2/LICENSE
--rw-r--r--   0        0        0      979 2023-06-23 09:08:17.765678 openoligo-0.1.2/README.md
--rw-r--r--   0        0        0      490 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/__init__.py
--rw-r--r--   0        0        0     1329 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/cartridge.py
--rw-r--r--   0        0        0     1826 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/container/types.py
--rw-r--r--   0        0        0      761 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/__init__.py
--rw-r--r--   0        0        0     2941 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/gpio.py
--rw-r--r--   0        0        0     2268 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/manifold.py
--rw-r--r--   0        0        0      733 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/rpi_pins.py
--rw-r--r--   0        0        0     4239 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/switch.py
--rw-r--r--   0        0        0     1873 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/driver/types.py
--rw-r--r--   0        0        0      300 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/log_config.py
--rw-r--r--   0        0        0      250 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/__init__.py
--rw-r--r--   0        0        0      909 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/flow_sequence.py
--rw-r--r--   0        0        0       94 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/steps/types.py
--rw-r--r--   0        0        0      164 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/utils/__init__.py
--rw-r--r--   0        0        0      666 2023-06-23 09:08:17.765678 openoligo-0.1.2/openoligo/utils/wait.py
--rw-r--r--   0        0        0     1037 2023-06-23 09:08:17.765678 openoligo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 openoligo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 07:51:40.182072 openoligo-0.1.3/LICENSE
+-rw-r--r--   0        0        0      790 2023-06-29 07:51:40.182072 openoligo-0.1.3/README.md
+-rw-r--r--   0        0        0      446 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/__init__.py
+-rw-r--r--   0        0        0     3971 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/board.py
+-rw-r--r--   0        0        0     3799 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/devices.py
+-rw-r--r--   0        0        0     3547 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/gpio.py
+-rw-r--r--   0        0        0     4365 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/types.py
+-rw-r--r--   0        0        0     4261 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/instrument.py
+-rw-r--r--   0        0        0      912 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/log_config.py
+-rw-r--r--   0        0        0       52 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/protocols/__init__.py
+-rw-r--r--   0        0        0     3137 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/protocols/dna_synthesis.py
+-rw-r--r--   0        0        0      157 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/__init__.py
+-rw-r--r--   0        0        0     2341 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/flow.py
+-rw-r--r--   0        0        0     1292 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/types.py
+-rw-r--r--   0        0        0      261 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/sim.py
+-rw-r--r--   0        0        0      402 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/singleton.py
+-rw-r--r--   0        0        0     1320 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/wait.py
+-rw-r--r--   0        0        0     1243 2023-06-29 07:51:40.190071 openoligo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 openoligo-0.1.3/PKG-INFO
```

### Comparing `openoligo-0.1.2/LICENSE` & `openoligo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.2/README.md` & `openoligo-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 # OpenOligo
 
 [![PyPI version](https://badge.fury.io/py/openoligo.svg)](https://badge.fury.io/py/openoligo)
-![Coverage](./.github/coverage.svg)
+![Coverage](https://raw.githubusercontent.com/TechnocultureResearch/OpenOligo/dev/.github/coverage.svg)
 [![Lint OpenOligo](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/lint.yaml/badge.svg)](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/lint.yaml)
 [![Test OpenOligo](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/test.yaml/badge.svg)](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/test.yaml)
 
 OpenOligo is an open-source platform for programmatically interacting with and managing DNA synthesis processes.
 
 ## Getting Started
 ```sh
 pip install openoligo
 ```
 
 ### A simple Example
 
 ```py
-from openoligo import Manifold, MockValve
-from openoligo.steps import perform_flow_sequence
-from openoligo.utils import ms
-
-m = Manifold(MockValve, 4)
-
-perform_flow_sequence(
-    m,
-    [
-        (0, ms(100)),
-        (2, 1),
-        (1, ms(200)),
-    ],
-)
 ```
```

### Comparing `openoligo-0.1.2/pyproject.toml` & `openoligo-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 [tool.poetry]
 name = "OpenOligo"
-version = "0.1.2"
+version = "0.1.3"
 description = "An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes."
 license = "Apache-2.0"
 authors = ["Satyam Tiwary <satyam@technoculture.io>"]
 readme = "README.md"
 keywords = ["DNA", "synthesis", "genetics", "open-source"]
 
 [tool.poetry.scripts]
-oligo-server= 'app.server:main'
+oligo-server = 'app.server:main'
+oligo-synth = 'examples.dna_synthesis:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.4.2"
+python-dotenv = "^1.0.0"
+biopython = "^1.81"
+tqdm = "^4.65.0"
+fastapi = "^0.98.0"
+pdoc3 = "^0.10.0"
+pdocs = "^1.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 flake8 = "^3.9.2"
 black = "^23.3.0"
 pylint = "^2.17.4"
 mypy = "^1.3.0"
 isort = "^5.12.0"
 coverage-badge = "^1.1.0"
 jupyter = "^1.0.0"
 jupyterlab = "^4.0.2"
+# ansible = "^8.1.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
-addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=80"
+addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=90"
 
 [tool.coverage.run]
 source = ["openoligo"]
 omit = ["**/types.py"]
 
 [tool.poetry.extras]
 rpi = ["RPi.GPIO"]
+bb = ["Adafruit_BBIO"]
```

### Comparing `openoligo-0.1.2/PKG-INFO` & `openoligo-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 Metadata-Version: 2.1
 Name: openoligo
-Version: 0.1.2
+Version: 0.1.3
 Summary: An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes.
 License: Apache-2.0
 Keywords: DNA,synthesis,genetics,open-source
 Author: Satyam Tiwary
 Author-email: satyam@technoculture.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: bb
 Provides-Extra: rpi
+Requires-Dist: biopython (>=1.81,<2.0)
+Requires-Dist: fastapi (>=0.98.0,<0.99.0)
+Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
+Requires-Dist: pdocs (>=1.2.0,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenOligo
 
 [![PyPI version](https://badge.fury.io/py/openoligo.svg)](https://badge.fury.io/py/openoligo)
-![Coverage](./.github/coverage.svg)
+![Coverage](https://raw.githubusercontent.com/TechnocultureResearch/OpenOligo/dev/.github/coverage.svg)
 [![Lint OpenOligo](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/lint.yaml/badge.svg)](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/lint.yaml)
 [![Test OpenOligo](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/test.yaml/badge.svg)](https://github.com/TechnocultureResearch/OpenOligo/actions/workflows/test.yaml)
 
 OpenOligo is an open-source platform for programmatically interacting with and managing DNA synthesis processes.
 
 ## Getting Started
 ```sh
 pip install openoligo
 ```
 
 ### A simple Example
 
 ```py
-from openoligo import Manifold, MockValve
-from openoligo.steps import perform_flow_sequence
-from openoligo.utils import ms
-
-m = Manifold(MockValve, 4)
-
-perform_flow_sequence(
-    m,
-    [
-        (0, ms(100)),
-        (2, 1),
-        (1, ms(200)),
-    ],
-)
 ```
```

