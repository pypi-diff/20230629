# Comparing `tmp/threedi-scenario-downloader-1.1.tar.gz` & `tmp/threedi-scenario-downloader-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-scenario-downloader-1.1.tar", last modified: Tue Jun 13 11:22:20 2023, max compression
+gzip compressed data, was "threedi-scenario-downloader-1.2.tar", last modified: Thu Jun 29 14:44:45 2023, max compression
```

## Comparing `threedi-scenario-downloader-1.1.tar` & `threedi-scenario-downloader-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350441 threedi-scenario-downloader-1.1/
--rw-r--r--   0 reinout    (501) staff       (20)     2655 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/CHANGES.rst
--rw-r--r--   0 reinout    (501) staff       (20)     1111 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/LICENSE
--rw-r--r--   0 reinout    (501) staff       (20)      203 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)     6799 2023-06-13 11:22:20.350497 threedi-scenario-downloader-1.1/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     3747 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      159 2023-06-13 11:22:20.350701 threedi-scenario-downloader-1.1/setup.cfg
--rw-r--r--   0 reinout    (501) staff       (20)      974 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/setup.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.348892 threedi-scenario-downloader-1.1/threedi_scenario_downloader/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)    29227 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/downloader.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350083 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     1379 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_batch.py
--rw-r--r--   0 reinout    (501) staff       (20)     2070 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader.py
--rw-r--r--   0 reinout    (501) staff       (20)     4819 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader_manual.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350329 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/
--rw-r--r--   0 reinout    (501) staff       (20)       31 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      366 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/batch.csv
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.349643 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)     6799 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      761 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/not-zip-safe
--rw-r--r--   0 reinout    (501) staff       (20)       67 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)       28 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.708693 threedi-scenario-downloader-1.2/
+-rw-r--r--   0 reinout    (501) staff       (20)     2769 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/CHANGES.rst
+-rw-r--r--   0 reinout    (501) staff       (20)     1111 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)      203 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)     6913 2023-06-29 14:44:45.708743 threedi-scenario-downloader-1.2/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     3747 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      159 2023-06-29 14:44:45.708943 threedi-scenario-downloader-1.2/setup.cfg
+-rw-r--r--   0 reinout    (501) staff       (20)      974 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/setup.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.707148 threedi-scenario-downloader-1.2/threedi_scenario_downloader/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)    30909 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/downloader.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.708344 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1379 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_batch.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2070 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_downloader.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4900 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_downloader_manual.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.708583 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/testdata/
+-rw-r--r--   0 reinout    (501) staff       (20)       31 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/testdata/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      366 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/testdata/batch.csv
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-29 14:44:45.707904 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)     6913 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      761 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 reinout    (501) staff       (20)       67 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       28 2023-06-29 14:44:45.000000 threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/top_level.txt
```

### Comparing `threedi-scenario-downloader-1.1/CHANGES.rst` & `threedi-scenario-downloader-1.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.2 (2023-06-29)
+----------------
+
+- Basic sub-endpoint added.
+
+- Small fixes.
+
+- Resolution is now guaranteed.
+
+
 1.1 (2023-06-13)
 ----------------
 
 - Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
 - Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
 - Bugfix with width and height
```

### Comparing `threedi-scenario-downloader-1.1/LICENSE` & `threedi-scenario-downloader-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.1/PKG-INFO` & `threedi-scenario-downloader-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-scenario-downloader
-Version: 1.1
+Version: 1.2
 Summary: Tools for downloading results for 3Di scenarios
 Home-page: https://github.com/nens/threedi-scenario-downloader
 Author: Emiel Verstegen
 Author-email: emiel.verstegen@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -117,14 +117,24 @@
 
   $ bin/pip install -r requirements.txt
 
 
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.2 (2023-06-29)
+----------------
+
+- Basic sub-endpoint added.
+
+- Small fixes.
+
+- Resolution is now guaranteed.
+
+
 1.1 (2023-06-13)
 ----------------
 
 - Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
 - Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
 - Bugfix with width and height
