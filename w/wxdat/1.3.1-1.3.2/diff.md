# Comparing `tmp/wxdat-1.3.1.tar.gz` & `tmp/wxdat-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxdat-1.3.1.tar", max compression
+gzip compressed data, was "wxdat-1.3.2.tar", max compression
```

## Comparing `wxdat-1.3.1.tar` & `wxdat-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.3.1/LICENSE
--rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.3.1/README.md
--rw-r--r--   0        0        0      663 2023-06-29 19:14:59.106276 wxdat-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.3.1/src/wxdat/__init__.py
--rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.3.1/src/wxdat/__main__.py
--rw-r--r--   0        0        0     5932 2023-06-29 18:55:36.438028 wxdat-1.3.1/src/wxdat/config.py
--rw-r--r--   0        0        0     3711 2023-06-29 18:58:07.039970 wxdat-1.3.1/src/wxdat/database.py
--rw-r--r--   0        0        0     6276 2023-06-29 18:58:07.040077 wxdat-1.3.1/src/wxdat/metrics.py
--rw-r--r--   0        0        0     6892 2023-06-29 18:54:36.448538 wxdat-1.3.1/src/wxdat/providers/__init__.py
--rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.3.1/src/wxdat/providers/accuweather.py
--rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.3.1/src/wxdat/providers/ambientwx.py
--rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.3.1/src/wxdat/providers/noaa.py
--rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.3.1/src/wxdat/providers/openweather.py
--rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.3.1/src/wxdat/providers/wunderground.py
--rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.3.1/src/wxdat/units/__init__.py
--rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.3.1/src/wxdat/units/distance.py
--rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.3.1/src/wxdat/units/pressure.py
--rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.3.1/src/wxdat/units/quantity.py
--rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.3.1/src/wxdat/units/rate.py
--rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.3.1/src/wxdat/units/temperature.py
--rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.3.1/src/wxdat/units/velocity.py
--rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.3.1/src/wxdat/units/volume.py
--rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.3.1/src/wxdat/units/weight.py
--rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.3.1/src/wxdat/version.py
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 wxdat-1.3.1/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 wxdat-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.3.2/README.md
+-rw-r--r--   0        0        0      663 2023-06-29 19:32:20.115373 wxdat-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.3.2/src/wxdat/__init__.py
+-rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.3.2/src/wxdat/__main__.py
+-rw-r--r--   0        0        0     5932 2023-06-29 18:55:36.438028 wxdat-1.3.2/src/wxdat/config.py
+-rw-r--r--   0        0        0     3711 2023-06-29 18:58:07.039970 wxdat-1.3.2/src/wxdat/database.py
+-rw-r--r--   0        0        0     6284 2023-06-29 19:32:11.280557 wxdat-1.3.2/src/wxdat/metrics.py
+-rw-r--r--   0        0        0     6892 2023-06-29 18:54:36.448538 wxdat-1.3.2/src/wxdat/providers/__init__.py
+-rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.3.2/src/wxdat/providers/accuweather.py
+-rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.3.2/src/wxdat/providers/ambientwx.py
+-rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.3.2/src/wxdat/providers/noaa.py
+-rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.3.2/src/wxdat/providers/openweather.py
+-rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.3.2/src/wxdat/providers/wunderground.py
+-rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.3.2/src/wxdat/units/__init__.py
+-rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.3.2/src/wxdat/units/distance.py
+-rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.3.2/src/wxdat/units/pressure.py
+-rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.3.2/src/wxdat/units/quantity.py
+-rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.3.2/src/wxdat/units/rate.py
+-rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.3.2/src/wxdat/units/temperature.py
+-rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.3.2/src/wxdat/units/velocity.py
+-rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.3.2/src/wxdat/units/volume.py
+-rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.3.2/src/wxdat/units/weight.py
+-rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.3.2/src/wxdat/version.py
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 wxdat-1.3.2/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 wxdat-1.3.2/PKG-INFO
```

### Comparing `wxdat-1.3.1/LICENSE` & `wxdat-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/README.md` & `wxdat-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/pyproject.toml` & `wxdat-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wxdat"
-version = "1.3.1"
+version = "1.3.2"
 description = "Weather data explorer."
 authors = ["jheddings <jheddings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `wxdat-1.3.1/src/wxdat/__main__.py` & `wxdat-1.3.2/src/wxdat/__main__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/config.py` & `wxdat-1.3.2/src/wxdat/config.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/database.py` & `wxdat-1.3.2/src/wxdat/database.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/metrics.py` & `wxdat-1.3.2/src/wxdat/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Metrics provider for wxdat."""
 
 from typing import Optional
 
 from prometheus_client import Counter, Gauge
 
 PROVIDER_REQUESTS = Counter(
-    "wxdat_provider_",
+    "wxdat_provider_requests",
     "Total requests made to a provider.",
     labelnames=["station", "provider", "method"],
 )
 
 STATION_READINGS = Counter(
     "wxdat_station_readings",
     "Readings recorded by the station.",
```

### Comparing `wxdat-1.3.1/src/wxdat/providers/__init__.py` & `wxdat-1.3.2/src/wxdat/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/providers/accuweather.py` & `wxdat-1.3.2/src/wxdat/providers/accuweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/providers/ambientwx.py` & `wxdat-1.3.2/src/wxdat/providers/ambientwx.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/providers/noaa.py` & `wxdat-1.3.2/src/wxdat/providers/noaa.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/providers/openweather.py` & `wxdat-1.3.2/src/wxdat/providers/openweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/providers/wunderground.py` & `wxdat-1.3.2/src/wxdat/providers/wunderground.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/__init__.py` & `wxdat-1.3.2/src/wxdat/units/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/distance.py` & `wxdat-1.3.2/src/wxdat/units/distance.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/pressure.py` & `wxdat-1.3.2/src/wxdat/units/pressure.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/quantity.py` & `wxdat-1.3.2/src/wxdat/units/quantity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/rate.py` & `wxdat-1.3.2/src/wxdat/units/rate.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/temperature.py` & `wxdat-1.3.2/src/wxdat/units/temperature.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/velocity.py` & `wxdat-1.3.2/src/wxdat/units/velocity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/volume.py` & `wxdat-1.3.2/src/wxdat/units/volume.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/units/weight.py` & `wxdat-1.3.2/src/wxdat/units/weight.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/src/wxdat/version.py` & `wxdat-1.3.2/src/wxdat/version.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.1/setup.py` & `wxdat-1.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'sqlalchemy>=2.0.17,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wxdat = wxdat.__main__:main']}
 
 setup_kwargs = {
     'name': 'wxdat',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'Weather data explorer.',
     'long_description': "# wxdat #\n\n[![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)\n[![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)\n[![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)\n\nA general purpose weather data recorder & explorer.\n\n![dashboard](docs/images/dashboard.png)\n\nWhile the primary purpose of this library is to record weather data, it can also be\nused as a framework for collecting weather information in other apps.\n\n## Installation ##\n\nInstall the published package using pip:\n\n```shell\npip3 install wxdat\n```\n\nThis project uses `poetry` to manage dependencies and a local virtual environment.  To\nget started, clone the repository and install the dependencies with the following:\n\n```shell\npoetry install\n```\n\n## Usage ##\n\nRun the module and tell it which config file to use.\n\n```shell\npython3 -m wxdat --config wxdat.yaml\n```\n\nIf you are using `poetry` to manage the virtual environment, use the following:\n\n```shell\npoetry run python -m wxdat --config wxdat.yaml\n```\n\n## Configuration ##\n\nThe configuration file is a YAML document with a list of stations to export.  See the\nincluded default file for more details.\n\nAll stations have the following configuration values:\n* name - must be unique\n* type - the support station type\n\n## Supported Stations ##\n\nEventually, I'd like to add local stations, not just online sources.  Please see\nthe example configuration file for details on each provider.\n\n* AccuWeather\n* Ambient Weather Network\n* OpenWeatherMap\n* National Weather Service (NOAA)\n* Weather Underground\n\n## Unit Conversion ##\n\n`wxdat` also includes a limited set of conversion helpers for working with units.  In\ngeneral, the pattern for using them is:\n\n```python\nfrom wxdat import units\n\n# convert 100.0 from celsius to fahrenheit\ntemp = units.degC(100).degf\n```\n\n## Contributing ##\n\nTo submit a new issue, please visit the [Issues](https://github.com/jheddings/wxdat/issues)\npage.\n\nIf you are unsure where to start, create a post in the\n[Discussions](https://github.com/jheddings/wxdat/discussions) area.\n\nAdditionally, [Pull Requests](https://github.com/jheddings/wxdat/pulls) are welcome.\n",
     'author': 'jheddings',
     'author_email': 'jheddings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wxdat-1.3.1/PKG-INFO` & `wxdat-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxdat
-Version: 1.3.1
+Version: 1.3.2
 Summary: Weather data explorer.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

