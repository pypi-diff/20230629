# Comparing `tmp/hvps-0.0.2.tar.gz` & `tmp/hvps-0.0.3.tar.gz`

## Comparing `hvps-0.0.2.tar` & `hvps-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hvps-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hvps-0.0.2/.github/CODEOWNERS
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 hvps-0.0.2/.github/workflows/build-test.yml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hvps-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hvps-0.0.2/bindings/nodejs/cli.js
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hvps-0.0.2/bindings/nodejs/index.js
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 hvps-0.0.2/bindings/nodejs/package-lock.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hvps-0.0.2/bindings/nodejs/package.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.2/src/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/__init__.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/__main__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/caen/__init__.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/caen/channel.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/caen/module.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/iseg/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/commands/iseg/channel.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/channel.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/hvps.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/module.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/caen/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/caen/caen.py
--rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/caen/channel.py
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/caen/module.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/iseg/__init__.py
--rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/iseg/channel.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/iseg/iseg.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/devices/iseg/module.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/utils/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hvps-0.0.2/src/hvps/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_caen_commands.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_caen_serial.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_cli.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_iseg_commands.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_iseg_serial.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 hvps-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 hvps-0.0.2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hvps-0.0.2/LICENSE
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 hvps-0.0.2/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hvps-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 hvps-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hvps-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hvps-0.0.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 hvps-0.0.3/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 hvps-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 hvps-0.0.3/bindings/nodejs/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hvps-0.0.3/bindings/nodejs/cli.js
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 hvps-0.0.3/bindings/nodejs/index.js
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 hvps-0.0.3/bindings/nodejs/package-lock.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hvps-0.0.3/bindings/nodejs/package.json
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/__main__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/caen/__init__.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/caen/channel.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/caen/module.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/iseg/__init__.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/iseg/channel.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/commands/iseg/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/channel.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/hvps.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/caen/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/caen/caen.py
+-rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/caen/channel.py
+-rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/caen/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/__init__.py
+-rw-r--r--   0        0        0    39273 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/channel.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/iseg.py
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/module.py
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/output.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/devices/iseg/script.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/utils/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hvps-0.0.3/src/hvps/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_caen_commands.py
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_caen_serial.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_iseg_commands.py
+-rw-r--r--   0        0        0    10901 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_iseg_serial.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hvps-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hvps-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hvps-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 hvps-0.0.3/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hvps-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 hvps-0.0.3/PKG-INFO
```

### Comparing `hvps-0.0.2/.github/workflows/build-test.yml` & `hvps-0.0.3/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/.github/workflows/python-publish.yml` & `hvps-0.0.3/.github/workflows/publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Upload Python Package to PyPI
+name: Upload Python Package to PyPI and nodejs bindings to npm
 
 on:
   release:
     types: [ published ]
 
 jobs:
   build:
@@ -22,18 +22,23 @@
 
       - name: Build package 📦
         run: python -m build
 
       - name: Install package 📦
         run: python -m pip install .
 
-      - name: Verify package version matches tag
+      - name: Verify python package version matches tag
         run: |
           python -c "import hvps; assert '${{ github.event.release.tag_name }}' == 'v' + hvps.__version__"
 
+      - name: Verify npm package version matches tag
+        run: |
+          cd bindings/nodejs
+          python -c "import os,json;version=json.load(open('package.json'))['version'];assert '${{ github.event.release.tag_name }}' == 'v' + version"
+
       - name: Cache dist directory
         uses: actions/cache@v3
         with:
           path: dist
           key: ${{ runner.os }}-dist-${{ github.sha }}-${{ github.run_id}}-${{ github.run_number }}
 
   publish-to-pypi-test:
@@ -64,7 +69,32 @@
           key: ${{ runner.os }}-dist-${{ github.sha }}-${{ github.run_id}}-${{ github.run_number }}
 
       - name: Publish package 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
+
+  publish-to-npm:
+    needs: [ publish-to-pypi ]
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v3
+
+      - uses: actions/setup-node@v3
+        with:
+          node-version: 18
+          cache: 'npm'
+          cache-dependency-path: bindings/nodejs/package-lock.json
+
+      - name: Move to nodejs bindings
+        run: cd bindings/nodejs
+
+      - name: Install dependencies
+        run: npm ci
+
+      - name: Publish to npm
+        run: npm publish
+        env:
+          NODE_AUTH_TOKEN: ${{ secrets.NPM_TOKEN }}
```

### Comparing `hvps-0.0.2/bindings/nodejs/cli.js` & `hvps-0.0.3/bindings/nodejs/cli.js`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/bindings/nodejs/index.js` & `hvps-0.0.3/bindings/nodejs/index.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,12 @@
 const {
     execSync
 } = require('child_process');
-
+const packageJson = require('./package.json');
+const version = packageJson.version;
 
 class ExecutionContext {
     constructor(pythonPath) {
         this.python = pythonPath;
         // check if python path is correct and use absolute path
         this.python = this.getPythonPath();
 
@@ -35,21 +36,28 @@
             console.error(`Error executing command (${command}): ${err}`);
             throw err;
         }
     }
 
     getPackageVersion() {
         const command = `${this.python} -m hvps --version`;
+        let pythonPackageVersion;
         try {
-            return execSync(command, {
+            pythonPackageVersion = execSync(command, {
                 encoding: 'utf-8'
             }).trim();
         } catch (err) {
-            throw new Error(`Error executing command (${command}). Please make sure the package is installed.`);
+            throw new Error(`Error executing command (${command}). Please make sure the HVPS python package is installed. To install a specific version, run: '${this.python} -m pip install hvps==${version}'`);
         }
+
+        if (pythonPackageVersion !== version) {
+            throw new Error("Mismatch between the version of the HVPS python package and the version of the HVPS nodejs package.");
+        }
+
+        return pythonPackageVersion;
     }
 
     print() {
         console.log(`Python version: ${this.getPythonVersion()}`);
         console.log(`Python path: ${this.getPythonPath()}`);
         console.log(`Package version: ${this.getPackageVersion()}`);
     }
```

### Comparing `hvps-0.0.2/bindings/nodejs/package-lock.json` & `hvps-0.0.3/bindings/nodejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/bindings/nodejs/package.json` & `hvps-0.0.3/bindings/nodejs/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.0.3'"}*

```diff
@@ -17,9 +17,9 @@
     "repository": {
         "type": "git",
         "url": "git+https://github.com/lobis/hvps.git"
     },
     "scripts": {
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "0.0.2"
+    "version": "0.0.3"
 }
```

