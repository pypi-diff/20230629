# Comparing `tmp/dusseldorf-0.2.0.tar.gz` & `tmp/dusseldorf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dusseldorf-0.2.0.tar", max compression
+gzip compressed data, was "dusseldorf-1.0.0.tar", max compression
```

## Comparing `dusseldorf-0.2.0.tar` & `dusseldorf-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/LICENSE
--rw-r--r--   0        0        0     9344 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/README.md
--rw-r--r--   0        0        0      403 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/dusseldorf/__init__.py
--rw-r--r--   0        0        0     5835 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/dusseldorf/dusseldorf.py
--rw-r--r--   0        0        0      296 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/dusseldorf/exceptions.py
--rw-r--r--   0        0        0     3181 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/dusseldorf/models.py
--rw-r--r--   0        0        0        0 2023-03-21 01:41:56.057065 dusseldorf-0.2.0/dusseldorf/py.typed
--rw-r--r--   0        0        0     3800 2023-03-21 01:42:15.521499 dusseldorf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10846 1970-01-01 00:00:00.000000 dusseldorf-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9426 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/README.md
+-rw-r--r--   0        0        0     3720 2023-06-29 11:54:27.066524 dusseldorf-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      403 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/src/dusseldorf/__init__.py
+-rw-r--r--   0        0        0     5959 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/src/dusseldorf/dusseldorf.py
+-rw-r--r--   0        0        0      296 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/src/dusseldorf/exceptions.py
+-rw-r--r--   0        0        0     3436 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/src/dusseldorf/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:54:06.870341 dusseldorf-1.0.0/src/dusseldorf/py.typed
+-rw-r--r--   0        0        0    10728 1970-01-01 00:00:00.000000 dusseldorf-1.0.0/PKG-INFO
```

### Comparing `dusseldorf-0.2.0/LICENSE` & `dusseldorf-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dusseldorf-0.2.0/README.md` & `dusseldorf-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,23 @@
 <details>
     <summary>Click here to get more details</summary>
 
 ### Disabled parking spaces
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
-| `entry_id` | integer | The ID of the parking spot |
-| `name` | string | The name of the parking spot |
+| `entry_id` | string | The ID of the parking spot |
 | `number` | integer | The number of parking spots on this location |
 | `address` | string | The address of the parking spot |
+| `district` | string | The district location of the parking spot |
 | `time_limit` | string | Some locations have window times where the location is only specific for disabled parking, outside these times everyone is allowed to park there |
 | `note` | string | Some locations have a note about the parking spot |
 | `longitude` | float | The longitude of the parking spot |
 | `latitude` | float | The latitude of the parking spot |
+| `last_update` | datetime | The last time the data was updated |
 
 ### Park and Rides
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `entry_id` | integer | The ID of the park and ride |
 | `name` | string | The name of the park and ride |
```

### Comparing `dusseldorf-0.2.0/dusseldorf/dusseldorf.py` & `dusseldorf-1.0.0/src/dusseldorf/dusseldorf.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,20 @@
     """Main class for handling data fetchting from Open Data Platform of Dusseldorf."""
 
     request_timeout: float = 10.0
     session: ClientSession | None = None
 
     _close_session: bool = False
 
