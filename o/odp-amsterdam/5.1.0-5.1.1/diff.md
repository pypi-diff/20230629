# Comparing `tmp/odp_amsterdam-5.1.0.tar.gz` & `tmp/odp_amsterdam-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_amsterdam-5.1.0.tar", max compression
+gzip compressed data, was "odp_amsterdam-5.1.1.tar", max compression
```

## Comparing `odp_amsterdam-5.1.0.tar` & `odp_amsterdam-5.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-02-24 02:39:42.438397 odp_amsterdam-5.1.0/LICENSE
--rw-r--r--   0        0        0     9384 2023-02-24 02:39:42.438397 odp_amsterdam-5.1.0/README.md
--rw-r--r--   0        0        0      434 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/__init__.py
--rw-r--r--   0        0        0      469 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/const.py
--rw-r--r--   0        0        0      383 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/exceptions.py
--rw-r--r--   0        0        0     4279 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/models.py
--rw-r--r--   0        0        0     6121 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/odp_amsterdam.py
--rw-r--r--   0        0        0        0 2023-02-24 02:39:42.442397 odp_amsterdam-5.1.0/odp_amsterdam/py.typed
--rw-r--r--   0        0        0     3786 2023-02-24 02:39:58.146397 odp_amsterdam-5.1.0/pyproject.toml
--rw-r--r--   0        0        0    10386 1970-01-01 00:00:00.000000 odp_amsterdam-5.1.0/setup.py
--rw-r--r--   0        0        0    10898 1970-01-01 00:00:00.000000 odp_amsterdam-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-29 19:35:26.069002 odp_amsterdam-5.1.1/LICENSE
+-rw-r--r--   0        0        0     9384 2023-06-29 19:35:26.069002 odp_amsterdam-5.1.1/README.md
+-rw-r--r--   0        0        0     3738 2023-06-29 19:35:43.365161 odp_amsterdam-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/__init__.py
+-rw-r--r--   0        0        0      469 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/const.py
+-rw-r--r--   0        0        0      383 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/exceptions.py
+-rw-r--r--   0        0        0     4528 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/models.py
+-rw-r--r--   0        0        0     6103 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/odp_amsterdam.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:35:26.073002 odp_amsterdam-5.1.1/src/odp_amsterdam/py.typed
+-rw-r--r--   0        0        0    10698 1970-01-01 00:00:00.000000 odp_amsterdam-5.1.1/PKG-INFO
```

### Comparing `odp_amsterdam-5.1.0/LICENSE` & `odp_amsterdam-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odp_amsterdam-5.1.0/README.md` & `odp_amsterdam-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `odp_amsterdam-5.1.0/odp_amsterdam/models.py` & `odp_amsterdam-5.1.1/src/odp_amsterdam/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,30 +22,31 @@
     coordinates: list[float]
 
     @classmethod
     def from_json(cls: type[ParkingSpot], data: dict[str, Any]) -> ParkingSpot:
         """Return ParkingSpot object from a dictionary.
 
         Args:
+        ----
             data: The JSON data from the API.
 
-        Returns
+        Returns:
         -------
             An ParkingSpot object.
         """
         attr = data["properties"]
         regimes = attr["regimes"][0]
         return cls(
             spot_id=attr["id"],
             spot_type=attr["eType"] or None,
             spot_description=regimes["eTypeDescription"] or None,
             street=filter_unknown(attr["straatnaam"]),
             number=int(attr["aantal"]),
             orientation=filter_unknown(attr["type"]),
-            coordinates=data["geometry"]["coordinates"],
+            coordinates=data["geometry"]["coordinates"][0],
         )
 
 
 @dataclass
 class Garage:
     """Object representing an Garage model response from the API."""
 
@@ -61,83 +62,97 @@
     latitude: float
 
     @classmethod
     def from_json(cls: type[Garage], data: dict[str, Any]) -> Garage:
         """Return Garage object from a dictionary.
 
         Args:
+        ----
             data: The JSON data from the API.
 
-        Returns
+        Returns:
         -------
             An Garage object.
         """
         latitude, longitude = split_coordinates(str(data["geometry"]["coordinates"]))
         attr = data["properties"]
         return cls(
             garage_id=data["Id"],
             garage_name=correct_name(data["properties"]["Name"]),
             state=attr.get("State"),
             free_space_short=int(attr["FreeSpaceShort"]),
-            free_space_long=None
-            if attr["FreeSpaceLong"] == ""
-            else int(attr["FreeSpaceLong"]),
+            free_space_long=set_long_parking(attr["FreeSpaceLong"]),
             short_capacity=int(attr["ShortCapacity"]),
-            long_capacity=None
-            if attr["LongCapacity"] == ""
-            else int(attr["LongCapacity"]),
+            long_capacity=set_long_parking(attr["LongCapacity"]),
             availability_pct=calculate_pct(
                 attr.get("FreeSpaceShort"),
                 attr.get("ShortCapacity"),
             ),
             longitude=longitude,
             latitude=latitude,
         )
 
 
+def set_long_parking(data: str) -> int | None:
+    """Set the long parking capacity/free space value.
+
+    Args:
+    ----
+        data: The data to be set.
+
+    Returns:
+    -------
+        The long parking capacity/free space.
+    """
+    return None if not data else int(data)
+
+
 def split_coordinates(data: str) -> tuple[float, float]:
     """Split the coordinate data in separate variables.
 
     Args:
+    ----
         data: The data to be split.
 
-    Returns
+    Returns:
     -------
         The coordinates.
     """
     longitude, latitude = data.split(", ")
     longitude = longitude.replace("[", "")
     latitude = latitude.replace("]", "")
     return float(latitude), float(longitude)
 
 
 def calculate_pct(current: int, total: int) -> float | None:
     """Calculate the percentage of free parking spots.
 
     Args:
+    ----
         current: The current amount of free parking spots.
         total: The total amount of parking spots.
 
-    Returns
+    Returns:
     -------
         The percentage of free parking spots.
     """
     try:
         return round((float(current) / float(total)) * 100, 1)
     except ZeroDivisionError:
         return None
 
 
 def correct_name(name: str) -> str:
     """Change parking garage name for consistency if needed.
 
     Args:
+    ----
         name: The name of the parking garage.
 
-    Returns
+    Returns:
     -------
         The corrected name.
     """
     for value in FILTER_NAMES:
         # Remove parts from name string.
         name = name.replace(value, "")
 
@@ -147,16 +162,17 @@
     return name
 
 
 def filter_unknown(data: str) -> str | None:
     """Filter unknown data from the API.
 
     Args:
+    ----
         data: The data to be filtered.
 
-    Returns
+    Returns:
     -------
         The filtered data.
     """
     if data in FILTER_UNKNOWN:
         return None
     return data
```

