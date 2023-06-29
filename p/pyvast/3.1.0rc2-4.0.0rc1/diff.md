# Comparing `tmp/pyvast-3.1.0rc2.tar.gz` & `tmp/pyvast-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvast-3.1.0rc2.tar", max compression
+gzip compressed data, was "pyvast-4.0.0rc1.tar", max compression
```

## Comparing `pyvast-3.1.0rc2.tar` & `pyvast-4.0.0rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1846 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/README.md
--rw-r--r--   0        0        0     1521 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0       75 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/__init__.py
--rw-r--r--   0        0        0     5812 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/apps/thehive.py
--rw-r--r--   0        0        0     7825 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/utils/arrow.py
--rw-r--r--   0        0        0     2058 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/utils/asyncio.py
--rw-r--r--   0        0        0      736 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/utils/config.py
--rw-r--r--   0        0        0     1925 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/utils/logging.py
--rw-r--r--   0        0        0       70 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/vast/__init__.py
--rw-r--r--   0        0        0     2879 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/vast/cli.py
--rw-r--r--   0        0        0     3637 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/vast/convert.py
--rw-r--r--   0        0        0     6119 2023-05-11 20:49:10.905606 pyvast-3.1.0rc2/pyvast/vast/vast.py
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 pyvast-3.1.0rc2/setup.py
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 pyvast-3.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1846 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/README.md
+-rw-r--r--   0        0        0     1524 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/__init__.py
+-rw-r--r--   0        0        0     5814 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/apps/thehive.py
+-rw-r--r--   0        0        0     7461 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/utils/arrow.py
+-rw-r--r--   0        0        0     2058 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/utils/asyncio.py
+-rw-r--r--   0        0        0      736 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/utils/config.py
+-rw-r--r--   0        0        0     1925 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/utils/logging.py
+-rw-r--r--   0        0        0       70 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/vast/__init__.py
+-rw-r--r--   0        0        0     2879 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/vast/cli.py
+-rw-r--r--   0        0        0     3637 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/vast/convert.py
+-rw-r--r--   0        0        0     6121 2023-06-29 08:13:21.230663 pyvast-4.0.0rc1/pyvast/vast/vast.py
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 pyvast-4.0.0rc1/setup.py
+-rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 pyvast-4.0.0rc1/PKG-INFO
```

### Comparing `pyvast-3.1.0rc2/README.md` & `pyvast-4.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyproject.toml` & `pyvast-4.0.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvast"
-version = "3.1.0-rc2"
+version = "4.0.0-rc1"
 description = "A security telemetry engine for detection and response"
 authors = ["Tenzir <engineering@tenzir.com>"]
 maintainers = ["Tenzir <engineering@tenzir.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -25,15 +25,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8"
 coloredlogs = "^15.0"
 dynaconf = "^3.1"
 numpy = "^1.24"
 pandas = ">=1.5,<3.0"
-pyarrow = "^11.0"
+pyarrow = ">=11,<13"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 pytest-asyncio = "^0.21.0"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto" # required for async fixtures
```

### Comparing `pyvast-3.1.0rc2/pyvast/apps/thehive.py` & `pyvast-4.0.0rc1/pyvast/apps/thehive.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             raise e
 
 
 async def run_async():
     vast_cli = VAST()
     await vast_cli.status(60, retry_delay=1)
     await wait_for_thehive("/api/v1/user/current", 180)
-    expr = '#type == "suricata.alert"'
+    expr = '#schema == "suricata.alert"'
     # We don't use "UNIFIED" to specify a limit on the HISTORICAL backfill
     logger.info("Starting retro filling...")
     hist_iter = vast_cli.export(expr, ExportMode.HISTORICAL, limit=BACKFILL_LIMIT)
     async for row in to_json_rows(hist_iter):
         await on_suricata_alert(row.data)
     logger.info("Starting live forwarding...")
     cont_iter = vast_cli.export(expr, ExportMode.CONTINUOUS)
```

### Comparing `pyvast-3.1.0rc2/pyvast/utils/arrow.py` & `pyvast-4.0.0rc1/pyvast/utils/arrow.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 
 class IPScalar(pa.ExtensionScalar):
     def as_py(self) -> ip.IPv4Address | ip.IPv6Address | None:
         return None if self.value is None else unpack_ip(self.value.as_py())
 
 
 class IPType(pa.ExtensionType):
-    # NOTE: The identifier for the extension type of VAST's ip type has not
-    # changed when the type was renamed from address to ip because that would be
-    # a breaking change. This is fixable by registering two separate extension
-    # types with the same functionality but different ids, but that's a lot of
-    # effort for something users don't usually see.
-    ext_name = "vast.address"
+    ext_name = "tenzir.ip"
     ext_type = pa.binary(16)
 
     def __init__(self):
         pa.ExtensionType.__init__(self, self.ext_type, self.ext_name)
 
     def __arrow_ext_serialize__(self) -> bytes:
         return self.ext_name.encode()
@@ -46,15 +41,15 @@
         length = self.value[1].as_py()
         if address is None or length is None:
             return None
         return ip.ip_network((address, length), strict=False)
 
 
 class SubnetType(pa.ExtensionType):
-    ext_name = "vast.subnet"
+    ext_name = "tenzir.subnet"
     ext_type = pa.struct([("address", IPType()), ("length", pa.uint8())])
 
     def __init__(self):
         pa.ExtensionType.__init__(self, self.ext_type, self.ext_name)
 
     def __arrow_ext_serialize__(self) -> bytes:
         return self.ext_name.encode()
@@ -86,15 +81,15 @@
     underlying integer type of represented the enum."""
 
     # VAST's flatbuffer type representation uses a 32-bit unsigned integer. We
     # use an 8-bit type here only for backwards compatibility to the legacy
     # type. Eventually this will be a 32-bit type as well.
     DICTIONARY_INDEX_TYPE = pa.uint8()
 
-    ext_name = "vast.enumeration"
+    ext_name = "tenzir.enumeration"
     ext_type = pa.dictionary(DICTIONARY_INDEX_TYPE, pa.string())
 
     def __init__(self, fields: dict[str, int]):
         self._fields = fields
         pa.ExtensionType.__init__(self, self.ext_type, self.ext_name)
 
     @property
@@ -116,15 +111,15 @@
 
     def __arrow_ext_scalar_class__(self):
         return EnumScalar
 
 
 def names(schema: pa.Schema):
     meta = schema.metadata
-    return [meta[key].decode() for key in meta if key.startswith(b"VAST:name:")]
+    return [meta[key].decode() for key in meta if key.startswith(b"TENZIR:name:")]
 
 
 def name(schema: pa.Schema):
     xs = names(schema)
     return xs[0] if xs[0] else ""
```

### Comparing `pyvast-3.1.0rc2/pyvast/utils/asyncio.py` & `pyvast-4.0.0rc1/pyvast/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyvast/utils/config.py` & `pyvast-4.0.0rc1/pyvast/utils/config.py`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyvast/utils/logging.py` & `pyvast-4.0.0rc1/pyvast/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyvast/vast/cli.py` & `pyvast-4.0.0rc1/pyvast/vast/cli.py`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyvast/vast/convert.py` & `pyvast-4.0.0rc1/pyvast/vast/convert.py`

 * *Files identical despite different names*

### Comparing `pyvast-3.1.0rc2/pyvast/vast/vast.py` & `pyvast-4.0.0rc1/pyvast/vast/vast.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,27 +156,27 @@
         start = time.time()
         while True:
             proc = await self.cli.status(**kwargs).exec()
             stdout, stderr = await proc.communicate()
             logger.debug(stderr.decode())
             if proc.returncode == 0:
                 result = json.loads(stdout.decode("utf-8"))
-                assert isinstance(result, dict), 'Argument of wrong type!'
+                assert isinstance(result, dict), "Argument of wrong type!"
                 return result
             else:
                 duration = time.time() - start
                 if duration > timeout:
                     msg = f"VAST status failed with code {proc.returncode}"
                     raise Exception(msg)
                 await asyncio.sleep(retry_delay)
 
     async def count(self, *args, **kwargs) -> int:
         """
         Executes the VAST count command and return the response number.
-        Examples: `count()`, `count("#type == /suricata.alert/", estimate=True)`.
+        Examples: `count()`, `count("#schema == /suricata.alert/", estimate=True)`.
         """
         proc = await self.cli.count(*args, **kwargs).exec()
         stdout, stderr = await proc.communicate()
         logger.debug(stderr.decode())
         if proc.returncode != 0:
             msg = f"VAST count failed with code {proc.returncode}"
             raise Exception(msg)
```

### Comparing `pyvast-3.1.0rc2/setup.py` & `pyvast-4.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 {'': ['*']}
 
 install_requires = \
 ['coloredlogs>=15.0,<16.0',
  'dynaconf>=3.1,<4.0',
  'numpy>=1.24,<2.0',
  'pandas>=1.5,<3.0',
- 'pyarrow>=11.0,<12.0']
+ 'pyarrow>=11,<13']
 
 extras_require = \
 {':extra == "thehive"': ['aiohttp>=3.8,<4.0']}
 
 entry_points = \
 {'console_scripts': ['app-thehive-count-alerts = '
                      'pyvast.apps.thehive:count_alerts',
                      'app-thehive-run = pyvast.apps.thehive:run']}
 
 setup_kwargs = {
     'name': 'pyvast',
-    'version': '3.1.0rc2',
+    'version': '4.0.0rc1',
     'description': 'A security telemetry engine for detection and response',
     'long_description': '# VAST Python\n\nThe Python package of VAST provides a flexible control plane to integrate VAST\nwith other security tools.\n\n> **Note**\n> The Python effort is still highly experimental and subject to rapid change.\n> Please do not consider it for production use.\n\n## Usage\n\nTo get started, clone the VAST repository and install the Python package via\n[Poetry](https://python-poetry.org/docs/):\n\n```bash\ngit clone https://github.com/tenzir/vast.git\ncd vast/python\npoetry install\n```\n\n## Development\n\nWe recommend that you work with an editable installation, which is the default\nfor `poetry install`.\n\n### Unit Tests\n\nRun the unit tests via pytest:\n\n```bash\npoetry run pytest\n```\n\n### Integration Tests\n\nRun the integrations tests via Docker Compose and pytest:\n\n```bash\n./docker-poetry-run.sh pytest -v\n```\n\n## Packaging\n\nThe following instructions concern maintainers who want to publish the Python\npackage to PyPI.\n\n> **Note**\n> Our releasing scripts and CI run these steps automatically. You do not need to\n> intervene anywhere. The instructions below merely document the steps taken.\n\n### Bump the version\n\nPrior to releasing a new version, bump the version, e.g.:\n\n```bash\npoetry version 2.3.1\n```\n\nThis updates the `pyproject.toml` file.\n\n### Publish to Test PyPI\n\n1. Add a Test PyPi repository:\n\n   ```bash\n   poetry config repositories.test-pypi https://test.pypi.org/legacy/\n   ```\n\n2. Get the token from <https://test.pypi.org/manage/account/token/>.\n\n3. Store the token:\n\n  ```bash\n  poetry config pypi-token.test-pypi pypi-XXXXXXXX\n  ```\n\n4. Publish:\n  \n   ```bash\n   poetry publish --build -r test-pypi\n   ```\n\n### Publish to PyPI\n\n1. Get the token from <https://pypi.org/manage/account/token/>.\n\n2. Store the token:\n\n  ```bash\n  poetry config pypi-token.pypi pypi-XXXXXXXX\n  ```\n\n3. Publish\n\n   ```bash\n   poetry publish --build\n   ```\n',
     'author': 'Tenzir',
     'author_email': 'engineering@tenzir.com',
     'maintainer': 'Tenzir',
     'maintainer_email': 'engineering@tenzir.com',
     'url': 'https://vast.io',
```

### Comparing `pyvast-3.1.0rc2/PKG-INFO` & `pyvast-4.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvast
-Version: 3.1.0rc2
+Version: 4.0.0rc1
 Summary: A security telemetry engine for detection and response
 Home-page: https://vast.io
 License: BSD-3-Clause
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Maintainer: Tenzir
 Maintainer-email: engineering@tenzir.com
@@ -24,15 +24,15 @@
 Classifier: Topic :: System :: Distributed Computing
 Provides-Extra: thehive
 Requires-Dist: aiohttp (>=3.8,<4.0) ; extra == "thehive"
 Requires-Dist: coloredlogs (>=15.0,<16.0)
 Requires-Dist: dynaconf (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: pandas (>=1.5,<3.0)
-Requires-Dist: pyarrow (>=11.0,<12.0)
+Requires-Dist: pyarrow (>=11,<13)
 Project-URL: Documentation, https://vast.io/docs
 Project-URL: Repository, https://github.com/tenzir/vast
 Description-Content-Type: text/markdown
 
 # VAST Python
 
 The Python package of VAST provides a flexible control plane to integrate VAST
```

