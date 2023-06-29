# Comparing `tmp/dojo_truant-2023.6.15.1.tar.gz` & `tmp/dojo_truant-2023.6.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.15.1.tar", last modified: Thu Jun 15 19:10:10 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.29.0.tar", last modified: Thu Jun 29 18:15:43 2023, max compression
```

## Comparing `dojo_truant-2023.6.15.1.tar` & `dojo_truant-2023.6.29.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/jira_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/jira_product_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:15:43.223659 dojo_truant-2023.6.29.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-29 18:15:43.223659 dojo_truant-2023.6.29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:15:43.223659 dojo_truant-2023.6.29.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/import_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:15:43.223659 dojo_truant-2023.6.29.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-29 18:15:43.000000 dojo_truant-2023.6.29.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-29 18:15:43.000000 dojo_truant-2023.6.29.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:15:43.000000 dojo_truant-2023.6.29.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 18:15:43.000000 dojo_truant-2023.6.29.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 18:15:43.000000 dojo_truant-2023.6.29.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-29 18:15:27.000000 dojo_truant-2023.6.29.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:15:43.223659 dojo_truant-2023.6.29.0/setup.cfg
```

### Comparing `dojo_truant-2023.6.15.1/LICENSE.txt` & `dojo_truant-2023.6.29.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/PKG-INFO` & `dojo_truant-2023.6.29.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.15.1
+Version: 2023.6.29.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.15.1/dojo/__init__.py` & `dojo_truant-2023.6.29.0/dojo/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 from .finding import Finding
 from .stub_finding import Stub_Finding
 
 from .jira_instance import Jira_Instance
 from .jira_product_configuration import Jira_Product_Configuration
 