### Comparing `hvps-0.0.2/src/hvps/__main__.py` & `hvps-0.0.3/src/hvps/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hvps import __version__ as hvps_version, Caen, Iseg
+from hvps import __version__ as hvps_version, Caen
 from hvps.commands.caen.module import _set_module_commands, _mon_module_commands
 from hvps.commands.caen.channel import _set_channel_commands, _mon_channel_commands
 
 from serial.tools import list_ports
 
 import argparse
 import logging
@@ -51,15 +51,15 @@
         "value",
         nargs="?",
         default=None,
         help="Value to set parameter to, if applicable",
     )
 
     # iseg
-    iseg_parser = subparsers.add_parser("iseg", help="iseg HVPS")
+    subparsers.add_parser("iseg", help="iseg HVPS")
 
     args = parser.parse_args()
     logging.basicConfig(level=args.log.upper())
     if args.ports:
         ports = [port.device for port in list_ports.comports()]
         print(f"Number of ports available: {len(ports)}")
         for port in ports:
```

### Comparing `hvps-0.0.2/src/hvps/commands/caen/__init__.py` & `hvps-0.0.3/src/hvps/commands/caen/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 from __future__ import annotations
 import re
 
-from .module import (
-    _get_mon_module_command,
-    _get_set_module_command,
-)
-from .channel import (
-    _get_mon_channel_command,
-    _get_set_channel_command,
-)
-
 import logging
 import serial
 
 
 def _write_command(
     ser: serial.Serial, bd: int, command: bytes, response: bool = True
 ) -> str | None:
@@ -51,15 +42,16 @@
     Raises:
         ValueError: If the response is invalid, cannot be decoded, or does not match the expected pattern.
     """
     logger = logging.getLogger(__name__)
     logger.debug(f"Response: {response}")
     if response == b"":
         raise ValueError(
-            "Empty response. There was no response from the device. Check that the device is connected and correctly configured (baudrate)."
+            "Empty response. There was no response from the device. Check that the device is connected and correctly "
+            "configured (baudrate)."
         )
 
     try:
         response: str = response.decode("utf-8").strip()
     except UnicodeDecodeError:
         raise ValueError(f"Invalid response: {response}")
```

### Comparing `hvps-0.0.2/src/hvps/commands/caen/channel.py` & `hvps-0.0.3/src/hvps/commands/caen/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/commands/caen/module.py` & `hvps-0.0.3/src/hvps/commands/caen/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/devices/channel.py` & `hvps-0.0.3/src/hvps/devices/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/devices/hvps.py` & `hvps-0.0.3/src/hvps/devices/hvps.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/devices/module.py` & `hvps-0.0.3/src/hvps/devices/module.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/devices/caen/channel.py` & `hvps-0.0.3/src/hvps/devices/caen/channel.py`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/src/hvps/devices/caen/module.py` & `hvps-0.0.3/src/hvps/devices/caen/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from functools import cached_property
-from typing import List
 
 from ...commands.caen.module import _get_mon_module_command, _get_set_module_command
 from ...commands.caen import _write_command
 from ...utils.utils import string_number_to_bit_array
 from .channel import Channel
 from ..module import Module as BaseModule
```

### Comparing `hvps-0.0.2/src/hvps/devices/iseg/channel.py` & `hvps-0.0.3/src/hvps/devices/iseg/module.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,731 +1,651 @@
-import serial
+from __future__ import annotations
+from functools import cached_property
 from typing import List
 
-from ...commands.iseg.channel import (
-    _get_set_channel_command,
-    _get_mon_channel_command,
-)
-from ...commands.iseg import _write_command
-
-from ..channel import Channel as BaseChannel
-
-
-class Channel(BaseChannel):
-    def set_voltage(self, vset: float):
-        """
-        Set the channel voltage set.
-
-        Args:
-            vset (float): The voltage set value to set in Volt.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT", vset)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
-
-    def switch_on_high_voltage(self):
-        """
-        Switch on the high voltage with the configured ramp speed.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT", "ON")
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
-
-    def switch_off_high_voltage(self):
-        """
-        Switch off the high voltage with the configured ramp speed.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT", "OFF")
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
-
-    def shutdown_channel_high_voltage(self):
-        """
-        Shut down the channel high voltage (without ramp). The channel stays in Emergency Off until the command EMCY CLR is given.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT EMCY", "OFF")
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+import serial
 
-    def clear_channel_emergency_off(self):
-        """
-        Clear the channel from state emergency off. The channel goes to state off.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT EMCY", "CLR")
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+from ...commands.iseg.module import _get_mon_module_command, _get_set_module_command
+from ...commands.iseg import _write_command
+from ...utils.utils import string_number_to_bit_array
+from .channel import Channel
+from ..module import Module as BaseModule
+from .channel import Channel
 
-    def set_voltage_bounds(self, vbounds: float):
-        """
-        Set the channel voltage bounds.
 
-        Args:
-            vbounds (float): The voltage bounds value to set in Volt.
-        """
-        command = _get_set_channel_command(self._channel, ":VOLT:BOUNDS", vbounds)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+class Module(BaseModule):
+    def channel(self, channel: int) -> Channel:
+        return super().channel(channel)
 
-    def set_current(self, iset: float):
-        """
-        Set the channel current set.
+    def __init__(self, _serial: serial.Serial):
+        self._serial = _serial
+        self._channels: List[Channel] = []
 
-        Args:
-            iset (float): The current set value to set in Ampere.
-        """
-        command = _get_set_channel_command(self._channel, ":CURR", iset)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+    @cached_property
+    def number_of_channels(self) -> int:
+        """The number of channels in the module.
 
-    def set_current_bounds(self, ibounds: float):
+        Returns:
+            int: The number of channels.
         """
-        Set the channel current bounds.
+        command = _get_mon_module_command(":READ:MODULE:CHANNELNUMBER")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
-        Args:
-            ibounds (float): The current bounds value to set in Ampere.
+    @property
+    def firmware_release(self) -> str:
         """
-        command = _get_set_channel_command(self._channel, ":CURR:BOUNDS", ibounds)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        Read out Firmware Release (XX.X)
 
-    def clear_event_status(self):
-        """
-        Clear the Channel Event Status register.
+        Returns:
+            str: The firmware release.
         """
-        command = _get_set_channel_command(self._channel, ":EVENT CLEAR", None)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        command = _get_mon_module_command(":READ:FIRMWARE:RELEASE")
+        response = _write_command(self._serial, command, str)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return response[0]
 
-    def clear_event_bits(self, bits):
+    @property
+    def module_status(self) -> dict:
         """
-        Clears single bits or bit combinations in the Channel Event Status register by writing a one to the corresponding bit position.
+        Read out module status register
 
