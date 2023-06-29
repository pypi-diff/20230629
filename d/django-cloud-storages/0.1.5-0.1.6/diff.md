# Comparing `tmp/django_cloud_storages-0.1.5.tar.gz` & `tmp/django_cloud_storages-0.1.6.tar.gz`

## Comparing `django_cloud_storages-0.1.5.tar` & `django_cloud_storages-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/cloud_storages/__init__.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/__init__.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_cloud_storages-0.1.6/PKG-INFO
```

### Comparing `django_cloud_storages-0.1.5/requirements.txt` & `django_cloud_storages-0.1.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.5/cloud_storages/utils.py` & `django_cloud_storages-0.1.6/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.5/cloud_storages/backends/appwrite.py` & `django_cloud_storages-0.1.6/cloud_storages/backends/appwrite.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 @deconstructible
 class AppWriteStorage(Storage):
     CHUNK_SIZE = 4 * 1024 * 1024
     MAX_FILE_NAME_LENGTH = 30
     def __init__(self):
+        self.CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT = setting('CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT', False)
         self.APPWRITE_API_KEY = setting('APPWRITE_API_KEY')
         self.APPWRITE_PROJECT_ID = setting('APPWRITE_PROJECT_ID')
         self.APPWRITE_BUCKET_ID = setting('APPWRITE_BUCKET_ID')
         self.APPWRITE_API_ENDPOINT = setting('APPWRITE_API_ENDPOINT', "https://cloud.appwrite.io/v1")
         self.MEDIA_URL = setting('MEDIA_URL')
         
         self.client = Client()
@@ -114,27 +115,28 @@
         available for new content to be written to.
         """
         formatted_name = self.get_valid_name(name)
         new_name = formatted_name
         index = 0
         while(1):
             index += 1
-            if self.exists(new_name):
-                remote_file = self.open(new_name)
-                remote_file.open()
-                content.open()
-                remote_file_data = remote_file.read()
-                content_data = content.read()
-                remote_file.close()
-                content.close()
-                if remote_file_data == content_data:
-                    return (new_name, 'Exists')
-                else:
-                    new_name = self.get_alternative_name(formatted_name, index=index)
-                    continue
+            if self.exists(new_name): # check file existence with file name
+                if not self.CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT:
+                    # check file existence with file's contents
+                    remote_file = self.open(new_name)
+                    remote_file.open()
+                    content.open()
+                    remote_file_data = remote_file.read()
+                    content_data = content.read()
+                    remote_file.close()
+                    content.close()
+                    if remote_file_data == content_data:
+                        return (new_name, 'Exists')
+                new_name = self.get_alternative_name(formatted_name, index=index)
+                continue
             break
         return (new_name, None)
     
     def generate_filename(self, filename):
         """
         Validate the filename by calling get_valid_name() and return a filename
         to be passed to the save() method.
```

### Comparing `django_cloud_storages-0.1.5/cloud_storages/backends/dropbox.py` & `django_cloud_storages-0.1.6/cloud_storages/backends/dropbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 _DEFAULT_TIMEOUT = 100
 _DEFAULT_MODE = 'add'
 
 @deconstructible
 class DropBoxStorage(Storage):
     CHUNK_SIZE = 4 * 1024 * 1024
     def __init__(self):
+        self.CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT = setting('CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT', False)
         self.DROPBOX_OAUTH2_ACCESS_TOKEN = setting('DROPBOX_OAUTH2_ACCESS_TOKEN')
         self.DROPBOX_OAUTH2_REFRESH_TOKEN = setting('DROPBOX_OAUTH2_REFRESH_TOKEN')
         self.DROPBOX_APP_KEY = setting('DROPBOX_APP_KEY')
         self.DROPBOX_APP_SECRET = setting('DROPBOX_APP_SECRET')
         self.DROPBOX_ROOT_PATH = setting('DROPBOX_ROOT_PATH')
         self.MEDIA_URL = setting('MEDIA_URL')
         self.timeout = setting('DROPBOX_TIMEOUT', _DEFAULT_TIMEOUT)
@@ -71,27 +72,28 @@
         available for new content to be written to.
         """
         formatted_name = self.get_valid_name(name)
         new_name = formatted_name
         index = 0
         while(1):
             index += 1
-            if self.exists(new_name):
-                remote_file = self.open(new_name)
-                remote_file.open()
-                content.open()
-                remote_file_data = remote_file.read()
-                content_data = content.read()
-                remote_file.close()
-                content.close()
-                if remote_file_data == content_data:
-                    return (new_name, 'Exists')
-                else:
-                    new_name = self.get_alternative_name(formatted_name, index=index)
-                    continue
+            if self.exists(new_name): # check file existence with file name
+                if not self.CLOUD_STORAGE_CREATE_NEW_IF_SAME_CONTENT:
+                    # check file existence with file's contents
+                    remote_file = self.open(new_name)
+                    remote_file.open()
+                    content.open()
+                    remote_file_data = remote_file.read()
+                    content_data = content.read()
+                    remote_file.close()
+                    content.close()
+                    if remote_file_data == content_data:
+                        return (new_name, 'Exists')
+                new_name = self.get_alternative_name(formatted_name, index=index)
+                continue
             break
         return (new_name, None)
     
     def generate_filename(self, filename):
         """
         Validate the filename by calling get_valid_name() and return a filename
         to be passed to the save() method.
```

### Comparing `django_cloud_storages-0.1.5/.gitignore` & `django_cloud_storages-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.5/LICENSE` & `django_cloud_storages-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-0.1.5/pyproject.toml` & `django_cloud_storages-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "django", "requests", "dropbox", "appwrite"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-cloud-storages"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 description = "Cloud file storages for django."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_cloud_storages-0.1.5/PKG-INFO` & `django_cloud_storages-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