### Comparing `odp_amsterdam-5.1.0/odp_amsterdam/odp_amsterdam.py` & `odp_amsterdam-5.1.1/src/odp_amsterdam/odp_amsterdam.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,25 @@
         *,
         method: str = METH_GET,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the Open Data Platform API of Amsterdam.
 
         Args:
+        ----
             uri: Request URI, without '/', for example, 'status'
             method: HTTP method to use, for example, 'GET'
             params: Extra options to improve or limit the response.
 
-        Returns
+        Returns:
         -------
             A Python dictionary (text) with the response from
             the Open Data Platform API of Amsterdam.
 
-        Raises
+        Raises:
         ------
             ODPAmsterdamConnectionError: An error occurred while
                 communicating with the Open Data Platform API of Amsterdam.
             ODPAmsterdamError: Received an unexpected response from
                 the Open Data Platform API of Amsterdam.
         """
         version = metadata.version(__package__)
@@ -79,22 +80,18 @@
                     params=params,
                     headers=headers,
                     ssl=True,
                 )
                 response.raise_for_status()
         except asyncio.TimeoutError as exception:
             msg = "Timeout occurred while connecting to the Open Data Platform API."
-            raise ODPAmsterdamConnectionError(
-                msg,
-            ) from exception
+            raise ODPAmsterdamConnectionError(msg) from exception
         except (ClientError, socket.gaierror) as exception:
             msg = "Error occurred while communicating with the Open Data Platform API."
-            raise ODPAmsterdamConnectionError(
-                msg,
-            ) from exception
+            raise ODPAmsterdamConnectionError(msg) from exception
 
         types = ["application/json", "text/plain", "application/geo+json"]
         content_type = response.headers.get("Content-Type", "")
         if not any(item in content_type for item in types):
             text = await response.text()
             msg = "Unexpected content type response from the Open Data Platform API"
             raise ODPAmsterdamError(
@@ -108,18 +105,19 @@
         self,
         limit: int = 10,
         parking_type: str = "",
     ) -> list[ParkingSpot]:
         """Get all the parking locations.
 
         Args:
