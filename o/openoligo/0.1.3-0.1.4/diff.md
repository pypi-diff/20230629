# Comparing `tmp/openoligo-0.1.3.tar.gz` & `tmp/openoligo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.3.tar", max compression
+gzip compressed data, was "openoligo-0.1.4.tar", max compression
```

## Comparing `openoligo-0.1.3.tar` & `openoligo-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-06-29 07:51:40.182072 openoligo-0.1.3/LICENSE
--rw-r--r--   0        0        0      790 2023-06-29 07:51:40.182072 openoligo-0.1.3/README.md
--rw-r--r--   0        0        0      446 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/__init__.py
--rw-r--r--   0        0        0      560 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/__init__.py
--rw-r--r--   0        0        0     3971 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/board.py
--rw-r--r--   0        0        0     3799 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/devices.py
--rw-r--r--   0        0        0     3547 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/gpio.py
--rw-r--r--   0        0        0     4365 2023-06-29 07:51:40.186071 openoligo-0.1.3/openoligo/hal/types.py
--rw-r--r--   0        0        0     4261 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/instrument.py
--rw-r--r--   0        0        0      912 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/log_config.py
--rw-r--r--   0        0        0       52 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/protocols/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/protocols/dna_synthesis.py
--rw-r--r--   0        0        0      157 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/__init__.py
--rw-r--r--   0        0        0     2341 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/flow.py
--rw-r--r--   0        0        0     1292 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/steps/types.py
--rw-r--r--   0        0        0      261 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/__init__.py
--rw-r--r--   0        0        0      628 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/sim.py
--rw-r--r--   0        0        0      402 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/singleton.py
--rw-r--r--   0        0        0     1320 2023-06-29 07:51:40.190071 openoligo-0.1.3/openoligo/utils/wait.py
--rw-r--r--   0        0        0     1243 2023-06-29 07:51:40.190071 openoligo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 openoligo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 15:02:43.473844 openoligo-0.1.4/LICENSE
+-rw-r--r--   0        0        0      790 2023-06-25 07:46:12.264702 openoligo-0.1.4/README.md
+-rw-r--r--   0        0        0      446 2023-06-26 08:40:53.804108 openoligo-0.1.4/openoligo/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-29 09:09:57.109970 openoligo-0.1.4/openoligo/hal/__init__.py
+-rw-r--r--   0        0        0     3971 2023-06-27 18:50:16.320135 openoligo-0.1.4/openoligo/hal/board.py
+-rw-r--r--   0        0        0     3799 2023-06-29 09:09:57.132406 openoligo-0.1.4/openoligo/hal/devices.py
+-rw-r--r--   0        0        0     3584 2023-06-29 08:40:46.802559 openoligo-0.1.4/openoligo/hal/gpio.py
+-rw-r--r--   0        0        0     4365 2023-06-29 04:58:15.204050 openoligo-0.1.4/openoligo/hal/types.py
+-rw-r--r--   0        0        0     4261 2023-06-29 09:09:57.133908 openoligo-0.1.4/openoligo/instrument.py
+-rw-r--r--   0        0        0      912 2023-06-29 05:09:56.508723 openoligo-0.1.4/openoligo/log_config.py
+-rw-r--r--   0        0        0       52 2023-06-24 07:46:31.998299 openoligo-0.1.4/openoligo/protocols/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-29 09:09:31.145859 openoligo-0.1.4/openoligo/protocols/dna_synthesis.py
+-rw-r--r--   0        0        0      632 2023-06-29 09:10:53.278742 openoligo-0.1.4/openoligo/seq.py
+-rw-r--r--   0        0        0      157 2023-06-25 07:46:47.338022 openoligo-0.1.4/openoligo/steps/__init__.py
+-rw-r--r--   0        0        0     2341 2023-06-28 08:29:24.566340 openoligo-0.1.4/openoligo/steps/flow.py
+-rw-r--r--   0        0        0     1292 2023-06-28 14:40:11.940888 openoligo-0.1.4/openoligo/steps/types.py
+-rw-r--r--   0        0        0      261 2023-06-26 08:40:53.818037 openoligo-0.1.4/openoligo/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-29 09:09:31.128856 openoligo-0.1.4/openoligo/utils/sim.py
+-rw-r--r--   0        0        0      402 2023-06-27 11:25:14.508079 openoligo-0.1.4/openoligo/utils/singleton.py
+-rw-r--r--   0        0        0     1320 2023-06-28 14:40:37.043551 openoligo-0.1.4/openoligo/utils/wait.py
+-rw-r--r--   0        0        0     1263 2023-06-29 09:13:02.930980 openoligo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 openoligo-0.1.4/PKG-INFO
```

### Comparing `openoligo-0.1.3/LICENSE` & `openoligo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/README.md` & `openoligo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/hal/__init__.py` & `openoligo-0.1.4/openoligo/hal/__init__.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/hal/board.py` & `openoligo-0.1.4/openoligo/hal/board.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/hal/devices.py` & `openoligo-0.1.4/openoligo/hal/devices.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/hal/gpio.py` & `openoligo-0.1.4/openoligo/hal/gpio.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,23 +51,24 @@
 
 class RPiGPIO(GPIOInterface):
     """GPIO access on Raspberry Pi."""
 
     def __init__(self, gpio):
         """Import Board.GPIO"""
         self.gpio = gpio