-        Args:
-            bits (int | str): The bits or bit combinations to clear. Can be provided as an integer or a string representing the bit combination.
+        Returns:
+            str: The board alarm status value.
         """
-        command = _get_set_channel_command(self._channel, ":EVENT", bits)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        command = _get_mon_module_command(":READ:MODULE:STATUS")
+        response = _write_command(self._serial, command, dict)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
 
-    def set_trip_timeout(self, timeout):
-        """
-        Set the trip timeout with one millisecond resolution.
+        bit_array = string_number_to_bit_array(response[0])
+        bit_array = list(reversed(bit_array))
 
-        Args:
-            timeout (int): The timeout value to set in milliseconds. Must be in the range 1 to 4095 ms.
-        """
-        if not 1 <= timeout <= 4095:
-            raise ValueError("Timeout value must be in the range 1 to 4095 ms.")
-        command = _get_set_channel_command(self._channel, ":CONF:TRIP:TIME", timeout)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        # TODO: review this
+        return {
+            "Is Voltage Ramp Speed Limited": bit_array[21],
+            "Is Fast Ramp Down": bit_array[16],
+            "Is Kill Enable": bit_array[15],
+            "Is Temperature Good": bit_array[14],
+            "Is Supply Good": bit_array[13],
+            "Is Module Good": bit_array[12],
+            "Is Event Active": bit_array[11],
+            "Is Safety Loop Good": bit_array[10],
+            "Is No Ramp": bit_array[9],
+            "Is No Sum": bit_array[8],
+            "Is Input Error": bit_array[6],
+            "Is Service Is High": bit_array[4],
+            "Voltage On": bit_array[3],
+            "Is Fine Adjustment": bit_array[0],
+        }
 
-    def set_trip_action(self, action):
-        """
-        Set the action to be taken when a current trip occurs for the channel.
+    @property
+    def filter_averaging_steps(self) -> int:
+        """Query the digital filter averaging steps.
 
-        Args:
-            action (int): The action value to set. Possible values are:
-                          - 0: No action (Trip status flag will be set after timeout)
-                          - 1: Turn off the channel with ramp
-                          - 2: Shut down the channel without ramp
-                          - 3: Shut down the whole module without ramp
-                          - 4: Disable the Delayed Trip function
+        Returns:
+            int: The number of steps for filtering.
         """
-        if not 0 <= action <= 4:
-            raise ValueError(
-                "Invalid action value. Expected values are 0, 1, 2, 3, or 4."
-            )
-        command = _get_set_channel_command(self._channel, ":CONF:TRIP:ACTION", action)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        command = _get_mon_module_command(":CONF:AVER")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def trip_action(self):
-        """
-        Query the current action to be taken when a current trip occurs for the channel.
+    def kill_enable(self) -> int:
+        """Get the current value for the kill enable function.
 
         Returns:
-            int: The current action value.
+            int: The current kill enable value. 1 for enable, 0 for disable.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:TRIP:ACTION")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":CONF:KILL")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Unexpected response. Multiple action values received.")
-        if not 0 <= int(response[0]) <= 4:
-            raise ValueError(
-                "Invalid action value. Expected values are 0, 1, 2, 3, or 4."
-            )
+            raise ValueError("Wrong number of values were received, one value expected")
         return int(response[0])
 
-    def set_external_inhibit_action(self, action):
-        """
-        Set the action to be taken when an External Inhibit event occurs for the channel.
+    @property
+    def adjustment(self) -> int:
+        """Get the fine adjustment state.
 
-        Args:
-            action (int): The action value to set. Possible values are:
-                          - 0: No action (External Inhibit status flag will be set)
-                          - 1: Turn off the channel with ramp
-                          - 2: Shut down the channel without ramp
-                          - 3: Shut down the whole module without ramp
-                          - 4: Disable the External Inhibit function
+        Returns:
+            int: The current fine adjustment state. 1 for on, 0 for off.
         """
-        if not 0 <= action <= 4:
-            raise ValueError(
-                "Invalid action value. Expected values are 0, 1, 2, 3, or 4."
-            )
-        command = _get_set_channel_command(self._channel, ":CONF:INHP:ACTION", action)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        command = _get_mon_module_command(":CONF:ADJUST")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
-    def get_external_inhibit_action(self):
-        """
-        Query the action to be taken when an External Inhibit event occurs for the channel.
+    @property
+    def module_can_address(self) -> int:
+        """Query the module's CAN bus address.
 
         Returns:
-            int: The current action value.
+            int: The current CAN bus address of the module.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:INHP:ACTION")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":CONF:CAN:ADDR")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Unexpected response. Multiple action values received.")
-        if not 0 <= int(response[0]) <= 4:
-            raise ValueError(
-                "Invalid action value. Expected values are 0, 1, 2, 3, or 4."
-            )
+            raise ValueError("Wrong number of values were received, one value expected")
         return int(response[0])
 
-    def set_output_mode(self, mode):
-        """
-        Set the channel output mode.
-
-        Args:
-            mode (int): The output mode value to set.
-
-        Raises:
-            ValueError: If the specified mode value is not allowed.
+    @property
+    def module_can_bitrate(self) -> int:
+        """Query the module's CAN bus bit rate.
 
-        Output Mode allowed values: 1, 2, 3.
+        Returns:
+            int: The current CAN bus bit rate of the module.
         """
-        allowed_modes = [1, 2, 3]
-        if mode not in allowed_modes:
-            raise ValueError("Invalid output mode. Allowed modes are: 1, 2, 3.")
-        command = _get_set_channel_command(self._channel, ":CONF:OUTPUT:MODE", mode)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Last command haven't been processed.")
+        command = _get_mon_module_command(":CONF:CAN:BITRATE")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def output_mode(self):
-        """
-        Query the configured channel output mode.
+    def serial_baud_rate(
+        self,
+    ) -> (
+        int
+    ):  # Instruction is currently implemented for EHS devices with serial interface only
+        """Query the device's serial baud rate.
 
         Returns:
-            int: The current output mode value.
-
-        Output Mode allowed values: 1, 2, 3.
+            int: The current serial baud rate of the device.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:OUTPUT:MODE")
-        response = _write_command(self._serial, command)
-
+        command = _get_mon_module_command(":CONF:SERIAL:BAUD")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-
-        allowed_modes = [1, 2, 3]
-        if int(response[0]) not in allowed_modes:
-            raise ValueError("Invalid output mode. Allowed modes are: 1, 2, 3.")
+            raise ValueError("Wrong number of values were received, one value expected")
         return int(response[0])
 
     @property
-    def available_output_modes(self):
-        """
-        Query the available channel output modes as a list.
+    def serial_echo_enable(self) -> int:
+        """Check if serial echo is enabled or disabled.
 
         Returns:
