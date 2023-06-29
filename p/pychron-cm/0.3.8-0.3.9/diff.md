# Comparing `tmp/pychron-cm-0.3.8.tar.gz` & `tmp/pychron-cm-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychron-cm-0.3.8.tar", last modified: Thu Nov  4 17:03:44 2021, max compression
+gzip compressed data, was "/Users/ross/Programming/PychronLabsLLC/pcm/dist/tmp7w410v7r/pychron-cm-0.3.9.tar", last modified: Thu Nov  4 17:15:27 2021, max compression
```

## Comparing `pychron-cm-0.3.8.tar` & `pychron-cm-0.3.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      786 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/pcm/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6825 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/pcm/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/alt_config.xml.template
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/arar_constants.ini.template
--rw-r--r--   0 runner    (1001) docker     (121)      785 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/canvas.xml.template
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/canvas.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/canvas_config.xml.template
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/defaults.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/experiment_defaults.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)      275 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/extraction.template
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/extractionline.ini.template
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/general.ini.template
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/initialization.xml.template
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/launcher_mac.template
--rw-r--r--   0 runner    (1001) docker     (121)      538 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/launcher_mac_conda.template
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/launcher_pc.template
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/procedure.template
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/startup_tests.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/system_monitor.cfg.template
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/unknown.template
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/update.ini.template
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/templates/valves.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pcm/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/pychron_cm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-11-04 17:03:44.000000 pychron-cm-0.3.8/pychron_cm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-04 17:03:44.028690 pychron-cm-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-11-04 17:03:36.000000 pychron-cm-0.3.8/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/
+-rw-r--r--   0 ross       (501) staff       (20)     1164 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/PKG-INFO
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     1164 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1102 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)       37 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/entry_points.txt
+-rw-r--r--   0 ross       (501) staff       (20)       13 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)        4 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pychron_cm.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)    11357 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      118 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       32 2021-11-04 17:00:07.000000 pychron-cm-0.3.9/MANIFEST.in
+-rw-r--r--   0 ross       (501) staff       (20)      786 2021-10-31 14:22:51.000000 pychron-cm-0.3.9/README.md
+-rw-r--r--   0 ross       (501) staff       (20)     1703 2021-11-04 17:15:13.000000 pychron-cm-0.3.9/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pcm/
+-rw-r--r--   0 ross       (501) staff       (20)     1176 2021-11-04 16:05:57.000000 pychron-cm-0.3.9/pcm/render.py
+-rw-r--r--   0 ross       (501) staff       (20)     1819 2021-11-04 16:13:45.000000 pychron-cm-0.3.9/pcm/util.py
+-rw-r--r--   0 ross       (501) staff       (20)      796 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     6825 2021-11-04 16:13:45.000000 pychron-cm-0.3.9/pcm/cli.py
+-rw-r--r--   0 ross       (501) staff       (20)     1281 2021-11-04 16:27:38.000000 pychron-cm-0.3.9/pcm/requirements.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/pcm/templates/
+-rw-r--r--   0 ross       (501) staff       (20)      538 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/launcher_mac_conda.template
+-rw-r--r--   0 ross       (501) staff       (20)       25 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/system_monitor.cfg.template
+-rw-r--r--   0 ross       (501) staff       (20)      424 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/procedure.template
+-rw-r--r--   0 ross       (501) staff       (20)     1958 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/initialization.xml.template
+-rw-r--r--   0 ross       (501) staff       (20)      140 2021-11-02 06:17:26.000000 pychron-cm-0.3.9/pcm/templates/update.ini.template
+-rw-r--r--   0 ross       (501) staff       (20)      785 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/canvas.xml.template
+-rw-r--r--   0 ross       (501) staff       (20)      182 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/extractionline.ini.template
+-rw-r--r--   0 ross       (501) staff       (20)     1298 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/defaults.yaml.template
+-rw-r--r--   0 ross       (501) staff       (20)      261 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/alt_config.xml.template
+-rw-r--r--   0 ross       (501) staff       (20)      199 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/experiment_defaults.yaml.template
+-rw-r--r--   0 ross       (501) staff       (20)       84 2021-11-02 06:09:04.000000 pychron-cm-0.3.9/pcm/templates/general.ini.template
+-rw-r--r--   0 ross       (501) staff       (20)       37 2021-11-03 04:25:10.000000 pychron-cm-0.3.9/pcm/templates/arar_constants.ini.template
+-rw-r--r--   0 ross       (501) staff       (20)      275 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/extraction.template
+-rw-r--r--   0 ross       (501) staff       (20)      551 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/valves.yaml.template
+-rw-r--r--   0 ross       (501) staff       (20)      693 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/canvas.yaml.template
+-rw-r--r--   0 ross       (501) staff       (20)     2417 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/unknown.template
+-rw-r--r--   0 ross       (501) staff       (20)      319 2021-10-31 13:24:40.000000 pychron-cm-0.3.9/pcm/templates/launcher_mac.template
+-rw-r--r--   0 ross       (501) staff       (20)      560 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/startup_tests.yaml.template
+-rw-r--r--   0 ross       (501) staff       (20)      261 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/canvas_config.xml.template
+-rw-r--r--   0 ross       (501) staff       (20)      580 2021-10-18 21:32:56.000000 pychron-cm-0.3.9/pcm/templates/launcher_pc.template
+-rw-r--r--   0 ross       (501) staff       (20)     7247 2021-11-04 17:11:12.000000 pychron-cm-0.3.9/pcm/func.py
+-rw-r--r--   0 ross       (501) staff       (20)       38 2021-11-04 17:15:27.000000 pychron-cm-0.3.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pychron-cm-0.3.8/LICENSE` & `pychron-cm-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/PKG-INFO` & `pychron-cm-0.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychron-cm
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pychron configuration manager
 Home-page: https://github.com/PychronLabsLLC/pcm
 Author: Jake Ross
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pychron-cm-0.3.8/README.md` & `pychron-cm-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/__init__.py` & `pychron-cm-0.3.9/pcm/__init__.py`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/cli.py` & `pychron-cm-0.3.9/pcm/cli.py`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/func.py` & `pychron-cm-0.3.9/pcm/func.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     user_file = os.path.join(root, "users.yaml")
     t = {
         "users": [
             "root",
         ],
         "last_login": "root",
     }
