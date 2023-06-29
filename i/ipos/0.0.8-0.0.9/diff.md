# Comparing `tmp/ipos-0.0.8.tar.gz` & `tmp/ipos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.8.tar", last modified: Tue Jun 27 18:27:10 2023, max compression
+gzip compressed data, was "ipos-0.0.9.tar", last modified: Tue Jun 27 19:20:39 2023, max compression
```

## Comparing `ipos-0.0.8.tar` & `ipos-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.057903 ipos-0.0.8/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.8/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:27:10.057791 ipos-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.056506 ipos-0.0.8/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     5889 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.8/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    23982 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.057613 ipos-0.0.8/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.8/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 18:23:59.000000 ipos-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 18:27:10.057941 ipos-0.0.8/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 19:20:39.692983 ipos-0.0.9/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.9/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 19:20:39.692846 ipos-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 19:20:39.691537 ipos-0.0.9/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 19:20:32.000000 ipos-0.0.9/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     6103 2023-06-27 19:20:32.000000 ipos-0.0.9/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.9/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24490 2023-06-27 19:20:32.000000 ipos-0.0.9/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 19:20:39.692580 ipos-0.0.9/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.9/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 19:20:39.000000 ipos-0.0.9/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 18:28:16.000000 ipos-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 19:20:39.693029 ipos-0.0.9/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.9/setup.py
```

### Comparing `ipos-0.0.8/LICENSE` & `ipos-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.8/PKG-INFO` & `ipos-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.8
+Version: 0.0.9
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.8/README.md` & `ipos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.8/ipos/_modidx.py` & `ipos-0.0.9/ipos/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
                           'ipos.imp.GlobalImport.__enter__': ('core.html#globalimport.__enter__', 'ipos/imp.py'),
                           'ipos.imp.GlobalImport.__exit__': ('core.html#globalimport.__exit__', 'ipos/imp.py'),
                           'ipos.imp.Imp': ('core.html#imp', 'ipos/imp.py'),
                           'ipos.imp.Imp.__enter__': ('core.html#imp.__enter__', 'ipos/imp.py'),
                           'ipos.imp.Imp.__exit__': ('core.html#imp.__exit__', 'ipos/imp.py'),
                           'ipos.imp.Imp.__getitem__': ('core.html#imp.__getitem__', 'ipos/imp.py'),
                           'ipos.imp.Imp.__post_init__': ('core.html#imp.__post_init__', 'ipos/imp.py'),
+                          'ipos.imp.Imp._import': ('core.html#imp._import', 'ipos/imp.py'),
                           'ipos.imp.Imp.load': ('core.html#imp.load', 'ipos/imp.py'),
+                          'ipos.imp.Imp.squash_all_name_errors': ('core.html#imp.squash_all_name_errors', 'ipos/imp.py'),
                           'ipos.imp.ImpItem': ('core.html#impitem', 'ipos/imp.py'),
                           'ipos.imp.ImpItem.__eq__': ('core.html#impitem.__eq__', 'ipos/imp.py'),
                           'ipos.imp.ImpItem.__post_init__': ('core.html#impitem.__post_init__', 'ipos/imp.py'),
                           'ipos.imp.ImpItem.has_alias': ('core.html#impitem.has_alias', 'ipos/imp.py'),
                           'ipos.imp.ImpItem.varname': ('core.html#impitem.varname', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec': ('core.html#impspec', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec.__post_init__': ('core.html#impspec.__post_init__', 'ipos/imp.py'),
```

### Comparing `ipos-0.0.8/ipos/imp.py` & `ipos-0.0.9/ipos/imp.py`

 * *Files 2% similar despite different names*

```diff
@@ -671,15 +671,16 @@
         expected_items = []
         for subspec in self.subspecs:
             expected_items.extend(subspec.expected_items())
         return expected_items
     
     def squash_all_name_errors(self):
         for name in self.all_expected_items():
-            self.squash_name_error(name)        
+            self.squash_name_error(name)    
+        return self    
 
 # %% ../nbs/00_core.ipynb 27
 @dataclass
 class Imp(BaseImp):
     """
     Import Module class.
     
@@ -722,25 +723,36 @@
     fallbacks: Optional[Dict[str, Any]] = field(default_factory=dict, repr=False)
     lazy: Optional[bool] = field(default=True)
     delay: Optional[bool] = field(default=False)
 
     _ : KW_ONLY
     _module: Module = field(init=False, repr=False, default=None)
     _spec: ImpSpec = field(init=False, repr=False, default=None)
+    _squash_name_errors: Optional[bool] = field(default=True)
+    _reload: Optional[bool] = field(default=False)
 
-    def load(self):
+    def _import(self):
+        prev = sys.modules.get(self.name, None)
+        if prev is not None and not self._reload:
+            return self
         self._spec = ImpSpec(self.name, self.nick, self.lazy, self.subspecs, self.fallbacks)
-        self._updates = self._spec._import()              
+        self._updates = self._spec._import()
         self._module = sys.modules[self.name]
         self.update_namespace(self._updates, self.namespace)
+        return self
+
+    def load(self):
+        self._import()
+        if self._squash_name_errors:
+            self.squash_all_name_errors()
+        return self
 
     def __post_init__(self):
         if isinstance(self.fallbacks, dict):
-            self.fallbacks = Fallbacks.from_dict(self.fallbacks)
-            
+            self.fallbacks = Fallbacks.from_dict(self.fallbacks)            
         if not self.delay:
             self.load()
 
     
     
     def __enter__(self):
         """
@@ -781,9 +793,12 @@
         Returns
         -------
         Any
             The attribute from the imported module.
         """
         return getattr(self._module, key, None)
 
+    def squash_all_name_errors(self):
+        self._spec.squash_all_name_errors()
+        return self
```

### Comparing `ipos-0.0.8/ipos.egg-info/PKG-INFO` & `ipos-0.0.9/ipos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.8
+Version: 0.0.9
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.8/settings.ini` & `ipos-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ipos
 lib_name = ipos
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ipos
 nbs_path = nbs
 recursive = True
```

### Comparing `ipos-0.0.8/setup.py` & `ipos-0.0.9/setup.py`

 * *Files identical despite different names*