+from .import_scan import Import_Scan
+
 from .write_chain import write_chain
 
 
 ID_LOOKUPS = {"prod_type": Product_Type,
               "group": Dojo_Group,
               "engagement": Engagement,
               "test_type": Test_Type,
```

### Comparing `dojo_truant-2023.6.15.1/dojo/api.py` & `dojo_truant-2023.6.29.0/dojo/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,33 @@
     _post_endpoint = None
     _type = "Unknown"
     _model_validation = {}
     _obj_iterate = None
     _comp_ignore_keys = ["updated", "created", "prefetch", "target_start", "target_end"]
 
     _id_column = "id"
+    _default_action = None
+    _no_get = False
+    _no_search = False
+    _no_new = False
 
     def __init__(self, **kwargs):
 
         self.logger = logging.getLogger("DAPI")
         self.endpoint = kwargs.get("endpoint", self._endpoint)
         self.post_endpoint = kwargs.get("post_endpoint", self._post_endpoint)
         self.host = kwargs.get("host", None)
         self.type = kwargs.get("type", self._type)
 
         self.allowed_methods = kwargs.get("allowed_methods", self._allowed_methods)
 
         self.logger.debug(kwargs)
 
+        self.kwargs = kwargs
+
         if kwargs.get("token", None) is None:
             if kwargs.get("username", None) is None or kwargs.get("password", None) is None:
                 raise ValueError("I need a token or a username/password combination to work")
             else:
                 self.token = self.get_token(username=kwargs.get("username", None),
                                             password=kwargs.get("password", None)
                                             )
@@ -46,16 +52,15 @@
 
         else:
             self.token = kwargs["token"]
 
         self.data = kwargs.get("data", None)
         self.id = kwargs.get("id", None)
 
-        self.action = kwargs.get("action", None)
-        self.kwargs = kwargs
+        self.action = kwargs.get("action", self._default_action)
 
         if self.action == "get":
 
             self.get_obj()
         elif self.action == "new":
 
             self.new_obj()
@@ -145,41 +150,59 @@
     def get_obj(self):
 
         '''
         Get's the Object
         :return: data
         '''
 
-        obj_data = self.api_call(endpoint=self.endpoint.safe_substitute(id=self.id),
-                                 method="GET")
+        if self.kwargs.get("no_get", self._no_get) is True:
+            obj_data = None
+
+        else:
+            obj_data = self.api_call(endpoint=self.endpoint.safe_substitute(id=self.id),
+                                     method="GET")
 
-        self.logger.debug(obj_data)
+            self.logger.debug(obj_data)
 
         self.data = obj_data
 
     def new_obj(self):
 
         '''
 
         :return: id, data
         '''
 
         id = None
         data = None
 
-        if self.validate_obj(enforce_all=True) is True:
-            self.logger.debug(self.data)
-            data = self.api_call(endpoint=self.post_endpoint,
-                                 method="POST",
-                                 json=self.data)
 
-            if data is not None:
-                id = data[self.kwargs.get("id_column", self._id_column)]
+        if self.kwargs.get("no_new", self._no_new) is True:
+            id = None
+            data = None
         else:
-            self.logger.error("Validation of New Object Failed")
+            post_kwargs = {}
+
+            if self.validate_obj(enforce_all=True) is True:
+                self.logger.debug(self.data)
+                if self.kwargs.get("files", None) is None:
+                    post_kwargs["json"] = self.data
+                else:
+                    post_kwargs["data"] = self.data
+                    post_kwargs["ctype_json"] = False
+                    post_kwargs["accept_json"] = False
+                    post_kwargs["files"] = self.kwargs["files"]
+
+                data = self.api_call(endpoint=self.post_endpoint,
+                                     method="POST", **post_kwargs)
+
+                if data is not None:
+                    id = data[self.kwargs.get("id_column", self._id_column)]
+            else:
+                self.logger.error("Validation of New Object Failed")
 
 
         self.id = id
         self.data = data
 
     def search_for_obj(self):
 
@@ -187,31 +210,36 @@
 
         :return: id, data
         '''
 
         id = None
         data = None
 
-        if self.validate_obj() is True:
-            search_obj_data = self.api_call(endpoint=self.post_endpoint,
-                                            method="GET",
-                                            params=self.data)
-
-            self.logger.debug(search_obj_data)
-
-            if search_obj_data["count"] > 0:
-                # I've found an object
-                data = pyjq.first(self.kwargs.get("obj_iterate", self._obj_iterate),
-                                  search_obj_data)
-                id = data[self.kwargs.get("id_column", self._id_column)]
-            else:
-                self.logger.warning("Unable to find object with given terms.")
-
+        if self.kwargs.get("no_search", self._no_search) is True:
+            id = None
+            data = None
         else:
-            self.logger.error("Unable to process search terms")
+
+            if self.validate_obj() is True:
+                search_obj_data = self.api_call(endpoint=self.post_endpoint,
+                                                method="GET",
+                                                params=self.data)
+
+                self.logger.debug(search_obj_data)
+
+                if search_obj_data["count"] > 0:
+                    # I've found an object
+                    data = pyjq.first(self.kwargs.get("obj_iterate", self._obj_iterate),
+                                      search_obj_data)
+                    id = data[self.kwargs.get("id_column", self._id_column)]
+                else:
+                    self.logger.warning("Unable to find object with given terms.")
+
+            else:
+                self.logger.error("Unable to process search terms")
 
         self.id = id
         self.data = data
 
 
     def validate_obj(self, enforce_all=False):
 
@@ -330,14 +358,18 @@
         if kwargs.get("accept_json", True) is True:
             request_kwargs["headers"] = {"accept": "application/json",
                                          **request_kwargs.get("headers", {})}
 
         if kwargs.get("ctype_json", True) is True:
             request_kwargs["headers"] = {"Content-Type": "application/json",
                                          **request_kwargs.get("headers", {})}
+        elif kwargs.get("ctype_form", False) is True:
+            request_kwargs["headers"] = {"Content-Type": "multipart/form-data",
+                                         **request_kwargs.get("headers", {})}
+
 
 
         for x in ["params", "data", "json", "headers", "cookies", "files", "timeout"]:
             if x in kwargs.keys():
                 if x not in ["headers", "params"]:
                     # Not a dictionary type
                     request_kwargs[x] = kwargs[x]
@@ -357,10 +389,11 @@
             else:
                 if return_json is True:
                     response = this_request.json()
                 else:
                     response = this_request.text
 
             self.logger.debug(this_request.headers)
-            self.logger.debug(this_request.status_code)
+            self.logger.info(this_request.status_code)
+            self.logger.debug(this_request.text)
 
         return response
```

### Comparing `dojo_truant-2023.6.15.1/dojo/development_environment.py` & `dojo_truant-2023.6.29.0/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/dojo_group.py` & `dojo_truant-2023.6.29.0/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/engagement.py` & `dojo_truant-2023.6.29.0/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/finding.py` & `dojo_truant-2023.6.29.0/dojo/finding.py`

 * *Files 12% similar despite different names*

```diff
@@ -135,26 +135,51 @@
     _type = "finding"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.logger = logging.getLogger("DAPI.Finding")
 
-    #def add_note(self, note_text):
+        # def add_note(self, note_text):
 
         '''
         Adds a Note to a Finding
         '''
 
-    #def add_tag(self, tag):
+    def get_tags(self):
+
+        '''
+        Return list of tags
+        '''
+
+        existing_tag_endpoint = "api/v2/findings/{}/tags/".format(self.id)
+
+        update_tag_json = self.api_call(endpoint=existing_tag_endpoint,
+                                        method="GET",
+                                        token=True,
+                                        return_json=True)
+
+        return update_tag_json.get("tags", list())
+
+    def add_tag(self, tag=None):
 
         '''
         Adds a Tag to a Finding
         '''
 
+        existing_tag_endpoint = "api/v2/findings/{}/tags/".format(self.id)
+
+        tag_json = {"tags":[tag]}
+
+        update_tag_json = self.api_call(endpoint=existing_tag_endpoint,
+                                        method="POST",
+                                        token=True,
+                                        json=tag_json,
+                                        return_json=True)
+
     def add_meta(self, name=None, value=None, overwrite=False):
 
         '''
         Adds a Metadata Object to this Finding
         '''
 
         existing_metadata_endpoint = "api/v2/findings/{}/metadata/".format(self.id)
```

### Comparing `dojo_truant-2023.6.15.1/dojo/jira_instance.py` & `dojo_truant-2023.6.29.0/dojo/jira_instance.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/jira_product_configuration.py` & `dojo_truant-2023.6.29.0/dojo/jira_product_configuration.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/product.py` & `dojo_truant-2023.6.29.0/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/product_type.py` & `dojo_truant-2023.6.29.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/stub_finding.py` & `dojo_truant-2023.6.29.0/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/test.py` & `dojo_truant-2023.6.29.0/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/test_type.py` & `dojo_truant-2023.6.29.0/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo/write_chain.py` & `dojo_truant-2023.6.29.0/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.15.1/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.29.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.15.1
+Version: 2023.6.29.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.15.1/pyproject.toml` & `dojo_truant-2023.6.29.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.15.1"
+version = "2023.6.29.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

