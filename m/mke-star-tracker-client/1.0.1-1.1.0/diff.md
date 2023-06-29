# Comparing `tmp/mke_star_tracker_client-1.0.1.tar.gz` & `tmp/mke_star_tracker_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_star_tracker_client-1.0.1.tar", last modified: Thu Jun 29 09:35:42 2023, max compression
+gzip compressed data, was "mke_star_tracker_client-1.1.0.tar", last modified: Thu Jun 29 15:20:15 2023, max compression
```

## Comparing `mke_star_tracker_client-1.0.1.tar` & `mke_star_tracker_client-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:35:42.407960 mke_star_tracker_client-1.0.1/
--rw-rw-rw-   0        0        0    35823 2022-06-30 13:00:25.000000 mke_star_tracker_client-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1249 2023-06-29 09:35:42.407960 mke_star_tracker_client-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-01-10 18:58:33.000000 mke_star_tracker_client-1.0.1/README.rst
--rw-rw-rw-   0        0        0      968 2023-06-29 09:35:42.411869 mke_star_tracker_client-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      372 2023-01-15 15:05:16.000000 mke_star_tracker_client-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:35:42.377878 mke_star_tracker_client-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 09:35:42.396088 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client/
--rw-rw-rw-   0        0        0       21 2023-06-29 09:33:32.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client/__init__.py
--rw-rw-rw-   0        0        0     5672 2023-06-29 09:32:54.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client/star_tracker_client.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:35:42.406103 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/
--rw-rw-rw-   0        0        0     1249 2023-06-29 09:35:41.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-29 09:35:42.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:35:41.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-29 09:35:41.000000 mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 15:20:15.571983 mke_star_tracker_client-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2022-06-30 13:00:25.000000 mke_star_tracker_client-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1249 2023-06-29 15:20:15.571983 mke_star_tracker_client-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-01-10 18:58:33.000000 mke_star_tracker_client-1.1.0/README.rst
+-rw-rw-rw-   0        0        0      968 2023-06-29 15:20:15.572983 mke_star_tracker_client-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      372 2023-01-15 15:05:16.000000 mke_star_tracker_client-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:20:15.562009 mke_star_tracker_client-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 15:20:15.566996 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client/
+-rw-rw-rw-   0        0        0       21 2023-06-29 15:18:54.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client/__init__.py
+-rw-rw-rw-   0        0        0     5424 2023-06-29 15:18:17.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client/star_tracker_client.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:20:15.570985 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/
+-rw-rw-rw-   0        0        0     1249 2023-06-29 15:20:15.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-29 15:20:15.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:20:15.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-29 15:20:15.000000 mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/top_level.txt
```

### Comparing `mke_star_tracker_client-1.0.1/LICENSE` & `mke_star_tracker_client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_star_tracker_client-1.0.1/PKG-INFO` & `mke_star_tracker_client-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_star_tracker_client
-Version: 1.0.1
+Version: 1.1.0
 Summary: MeerKAT Extension (MKE) star tracker optical camera system client
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke_star_tracker_client
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke_star_tracker_client/issues
 Platform: UNKNOWN
```

### Comparing `mke_star_tracker_client-1.0.1/setup.cfg` & `mke_star_tracker_client-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_star_tracker_client-1.0.1/src/mke_star_tracker_client/star_tracker_client.py` & `mke_star_tracker_client-1.1.0/src/mke_star_tracker_client/star_tracker_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,38 +43,28 @@
             route += f'/{self.ard_com}'
         ret = self._get(route).json()
         return ret['ret']
 
 
 
     def ard_flap_open(self):
-        cmd = 'MOVE_OPEN' 
-        res = self._get_ard(cmd)
-        return res == cmd
+        return self._get_ard('MOVE_OPEN' )
 
     def ard_flap_close(self):
-        cmd = 'MOVE_CLOSE' 
-        res = self._get_ard(cmd)
-        return res == cmd
+        return self._get_ard('MOVE_CLOSE' )
 
     def ard_flap_stop(self):
-        cmd = 'MOVE_STOP' 
-        res = self._get_ard(cmd)
-        return res == 'STOP'
+        return self._get_ard('MOVE_STOP')
 
 
     def ard_power_on(self):
-        cmd = 'CAM_ON' 
-        res = self._get_ard(cmd)
-        return res == 'SWITCH1 ON'
+        return self._get_ard('CAM_ON' )
 
     def ard_power_off(self):
-        cmd = 'CAM_OFF' 
-        res = self._get_ard(cmd)
-        return res == 'SWITCH1 OFF'
+        return self._get_ard('CAM_OFF' )
 
 
     def ard_state_flap(self):
         return self._get_ard('STATE_FLAP')
 
     def ard_state_version(self):
         return self._get_ard('STATE_VERSION')
```

### Comparing `mke_star_tracker_client-1.0.1/src/mke_star_tracker_client.egg-info/PKG-INFO` & `mke_star_tracker_client-1.1.0/src/mke_star_tracker_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-star-tracker-client
-Version: 1.0.1
+Version: 1.1.0
 Summary: MeerKAT Extension (MKE) star tracker optical camera system client
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke_star_tracker_client
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke_star_tracker_client/issues
 Platform: UNKNOWN
```

