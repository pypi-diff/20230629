# Comparing `tmp/lollms-2.1.1.tar.gz` & `tmp/lollms-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.1.tar", last modified: Thu Jun 29 21:34:46 2023, max compression
+gzip compressed data, was "lollms-2.1.2.tar", last modified: Thu Jun 29 21:36:51 2023, max compression
```

## Comparing `lollms-2.1.1.tar` & `lollms-2.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:34:46.959804 lollms-2.1.1/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:34:46.958804 lollms-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 21:34:46.938806 lollms-2.1.1/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.1/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:34:46.956804 lollms-2.1.1/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.1/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.1/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.1/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:34:46.957807 lollms-2.1.1/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.1/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30411 2023-06-29 21:21:16.000000 lollms-2.1.1/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.1/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.1/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7237 2023-06-29 21:22:56.000000 lollms-2.1.1/lollms/main_config.py
--rw-rw-rw-   0        0        0    13153 2023-06-29 21:34:03.000000 lollms-2.1.1/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.1/lollms/personality.py
--rw-rw-rw-   0        0        0    32662 2023-06-29 21:25:36.000000 lollms-2.1.1/lollms/server.py
--rw-rw-rw-   0        0        0    11026 2023-06-29 21:24:59.000000 lollms-2.1.1/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.1/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:34:46.955806 lollms-2.1.1/lollms.egg-info/
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 21:34:46.000000 lollms-2.1.1/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:34:46.959804 lollms-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 21:34:34.000000 lollms-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:36:51.446695 lollms-2.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:36:51.446695 lollms-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 21:36:51.427685 lollms-2.1.2/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.2/lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:36:51.443693 lollms-2.1.2/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.2/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.2/lollms/binding.py
+-rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.2/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:36:51.445695 lollms-2.1.2/lollms/configs/
+-rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.2/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0    30411 2023-06-29 21:21:16.000000 lollms-2.1.2/lollms/console.py
+-rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.2/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.2/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7237 2023-06-29 21:22:56.000000 lollms-2.1.2/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13155 2023-06-29 21:36:44.000000 lollms-2.1.2/lollms/paths.py
+-rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.2/lollms/personality.py
+-rw-rw-rw-   0        0        0    32662 2023-06-29 21:25:36.000000 lollms-2.1.2/lollms/server.py
+-rw-rw-rw-   0        0        0    11026 2023-06-29 21:24:59.000000 lollms-2.1.2/lollms/settings.py
+-rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.2/lollms/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:36:51.442694 lollms-2.1.2/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 21:36:51.000000 lollms-2.1.2/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:36:51.446695 lollms-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-06-29 21:36:48.000000 lollms-2.1.2/setup.py
```

### Comparing `lollms-2.1.1/LICENSE` & `lollms-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/PKG-INFO` & `lollms-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.1/README.md` & `lollms-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/assets/logo.png` & `lollms-2.1.2/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/binding.py` & `lollms-2.1.2/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/config.py` & `lollms-2.1.2/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/configs/config.yaml` & `lollms-2.1.2/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/console.py` & `lollms-2.1.2/lollms/console.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/helpers.py` & `lollms-2.1.2/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/langchain_integration.py` & `lollms-2.1.2/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/main_config.py` & `lollms-2.1.2/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/paths.py` & `lollms-2.1.2/lollms/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         else:
             # Pull the repository if it already exists
             ASCIIColors.info("Personalities zoo found in your personal space.\nPulling last personalities zoo")
             subprocess.run(["git", "-C", self.bindings_zoo_path, "pull"])            
 
 
     def copy_default_config(self):
-        local_config_path = self.personal_configuration_path / self.tool_prefix+"local_config.yaml"
+        local_config_path = self.personal_configuration_path / f"{self.tool_prefix}local_config.yaml"
         if not local_config_path.exists():
             shutil.copy(self.default_cfg_path, str(local_config_path))
 
     def resetPaths(self, force_local=None):
         global_paths_cfg_path = Path(f"./{self.tool_prefix}global_paths_cfg.yaml")
         
         if force_local is None:
```

### Comparing `lollms-2.1.1/lollms/personality.py` & `lollms-2.1.2/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/server.py` & `lollms-2.1.2/lollms/server.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/settings.py` & `lollms-2.1.2/lollms/settings.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms/types.py` & `lollms-2.1.2/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.1/lollms.egg-info/PKG-INFO` & `lollms-2.1.2/lollms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.1/setup.py` & `lollms-2.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.1",
+    version="2.1.2",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