```

### Comparing `threedi-scenario-downloader-1.1/README.rst` & `threedi-scenario-downloader-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.1/setup.py` & `threedi-scenario-downloader-1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "1.1"
+version = "1.2"
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 install_requires = ["requests"]
 tests_require = ["pytest", "mock", "pytest-cov", "pytest-flakes", "pytest-black"]
 setup(
     name="threedi-scenario-downloader",
     version=version,
     description="Tools for downloading results for 3Di scenarios",
```

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader/downloader.py` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,30 @@
     "model_name": "model_name__icontains",
     "organisation": "organisation__icontains",
     "organisation__unique_id": "organisation__unique_id",
     "username": "username__icontains",
     "offset": "offset",
 }
 
+#results endpoint
 WATER_DEPTH = "depth-dtri"
 MAX_WATER_DEPTH = "depth-max-dtri"
-
 WATER_LEVEL = "s1-dtri"
+RATE_OF_RISE = "rise-velocity-quad"
+PRECIPITATION = "rain-quad"
+
+#basic sub-endpoint
+MAX_FLOW_VELOCITY = "ucr-max-quad"
 MAX_WATER_LEVEL = "s1-max-dtri"
 
+#arrival sub-endpoint
 ARRIVAL_TIME = "depth-first-dtri"
+
+#damage sub-endpoint
 TOTAL_DAMAGE = "total-damage"
-PRECIPITATION = "rain-quad"
 
 
 def set_logging_level(level):
     """set logging level to the supplied level"""
 
     log.level = level
 
@@ -172,26 +179,30 @@
     for result in result_list:
         if result["code"] == "logfiles":
             url = result["attachment_url"]
             return url
 
 
 def get_raster_url(scenario_uuid, raster_code, subendpoint=None):
-    result_list = get_scenario_instance_results(scenario_uuid, subendpoint)
+    result_list = get_scenario_instance_results(
+        scenario_uuid=scenario_uuid, subendpoint=subendpoint
+    )
 
     for result in result_list:
         if result["code"] == raster_code:
             raster_url = result["raster"]
             return raster_url
 
 
 def get_raster(scenario_uuid, raster_code, subendpoint=None):
     """return json of raster based on scenario uuid and raster type"""
 
-    raster_url = get_raster_url(scenario_uuid, raster_code, subendpoint)
+    raster_url = get_raster_url(
+        scenario_uuid=scenario_uuid, raster_code=raster_code, subendpoint=subendpoint
+    )
 
     r = requests.get(url=raster_url, auth=("__key__", get_api_key()),)
     r.raise_for_status()
 
     raster = r.json()
     return raster
 
@@ -201,28 +212,36 @@
 ):
     """create Lizard raster task"""
     x1 = scenario_instance["origin_x"]
     y1 = scenario_instance["origin_y"]
     x2 = scenario_instance["upper_bound_x"]
     y2 = scenario_instance["upper_bound_y"]
 
-    bbox = "{},{},{},{}".format(x1, y1, x2, y2)
-
     if projection is None:
         projection = raster["projection"]
 
     if resolution is None:
         pixelsize_x = abs(scenario_instance["pixelsize_x"])
         pixelsize_y = abs(scenario_instance["pixelsize_y"])
     else:
         pixelsize_x = resolution
         pixelsize_y = resolution
 
