# Comparing `tmp/wxdat-1.2.0.tar.gz` & `tmp/wxdat-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxdat-1.2.0.tar", max compression
+gzip compressed data, was "wxdat-1.3.1.tar", max compression
```

## Comparing `wxdat-1.2.0.tar` & `wxdat-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.2.0/LICENSE
--rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.2.0/README.md
--rw-r--r--   0        0        0      663 2023-06-21 03:13:56.848313 wxdat-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.2.0/src/wxdat/__init__.py
--rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.2.0/src/wxdat/__main__.py
--rw-r--r--   0        0        0     6398 2023-03-19 14:53:46.008303 wxdat-1.2.0/src/wxdat/config.py
--rw-r--r--   0        0        0     3683 2023-06-21 03:18:47.374073 wxdat-1.2.0/src/wxdat/database.py
--rw-r--r--   0        0        0     5515 2023-03-19 14:53:46.009092 wxdat-1.2.0/src/wxdat/metrics.py
--rw-r--r--   0        0        0     6504 2023-03-19 15:23:37.615963 wxdat-1.2.0/src/wxdat/providers/__init__.py
--rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.2.0/src/wxdat/providers/accuweather.py
--rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.2.0/src/wxdat/providers/ambientwx.py
--rw-r--r--   0        0        0     6663 2023-02-14 14:12:56.230852 wxdat-1.2.0/src/wxdat/providers/darksky.py
--rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.2.0/src/wxdat/providers/noaa.py
--rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.2.0/src/wxdat/providers/openweather.py
--rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.2.0/src/wxdat/providers/wunderground.py
--rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.2.0/src/wxdat/units/__init__.py
--rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.2.0/src/wxdat/units/distance.py
--rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.2.0/src/wxdat/units/pressure.py
--rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.2.0/src/wxdat/units/quantity.py
--rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.2.0/src/wxdat/units/rate.py
--rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.2.0/src/wxdat/units/temperature.py
--rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.2.0/src/wxdat/units/velocity.py
--rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.2.0/src/wxdat/units/volume.py
--rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.2.0/src/wxdat/units/weight.py
--rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.2.0/src/wxdat/version.py
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 wxdat-1.2.0/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 wxdat-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.3.1/README.md
+-rw-r--r--   0        0        0      663 2023-06-29 19:14:59.106276 wxdat-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.3.1/src/wxdat/__init__.py
+-rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.3.1/src/wxdat/__main__.py
+-rw-r--r--   0        0        0     5932 2023-06-29 18:55:36.438028 wxdat-1.3.1/src/wxdat/config.py
+-rw-r--r--   0        0        0     3711 2023-06-29 18:58:07.039970 wxdat-1.3.1/src/wxdat/database.py
+-rw-r--r--   0        0        0     6276 2023-06-29 18:58:07.040077 wxdat-1.3.1/src/wxdat/metrics.py
+-rw-r--r--   0        0        0     6892 2023-06-29 18:54:36.448538 wxdat-1.3.1/src/wxdat/providers/__init__.py
+-rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.3.1/src/wxdat/providers/accuweather.py
+-rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.3.1/src/wxdat/providers/ambientwx.py
+-rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.3.1/src/wxdat/providers/noaa.py
+-rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.3.1/src/wxdat/providers/openweather.py
+-rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.3.1/src/wxdat/providers/wunderground.py
+-rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.3.1/src/wxdat/units/__init__.py
+-rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.3.1/src/wxdat/units/distance.py
+-rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.3.1/src/wxdat/units/pressure.py
+-rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.3.1/src/wxdat/units/quantity.py
+-rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.3.1/src/wxdat/units/rate.py
+-rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.3.1/src/wxdat/units/temperature.py
+-rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.3.1/src/wxdat/units/velocity.py
+-rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.3.1/src/wxdat/units/volume.py
+-rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.3.1/src/wxdat/units/weight.py
+-rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.3.1/src/wxdat/version.py
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 wxdat-1.3.1/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 wxdat-1.3.1/PKG-INFO
```

### Comparing `wxdat-1.2.0/LICENSE` & `wxdat-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/README.md` & `wxdat-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/pyproject.toml` & `wxdat-1.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "wxdat"
-version = "1.2.0"
+version = "1.3.1"
 description = "Weather data explorer."
 authors = ["jheddings <jheddings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 click = "^8.1.3"
-prometheus-client = "^0.16.0"
+prometheus-client = "^0.17.0"
 pydantic = "^1.10.9"
-sqlalchemy = "^2.0.16"
+sqlalchemy = "^2.0.17"
 psycopg2 = "^2.9.6"
 ratelimit = "^2.2.1"
 pyyaml = "^6.0"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
-pytest = "^7.3.2"
+pytest = "^7.4.0"
 pytest-vcr = "^1.0.2"
 coverage = "^7.2.7"
 
 [tool.poetry.scripts]
 wxdat = "wxdat.__main__:main"
 
 [build-system]
```

### Comparing `wxdat-1.2.0/src/wxdat/__main__.py` & `wxdat-1.3.1/src/wxdat/__main__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/config.py` & `wxdat-1.3.1/src/wxdat/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import yaml
 from pydantic import BaseModel, validator
 
 from .providers import (
     WeatherProvider,
     accuweather,
     ambientwx,
-    darksky,
     noaa,
     openweather,
     wunderground,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -124,32 +123,14 @@
             name=self.name,
             api_key=self.api_key,
             latitude=self.latitude,
             longitude=self.longitude,
         )
 
 
-class DarkSkyConfig(StationConfig, provider=WeatherProvider.DARKSKY):
-    """Station configuration for Dark Sky."""
-
-    api_key: str
-    latitude: float
-    longitude: float
-
-    def initialize(self):
-        """Initialize a new Dark Sky station based on this config."""
-
-        return darksky.Station(
-            name=self.name,
-            api_key=self.api_key,
-            latitude=self.latitude,
-            longitude=self.longitude,
-        )
-
-
 class WeatherUndergroundConfig(StationConfig, provider=WeatherProvider.WUNDERGROUND):
     """Station configuration for Weather Underground."""
 
     api_key: str
     station_id: str
 
     def initialize(self):
```

### Comparing `wxdat-1.2.0/src/wxdat/database.py` & `wxdat-1.3.1/src/wxdat/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Database connection and models for wxdat."""
 import logging
 
 import sqlalchemy as sql
-from prometheus_client import Counter
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import declarative_base, sessionmaker
 
+from . import metrics
+
 logger = logging.getLogger(__name__)
 
 
-MagicTable = declarative_base()
+WeatherData = declarative_base()
 MagicSession = sessionmaker()
 
 
-class HourlyForecast(MagicTable):
+class HourlyForecast(WeatherData):
     """Define fields for hourly forecast data."""
 
     __tablename__ = "hourly_forecast"
 
     timestamp = sql.Column(sql.DateTime(True), primary_key=True)
     provider = sql.Column(sql.String(256), primary_key=True)
     station_id = sql.Column(sql.String(256), primary_key=True)
@@ -42,15 +43,15 @@
     visibility = sql.Column(sql.Float())
     uv_index = sql.Column(sql.Float())
     ozone = sql.Column(sql.Float())
 
     remarks = sql.Column(sql.Text())
 
 
-class CurrentConditions(MagicTable):
+class CurrentConditions(WeatherData):
     """Define data fields for current conditions."""
 
     __tablename__ = "current_conditions"
 
     timestamp = sql.Column(sql.DateTime(True), primary_key=True)
     provider = sql.Column(sql.String(256), primary_key=True)
     station_id = sql.Column(sql.String(256), primary_key=True)
@@ -91,36 +92,39 @@
         """Connect to a database specified by the connection URL."""
 
         logger.debug("Connecting to database: %s", url)
         self.engine = sql.create_engine(url)
 
         self.migrate()
 
-        self.session_attempts = Counter(
-            "wxdat_session_attempts",
-            "Session initialzation requests.",
-        )
+        self.metrics = metrics.DatabaseMetrics(self.engine)
 
         # configure the session class to use our engine
         MagicSession.configure(bind=self.engine)
 
     def migrate(self):
         # TODO create / migrate schema as needed
-        MagicTable.metadata.create_all(self.engine)
+        WeatherData.metadata.create_all(self.engine)
 
     def session(self):
         """Starts a new session with the database engine."""
-        self.session_attempts.inc()
+        self.metrics.sessions.inc()
+
         return MagicSession()
 
-    def save(self, entry: MagicTable):
+    def save(self, entry: WeatherData):
+        self.metrics.writes.inc()
+
         with self.session() as session:
             try:
                 session.merge(entry)
                 session.commit()
 
             except SQLAlchemyError:
                 logger.exception("Error saving entry; rolling back")
                 session.rollback()
+                self.metrics.errors.inc()
                 return False
 
+        self.metrics.commits.inc()
+
         return True
```

### Comparing `wxdat-1.2.0/src/wxdat/metrics.py` & `wxdat-1.3.1/src/wxdat/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Metrics provider for wxdat."""
 
 from typing import Optional
 
 from prometheus_client import Counter, Gauge
 
-from .database import CurrentConditions
-
 PROVIDER_REQUESTS = Counter(
-    "wxdat_provider_get_requests",
-    "Total GET requests made to a provider.",
+    "wxdat_provider_",
+    "Total requests made to a provider.",
     labelnames=["station", "provider", "method"],
 )
 
+STATION_READINGS = Counter(
+    "wxdat_station_readings",
+    "Readings recorded by the station.",
+    labelnames=["station"],
+)
+
 STATION_FAILED = Counter(
     "wxdat_station_failed",
-    "Failed requests made by the station.",
+    "Failures during station readings.",
     labelnames=["station"],
 )
 
 STATION_ERRORS = Counter(
     "wxdat_station_errors",
     "Errors reported by the station.",
     labelnames=["station"],
@@ -26,49 +30,49 @@
 
 CURRENT_TEMPERATURE = Gauge(
     "wxdat_current_temperature",
     "Current temperature reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_FEELS_LIKE = Gauge(
     "wxdat_current_feels_like_temperature",
     "Current 'feels like' temperature reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_DEWPOINT = Gauge(
     "wxdat_current_dewpoint",
     "Current dewpoint reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_WIND_SPEED = Gauge(
     "wxdat_current_wind_spped",
     "Current wind speed reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_WIND_GUSTS = Gauge(
     "wxdat_current_wind_gusts",
     "Current wind gusts reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_WIND_BEARING = Gauge(
     "wxdat_current_wind_bearing",
     "Current wind bearing reported by the station.",
     labelnames=["station"],
 )
 
+TOTAL_PRECIP = Counter(
+    "wxdat_precipitation",
+    "Precipitation reported by the station.",
+    labelnames=["station"],
+)
 
 CURRENT_HUMIDITY = Gauge(
     "wxdat_current_humidity",
     "Current humidity reported by the station.",
     labelnames=["station"],
 )
 
@@ -80,63 +84,68 @@
 
 CURRENT_ABS_PRESSURE = Gauge(
     "wxdat_current_abs_pressure",
     "Current absolute pressure reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_CLOUDS = Gauge(
     "wxdat_current_clouds",
     "Current cloud cover reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_VISIBILITY = Gauge(
     "wxdat_current_visibility",
     "Current visibility reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_UV_INDEX = Gauge(
     "wxdat_current_uv_index",
     "Current UV index reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_OZONE = Gauge(
     "wxdat_current_ozone",
     "Current ozone reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_SOLAR_LUX = Gauge(
     "wxdat_current_solar_lux",
     "Current solar level reported by the station.",
     labelnames=["station"],
 )
 
-
 CURRENT_SOLAR_RAD = Gauge(
     "wxdat_current_solar_radiation",
     "Current solar radiation reported by the station.",
     labelnames=["station"],
 )
 
 
+class DatabaseMetrics:
+    def __init__(self, engine):
+        self._engine = engine
+
+        self.sessions = Counter("wxdat_session_created", "Database sessions created")
+        self.writes = Counter("wxdat_session_writes", "Database write attemps")
+        self.commits = Counter("wxdat_session_commits", "Database commits completed")
+        self.errors = Counter("wxdat_session_errors", "Database session errors")
+
+
 class BaseStationMetrics:
     def __init__(self, station):
+        self.readings = STATION_READINGS.labels(station=station.name)
         self.errors = STATION_ERRORS.labels(station=station.name)
         self.failed = STATION_FAILED.labels(station=station.name)
 
-        self.get_req = PROVIDER_REQUESTS.labels(
+        self.requests = PROVIDER_REQUESTS.labels(
             method="get",
             provider=station.provider.value,
             station=station.name,
         )
 
 
 class WeatherConditionMetrics:
@@ -147,42 +156,40 @@
         self.feels_like = CURRENT_FEELS_LIKE.labels(station=name)
         self.dew_point = CURRENT_DEWPOINT.labels(station=name)
 
         self.wind_speed = CURRENT_WIND_SPEED.labels(station=name)
         self.wind_gusts = CURRENT_WIND_GUSTS.labels(station=name)
         self.wind_bearing = CURRENT_WIND_BEARING.labels(station=name)
 
+        self.precipitation = TOTAL_PRECIP.labels(station=name)
         self.humidity = CURRENT_HUMIDITY.labels(station=name)
 
         self.rel_pressure = CURRENT_REL_PRESSURE.labels(station=name)
         self.abs_pressure = CURRENT_ABS_PRESSURE.labels(station=name)
 
         self.cloud_cover = CURRENT_CLOUDS.labels(station=name)
         self.visibility = CURRENT_VISIBILITY.labels(station=name)
         self.uv_index = CURRENT_UV_INDEX.labels(station=name)
         self.ozone = CURRENT_OZONE.labels(station=name)
 
         self.solar_lux = CURRENT_SOLAR_LUX.labels(station=name)
         self.solar_rad = CURRENT_SOLAR_RAD.labels(station=name)
 
     def _update_gauge(self, gauge: Gauge, val: Optional[float] = None):
-        if val is None:
-            return False
-
-        gauge.set(val)
-
-        return True
+        if val is not None:
+            gauge.set(val)
 
-    def __call__(self, current_conditions: CurrentConditions):
+    def update(self, current_conditions):
         self._update_gauge(self.temperature, current_conditions.temperature)
         self._update_gauge(self.feels_like, current_conditions.feels_like)
         self._update_gauge(self.dew_point, current_conditions.dew_point)
         self._update_gauge(self.wind_speed, current_conditions.wind_speed)
         self._update_gauge(self.wind_gusts, current_conditions.wind_gusts)
         self._update_gauge(self.wind_bearing, current_conditions.wind_bearing)
+        self._update_gauge(self.precipitation, current_conditions.precip_total)
         self._update_gauge(self.humidity, current_conditions.humidity)
         self._update_gauge(self.rel_pressure, current_conditions.rel_pressure)
         self._update_gauge(self.abs_pressure, current_conditions.abs_pressure)
         self._update_gauge(self.cloud_cover, current_conditions.cloud_cover)
         self._update_gauge(self.visibility, current_conditions.visibility)
         self._update_gauge(self.uv_index, current_conditions.uv_index)
         self._update_gauge(self.ozone, current_conditions.ozone)
```

### Comparing `wxdat-1.2.0/src/wxdat/providers/__init__.py` & `wxdat-1.3.1/src/wxdat/providers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 logger = logging.getLogger(__name__)
 
 
 class WeatherProvider(str, Enum):
     ACCUWEATHER = "AccuWeather"
     AMBIENT = "AmbientWeather"
-    DARKSKY = "DarkSky"
     NOAA = "NOAA"
     OPENWEATHERMAP = "OpenWeatherMap"
     WUNDERGROUND = "WUndergroundPWS"
 
 
 class BaseStation(ABC):
     def __init__(self, name):
@@ -66,29 +65,29 @@
 
         if headers is not None:
             full_headers.update(headers)
 
         try:
             resp = requests.get(url, params=params, headers=full_headers)
             self.logger.debug("=> HTTP %d: %s", resp.status_code, resp.reason)
-            self.metrics.get_req.inc()
+            self.metrics.requests.inc()
 
         except ConnectionError:
             self.logger.warning("Unable to download data; connection error")
             self.metrics.errors.inc()
             return None
 
         except Exception:
             self.logger.exception("Unable to download data; unhandled exception")
             self.metrics.errors.inc()
             return None
 
         if not resp.ok:
             self.logger.warning("Unable to download data; HTTP %d", resp.status_code)
-            self.metrics.failed.inc()
+            self.metrics.errors.inc()
             return None
 
         return resp
 
 
 class DataRecorder:
     """Records data from a specific BaseStation."""
@@ -177,18 +176,25 @@
         if wx_data is None:
             self.logger.debug(
                 "Station '%s' did not provide current weather.",
                 self.station.name,
             )
             return False
 
-        self.metrics(wx_data)
+        self.metrics.update(wx_data)
 
         self.logger.debug("-- saving current data @ %s", wx_data.timestamp)
-        return self.database.save(wx_data)
+
+        # if we succesfully record the data, update the total readings for the station...  it's a bit
+        # hacky to reach into the station this way, but this is the only place we can be sure that the
+        # data has been stored in the database and have reference to the station identifiers
+        if self.database.save(wx_data):
+            self.station.metrics.readings.inc()
+        else:
+            self.station.metrics.failed.inc()
 
     def record_hourly_forecast(self):
         """Record the hourly forecast from the internal station."""
 
         self.logger.info("Reading hourly forecast -- %s", self.station.name)
         forecast = self.station.hourly_forecast
```

### Comparing `wxdat-1.2.0/src/wxdat/providers/accuweather.py` & `wxdat-1.3.1/src/wxdat/providers/accuweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/providers/ambientwx.py` & `wxdat-1.3.1/src/wxdat/providers/ambientwx.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/providers/noaa.py` & `wxdat-1.3.1/src/wxdat/providers/noaa.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/providers/openweather.py` & `wxdat-1.3.1/src/wxdat/providers/openweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/providers/wunderground.py` & `wxdat-1.3.1/src/wxdat/providers/wunderground.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/__init__.py` & `wxdat-1.3.1/src/wxdat/units/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/distance.py` & `wxdat-1.3.1/src/wxdat/units/distance.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/pressure.py` & `wxdat-1.3.1/src/wxdat/units/pressure.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/quantity.py` & `wxdat-1.3.1/src/wxdat/units/quantity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/rate.py` & `wxdat-1.3.1/src/wxdat/units/rate.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/temperature.py` & `wxdat-1.3.1/src/wxdat/units/temperature.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/velocity.py` & `wxdat-1.3.1/src/wxdat/units/velocity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/volume.py` & `wxdat-1.3.1/src/wxdat/units/volume.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/units/weight.py` & `wxdat-1.3.1/src/wxdat/units/weight.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/src/wxdat/version.py` & `wxdat-1.3.1/src/wxdat/version.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.2.0/setup.py` & `wxdat-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'gitpython>=3.1.31,<4.0.0',
- 'prometheus-client>=0.16.0,<0.17.0',
+ 'prometheus-client>=0.17.0,<0.18.0',
  'psycopg2>=2.9.6,<3.0.0',
  'pydantic>=1.10.9,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'ratelimit>=2.2.1,<3.0.0',
  'requests>=2.31.0,<3.0.0',
- 'sqlalchemy>=2.0.16,<3.0.0']
+ 'sqlalchemy>=2.0.17,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wxdat = wxdat.__main__:main']}
 
 setup_kwargs = {
     'name': 'wxdat',
-    'version': '1.2.0',
+    'version': '1.3.1',
     'description': 'Weather data explorer.',
     'long_description': "# wxdat #\n\n[![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)\n[![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)\n[![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)\n\nA general purpose weather data recorder & explorer.\n\n![dashboard](docs/images/dashboard.png)\n\nWhile the primary purpose of this library is to record weather data, it can also be\nused as a framework for collecting weather information in other apps.\n\n## Installation ##\n\nInstall the published package using pip:\n\n```shell\npip3 install wxdat\n```\n\nThis project uses `poetry` to manage dependencies and a local virtual environment.  To\nget started, clone the repository and install the dependencies with the following:\n\n```shell\npoetry install\n```\n\n## Usage ##\n\nRun the module and tell it which config file to use.\n\n```shell\npython3 -m wxdat --config wxdat.yaml\n```\n\nIf you are using `poetry` to manage the virtual environment, use the following:\n\n```shell\npoetry run python -m wxdat --config wxdat.yaml\n```\n\n## Configuration ##\n\nThe configuration file is a YAML document with a list of stations to export.  See the\nincluded default file for more details.\n\nAll stations have the following configuration values:\n* name - must be unique\n* type - the support station type\n\n## Supported Stations ##\n\nEventually, I'd like to add local stations, not just online sources.  Please see\nthe example configuration file for details on each provider.\n\n* AccuWeather\n* Ambient Weather Network\n* OpenWeatherMap\n* National Weather Service (NOAA)\n* Weather Underground\n\n## Unit Conversion ##\n\n`wxdat` also includes a limited set of conversion helpers for working with units.  In\ngeneral, the pattern for using them is:\n\n```python\nfrom wxdat import units\n\n# convert 100.0 from celsius to fahrenheit\ntemp = units.degC(100).degf\n```\n\n## Contributing ##\n\nTo submit a new issue, please visit the [Issues](https://github.com/jheddings/wxdat/issues)\npage.\n\nIf you are unsure where to start, create a post in the\n[Discussions](https://github.com/jheddings/wxdat/discussions) area.\n\nAdditionally, [Pull Requests](https://github.com/jheddings/wxdat/pulls) are welcome.\n",
     'author': 'jheddings',
     'author_email': 'jheddings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wxdat-1.2.0/PKG-INFO` & `wxdat-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: wxdat
-Version: 1.2.0
+Version: 1.3.1
 Summary: Weather data explorer.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
+Requires-Dist: prometheus-client (>=0.17.0,<0.18.0)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sqlalchemy (>=2.0.16,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
 Description-Content-Type: text/markdown
 
 # wxdat #
 
 [![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)
 [![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)
 [![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)
```