-            list: The list of available output mode values.
-
+            int: 1 if serial echo is enabled, 0 if disabled.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:OUTPUT:MODE:LIST")
-        response = _write_command(self._serial, command)
-
-        if 0 >= len(response) > 3:
-            raise ValueError("Invalid number of output modes received.")
+        command = _get_mon_module_command(":CONF:SERIAL:ECHO")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
-        try:
-            output_values = [int(mode) for mode in response]
-        except ValueError:
-            raise ValueError("Invalid output mode value received.")
+    @property
+    def serial_echo_enabled(self) -> bool:
+        return self.serial_echo_enable == 1
 
-        allowed_modes = [1, 2, 3]
-        for mode in output_values:
-            if mode not in allowed_modes:
-                raise ValueError(
-                    f"Invalid output mode. Allowed modes are: {allowed_modes}"
-                )
+    @property
+    def serial_echo_disabled(self) -> bool:
+        return self.serial_echo_enable == 0
 
-        return output_values
+    @property
+    def module_voltage_limit(self) -> float:
+        """Query the module's voltage limit in percent.
 
-    def set_output_polarity(self, polarity: str):
+        Returns:
+            float: The current voltage limit of the module.
         """
-        Set the output polarity of the channel.
-
-        Args:
-            polarity (str): The output polarity to set. Valid values are "p" for positive and "n" for negative.
+        command = _get_mon_module_command(":READ:VOLT:LIM")
+        response = _write_command(self._serial, command, float)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return float(response[0].rstrip("%"))
 
-        Raises:
-            ValueError: If an invalid polarity value is provided.
+    @property
+    def module_current_limit(self) -> float:
+        """Query the module's current limit in percent.
 
-        Example:
-            channel.set_output_polarity("n")
+        Returns:
+            float: The current current limit of the module.
         """
-        if polarity not in ["p", "n"]:
-            raise ValueError(
-                "Invalid polarity value. Valid values are 'p' for positive and 'n' for negative."
-            )
-        command = _get_set_channel_command(self._channel, ":CONF:OUTPUT:POL", polarity)
-        response = _write_command(self._serial, command)
-        if int(response[0]) != 1:
-            raise ValueError("Not all commands before this query have been processed.")
+        command = _get_mon_module_command(":READ:CURR:LIM")
+        response = _write_command(self._serial, command, float)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return float(response[0].rstrip("%"))
 
     @property
-    def output_polarity(self):
-        """
-        Query the current output polarity of the channel.
+    def module_voltage_ramp_speed(self) -> float:
+        """Query the module's voltage ramp speed in percent/second.
 
         Returns:
-            str: The current output polarity. "p" for positive, "n" for negative.
-
-        Example:
-            polarity = channel.output_polarity
-            print(polarity)  # Example output: "n"
+            float: The current voltage ramp speed of the module.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:OUTPUT:POL")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:RAMP:VOLT")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
-            raise ValueError("Not all commands before this query have been processed.")
-        return response[0]
+            raise ValueError("Wrong number of values were received, one value expected")
+        return float(response[0][:3])
 
     @property
-    def available_output_polarities(self):
-        """
-        Query the available channel output polarities as a list.
+    def module_current_ramp_speed(self) -> float:
+        """Query the module's current ramp speed in percent/second.
 
         Returns:
-            list: The list of available output polarity values.
-
-        Output Polarity List:
-            "p" - Positive
-            "n" - Negative
-
-        Example:
-            polarities = channel.available_output_polarities
-            print(polarities)  # Example output: ["p", "n"]
+            float: The current current ramp speed of the module.
         """
-        command = _get_mon_channel_command(self._channel, ":CONF:OUTPUT:POL:LIST")
-        response = _write_command(self._serial, command)
-
-        if len(response) != 2:
-            raise ValueError("Wrong number of values were sent, two values expected")
-
-        for polarity in response:
-            if polarity not in ["p", "n"]:
-                raise ValueError(
-                    "Invalid polarity value. Valid values are 'p' for positive and 'n' for negative."
-                )
-
-        return response
+        command = _get_mon_module_command(":READ:RAMP:CURR")
+        response = _write_command(self._serial, command, float)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return float(response[0][:3])
 
     @property
-    def voltage_set(self):
-        """
-        Query the voltage set Vset in Volt.
+    def module_control_register(self) -> int:
+        """Query the Module Control register.
 
         Returns:
-            float: The voltage set Vset in Volt.
-
-        Example:
-            voltage = channel.voltage_set
-            print(voltage)  # Example output: 1234.0
+            int: The value of the Module Control register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:CONTROL")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-        return float(response[0][:-1])
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def voltage_limit(self):
-        """
-        Query the voltage limit Vlim in Volt.
+    def module_status_register(self) -> int:
+        """Query the Module Status register.
 
         Returns:
-            float: The voltage limit Vlim in Volt.
-
-        Example:
-            limit = channel.voltage_limit
-            print(limit)  # Example output: 3000.0
+            int: The value of the Module Status register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:LIM")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:STATUS")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-        return float(response[0][:-1])
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def voltage_nominal(self):
-        """
-        Query the channel voltage nominal Vnom in Volt.
+    def module_event_status_register(self) -> int:
+        """Query the Module Event Status register.
 
         Returns:
-            float: The channel voltage nominal Vnom in Volt.
-
-        Example:
-            nominal = channel.voltage_nominal
-            print(nominal)  # Example output: 6000.0
+            int: The value of the Module Event Status register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:NOM")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:EVENT:STATUS")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-        return float(response[0][:-1])
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def voltage_mode(self):
-        """
-        Query the configured channel voltage mode with polarity sign in Volt.
+    def module_event_mask_register(self) -> int:
+        """Query the Module Event Mask register.
 
         Returns:
-            str: The configured channel voltage mode with polarity sign in Volt.
-
-        Example:
-            mode = channel.voltage_mode
-            print(mode)  # Example output: "6.0E3V"
+            int: The value of the Module Event Mask register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:MODE")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:EVENT:MASK")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-        return float(response[0][:-1])
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def voltage_mode_list(self):
-        """
-        Query the available channel voltage modes as a list.
+    def module_event_channel_status_register(self) -> int:
+        """Query the Module Event Channel Status register.
 
         Returns:
-            List[str]: The 3 available channel voltage modes as a list of strings.
-
-        Example:
-            mode_list = channel.voltage_mode_list
-            print(mode_list)  # Example output: ["2.0E3V", "4.0E3V", "6.0E3V"]
+            int: The value of the Module Event Channel Status register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:MODE:LIST")
-        response = _write_command(self._serial, command)
-        if len(response) != 3:
-            raise ValueError("Wrong number of values were sent, three values expected")
-        return [float(modes[:-1]) for modes in response]
+        command = _get_mon_module_command(":READ:MODULE:EVENT:CHANSTAT")
+        response = _write_command(self._serial, command, int)
+        if len(response) != 1:
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def voltage_bounds(self):
-        """
-        Query the channel voltage bounds in Volt.
+    def module_event_channel_mask_register(self) -> int:
+        """Query the Module Event Channel Mask register.
 
         Returns:
-            str: The channel voltage bounds in Volt.
-
-        Example:
-            bounds = channel.voltage_bounds
-            print(bounds)  # Example output: "0.00000E3V"
+            int: The value of the Module Event Channel Mask register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:BOUNDS")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:EVENT:CHANMASK")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
-            raise ValueError("Wrong number of values were sent, one value expected")
-        return float(response[0][:-1])
+            raise ValueError("Wrong number of values were received, one value expected")
+        return int(response[0])
 
     @property
-    def is_set_on(self) -> bool:
-        """
-        Query the channel control bit "Set On".
+    def module_supply_voltage(self) -> List[float]:
+        """Query the module supply voltages.
 
         Returns:
-            bool: True if the channel control bit is set on, False otherwise.
-
-        Example:
-            is_on = channel.is_set_on
-            print(is_on)  # Example output: True
+            Tuple[str, str, str, str, str, str]: The module supply voltages.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:ON")
-        response = _write_command(self._serial, command)
-        if len(response) != 1:
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY? (@0-6)")
+        response = _write_command(self._serial, command, List[float])
+        if len(response) != 7:
             raise ValueError("Wrong number of values were received, one value expected")
-        return int(response[0][:-1]) == 1
+
+        return [float(string[:-1]) for string in response]
 
     @property
-    def is_set_emergency_off(self) -> bool:
-        """
-        Query the channel control bit "Set Emergency Off".
+    def module_supply_voltage_p24v(self) -> float:
+        """Query the module supply voltage +24 Volt.
 
         Returns:
-            bool: True if the channel control bit is set to Emergency Off, False otherwise.
-
-        Example:
-            is_emergency_off = channel.is_set_emergency_off
-            print(is_emergency_off)  # Example output: False
+            float: The module supply voltage +24 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:VOLT:EMCY")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:P24V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return int(response[0][:-1]) == 1
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_set(self) -> float:
-        """
-        Query the current set (Iset) in Ampere.
+    def module_supply_voltage_n24v(self) -> float:
+        """Query the module supply voltage -24 Volt.
 
         Returns:
-            float: The current set value.
-
-        Example:
-            current = channel.current_set
-            print(current)  # Example output: 50.000E-6
-
+            float: The module supply voltage -24 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:N24V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(
-            response[0][:-1]
-        )  # Remove the last character from the response (unit)
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_limit(self) -> float:
-        """
-        Query the current limit (Ilim) in Ampere.
+    def module_supply_voltage_p5v(self) -> float:
+        """Query the module supply voltage +5 Volt.
 
         Returns:
-            float: The current limit value.
-
-        Example:
-            limit = channel.current_limit
-            print(limit)  # Example output: 5.00000E-3
-
+            float: The module supply voltage +5 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR:LIM")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:P5V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(
-            response[0][:-1]
-        )  # Remove the last character from the response (unit)
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_nominal(self) -> float:
-        """
-        Query the current nominal (Inom) in Ampere.
+    def module_supply_voltage_p3v(self) -> float:
+        """Query the module internal supply voltage +3.3 Volt.
 
         Returns:
-            float: The current nominal value.
-
-        Example:
-            nominal = channel.current_nominal
-            print(nominal)  # Example output: 6.00000E-3
-
+            float: The module internal supply voltage +3.3 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR:NOM")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:P3V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(
-            response[0][:-1]
-        )  # Remove the last character from the response (unit)
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_mode(self) -> float:
-        """
-        Query the configured channel current mode in Ampere.
+    def module_supply_voltage_p12v(self) -> float:
+        """Query the module internal supply voltage +12 Volt.
 
         Returns:
-            float: The current mode value.
-
-        Example:
-            mode = channel.current_mode
-            print(mode)  # Example output: 2.00000E-3
-
+            float: The module internal supply voltage +12 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR:MODE")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:P12V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(
-            response[0][:-1]
-        )  # Remove the last character from the response (unit)
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_mode_list(self) -> List[float]:
-        """
-        Query the available channel current modes as a list.
+    def module_supply_voltage_n12v(self) -> float:
+        """Query the module internal supply voltage -12 Volt.
 
         Returns:
-            List[float]: The list of available current modes.
-
-        Example:
-            modes = channel.current_mode_list
-            print(modes)  # Example output: [6.0E-3, 4.0E-3, 2.0E-3]
-
+            float: The module internal supply voltage -12 Volt.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR:MODE:LIST")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SUPPLY:N12V")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        modes = [
-            float(mode[:-1]) for mode in response
-        ]  # Remove the last character from each mode (unit)
-        return modes
+        voltage = response[0][:-1]
+        return float(voltage)
 
     @property
-    def current_bounds(self) -> float:
-        """
-        Query the channel current bounds in Ampere.
+    def module_temperature(self) -> float:
+        """Query the module temperature in degree Celsius.
 
         Returns:
-            float: The channel current bounds.
-
-        Example:
-            bounds = channel.current_bounds
-            print(bounds)  # Example output: 0.00000E-3
-
+            float: The module temperature in degree Celsius.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:CURR:BOUNDS")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:TEMPERATURE")
+        response = _write_command(self._serial, command, float)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-1])
+        temperature = response[0][:-1]
+        return float(temperature)
 
     @property
-    def current_ramp_speed(self) -> float:
-        """
-        Query the channel current ramp speed in Ampere/second.
+    def setvalue_changes_counter(self) -> int:
+        """Query the setvalue changes counter.
 
         Returns:
-            float: The channel current ramp speed.
-
-        Example:
-            speed = channel.current_ramp_speed
-            print(speed)  # Example output: 2.0000E-3
-
+            int: The setvalue changes counter.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:CURR")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:MODULE:SETVALUE")
+        response = _write_command(self._serial, command, int)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        return int(response[0])
 
     @property
-    def voltage_ramp_speed(self) -> float:
-        """
-        Query the channel voltage ramp speed in Volt/second.
+    def firmware_name(self) -> str:
+        """Query the module's firmware name.
 
         Returns:
-            float: The channel voltage ramp speed.
-
-        Example:
-            speed = channel.voltage_ramp_speed
-            print(speed)  # Example output: 0.25000E3
-
+            str: The firmware name.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:VOLT")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":READ:FIRMWARE:NAME")
+        response = _write_command(self._serial, command, str)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        return response[0]
 
     @property
-    def voltage_ramp_speed_minimum(self) -> float:
-        """
-        Query the channel voltage ramp speed minimum in Volt/second.
+    def configuration_mode(self) -> bool:
+        """Check if the device is in configuration mode.
 
         Returns:
-            float: The channel voltage ramp speed minimum.
-
-        Example:
-            speed_min = channel.voltage_ramp_speed_minimum
-            print(speed_min)  # Example output: 0.00005E3
-
+            bool: true if in configuration mode, otherwise false.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:VOLT:MIN")
-        response = _write_command(self._serial, command)
+        command = _get_mon_module_command(":SYSTEM:USER:CONFIG")
+        response = _write_command(self._serial, command, bool)
         if len(response) != 1:
             raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        return int(response[0]) == 1
 
-    @property
-    def voltage_ramp_speed_maximum(self) -> float:
+    # Setters
+
+    @serial_baud_rate.setter
+    def serial_baud_rate(self, baud_rate: int) -> None:
+        """Set the device's serial baud rate.
+
+        Args:
+            baud_rate (int): The serial baud rate to set.
         """
-        Query the channel voltage ramp speed maximum in Volt/second.
+        command = _get_set_module_command(":CONF:SERIAL:BAUD", baud_rate)
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != baud_rate:
+            raise ValueError("Last command hasn't been processed.")
+
+    @serial_echo_enable.setter
+    def serial_echo_enable(self, enabled: int) -> None:
+        """Enable or disable serial echo.
 