+        self.gpio.setmode(self.gpio.BOARD)
+        self.gpio.setwarnings(False)
 
     def setup(self):
         """Set up all pins."""
         for pin in Board:
             self.setup_pin(pin)
 
     def setup_pin(self, pin: Board, mode: GpioMode = GpioMode.OUT) -> None:
         """Set up a GPIO pin."""
-        self.gpio.setmode(self.gpio.BOARD)
         self.gpio.setup(pin.value, self.gpio.OUT if mode == GpioMode.OUT else self.gpio.IN)
 
     def set(self, pin: Board, value: bool) -> None:
         """Set the output value of a GPIO pin."""
         super().set(pin, value)
         self.gpio.output(pin.value, self.gpio.HIGH if value else self.gpio.LOW)
```

### Comparing `openoligo-0.1.3/openoligo/hal/types.py` & `openoligo-0.1.4/openoligo/hal/types.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/instrument.py` & `openoligo-0.1.4/openoligo/instrument.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/log_config.py` & `openoligo-0.1.4/openoligo/log_config.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/protocols/dna_synthesis.py` & `openoligo-0.1.4/openoligo/protocols/dna_synthesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 DNA Snthesis Protocol
 """
 import logging
 from time import time
 
-from Bio.Seq import Seq  # type: ignore
 from tqdm import tqdm
 
 from openoligo import utils
 from openoligo.instrument import Instrument
+from openoligo.seq import Seq
 from openoligo.steps.flow import dry_all, send_to_waste_rxn, solvent_wash_all
 from openoligo.steps.types import step
 from openoligo.utils import wait_async
 
 
 @step
 async def detritylate(instrument: Instrument) -> None:
```

### Comparing `openoligo-0.1.3/openoligo/steps/flow.py` & `openoligo-0.1.4/openoligo/steps/flow.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/steps/types.py` & `openoligo-0.1.4/openoligo/steps/types.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/openoligo/utils/sim.py` & `openoligo-0.1.4/openoligo/utils/sim.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Sets some parameters for the simulation.
 """
 import logging
 import os
 
-from openoligo.hal.types import __platform__, Platform
+from openoligo.hal.types import Platform, __platform__
 
 # Simulation parameters
 # Can be set using env variable OO_SIM_SPEED=1000
 # SIMULATION_SPEEDUP_FACTOR = 1 if is_rpi() else int(os.environ.get("OO_SIM_SPEED", 1000))
 if os.environ.get("OO_SIM_SPEED") or __platform__ == Platform.SIM:
     SIMULATION_SPEEDUP_FACTOR = int(os.environ.get("OO_SIM_SPEED", 1000))
 else:
```

### Comparing `openoligo-0.1.3/openoligo/utils/wait.py` & `openoligo-0.1.4/openoligo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.3/pyproject.toml` & `openoligo-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "OpenOligo"
-version = "0.1.3"
+version = "0.1.4"
 description = "An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes."
 license = "Apache-2.0"
 authors = ["Satyam Tiwary <satyam@technoculture.io>"]
 readme = "README.md"
 keywords = ["DNA", "synthesis", "genetics", "open-source"]
 
 [tool.poetry.scripts]
 oligo-server = 'app.server:main'
 oligo-synth = 'examples.dna_synthesis:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.4.2"
 python-dotenv = "^1.0.0"
-biopython = "^1.81"
 tqdm = "^4.65.0"
 fastapi = "^0.98.0"
-pdoc3 = "^0.10.0"
 pdocs = "^1.2.0"
 
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
+setuptools = "^68.0.0"
+wheel = "^0.40.0"
+twine = "^4.0.2"
 # ansible = "^8.1.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
```

### Comparing `openoligo-0.1.3/PKG-INFO` & `openoligo-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: openoligo
-Version: 0.1.3
+Version: 0.1.4
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
 Provides-Extra: bb
 Provides-Extra: rpi
-Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: fastapi (>=0.98.0,<0.99.0)
-Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
 Requires-Dist: pdocs (>=1.2.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenOligo
```

