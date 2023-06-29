# Comparing `tmp/od_standards_calibration_plugin-1.0.1-py3-none-any.whl.zip` & `tmp/od_standards_calibration_plugin-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8752 bytes, number of entries: 9
+Zip file size: 8741 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      119 b- defN 23-Jun-20 18:50 od_standards_calibration_plugin/__init__.py
--rw-r--r--  2.0 unx    18352 b- defN 23-Jun-22 18:49 od_standards_calibration_plugin/od_calibration_from_standards.py
+-rw-r--r--  2.0 unx    18334 b- defN 23-Jun-29 16:26 od_standards_calibration_plugin/od_calibration_from_standards.py
 -rw-r--r--  2.0 unx      137 b- defN 23-Jun-20 18:56 od_standards_calibration_plugin/ui/contrib/jobs/od_standards_calibration_plugin.yaml
--rw-rw-r--  2.0 unx     1055 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1220 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       32 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/RECORD
-9 files, 22084 bytes uncompressed, 6970 bytes compressed:  68.4%
+-rw-rw-r--  2.0 unx     1055 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       32 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-29 16:29 od_standards_calibration_plugin-1.0.2.dist-info/RECORD
+9 files, 22066 bytes uncompressed, 6959 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: od_standards_calibration_plugin/od_calibration_from_standards.py
 Comment: 
 
 Filename: od_standards_calibration_plugin/ui/contrib/jobs/od_standards_calibration_plugin.yaml
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/METADATA
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/WHEEL
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/entry_points.txt
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/top_level.txt
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.1.dist-info/RECORD
+Filename: od_standards_calibration_plugin-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## od_standards_calibration_plugin/od_calibration_from_standards.py

```diff
@@ -329,15 +329,15 @@
         maximum_od600=max(od600_values),
         minimum_od600=0,
         minimum_voltage=min(voltages),
         maximum_voltage=max(voltages),
         curve_data_=curve_data_,
         curve_type=curve_type,
         voltages=voltages,
-        inferred_od600s=od600_values,
+        od600s=od600_values,
         ir_led_intensity=float(config["od_config"]["ir_led_intensity"]),
         pd_channel=signal_channel,
     )
 
     with local_persistant_storage("od_calibrations") as cache:
         cache[name] = encode(data_blob)
 
@@ -447,15 +447,15 @@
 
 
 def display(name: str | None) -> None:
     from pprint import pprint
 
     def display_from_calibration_blob(data_blob) -> None:
         voltages = data_blob["voltages"]
-        ods = data_blob["inferred_od600s"]
+        ods = data_blob["od600s"]
         name, angle = data_blob["name"], data_blob["angle"]
         click.echo()
         click.echo(click.style(f"Calibration `{name}`", underline=True, bold=True))
         plot_data(
             ods,
             voltages,
             title=f"`{name}`, calibration of {angle}°",
```

## Comparing `od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt` & `od_standards_calibration_plugin-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `od_standards_calibration_plugin-1.0.1.dist-info/METADATA` & `od_standards_calibration_plugin-1.0.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-standards-calibration-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Calibrate OD using a set of standards.
 Home-page: https://github.com/odcambc/od_standards_calibration_plugin
 Author: Chris Macdonald
 Author-email: christian.macdonald@ucsf.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `od_standards_calibration_plugin-1.0.1.dist-info/RECORD` & `od_standards_calibration_plugin-1.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 od_standards_calibration_plugin/__init__.py,sha256=_GKELyAjuHmHfzjj59VIUqAf45yRquASX7gnVyPRXW8,119
-od_standards_calibration_plugin/od_calibration_from_standards.py,sha256=yPTCq3C7NrZ-1x1l4k19vPCOx4HlCj6mwRsHEI5ObQQ,18352
+od_standards_calibration_plugin/od_calibration_from_standards.py,sha256=w2VF4aqeXKwQffzjvB0bXFwgxEg9SJk0-0Rca8MoFy8,18334
 od_standards_calibration_plugin/ui/contrib/jobs/od_standards_calibration_plugin.yaml,sha256=4zxB1ccYllkPNYdMo5hDmgcFlaH64dZIpf-QAnGKpak,137
-od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt,sha256=4cGjN4WDkfnBYIZNxNLrtNoai7jxokShSPCzz-qtFN4,1055
-od_standards_calibration_plugin-1.0.1.dist-info/METADATA,sha256=6cbZARJmHCxyif9wWe3j1aryyppK2Kc6Hy1nU9u761I,1220
-od_standards_calibration_plugin-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-od_standards_calibration_plugin-1.0.1.dist-info/entry_points.txt,sha256=X5ffYTid8S_mCW4n3NKYxt6_sjo1y1xjeCSEWhqz4e4,87
-od_standards_calibration_plugin-1.0.1.dist-info/top_level.txt,sha256=0JZ5WivUVuXYnCe1EUs3mo0BghBx3u2JLwBsa_FW4PI,32
-od_standards_calibration_plugin-1.0.1.dist-info/RECORD,,
+od_standards_calibration_plugin-1.0.2.dist-info/LICENSE.txt,sha256=4cGjN4WDkfnBYIZNxNLrtNoai7jxokShSPCzz-qtFN4,1055
+od_standards_calibration_plugin-1.0.2.dist-info/METADATA,sha256=MN6axE380XJfkliyv1DXvqtIvf0BcWaidnL44KkrKPk,1220
+od_standards_calibration_plugin-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+od_standards_calibration_plugin-1.0.2.dist-info/entry_points.txt,sha256=X5ffYTid8S_mCW4n3NKYxt6_sjo1y1xjeCSEWhqz4e4,87
+od_standards_calibration_plugin-1.0.2.dist-info/top_level.txt,sha256=0JZ5WivUVuXYnCe1EUs3mo0BghBx3u2JLwBsa_FW4PI,32
+od_standards_calibration_plugin-1.0.2.dist-info/RECORD,,
```