-    width = math.ceil((x2 - x1) / pixelsize_x)
-    height = math.ceil((y2 - y1) / pixelsize_y)
+    width = abs((x2 - x1) / pixelsize_x)
+    height = abs((y2 - y1) / pixelsize_y)
+
+    # Check if pixelsize fits the extent, if not, to maintain pixelsize, enlarge the extent
+    if not width.is_integer():
+        width = math.ceil(width)
+        x2 = (width * pixelsize_x) + x1
+    if not height.is_integer():
+        height = math.ceil(height)
+        y2 = (height * pixelsize_y) + y1
+
+    bbox = "{},{},{},{}".format(x1, y1, x2, y2)
 
     url = "{}rasters/{}/data/".format(LIZARD_URL, raster["uuid"])
 
     # non temporal raster
     payload = {
         "width": width,
         "height": height,
@@ -332,14 +351,16 @@
     task_id_list = transform_to_list(var=None, length=len(scenario_list))
     task_url_list = transform_to_list(var=None, length=len(scenario_list))
 
     # Helper for subendpoints
     subendpoint_per_raster_code = {
         ARRIVAL_TIME: "arrival",
         TOTAL_DAMAGE: "damage",
+        MAX_FLOW_VELOCITY: "basic",
+        MAX_WATER_LEVEL: "basic",
     }
 
     # Wrong input error
     if len(scenario_list) != len(pathname_list):
         logging.debug("Scenarios and output should be of same length")
         raise ValueError("scenario_list and pathname_list are of different length")
 
@@ -476,101 +497,130 @@
                         "Task {} failed, status was: {}".format(task_uuid, task_status)
                     )
                     processed_list[index] = True
         sleep(5)
 
 
 def download_maximum_waterdepth_raster(
-    scenario_uuid, projection, resolution, bbox=None, pathname=None
+    scenario_uuid, projection=None, resolution=None, bbox=None, pathname=None
 ):
     """download Maximum waterdepth raster"""
     download_raster(
         scenario_uuid,
         MAX_WATER_DEPTH,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_maximum_waterlevel_raster(
-    scenario_uuid, projection, resolution, bbox=None, pathname=None
+    scenario_uuid, projection=None, resolution=None, bbox=None, pathname=None
 ):
     """download Maximum waterlevel raster"""
     download_raster(
         scenario_uuid,
         MAX_WATER_LEVEL,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
+def download_maximum_flow_velocity_raster(
+    scenario_uuid, projection=None, resolution=None, bbox=None, pathname=None
+):
+    """download Maximum waterdepth raster"""
+    download_raster(
+        scenario_uuid,
+        MAX_FLOW_VELOCITY,
+        projection=projection,
+        resolution=resolution,
+        bbox=bbox,
+        pathname=pathname,
+    )
+
+
 def download_total_damage_raster(
-    scenario_uuid, projection, resolution, bbox=None, pathname=None
+    scenario_uuid, projection=None, resolution=None, bbox=None, pathname=None
 ):
     """download Total Damage raster"""
     download_raster(
         scenario_uuid,
         TOTAL_DAMAGE,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_arrival_time_raster(
-    scenario_uuid, projection, resolution, bbox=None, pathname=None
+    scenario_uuid, projection=None, resolution=None, bbox=None, pathname=None
 ):
     """download arrival time raster"""
     download_raster(
         scenario_uuid,
         ARRIVAL_TIME,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_waterdepth_raster(
-    scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
+    scenario_uuid,
+    projection=None,
+    resolution=None,
+    time=None,
+    bbox=None,
+    pathname=None,
 ):
     """download snapshot of Waterdepth raster"""
     download_raster(
         scenario_uuid,
         WATER_DEPTH,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         time=time,
         pathname=pathname,
     )
 
 
 def download_waterlevel_raster(
-    scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
+    scenario_uuid,
+    projection=None,
+    resolution=None,
+    time=None,
+    bbox=None,
+    pathname=None,
 ):
     """download snapshot of Waterlevel raster"""
     download_raster(
         scenario_uuid,
         WATER_LEVEL,
         projection=projection,
         resolution=resolution,
         bbox=bbox,
         time=time,
         pathname=pathname,
     )
 
 
 def download_precipitation_raster(
-    scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
+    scenario_uuid,
+    projection=None,
+    resolution=None,
+    time=None,
+    bbox=None,
+    pathname=None,
 ):
     """download snapshot of precipitation raster"""
     download_raster(
         scenario_uuid,
         PRECIPITATION,
         projection=projection,
         resolution=resolution,
@@ -619,18 +669,20 @@
             attachment_links[result_name] = result["attachment_url"]
     if attachment_links:
         return attachment_links
     else:
         return None
 
 
-def rasters_in_scenario(scenario_json):
+def rasters_in_scenario(scenario_json, subendpoint=None):
     """return two lists of static and temporal rasters including 3di result name and code"""
     scenario_uuid = scenario_json["uuid"]
-    result_list = get_scenario_instance_results(scenario_uuid)
+    result_list = get_scenario_instance_results(
+        scenario_uuid=scenario_uuid, subendpoint=subendpoint
+    )
 
     temporal_rasters = []
     static_rasters = []
     for result in result_list:
 
         if result["raster"]:
 
@@ -644,19 +696,24 @@
                 temporal_rasters.append(raster_url)
             else:
                 static_rasters.append(raster_url)
     return static_rasters, temporal_rasters
 
 
 def get_raster_download_link(
-    raster, scenario_instance, resolution, projection, bbox=None, time=None
+    raster, scenario_instance, resolution=None, projection=None, bbox=None, time=None
 ):
     """get url to download raster"""
     task = create_raster_task(
-        raster, scenario_instance, resolution, projection, bbox, time
+        raster=raster,
+        scenario_instance=scenario_instance,
+        resolution=resolution,
+        projection=projection,
+        bbox=bbox,
+        time=time,
     )
     task_uuid = task["task_id"]
 
     logging.debug("Start waiting for task {} to finish".format(task_uuid))
     task_status = get_task_status(task_uuid)
     processing = True
     while processing:
@@ -671,39 +728,49 @@
             return download_url
         else:
             logging.debug("Task failed")
             return None
 
 
 def get_static_rasters_links(
-    static_rasters, projection, resolution, bbox=None, time=None
+    static_rasters, projection=None, resolution=None, bbox=None, time=None
 ):
     """return a dict of urls to geotiff files of static rasters in scenario
     the dict items are formatted as result_name: link.tif"""
     static_raster_urls = {}
     for static_raster in static_rasters:
         name = static_raster["name_3di"]
         static_raster_url = get_raster_download_link(
-            static_raster, projection, resolution, bbox, time
+            raster=static_raster,
+            projection=projection,
+            resolution=resolution,
+            bbox=bbox,
+            time=time,
         )
         static_raster_urls[name] = static_raster_url
     return static_raster_urls
 
 
 def get_temporal_raster_links(
-    temporal_raster, projection, resolution, bbox=None, interval_hours=None,
+    temporal_raster, projection=None, resolution=None, bbox=None, interval_hours=None,
 ):
     """return a dict of urls to geotiff files of a temporal raster
     the dict items are formatted as name_3di_datetime: link.tif"""
     temporal_raster_urls = {}
     name = temporal_raster["name_3di"]
-    timesteps = get_raster_timesteps(temporal_raster, interval_hours)
+    timesteps = get_raster_timesteps(
+        raster=temporal_raster, interval_hours=interval_hours
+    )
     for timestep in timesteps:
         download_url = get_raster_download_link(
-            temporal_raster, projection, resolution, bbox, timestep
+            raster=temporal_raster,
+            projection=projection,
+            resolution=resolution,
+            bbox=bbox,
+            time=timestep,
         )
         url_timestep = os.path.splitext(download_url)[0].split("_")[-1]
         # Lizard returns the nearest timestep based on the time=timestep request
         timestep_url_format = "{}Z".format(timestep.split(".")[0].replace("-", ""))
         if timestep_url_format == url_timestep:
             # when requested and retrieved timesteps are equal, use the timestep
             name_timestep = "_".join([name, timestep])
@@ -713,21 +780,25 @@
                 name, timestep_url_format, url_timestep
             )
         temporal_raster_urls[name_timestep] = download_url
     return temporal_raster_urls
 
 
 def get_temporal_rasters_links(
-    temporal_rasters, projection, resolution, bbox=None, interval_hours=None,
+    temporal_rasters, projection=None, resolution=None, bbox=None, interval_hours=None,
 ):
     """get links to all temporal rasters"""
     temporal_rasters_urls = {}
     for temporal_raster in temporal_rasters:
         temporal_raster_urls = get_temporal_raster_links(
-            temporal_raster, projection, resolution, bbox, interval_hours
+            temporal_raster=temporal_raster,
+            projection=projection,
+            resolution=resolution,
+            bbox=bbox,
+            interval_hours=interval_hours,
         )
         for name_timestep, download_url in temporal_raster_urls.items():
             temporal_rasters_urls.setdefault(name_timestep, download_url)
     return temporal_rasters_urls
 
 
 def to_datetime_obj(time_string):
@@ -797,15 +868,15 @@
         ]
     return timesteps
 
 
 def get_raster_from_json(scenario_json, raster_code, subendpoint=None):
     """return raster json object from scenario"""
     scenario_uuid = scenario_json["uuid"]
-    raster_url = get_raster_url(scenario_uuid, raster_code)
+    raster_url = get_raster_url(scenario_uuid=scenario_uuid, raster_code=raster_code)
 
     r = requests.get(url=raster_url, auth=("__key__", get_api_key()),)
 
     r.raise_for_status()
 
     raster = r.json()
     return raster
@@ -842,15 +913,15 @@
 
             if task_status == "SUCCESS":
                 # Task succesfull, check if file already exists
 
                 # Download if it doesn't exist, or if it do
                 if not os.path.isfile(pathname) or overwrite:
                     try:
-                        download_task(uuid, pathname)
+                        download_task(task_uuid=uuid, pathname=pathname)
                     except HTTPError as err:
                         if err.code == 503:
                             logging.debug(
                                 "503 Server Error: Lizard has lost it. Let's ignore this."
                             )
                             task_status = "UNKNOWN"
                         else:
```

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_batch.py` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader.py` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader_manual.py` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader/tests/test_downloader_manual.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         downloader.get_api_key() == config["credentials"]["api_key"]
     )
 
 
 def test_download_maximum_waterdepth_raster():
     downloader.download_maximum_waterdepth_raster(
         SCENARIO_UUID,
-        "EPSG:28992",
+        projection="EPSG:28992",
         resolution=1000,
         bbox=None,
         pathname="threedi_scenario_downloader/tests/testdata/max_waterdepth.tif",
     )
     assert os.path.isfile(
         "threedi_scenario_downloader/tests/testdata/max_waterdepth.tif"
     )
@@ -87,15 +87,20 @@
     assert static_rasters is not None and temporal_rasters is not None
 
 
 def test_get_raster_download_link():
     raster = downloader.get_raster(SCENARIO_UUID, "depth-max-dtri")
     scenario_instance = downloader.get_scenario_instance(SCENARIO_UUID)
     download_url = downloader.get_raster_download_link(
-        raster, scenario_instance, "EPSG:4326", 10, bbox=None, time=None
+        raster,
+        scenario_instance,
+        projection="EPSG:4326",
+        resolution=10,
+        bbox=None,
+        time=None,
     )
     assert download_url is not None
 
 
 def test_download_raster():
     file_path = "threedi_scenario_downloader/tests/testdata/max_wd.tif"
 
@@ -131,15 +136,15 @@
 
     for file_path in file_paths:
         assert os.path.isfile(file_path)
 
 
 def test_get_raster_timesteps():
     raster = downloader.get_raster(SCENARIO_UUID, "s1-dtri")
-    timesteps = downloader.get_raster_timesteps(raster, interval_hours=None)
+    timesteps = downloader.get_raster_timesteps(raster=raster, interval_hours=None)
     assert isinstance(timesteps, list) and all(
         isinstance(step, str) for step in timesteps
     )
 
 
 def test_get_raster_from_json():
     scenario_json = downloader.find_scenarios_by_model_slug(MODEL_UUID)[0]
```

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/PKG-INFO` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-scenario-downloader
-Version: 1.1
+Version: 1.2
 Summary: Tools for downloading results for 3Di scenarios
 Home-page: https://github.com/nens/threedi-scenario-downloader
 Author: Emiel Verstegen
 Author-email: emiel.verstegen@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -117,14 +117,24 @@
 
   $ bin/pip install -r requirements.txt
 
 
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.2 (2023-06-29)
+----------------
+
+- Basic sub-endpoint added.
+
+- Small fixes.
+
+- Resolution is now guaranteed.
+
+
 1.1 (2023-06-13)
 ----------------
 
 - Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
 - Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
 - Bugfix with width and height
```

### Comparing `threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/SOURCES.txt` & `threedi-scenario-downloader-1.2/threedi_scenario_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

