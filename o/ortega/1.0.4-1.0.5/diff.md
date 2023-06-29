# Comparing `tmp/ortega-1.0.4.tar.gz` & `tmp/ortega-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortega-1.0.4.tar", last modified: Mon Jun 19 03:00:36 2023, max compression
+gzip compressed data, was "ortega-1.0.5.tar", last modified: Thu Jun 29 17:25:11 2023, max compression
```

## Comparing `ortega-1.0.4.tar` & `ortega-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.054205 ortega-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 03:00:25.000000 ortega-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-19 03:00:36.054205 ortega-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 03:00:25.000000 ortega-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.050204 ortega-1.0.4/ortega/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/STPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/ortega.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.050204 ortega-1.0.4/ortega.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 03:00:36.000000 ortega-1.0.4/ortega.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 03:00:36.054205 ortega-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 03:00:25.000000 ortega-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 17:24:56.000000 ortega-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 17:25:11.406441 ortega-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-29 17:24:56.000000 ortega-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/ortega/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/STPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27324 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/ortega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-29 17:24:56.000000 ortega-1.0.5/ortega/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:25:11.406441 ortega-1.0.5/ortega.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 17:25:11.000000 ortega-1.0.5/ortega.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:25:11.406441 ortega-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 17:24:56.000000 ortega-1.0.5/setup.py
```

### Comparing `ortega-1.0.4/LICENSE` & `ortega-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ortega-1.0.4/README.md` & `ortega-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ortega-1.0.4/ortega/STPoint.py` & `ortega-1.0.5/ortega/STPoint.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.4/ortega/ellipses.py` & `ortega-1.0.5/ortega/ellipses.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.4/ortega/ortega.py` & `ortega-1.0.5/ortega/ortega.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
     df['diff_direction'] = df['P2_direction'] - df['P1_direction']
     df['diff_direction'] = df['diff_direction'].apply(math.cos)
     return df
 
 
 def interaction_compute_time_diff(df:pd.DataFrame):
-    df['diff_time'] = (df['P2_t_start'] - df['P1_t_start'])/ pd.Timedelta(hours=1)
+    df['diff_time'] = (df['P2_t_start'] - df['P1_t_start'])/ pd.Timedelta(minutes=1)
     return df
 
 
 class ORTEGA:
     # ORTEGA is the main class for interaction analysis, users need to initialize this object at the very beginning
     def __init__(
             self,
@@ -500,38 +500,40 @@
         """
         self.ellipses_list = self.__get_ellipse_list(self.df1, self.df2)  # all ellipses for two objects
         self.ellipses_list_id1 = [i for i in self.ellipses_list if i.pid == self.id1]
         self.ellipses_list_id2 = [i for i in self.ellipses_list if i.pid == self.id2]
         # these do not exclude large PPAs! Only after __get_spatiotemporal_intersect_pairs() we exclude large PPAs
         print(datetime.now(), 'Initialization success!')
 
-    def continues_analysis(self):
+    def interaction_analysis(self):
         spatial_pairs = self.__get_spatial_intersect_pairs()
         all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
 
         if not all_intersection_pairs:
             print(datetime.now(), 'Complete! No interaction found!')
-            return None
+            return None, None, None
         else:
+            print(datetime.now(), f'Complete! {len(all_intersection_pairs)} pairs of intersecting PPAs found!')
 
             # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
             df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
 
             # compute duration of interaction and output as a dataframe - df_duration
             print(datetime.now(), 'Compute continues events...')
             df_continues = check_continuous(df_all_intersection_pairs, self.id1, self.id2)
+            print(datetime.now(), f'Complete! {df_continues.shape[0]} interaction events identified!')
             if df_continues.shape[0] != 0:
-                return df_continues
+                return all_intersection_pairs, df_all_intersection_pairs, df_continues
             else:
-                return None
+                return None, None, None
 
-    def interaction_analysis(self):
+    def interaction_analysis2(self):
 
         print(datetime.now(), 'Implement interaction analysis...')
         # get list of intersecting Ellipse objects - all_intersection_pairs
         # all_intersection_pairs = self.__get_spatiotemporal_intersect_pairs()
         spatial_pairs = self.__get_spatial_intersect_pairs()
         all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
```

### Comparing `ortega-1.0.4/ortega/visualization.py` & `ortega-1.0.5/ortega/visualization.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.4/setup.py` & `ortega-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name='ortega',
-        version='1.0.4',
+        version='1.0.5',
         author='MOVE lab@UCSB',
         author_email="rongxiangsu@ucsb.edu",
         packages=["ortega"],
         url='https://github.com/move-ucsb/ORTEGA',
         license='MIT',
         description='ORTEGA',
         install_requires=[
```