-    async def _request(
+    async def _request(  # noqa: PLR0913
         self,
         uri: str,
         *,
+        host: str = "opendata.duesseldorf.de",
+        path: str = "/api/action/datastore/",
         method: str = hdrs.METH_GET,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the Open Data Platform API of Dusseldorf.
 
         Args:
         ----
@@ -49,16 +51,16 @@
             ODPDusseldorfConnectionError: Timeout occurred while
                 connecting to the Open Data Platform API.
             ODPDusseldorfError: If the data is not valid.
         """
         version = metadata.version(__package__)
         url = URL.build(
             scheme="https",
-            host="opendata.duesseldorf.de",
-            path="/api/action/datastore/",
+            host=host,
+            path=path,
         ).join(URL(uri))
 
         headers = {
             "Accept": "application/json",
             "User-Agent": f"PythonODPDusseldorf/{version}",
         }
 
@@ -94,34 +96,34 @@
             raise ODPDusseldorfError(
                 msg,
                 {"Content-Type": content_type, "Response": text},
             )
 
         return cast(dict[str, Any], await response.json())
 
-    async def disabled_parkings(self, limit: int = 10) -> list[DisabledParking]:
+    async def disabled_parkings(self) -> list[DisabledParking]:
         """Get list of disabled parkings.
 
-        Args:
-        ----
-            limit: Maximum number of disabled parkings to return.
-
-        Returns:
+        Returns
         -------
             A list of disabled parking objects.
         """
         results: list[DisabledParking] = []
         locations = await self._request(
-            "search.json",
+            host="maps.duesseldorf.de",
+            path="/services/verkehr/wfs",
+            uri="wfs",
             params={
-                "resource_id": "995914c7-4275-49c4-8441-426722336c3a",
-                "limit": limit,
+                "request": "GetFeature",
+                "typeName": "verkehr:behindertenparkplatz",
+                "outputFormat": "application/json",
+                "srsName": "EPSG:4326",
             },
         )
-        for item in locations["result"]["records"]:
+        for item in locations["features"]:
             results.append(DisabledParking.from_dict(item))
         return results
 
     async def garages(self, limit: int = 10) -> list[Garage]:
         """Get list of garages.
 
         Args:
@@ -130,15 +132,15 @@
 
         Returns:
         -------
             A list of garage objects.
         """
         results: list[Garage] = []
         locations = await self._request(
-            "search.json",
+            uri="search.json",
             params={
                 "resource_id": "53d63e70-0ed4-4175-9924-c45530d5bf29",
                 "limit": limit,
             },
         )
         for item in locations["result"]["records"]:
             results.append(Garage.from_dict(item))
@@ -153,15 +155,15 @@
 
         Returns:
         -------
             A list of park and ride objects.
         """
         results: list[ParkAndRide] = []
         locations = await self._request(
-            "search.json",
+            uri="search.json",
             params={
                 "resource_id": "1fd5b3f3-ea03-4922-9fae-3577fbc9f78a",
                 "limit": limit,
             },
         )
         for item in locations["result"]["records"]:
             results.append(ParkAndRide.from_dict(item))
```

### Comparing `dusseldorf-0.2.0/dusseldorf/models.py` & `dusseldorf-1.0.0/src/dusseldorf/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Models for Open Data Platform of Dusseldorf."""
 from __future__ import annotations
 
 from dataclasses import dataclass
+from datetime import datetime
 from typing import Any
 
 
 @dataclass
 class ParkAndRide:
     """Object representing a ParkAndRide."""
 
@@ -45,47 +46,52 @@
         )
 
 
 @dataclass
 class DisabledParking:
     """Object representing a DisabledParking."""
 
-    entry_id: int
-    name: str
+    entry_id: str
     number: int
     address: str
+    district: str
     time_limit: str | None
     note: str | None
+
     longitude: float
     latitude: float
+    last_update: datetime
 
     @classmethod
     def from_dict(cls: type[DisabledParking], data: dict[str, Any]) -> DisabledParking:
         """Return a DisabledParking object from a dictionary.
 
         Args:
         ----
             data: The data from the API.
 
         Returns:
         -------
             A DisabledParking object.
         """
+        attr = data["properties"]
+        coordinates = data["geometry"]["coordinates"]
         return cls(
-            entry_id=int(data["entry_id"]),
-            name=data["name"],
-            number=int(data["anzahl"]),
-            address=set_address(
-                data["strasse"],
-                data["hausnr"],
-            ),
-            time_limit=data.get("zeitbegrenzung") or None,
-            note=data.get("bemerkung") or None,
-            longitude=float(data["longitude"]),
-            latitude=float(data["latitude"]),
+            entry_id=data["id"].replace("behindertenparkplatz.", ""),
+            number=int(attr["anzahl"][:2]),
+            address=attr["adresse"].strip(),
+            district=attr["stadtteil"],
+            time_limit=attr.get("zeitbegrenzung") or None,
+            note=attr.get("beschreibung") or None,
+            longitude=float(coordinates[0]),
+            latitude=float(coordinates[1]),
+            last_update=datetime.strptime(
+                attr["_last_update"],
+                "%Y-%m-%d",
+            ).astimezone(),
         )
 
 
 @dataclass
 class Garage:
     """Object representing a Garage."""
```

### Comparing `dusseldorf-0.2.0/pyproject.toml` & `dusseldorf-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,132 @@
 [tool.poetry]
 name = "dusseldorf"
-version = "0.2.0"
+version = "1.0.0"
 description = "Asynchronous Python client providing Open Data information of dusseldorf"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-dusseldorf"
 repository = "https://github.com/klaasnicolaas/python-dusseldorf"
 documentation = "https://github.com/klaasnicolaas/python-dusseldorf"
 keywords = ["data", "platform", "dusseldorf", "parking", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "dusseldorf" }
+  { include = "dusseldorf", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-dusseldorf/issues"
 Changelog = "https://github.com/klaasnicolaas/python-dusseldorf/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.258"
-aresponses = "^2.1.6"
-black = ">=22.10,<24.0"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.4"
-coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.2"
-pre-commit = "^3.1.1"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.17.0"
-pytest = "^7.2.2"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.3.0"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["dusseldorf"]
+ruff = "0.0.275"
+aresponses = "2.1.6"
+black = "23.3.0"
+blacken-docs = "1.14.0"
+codespell = "2.2.5"
+coverage = {version = "7.2.7", extras = ["toml"]}
+mypy = "1.4.1"
+pre-commit = "3.3.3"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.1.0"
+yamllint = "1.32.0"
+covdefaults = "2.3.0"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["dusseldorf"]
 
+[tool.coverage.report]
+fail_under = 90
+show_missing = true
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.9"
 
+# flake8-mypy expects the two following for sensible formatting
+show_column_numbers = true
+
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_defs = true
 disallow_untyped_decorators = true
+disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.pylint.MASTER]
-extension-pkg-whitelist = [
-  "pydantic"
-]
-ignore= [
-  "tests"
-]
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "vw",
 ]
 
-[tool.pylint.DESIGN]
-max-attributes=20
-
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
+
+[tool.pylint.DESIGN]
+max-attributes = 20
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -152,9 +146,9 @@
 [tool.ruff.isort]
 known-first-party = ["dusseldorf"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `dusseldorf-0.2.0/PKG-INFO` & `dusseldorf-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dusseldorf
-Version: 0.2.0
+Version: 1.0.0
 Summary: Asynchronous Python client providing Open Data information of dusseldorf
 Home-page: https://github.com/klaasnicolaas/python-dusseldorf
 License: MIT
 Keywords: data,platform,dusseldorf,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -14,18 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-dusseldorf/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-dusseldorf/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-dusseldorf
 Project-URL: Repository, https://github.com/klaasnicolaas/python-dusseldorf
@@ -81,22 +77,23 @@
 <details>
     <summary>Click here to get more details</summary>
 
 ### Disabled parking spaces
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
-| `entry_id` | integer | The ID of the parking spot |
-| `name` | string | The name of the parking spot |
+| `entry_id` | string | The ID of the parking spot |
 | `number` | integer | The number of parking spots on this location |
 | `address` | string | The address of the parking spot |
+| `district` | string | The district location of the parking spot |
 | `time_limit` | string | Some locations have window times where the location is only specific for disabled parking, outside these times everyone is allowed to park there |
 | `note` | string | Some locations have a note about the parking spot |
 | `longitude` | float | The longitude of the parking spot |
 | `latitude` | float | The latitude of the parking spot |
+| `last_update` | datetime | The last time the data was updated |
 
 ### Park and Rides
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `entry_id` | integer | The ID of the park and ride |
 | `name` | string | The name of the park and ride |
```