-    util.write(user_file, t, yaml.dumps(t))
+    util.write(user_file, yaml.dumps(t))
 
     environment_file = os.path.join(root, "environments.yaml")
     pe = os.path.join(HOME, env)
     t = {
         "env": pe,
         "envs": [
             pe,
```

### Comparing `pychron-cm-0.3.8/pcm/render.py` & `pychron-cm-0.3.9/pcm/render.py`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/requirements.py` & `pychron-cm-0.3.9/pcm/requirements.py`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/canvas.xml.template` & `pychron-cm-0.3.9/pcm/templates/canvas.xml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/canvas.yaml.template` & `pychron-cm-0.3.9/pcm/templates/canvas.yaml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/defaults.yaml.template` & `pychron-cm-0.3.9/pcm/templates/defaults.yaml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/initialization.xml.template` & `pychron-cm-0.3.9/pcm/templates/initialization.xml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/launcher_mac_conda.template` & `pychron-cm-0.3.9/pcm/templates/launcher_mac_conda.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/launcher_pc.template` & `pychron-cm-0.3.9/pcm/templates/launcher_pc.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/startup_tests.yaml.template` & `pychron-cm-0.3.9/pcm/templates/startup_tests.yaml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/unknown.template` & `pychron-cm-0.3.9/pcm/templates/unknown.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/templates/valves.yaml.template` & `pychron-cm-0.3.9/pcm/templates/valves.yaml.template`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pcm/util.py` & `pychron-cm-0.3.9/pcm/util.py`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/pychron_cm.egg-info/PKG-INFO` & `pychron-cm-0.3.9/pychron_cm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychron-cm
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pychron configuration manager
 Home-page: https://github.com/PychronLabsLLC/pcm
 Author: Jake Ross
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pychron-cm-0.3.8/pychron_cm.egg-info/SOURCES.txt` & `pychron-cm-0.3.9/pychron_cm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pychron-cm-0.3.8/setup.py` & `pychron-cm-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pychron-cm",
-    version="0.3.8",
+    version="0.3.9",
     author="Jake Ross",
     description="Pychron configuration manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PychronLabsLLC/pcm",
     classifiers=[
         "Programming Language :: Python :: 3",
```