-        Returns:
-            float: The channel voltage ramp speed maximum.
+        Args:
+            enabled (int): 1 to enable serial echo, 0 to disable.
+        """
+        if enabled not in [0, 1]:
+            raise ValueError(
+                "Invalid serial echo value. Please choose 1 for enabled or 0 for disabled."
+            )
 
-        Example:
-            speed_max = channel.voltage_ramp_speed_maximum
-            print(speed_max)  # Example output: 1.20000E3
+        command = _get_set_module_command(":CONF:SERIAL:ECHO", enabled)
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @filter_averaging_steps.setter
+    def filter_averaging_steps(self, steps: int) -> None:
+        """Set the number of digital filter averaging steps.
 
+        Args:
+            steps (int): The number of steps for filtering. Accepts values 1, 16, 64, 256, 512, or 1024.
+
+        Raises:
+            ValueError: If an invalid number of steps is provided.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:VOLT:MAX")
-        response = _write_command(self._serial, command)
-        if len(response) != 1:
-            raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        valid_steps = [1, 16, 64, 256, 512, 1024]
+        if steps not in valid_steps:
+            raise ValueError(
+                f"Invalid number of steps. Please choose from {valid_steps}."
+            )
 
-    @property
-    def current_ramp_speed_minimum(self) -> float:
+        command = _get_set_module_command(":CONF:AVER", str(steps))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @kill_enable.setter
+    def kill_enable(self, enable: int) -> None:
+        """Set function kill enable (1) or kill disable (0).
+
+        Args:
+            enable (int): The kill enable value to set. Accepts 1 for enable or 0 for disable.
         """
-        Query the channel current ramp speed minimum in Ampere/second.
+        if enable not in [0, 1]:
+            raise ValueError(
+                "Invalid kill enable value. Please choose 1 for enable or 0 for disable."
+            )
 
-        Returns:
-            float: The channel current ramp speed minimum.
+        command = _get_set_module_command(":CONF:KILL", str(enable))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @adjustment.setter
+    def adjustment(self, value: int) -> None:
+        """Set the fine adjustment function on (1) or off (0).
+
+        Args:
+            value (int): The adjustment value to set. Accepts 1 for on or 0 for off.
+        """
+        if value not in [0, 1]:
+            raise ValueError(
+                "Invalid adjustment value. Please choose 1 for on or 0 for off."
+            )
 
-        Example:
-            speed_min = channel.current_ramp_speed_minimum
-            print(speed_min)  # Example output: 1.0000E-3
+        command = _get_set_module_command(":CONF:ADJUST", str(value))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @module_event_mask_register.setter
+    def module_event_mask_register(self, mask: int) -> None:
+        """Set the Module Event Mask register.
 
+        Args:
+            mask (int): The value to set in the Module Event Mask register.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:CURR:MIN")
-        response = _write_command(self._serial, command)
-        if len(response) != 1:
-            raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        command = _get_set_module_command(":CONF:EVENT:MASK", str(mask))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @module_event_channel_mask_register.setter
+    def module_event_channel_mask_register(self, mask: int) -> None:
+        """Set the Module Event Channel Mask register.
 
-    @property
-    def current_ramp_speed_maximum(self) -> float:
+        Args:
+            mask (int): The value to set in the Module Event Channel Mask register.
         """
-        Query the channel current ramp speed maximum in Ampere/second.
+        command = _get_set_module_command(":CONF:EVENT:CHANMASK", str(mask))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @module_can_address.setter
+    def module_can_address(self, address: int) -> None:
+        """Set the module's CAN bus address.
 
-        Returns:
-            float: The channel current ramp speed maximum.
+        Args:
+            address (int): The CAN bus address to set (0-63).
+        """
+        if not (0 <= address <= 63):
+            raise ValueError(
+                "Invalid CAN bus address. Please choose an address between 0 and 63."
+            )
 
-        Example:
-            speed_max = channel.current_ramp_speed_maximum
-            print(speed_max)  # Example output: 6.0000E-3
+        command = _get_set_module_command(":CONF:CAN:ADDR", str(address))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    @module_can_bitrate.setter
+    def module_can_bitrate(self, bitrate: int) -> None:
+        """Set the module's CAN bus bit rate.
 
+        Args:
+            bitrate (int): The CAN bus bit rate to set. Accepts 125000 or 250000.
         """
-        command = _get_mon_channel_command(self._channel, ":READ:RAMP:CURR:MAX")
-        response = _write_command(self._serial, command)
-        if len(response) != 1:
-            raise ValueError("Wrong number of values were received, one value expected")
-        return float(response[0][:-3])
+        if bitrate not in [125000, 250000]:
+            raise ValueError(
+                "Invalid CAN bus bitrate. Please choose either 125000 or 250000."
+            )
+
+        command = _get_set_module_command(":CONF:CAN:BITRATE", str(bitrate))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    def enter_configuration_mode(self, serial_number: int):
+        """Set the device to configuration mode to change the CAN bitrate or address.
+
+        Parameters:
+            serial_number (int): The device serial number.
+
+        """
+        command = _get_set_module_command(":SYSTEM:USER:CONFIG", str(serial_number))
+        _write_command(self._serial, command, None)
+
+    def exit_configuration_mode(self):
+        """Set the device back to normal mode."""
+        command = _get_set_module_command(":SYSTEM:USER:CONFIG", "0")
+        _write_command(self._serial, command, None)
+
+    def set_serial_echo_enabled(self) -> None:
+        """Enable serial echo."""
+        self.serial_echo_enable = 1
+
+    def set_serial_echo_disabled(self) -> None:
+        """Disable serial echo."""
+        self.serial_echo_enable = 0
+
+    def reset_module_event_status(self) -> None:
+        """Reset the Module Event Status register."""
+        command = _get_set_module_command(":CONF:EVENT CLEAR", "")
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
+
+    def clear_module_event_status_bits(self, bits: int) -> None:
+        """Clear single bits or bit combinations in the Module Event Status register.
+
+        Args:
+            bits (int): The bits to clear in the Module Event Status register.
+        """
+        command = _get_set_module_command(":CONF:EVENT", str(bits))
+        response = _write_command(self._serial, command, None)
+        if len(response) != 1 or int(response[0]) != 1:
+            raise ValueError("Last command hasn't been processed.")
```

### Comparing `hvps-0.0.2/src/hvps/utils/utils.py` & `hvps-0.0.3/src/hvps/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from serial.tools import list_ports
 from typing import List
 
 
 def string_number_to_bit_array(string) -> List[bool]:
     """