+        ----
             limit: The number of results to return.
             parking_type: The selected parking type number.
 
-        Returns
+        Returns:
         -------
             A list of ParkingSpot objects.
         """
         results: list[ParkingSpot] = []
         locations = await self._request(
             "v1/parkeervakken/parkeervakken",
             params={"_pageSize": limit, "eType": parking_type, "_format": "geojson"},
@@ -152,21 +150,22 @@
                 raise ODPAmsterdamError(msg) from exception
         return results
 
     async def garage(self, garage_id: str) -> Garage:
         """Get info from a single parking garage.
 
         Args:
+        ----
             garage_id: The ID of the garage.
 
-        Returns
+        Returns:
         -------
             A garage object.
 
-        Raises
+        Raises:
         ------
             ODPAmsterdamResultsError: When no results are found.
         """
         data = await self._request("dcatd/datasets/9ORkef6T-aU29g/purls/1")
         for item in data["features"]:
             if item["Id"] == garage_id:
                 return Garage.from_json(item)
```

### Comparing `odp_amsterdam-5.1.0/pyproject.toml` & `odp_amsterdam-5.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,132 @@
 [tool.poetry]
 name = "odp-amsterdam"
-version = "5.1.0"
+version = "5.1.1"
 description = "Asynchronous Python client providing Open Data information of Amsterdam"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-odp-amsterdam"
 repository = "https://github.com/klaasnicolaas/python-odp-amsterdam"
 documentation = "https://github.com/klaasnicolaas/python-odp-amsterdam"
 keywords = ["garages", "amsterdam", "car", "occupancy", "async", "client"]
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
-    { include = "odp_amsterdam" }
+  { include = "odp_amsterdam", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-odp-amsterdam/issues"
 Changelog = "https://github.com/klaasnicolaas/python-odp-amsterdam/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.247"
-aresponses = "^2.1.6"
-black = "^22.12"
-blacken-docs = "^1.13.0"
-codespell = "^2.2.2"
-coverage = {version = "^7.1", extras = ["toml"]}
-mypy = "^1.0"
-pre-commit = "^3.0.4"
-pre-commit-hooks = "^4.4.0"
-pylint = "^2.16.1"
-pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
-yamllint = "^1.29.0"
-covdefaults = "^2.2.2"
-
-[tool.black]
-target-version = ['py39']
-
-[tool.coverage.paths]
-source = ["odp_amsterdam"]
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
 source = ["odp_amsterdam"]
 
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
-max-attributes=15
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
+max-attributes = 15
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
 select = ["ALL"]
@@ -146,15 +140,15 @@
 ]
 
 [tool.ruff.flake8-pytest-style]
 mark-parentheses = false
 fixture-parentheses = false
 
 [tool.ruff.isort]
-known-first-party = ["gridnet"]
+known-first-party = ["odp_amsterdam"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `odp_amsterdam-5.1.0/setup.py` & `odp_amsterdam-5.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,263 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: odp-amsterdam
+Version: 5.1.1
+Summary: Asynchronous Python client providing Open Data information of Amsterdam
+Home-page: https://github.com/klaasnicolaas/python-odp-amsterdam
+License: MIT
+Keywords: garages,amsterdam,car,occupancy,async,client
+Author: Klaas Schoute
+Author-email: hello@student-techlife.com
+Maintainer: Klaas Schoute
+Maintainer-email: hello@student-techlife.com
+Requires-Python: >=3.9,<4.0
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.0.0)
+Requires-Dist: yarl (>=1.6.0)
+Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-odp-amsterdam/issues
+Project-URL: Changelog, https://github.com/klaasnicolaas/python-odp-amsterdam/releases
+Project-URL: Documentation, https://github.com/klaasnicolaas/python-odp-amsterdam
+Project-URL: Repository, https://github.com/klaasnicolaas/python-odp-amsterdam
+Description-Content-Type: text/markdown
 
-packages = \
-['odp_amsterdam']
+<!-- Header -->
+![alt Header of the odp Amsterdam package](https://raw.githubusercontent.com/klaasnicolaas/python-odp-amsterdam/main/assets/header_odp_amsterdam-min.png)
 
-package_data = \
-{'': ['*']}
+<!-- PROJECT SHIELDS -->
+[![GitHub Release][releases-shield]][releases]
+[![Python Versions][python-versions-shield]][pypi]
+![Project Stage][project-stage-shield]
+![Project Maintenance][maintenance-shield]
+[![License][license-shield]](LICENSE)
 
-install_requires = \
-['aiohttp>=3.0.0', 'yarl>=1.6.0']
-
-setup_kwargs = {
-    'name': 'odp-amsterdam',
-    'version': '5.1.0',
-    'description': 'Asynchronous Python client providing Open Data information of Amsterdam',
-    'long_description': '<!-- Header -->\n![alt Header of the odp Amsterdam package](https://raw.githubusercontent.com/klaasnicolaas/python-odp-amsterdam/main/assets/header_odp_amsterdam-min.png)\n\n<!-- PROJECT SHIELDS -->\n[![GitHub Release][releases-shield]][releases]\n[![Python Versions][python-versions-shield]][pypi]\n![Project Stage][project-stage-shield]\n![Project Maintenance][maintenance-shield]\n[![License][license-shield]](LICENSE)\n\n[![GitHub Activity][commits-shield]][commits-url]\n[![PyPi Downloads][downloads-shield]][downloads-url]\n[![GitHub Last Commit][last-commit-shield]][commits-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n\n[![Code Quality][code-quality-shield]][code-quality]\n[![Build Status][build-shield]][build-url]\n[![Typing Status][typing-shield]][typing-url]\n\n[![Maintainability][maintainability-shield]][maintainability-url]\n[![Code Coverage][codecov-shield]][codecov-url]\n\nAsynchronous Python client for the open datasets of Amsterdam (The Netherlands).\n\n## About\n\nA python package with which you can retrieve data from the Open Data Platform of Amsterdam via [their API][api]. This package was initially created to only retrieve parking data from the API, but the code base is made in such a way that it is easy to extend for other datasets from the same platform.\n\n## Installation\n\n```bash\npip install odp-amsterdam\n```\n\n## Datasets\n\nYou can read the following datasets with this package:\n\n- [Parking garages occupancy / Garages parkeerbezetting][garages] (53 garages)\n- [Parking locations / Parkeervakken][parking]\n\n<details>\n    <summary>Click here to get more details</summary>\n\n### Parking garages\n\nRead the occupancy of a parking garage in Amsterdam (The Netherlands), both for day visitors (short-term parking) and season ticket holders (long-term parking).\n\n**NOTE**: Not all parking garages have data for long-term parking.\n\n| Variable | Type | Description |\n| :------- | :--- | :---------- |\n| `garage_id` | string | The id of the garage |\n| `garage_name` | string | The name of the garage |\n| `state` | string | The state of the garage (`ok` or `problem`) |\n| `free_space_short` | integer | The number of free spaces for day visitors |\n| `free_space_long` | integer (or None) | The number of free spaces for season ticket holders |\n| `short_capacity` | integer | The total capacity of the garage for day visitors |\n| `long_capacity` | integer (or None) | The total capacity of the garage for season ticket holders |\n| `availability_pct` | float | The percentage of free parking spaces |\n| `longitude` | float | The longitude of the garage |\n| `latitude` | float | The latitude of the garage |\n\n### Parking locations\n\nYou can use the following parameters in your request:\n\n- **limit** (default: 10) - How many results you want to retrieve.\n- **parking_type** (default: "") - Filter based on the `eType` from the geojson data.\n\n| Variable | Type | Description |\n| :------- | :--- | :---------- |\n| `spot_id` | string | The id of the location |\n| `spot_type` | string (or None) | The type of the location (e.g. **E6a**) |\n| `spot_description` | string (or None) | The description of the location type |\n| `street` | string (or None) | The street name of the location |\n| `number` | integer (or None) | How many parking spots there are on this location |\n| `orientation` | string (or None) | The parking orientation of the location (**visgraag**, **langs** or **file**) |\n| `coordinates` | list[float] | The coordinates of the location |\n</details>\n\n## Usage\n\n```python\nimport asyncio\n\nfrom odp_amsterdam import ODPAmsterdam\n\n\nasync def main():\n    """Show example on using the ODP Amsterdam API client."""\n    async with ODPAmsterdam() as client:\n        # Parking locations\n        locations: list[ParkingSpot] = await client.location(\n            limit=5, parking_type="E6a"\n        )\n\n        # Garages\n        all_garages: list[Garage] = await client.all_garages()\n        garage: Garage = await client.garage(garage_id="ID_OF_GARAGE")\n\n        print(locations)\n        print(all_garages)\n        print(garage)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## Use cases\n\n[NIPKaart.nl][nipkaart]\n\nA website that provides insight into where disabled parking spaces are, based on data from users and municipalities. Operates mainly in the Netherlands, but also has plans to process data from abroad.\n\n## Contributing\n\nThis is an active open-source project. We are always open to people who want to\nuse the code or contribute to it.\n\nWe\'ve set up a separate document for our\n[contribution guidelines](CONTRIBUTING.md).\n\nThank you for being involved! :heart_eyes:\n\n## Setting up development environment\n\nThis Python project is fully managed using the [Poetry][poetry] dependency\nmanager.\n\nYou need at least:\n\n- Python 3.9+\n- [Poetry][poetry-install]\n\nInstall all packages, including all development requirements:\n\n```bash\npoetry install\n```\n\nPoetry creates by default an virtual environment where it installs all\nnecessary pip packages, to enter or exit the venv run the following commands:\n\n```bash\npoetry shell\nexit\n```\n\nSetup the pre-commit check, you must run this inside the virtual environment:\n\n```bash\npre-commit install\n```\n\n*Now you\'re all set to get started!*\n\nAs this repository uses the [pre-commit][pre-commit] framework, all changes\nare linted and tested with each commit. You can run all checks and tests\nmanually, using the following command:\n\n```bash\npoetry run pre-commit run --all-files\n```\n\nTo run just the Python tests:\n\n```bash\npoetry run pytest\n```\n\n## License\n\nMIT License\n\nCopyright (c) 2020-2023 Klaas Schoute\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n[api]: https://api.data.amsterdam.nl\n[nipkaart]: https://www.nipkaart.nl\n[garages]: https://data.amsterdam.nl/datasets/9ORkef6T-aU29g/actuele-beschikbaarheid-parkeergarages/\n[parking]: https://api.data.amsterdam.nl/v1/docs/datasets/parkeervakken.html\n\n<!-- MARKDOWN LINKS & IMAGES -->\n[build-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/tests.yaml/badge.svg\n[build-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/tests.yaml\n[code-quality-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/codeql.yaml/badge.svg\n[code-quality]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/codeql.yaml\n[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-odp-amsterdam.svg\n[commits-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/commits/main\n[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-odp-amsterdam/branch/main/graph/badge.svg?token=F6CE1S25NV\n[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-odp-amsterdam\n[downloads-shield]: https://img.shields.io/pypi/dm/odp-amsterdam\n[downloads-url]: https://pypistats.org/packages/odp-amsterdam\n[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-odp-amsterdam.svg\n[issues-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/issues\n[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-odp-amsterdam.svg\n[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-odp-amsterdam.svg\n[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg\n[maintainability-shield]: https://api.codeclimate.com/v1/badges/72d6baa9151bb0b0cfdf/maintainability\n[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-odp-amsterdam/maintainability\n[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg\n[pypi]: https://pypi.org/project/odp-amsterdam/\n[python-versions-shield]: https://img.shields.io/pypi/pyversions/odp-amsterdam\n[typing-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/typing.yaml/badge.svg\n[typing-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/typing.yaml\n[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-odp-amsterdam.svg\n[releases]: https://github.com/klaasnicolaas/python-odp-amsterdam/releases\n[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-odp-amsterdam.svg\n[stars-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/stargazers\n\n[poetry-install]: https://python-poetry.org/docs/#installation\n[poetry]: https://python-poetry.org\n[pre-commit]: https://pre-commit.com\n',
-    'author': 'Klaas Schoute',
-    'author_email': 'hello@student-techlife.com',
-    'maintainer': 'Klaas Schoute',
-    'maintainer_email': 'hello@student-techlife.com',
-    'url': 'https://github.com/klaasnicolaas/python-odp-amsterdam',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+[![GitHub Activity][commits-shield]][commits-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
+[![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
 
+[![Code Quality][code-quality-shield]][code-quality]
+[![Build Status][build-shield]][build-url]
+[![Typing Status][typing-shield]][typing-url]
+
+[![Maintainability][maintainability-shield]][maintainability-url]
+[![Code Coverage][codecov-shield]][codecov-url]
+
+Asynchronous Python client for the open datasets of Amsterdam (The Netherlands).
+
+## About
+
+A python package with which you can retrieve data from the Open Data Platform of Amsterdam via [their API][api]. This package was initially created to only retrieve parking data from the API, but the code base is made in such a way that it is easy to extend for other datasets from the same platform.
+
+## Installation
+
+```bash
+pip install odp-amsterdam
+```
+
+## Datasets
+
+You can read the following datasets with this package:
+
+- [Parking garages occupancy / Garages parkeerbezetting][garages] (53 garages)
+- [Parking locations / Parkeervakken][parking]
+
+<details>
+    <summary>Click here to get more details</summary>
+
+### Parking garages
+
+Read the occupancy of a parking garage in Amsterdam (The Netherlands), both for day visitors (short-term parking) and season ticket holders (long-term parking).
+
+**NOTE**: Not all parking garages have data for long-term parking.
+
+| Variable | Type | Description |
+| :------- | :--- | :---------- |
+| `garage_id` | string | The id of the garage |
+| `garage_name` | string | The name of the garage |
+| `state` | string | The state of the garage (`ok` or `problem`) |
+| `free_space_short` | integer | The number of free spaces for day visitors |
+| `free_space_long` | integer (or None) | The number of free spaces for season ticket holders |
+| `short_capacity` | integer | The total capacity of the garage for day visitors |
+| `long_capacity` | integer (or None) | The total capacity of the garage for season ticket holders |
+| `availability_pct` | float | The percentage of free parking spaces |
+| `longitude` | float | The longitude of the garage |
+| `latitude` | float | The latitude of the garage |
+
+### Parking locations
+
+You can use the following parameters in your request:
+
+- **limit** (default: 10) - How many results you want to retrieve.
+- **parking_type** (default: "") - Filter based on the `eType` from the geojson data.
+
+| Variable | Type | Description |
+| :------- | :--- | :---------- |
+| `spot_id` | string | The id of the location |
+| `spot_type` | string (or None) | The type of the location (e.g. **E6a**) |
+| `spot_description` | string (or None) | The description of the location type |
+| `street` | string (or None) | The street name of the location |
+| `number` | integer (or None) | How many parking spots there are on this location |
+| `orientation` | string (or None) | The parking orientation of the location (**visgraag**, **langs** or **file**) |
+| `coordinates` | list[float] | The coordinates of the location |
+</details>
+
+## Usage
+
+```python
+import asyncio
+
+from odp_amsterdam import ODPAmsterdam
+
+
+async def main():
+    """Show example on using the ODP Amsterdam API client."""
+    async with ODPAmsterdam() as client:
+        # Parking locations
+        locations: list[ParkingSpot] = await client.location(
+            limit=5, parking_type="E6a"
+        )
+
+        # Garages
+        all_garages: list[Garage] = await client.all_garages()
+        garage: Garage = await client.garage(garage_id="ID_OF_GARAGE")
+
+        print(locations)
+        print(all_garages)
+        print(garage)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+## Use cases
+
+[NIPKaart.nl][nipkaart]
+
+A website that provides insight into where disabled parking spaces are, based on data from users and municipalities. Operates mainly in the Netherlands, but also has plans to process data from abroad.
+
+## Contributing
+
+This is an active open-source project. We are always open to people who want to
+use the code or contribute to it.
+
+We've set up a separate document for our
+[contribution guidelines](CONTRIBUTING.md).
+
+Thank you for being involved! :heart_eyes:
+
+## Setting up development environment
+
+This Python project is fully managed using the [Poetry][poetry] dependency
+manager.
+
+You need at least:
+
+- Python 3.9+
+- [Poetry][poetry-install]
+
+Install all packages, including all development requirements:
+
+```bash
+poetry install
+```
+
+Poetry creates by default an virtual environment where it installs all
+necessary pip packages, to enter or exit the venv run the following commands:
+
+```bash
+poetry shell
+exit
+```
+
+Setup the pre-commit check, you must run this inside the virtual environment:
+
+```bash
+pre-commit install
+```
+
+*Now you're all set to get started!*
+
+As this repository uses the [pre-commit][pre-commit] framework, all changes
+are linted and tested with each commit. You can run all checks and tests
+manually, using the following command:
+
+```bash
+poetry run pre-commit run --all-files
+```
+
+To run just the Python tests:
+
+```bash
+poetry run pytest
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2020-2023 Klaas Schoute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+[api]: https://api.data.amsterdam.nl
+[nipkaart]: https://www.nipkaart.nl
+[garages]: https://data.amsterdam.nl/datasets/9ORkef6T-aU29g/actuele-beschikbaarheid-parkeergarages/
+[parking]: https://api.data.amsterdam.nl/v1/docs/datasets/parkeervakken.html
+
+<!-- MARKDOWN LINKS & IMAGES -->
+[build-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/tests.yaml/badge.svg
+[build-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/tests.yaml
+[code-quality-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/codeql.yaml/badge.svg
+[code-quality]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/codeql.yaml
+[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-odp-amsterdam.svg
+[commits-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/commits/main
+[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-odp-amsterdam/branch/main/graph/badge.svg?token=F6CE1S25NV
+[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-odp-amsterdam
+[downloads-shield]: https://img.shields.io/pypi/dm/odp-amsterdam
+[downloads-url]: https://pypistats.org/packages/odp-amsterdam
+[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-odp-amsterdam.svg
+[issues-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/issues
+[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-odp-amsterdam.svg
+[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-odp-amsterdam.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintainability-shield]: https://api.codeclimate.com/v1/badges/72d6baa9151bb0b0cfdf/maintainability
+[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-odp-amsterdam/maintainability
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
+[pypi]: https://pypi.org/project/odp-amsterdam/
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/odp-amsterdam
+[typing-shield]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/typing.yaml/badge.svg
+[typing-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/actions/workflows/typing.yaml
+[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-odp-amsterdam.svg
+[releases]: https://github.com/klaasnicolaas/python-odp-amsterdam/releases
+[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-odp-amsterdam.svg
+[stars-url]: https://github.com/klaasnicolaas/python-odp-amsterdam/stargazers
+
+[poetry-install]: https://python-poetry.org/docs/#installation
+[poetry]: https://python-poetry.org
+[pre-commit]: https://pre-commit.com
 
-setup(**setup_kwargs)
```

