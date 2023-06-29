# Comparing `tmp/lektor-chameleon-0.6.1.tar.gz` & `tmp/lektor-chameleon-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-chameleon-0.6.1.tar", last modified: Wed Dec  1 19:30:35 2021, max compression
+gzip compressed data, was "lektor-chameleon-0.7.tar", last modified: Thu Jun 29 18:21:23 2023, max compression
```

## Comparing `lektor-chameleon-0.6.1.tar` & `lektor-chameleon-0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2021-12-01 19:30:35.750826 lektor-chameleon-0.6.1/
--rw-r--r--   0 uyar      (1000) uyar      (1000)      554 2021-12-01 19:28:10.000000 lektor-chameleon-0.6.1/CHANGELOG.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1496 2021-12-01 15:53:38.000000 lektor-chameleon-0.6.1/LICENSE.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)      179 2021-12-01 15:53:38.000000 lektor-chameleon-0.6.1/MANIFEST.in
--rw-r--r--   0 uyar      (1000) uyar      (1000)     3725 2021-12-01 19:30:35.750826 lektor-chameleon-0.6.1/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1857 2021-12-01 17:46:04.000000 lektor-chameleon-0.6.1/README.rst
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2021-12-01 19:30:35.750826 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     3725 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)      319 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/SOURCES.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/dependency_links.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       63 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/entry_points.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       10 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/requires.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2021-12-01 19:30:35.000000 lektor-chameleon-0.6.1/lektor_chameleon.egg-info/top_level.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     3104 2021-12-01 19:18:11.000000 lektor-chameleon-0.6.1/lektor_chameleon.py
--rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2021-12-01 19:30:35.750826 lektor-chameleon-0.6.1/setup.cfg
--rw-r--r--   0 uyar      (1000) uyar      (1000)      962 2021-12-01 19:27:24.000000 lektor-chameleon-0.6.1/setup.py
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.395638 lektor-chameleon-0.7/
+-rw-------   0 uyar      (1000) uyar      (1000)     1496 2023-06-29 18:01:38.000000 lektor-chameleon-0.7/LICENSE.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     4181 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)     1486 2023-06-29 18:07:38.000000 lektor-chameleon-0.7/README.rst
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/lektor_chameleon/
+-rw-------   0 uyar      (1000) uyar      (1000)     3156 2023-06-29 18:14:47.000000 lektor-chameleon-0.7/lektor_chameleon/__init__.py
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/lektor_chameleon.egg-info/
+-rw-------   0 uyar      (1000) uyar      (1000)     4181 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)      308 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/SOURCES.txt
+-rw-------   0 uyar      (1000) uyar      (1000)        1 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/dependency_links.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       62 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/entry_points.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       79 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/requires.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       17 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/top_level.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     1377 2023-06-29 18:04:25.000000 lektor-chameleon-0.7/pyproject.toml
+-rw-------   0 uyar      (1000) uyar      (1000)       38 2023-06-29 18:21:23.395638 lektor-chameleon-0.7/setup.cfg
```

### Comparing `lektor-chameleon-0.6.1/LICENSE.txt` & `lektor-chameleon-0.7/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2018-2019 H. Turgut Uyar <uyar@tekir.org>
+Copyright 2018-2023 H. Turgut Uyar <uyar@tekir.org>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `lektor-chameleon-0.6.1/lektor_chameleon.py` & `lektor-chameleon-0.7/lektor_chameleon/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# Copyright (C) 2018-2021 H. Turgut Uyar <uyar@tekir.org>
+# Copyright (C) 2018-2023 H. Turgut Uyar <uyar@tekir.org>
 #
-# lektor-chameleon is released under the BSD license. Read the included
-# LICENSE.txt file for details.
+# lektor-chameleon is released under the BSD license.
+# Read the included LICENSE.txt file for details.
 
 from functools import partial
 
 from chameleon import PageTemplateLoader
 from chameleon.loader import TemplateLoader
 from lektor.context import get_ctx
-from lektor.pluginsystem import Plugin, get_plugin
+from lektor.pluginsystem import Plugin
 from markupsafe import Markup
 
 
-_CONTEXT_FILTERS = {"url", "asseturl", "markdown"}
+_CONTEXT_FILTERS = {
+    "url", "asseturl", "markdown",
+}
+
 _STR_FILTERS = {
-    "capitalize",
-    "center",
-    "indent",
-    "length",
-    "lower",
-    "replace",
-    "title",
-    "trim",
-    "truncate",
-    "upper",
-    "wordcount",
-    "wordwrap",
+    "capitalize", "center", "indent", "length", "lower", "replace", "title",
+    "trim", "truncate", "upper", "wordcount", "wordwrap",
+}
+
+_JINJA_ENV_FILTERS = {
+    "attr", "replace", "truncate", "wordwrap",
 }
-_JINJA_ENV_FILTERS = {"attr", "replace", "truncate", "wordwrap"}
 
 
 class Filter:
     def __init__(self, name, func):
         self.name = name
         self.func = func
         self.ctx = self.name in _CONTEXT_FILTERS
@@ -50,15 +46,16 @@
 
 chameleon_load = TemplateLoader.load
 
 
 def load_template(self, filename, *args, **kwargs):
     ctx = get_ctx()
     pt_ext = self.__class__.file_ext
-    if (pt_ext is not None) and (filename == ctx.source.datamodel.id + ".html"):
+    if (pt_ext is not None) and \
+            (filename == ctx.source.datamodel.id + ".html"):
         filename = ctx.source.datamodel.id + pt_ext
     template = chameleon_load(self, filename, *args, **kwargs)
     ctx.record_dependency(template.filename)
     return template
 
 
 def render_template(self, name, pad=None, this=None, values=None, alt=None):
@@ -87,15 +84,17 @@
             TemplateLoader.load = load_template
 
     def on_setup_env(self, **extra):
         if not self.enabled:
             return
 
         template_paths = self.env.jinja_env.loader.searchpath
-        self.env.chameleon_loader = PageTemplateLoader(template_paths, auto_reload=True)
+        self.env.chameleon_loader = PageTemplateLoader(template_paths,
+                                                       auto_reload=True)
 
-        filters = {n: Filter(n, f) for n, f in self.env.jinja_env.filters.items()}
+        filters = {n: Filter(n, f)
+                   for n, f in self.env.jinja_env.filters.items()}
         for f_name in _JINJA_ENV_FILTERS:
             filters[f_name] = filters[f_name](self.env.jinja_env)
         self.env.chameleon_filters = filters
 
         self.env.__class__.render_template = render_template
```