-    Converts a string representing a 16-bit integer into a list of bits.
+    Converts a string representing a 32-bit integer into a list of bits.
 
     Args:
         string (str): The string to convert. It must be a string representing an integer (e.g. "01024").
 
     Returns:
-        list: The list of 16 bits, from least significant to most significant.
+        list: The list of 32 bits, from least significant to most significant.
     """
 
     try:
         string_as_int = int(string)
     except ValueError:
         raise ValueError(f"Invalid string '{string}'. Must be an integer.")
 
-    return list(reversed([bool(int(bit)) for bit in f"{string_as_int:016b}"]))
+    return list(reversed([bool(int(bit)) for bit in f"{string_as_int:032b}"]))
 
 
 def get_serial_ports() -> List[str]:
     """
     Get a list of available serial ports.
 
     Returns:
```

### Comparing `hvps-0.0.2/tests/test_caen_commands.py` & `hvps-0.0.3/tests/test_caen_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import pytest
 
-from hvps.commands.caen import (
-    _parse_response,
-    _get_set_module_command,
-    _get_mon_module_command,
+from hvps.commands.caen import _parse_response
+from hvps.commands.caen.channel import (
     _get_set_channel_command,
     _get_mon_channel_command,
 )
 
+from hvps.commands.caen.module import (
+    _get_set_module_command,
+    _get_mon_module_command,
+)
+
 
 def test_caen_module_get_commands():
     with pytest.raises(ValueError):
         # invalid parameter name
         _get_mon_module_command(0, "TEST")
 
     with pytest.raises(ValueError):
@@ -19,25 +22,24 @@
         _get_mon_module_command(-1, "BDNAME")
 
     command = _get_mon_module_command(0, "BDNAME")
     assert command == b"$BD:00,CMD:MON,PAR:BDNAME\r\n"
 
 
 def test_caen_module_set_commands():
-    def test_caen_module_set_commands():
-        with pytest.raises(ValueError):
-            # invalid parameter name
-            _get_set_module_command(0, "TEST", 10)
-
-        with pytest.raises(ValueError):
-            # invalid board number
-            _get_set_module_command(-1, "BDNAME", 10)
+    with pytest.raises(ValueError):
+        # invalid parameter name
+        _get_set_module_command(0, "TEST", 10)
+
+    with pytest.raises(ValueError):
+        # invalid board number
+        _get_set_module_command(-1, "BDILKM", 10)
 
-        command = _get_set_module_command(0, "BDNAME", 10)
-        assert command == b"$BD:00,CMD:SET,PAR:BDNAME,VAL:10\r\n"
+    command = _get_set_module_command(0, "BDILKM", 10)
+    assert command == b"$BD:00,CMD:SET,PAR:BDILKM,VAL:10\r\n"
 
 
 def test_caen_channel_get_commands():
     with pytest.raises(ValueError):
         # invalid parameter name
         _get_mon_channel_command(0, 1, "TEST")
 
@@ -95,15 +97,15 @@
         # Invalid response format
         response = b"Invalid response\r\n"
         _parse_response(response)
 
     response = b"#BD:09,CMD:OK\r\n"
     bd, value = _parse_response(response)
     assert bd == 9
-    assert value == None
+    assert value is None
 
     with pytest.raises(ValueError):
         # number needs to be two digits
         response = b"#BD:9,CMD:OK\r\n"
         _parse_response(response)
 
     with pytest.raises(ValueError):
```

### Comparing `hvps-0.0.2/tests/test_caen_serial.py` & `hvps-0.0.3/tests/test_caen_serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def test_caen_module_monitor():
     # no ports available
     caen = Caen(
         port=serial_port,
         baudrate=serial_baud,
         connect=True,
         timeout=timeout,
-        verbosity=logging.DEBUG,
+        logging_level=logging.DEBUG,
     )
     print(
         f"Serial port status: connected: {caen.connected}, port: {caen.port}, baudrate: {caen.baudrate}, timeout: {caen.timeout}"
     )
     module = caen.module(0)
 
     control_mode = module.control_mode
@@ -94,15 +94,15 @@
 @serial_skip_decorator
 def test_caen_channel_serial():
     caen = Caen(
         port=serial_port,
         baudrate=serial_baud,
         connect=True,
         timeout=timeout,
-        verbosity=logging.DEBUG,
+        logging_level=logging.DEBUG,
     )
     print(
         f"Serial port status: connected: {caen.connected}, port: {caen.port}, baudrate: {caen.baudrate}, timeout: {caen.timeout}"
     )
     module = caen.module(0)
 
     for channel in module.channels:
```

### Comparing `hvps-0.0.2/tests/test_cli.py` & `hvps-0.0.3/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import subprocess
 import sys
-import pytest
 
 
 def run_main_with_arguments(arguments: list) -> tuple:
     main_file_path = os.path.join(
         os.path.dirname(__file__), "..", "src/hvps", "__main__.py"
     )
     main_file_path = os.path.abspath(main_file_path)
```

### Comparing `hvps-0.0.2/.gitignore` & `hvps-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -128,7 +128,10 @@
 # Pyre type checker
 .pyre/
 
 .idea/
 .vscode/
 
 node_modules/
+
+# ruff
+.ruff_cache/
```

### Comparing `hvps-0.0.2/LICENSE` & `hvps-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/README.md` & `hvps-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # HVPS
 
-[![PyPI version](https://badge.fury.io/py/caenhv.svg)](https://badge.fury.io/py/caenhv)
-[![Build and Test](https://github.com/lobis/caen-hv/actions/workflows/build-test.yml/badge.svg)](https://github.com/lobis/caen-hv/actions/workflows/build-test.yml)
-[![PyPI downloads](https://img.shields.io/pypi/dm/caenhv.svg)](https://pypi.org/project/caenhv/)
+[![PyPI version](https://badge.fury.io/py/hvps.svg)](https://badge.fury.io/py/hvps)
+[![npm version](https://badge.fury.io/js/hvps.svg)](https://badge.fury.io/js/hvps)
+
+[![PyPI downloads](https://img.shields.io/pypi/dm/hvps.svg)](https://pypi.org/project/hvps/)
 ![Python Version](https://img.shields.io/badge/python-3.8-blue.svg)
 
+[![Build and Test](https://github.com/lobis/hvps/actions/workflows/build-test.yml/badge.svg)](https://github.com/lobis/hvps/actions/workflows/build-test.yml)
+[![Upload Python Package to PyPI and nodejs bindings to npm](https://github.com/lobis/hvps/actions/workflows/publish.yml/badge.svg)](https://github.com/lobis/hvps/actions/workflows/publish.yml)
+
 ## 🤔 What is this?
 
 The goal of this Python package is to interface with different brands of high voltage power supplies in a uniform way.
 Currently only CAEN and iseg brands are supported. Communication is performed via serial port (over USB).
 
 ## ⚠️ Disclaimer
 
 The features of this package are based on my needs at the time of writing.
 I have done very limited testing on a single model (DT1471ET) but it should also work for other CAEN power supplies also
 supporting RS232.
 
 If you use this package, it is very possible you find a bug or some oversight.
-You are encouraged to make a [pull request](https://github.com/lobis/caen-hv/pulls) or to create
-an [issue](https://github.com/lobis/caen-hv/issues) to report a bug, to request additional features or to suggest
+You are encouraged to make a [pull request](https://github.com/lobis/hvps/pulls) or to create
+an [issue](https://github.com/lobis/hvps/issues) to report a bug, to request additional features or to suggest
 improvements.
 
 ## ⚙️ Installation
 
 Installation via `pip` is supported.
 To install the latest [published version](https://github.com/lobis/lecroy-scope/releases), run:
 
@@ -34,30 +38,32 @@
 
 ```bash
 pip install .[dev]
 ```
 
 ## 👨‍💻 Usage
 
+### CAEN
+
 ```python
-from hvps import CaenHV
+from hvps import Caen
 
 # automatically detect serial port and baudrate (can be manually set)
-caen = CaenHV()
+caen = Caen()
 # get the first module. CAEN supports multiple modules over the same connection
-# typically only one module should be present
+# typically only one module will be present
 module = caen.module(0)
 
 # get channel number 2
 channel = module.channel(2)
 
 # print current 'vset' and 'vmon' values
 print(f"vset: {channel.vset}")
 print(f"vmon: {channel.vmon}")
 
 # switch channel off and on
-channel.off()
-channel.on()
+channel.turn_off()
+channel.turn_on()
 
 # set a new value of 'vset'
 channel.vset = 300.0  # 300 V
 ```
```

### Comparing `hvps-0.0.2/pyproject.toml` & `hvps-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hvps-0.0.2/PKG-INFO` & `hvps-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvps
-Version: 0.0.2
+Version: 0.0.3
 Summary: An unofficial Python package 🐍📦 to interface with CAEN high voltage power supplies
 Project-URL: Download, https://github.com/lobis/hvps/releases
 Project-URL: Homepage, https://github.com/lobis/hvps
 Project-URL: Bug Tracker, https://github.com/lobis/hvps/issues
 Author-email: Luis Antonio Obis Aparicio <luis.antonio.obis@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
@@ -16,33 +16,37 @@
 Requires-Dist: pytest; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # HVPS
 
-[![PyPI version](https://badge.fury.io/py/caenhv.svg)](https://badge.fury.io/py/caenhv)
-[![Build and Test](https://github.com/lobis/caen-hv/actions/workflows/build-test.yml/badge.svg)](https://github.com/lobis/caen-hv/actions/workflows/build-test.yml)
-[![PyPI downloads](https://img.shields.io/pypi/dm/caenhv.svg)](https://pypi.org/project/caenhv/)
+[![PyPI version](https://badge.fury.io/py/hvps.svg)](https://badge.fury.io/py/hvps)
+[![npm version](https://badge.fury.io/js/hvps.svg)](https://badge.fury.io/js/hvps)
+
+[![PyPI downloads](https://img.shields.io/pypi/dm/hvps.svg)](https://pypi.org/project/hvps/)
 ![Python Version](https://img.shields.io/badge/python-3.8-blue.svg)
 
+[![Build and Test](https://github.com/lobis/hvps/actions/workflows/build-test.yml/badge.svg)](https://github.com/lobis/hvps/actions/workflows/build-test.yml)
+[![Upload Python Package to PyPI and nodejs bindings to npm](https://github.com/lobis/hvps/actions/workflows/publish.yml/badge.svg)](https://github.com/lobis/hvps/actions/workflows/publish.yml)
+
 ## 🤔 What is this?
 
 The goal of this Python package is to interface with different brands of high voltage power supplies in a uniform way.
 Currently only CAEN and iseg brands are supported. Communication is performed via serial port (over USB).
 
 ## ⚠️ Disclaimer
 
 The features of this package are based on my needs at the time of writing.
 I have done very limited testing on a single model (DT1471ET) but it should also work for other CAEN power supplies also
 supporting RS232.
 
 If you use this package, it is very possible you find a bug or some oversight.
-You are encouraged to make a [pull request](https://github.com/lobis/caen-hv/pulls) or to create
-an [issue](https://github.com/lobis/caen-hv/issues) to report a bug, to request additional features or to suggest
+You are encouraged to make a [pull request](https://github.com/lobis/hvps/pulls) or to create
+an [issue](https://github.com/lobis/hvps/issues) to report a bug, to request additional features or to suggest
 improvements.
 
 ## ⚙️ Installation
 
 Installation via `pip` is supported.
 To install the latest [published version](https://github.com/lobis/lecroy-scope/releases), run:
 
@@ -54,30 +58,32 @@
 
 ```bash
 pip install .[dev]
 ```
 
 ## 👨‍💻 Usage
 
+### CAEN
+
 ```python
-from hvps import CaenHV
+from hvps import Caen
 
 # automatically detect serial port and baudrate (can be manually set)
-caen = CaenHV()
+caen = Caen()
 # get the first module. CAEN supports multiple modules over the same connection
-# typically only one module should be present
+# typically only one module will be present
 module = caen.module(0)
 
 # get channel number 2
 channel = module.channel(2)
 
 # print current 'vset' and 'vmon' values
 print(f"vset: {channel.vset}")
 print(f"vmon: {channel.vmon}")
 
 # switch channel off and on
-channel.off()
-channel.on()
+channel.turn_off()
+channel.turn_on()
 
 # set a new value of 'vset'
 channel.vset = 300.0  # 300 V
 ```
```

