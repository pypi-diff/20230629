# Comparing `tmp/lollms-2.1.3.tar.gz` & `tmp/lollms-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.3.tar", last modified: Thu Jun 29 21:38:48 2023, max compression
+gzip compressed data, was "lollms-2.1.4.tar", last modified: Thu Jun 29 21:41:08 2023, max compression
```

## Comparing `lollms-2.1.3.tar` & `lollms-2.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:38:48.810864 lollms-2.1.3/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.3/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:38:48.809864 lollms-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 21:38:48.792864 lollms-2.1.3/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.3/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:38:48.807863 lollms-2.1.3/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.3/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.3/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.3/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:38:48.808864 lollms-2.1.3/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.3/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30411 2023-06-29 21:21:16.000000 lollms-2.1.3/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.3/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.3/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7237 2023-06-29 21:22:56.000000 lollms-2.1.3/lollms/main_config.py
--rw-rw-rw-   0        0        0    13160 2023-06-29 21:38:33.000000 lollms-2.1.3/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.3/lollms/personality.py
--rw-rw-rw-   0        0        0    32662 2023-06-29 21:25:36.000000 lollms-2.1.3/lollms/server.py
--rw-rw-rw-   0        0        0    11026 2023-06-29 21:24:59.000000 lollms-2.1.3/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.3/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:38:48.806861 lollms-2.1.3/lollms.egg-info/
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 21:38:48.000000 lollms-2.1.3/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:38:48.810864 lollms-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 21:38:44.000000 lollms-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:41:08.758619 lollms-2.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:41:08.757616 lollms-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 21:41:08.736608 lollms-2.1.4/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.4/lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:41:08.754608 lollms-2.1.4/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.4/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.4/lollms/binding.py
+-rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.4/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:41:08.756610 lollms-2.1.4/lollms/configs/
+-rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.4/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0    30411 2023-06-29 21:21:16.000000 lollms-2.1.4/lollms/console.py
+-rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.4/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.4/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.4/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13160 2023-06-29 21:38:33.000000 lollms-2.1.4/lollms/paths.py
+-rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.4/lollms/personality.py
+-rw-rw-rw-   0        0        0    32662 2023-06-29 21:25:36.000000 lollms-2.1.4/lollms/server.py
+-rw-rw-rw-   0        0        0    11026 2023-06-29 21:24:59.000000 lollms-2.1.4/lollms/settings.py
+-rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.4/lollms/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:41:08.753611 lollms-2.1.4/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 21:41:08.000000 lollms-2.1.4/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:41:08.758619 lollms-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-06-29 21:41:03.000000 lollms-2.1.4/setup.py
```

### Comparing `lollms-2.1.3/LICENSE` & `lollms-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/PKG-INFO` & `lollms-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.3/README.md` & `lollms-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/assets/logo.png` & `lollms-2.1.4/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/binding.py` & `lollms-2.1.4/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/config.py` & `lollms-2.1.4/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/configs/config.yaml` & `lollms-2.1.4/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/console.py` & `lollms-2.1.4/lollms/console.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/helpers.py` & `lollms-2.1.4/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/langchain_integration.py` & `lollms-2.1.4/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/main_config.py` & `lollms-2.1.4/lollms/main_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         
 
     @staticmethod
     def autoload(lollms_paths:LollmsPaths, config_path:str=None):
         # Configuration loading part
         original_cfg_path = lollms_paths.default_cfg_path
         if config_path is None:
-            local = lollms_paths.personal_configuration_path / lollms_paths.tool_prefix+"local_config.yaml"
+            local = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
             if not local.exists():
                 shutil.copy(original_cfg_path, local)
             cfg_path = local
         else:
             cfg_path = config_path
 
         if cfg_path.exists():
```

### Comparing `lollms-2.1.3/lollms/paths.py` & `lollms-2.1.4/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/personality.py` & `lollms-2.1.4/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/server.py` & `lollms-2.1.4/lollms/server.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/settings.py` & `lollms-2.1.4/lollms/settings.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms/types.py` & `lollms-2.1.4/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.3/lollms.egg-info/PKG-INFO` & `lollms-2.1.4/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.3/setup.py` & `lollms-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.3",
+    version="2.1.4",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

