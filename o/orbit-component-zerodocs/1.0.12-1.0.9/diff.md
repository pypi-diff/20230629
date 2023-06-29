# Comparing `tmp/orbit_component_zerodocs-1.0.12.tar.gz` & `tmp/orbit_component_zerodocs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_zerodocs-1.0.12.tar", max compression
+gzip compressed data, was "orbit_component_zerodocs-1.0.9.tar", max compression
```

## Comparing `orbit_component_zerodocs-1.0.12.tar` & `orbit_component_zerodocs-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.12/LICENSE.md
--rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.12/README.md
--rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/__init__.py
--rwxr-xr-x   0        0        0    20056 2023-06-12 12:33:24.211953 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/doc_python.py
--rw-r--r--   0        0        0     2356 2023-06-29 12:49:46.027418 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/plugin.py
--rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/APIs.py
--rw-r--r--   0        0        0    10936 2023-06-11 13:15:41.191009 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/Cache.py
--rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/Project.py
--rw-r--r--   0        0        0      270 2023-06-08 11:36:09.568981 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/Versions.py
--rw-r--r--   0        0        0        0 2023-06-29 13:18:43.151012 orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/version.py
--rw-r--r--   0        0        0     1400 2023-06-29 13:18:43.147012 orbit_component_zerodocs-1.0.12/pyproject.toml
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      220 2023-05-30 20:41:27.418669 orbit_component_zerodocs-1.0.9/README.md
+-rw-r--r--   0        0        0       71 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/__init__.py
+-rwxr-xr-x   0        0        0    19748 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py
+-rw-r--r--   0        0        0     1599 2023-06-08 11:28:29.403019 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/plugin.py
+-rw-r--r--   0        0        0     2934 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py
+-rw-r--r--   0        0        0    11017 2023-06-02 18:29:55.867494 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py
+-rw-r--r--   0        0        0     1814 2023-05-30 15:19:37.980465 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py
+-rw-r--r--   0        0        0      270 2023-06-08 11:36:09.568981 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Versions.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/version.py
+-rw-r--r--   0        0        0     1404 2023-06-08 17:29:59.004776 orbit_component_zerodocs-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 orbit_component_zerodocs-1.0.9/PKG-INFO
```

### Comparing `orbit_component_zerodocs-1.0.12/LICENSE.md` & `orbit_component_zerodocs-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/doc_python.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/doc_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,24 +317,22 @@
                 print(type(text))
                 return '???'
 
         def function_definition(module, klass, name):
             fn = klass['defs'][name]
             # base = self.BASE_URL if self._name == 'pynndb' else f'{self.EXAMPLE_URL}/{self._name}'
             # url = f'{base}/{module_name}.py#L{fn.get("line")}'
-            # url = 'need a module url'
-            # s = f'<a href="{url}" target="_blank">{method}{name}{method_end} </a>'
+            url = 'need a module url'
+            s = f'<a href="{url}" target="_blank">{method}{name}{method_end} </a>'
 
             docs = fn.get('docs')
             anns = fn.get('anns')
             args = fn.get('args')
             defs = fn.get('defs')
             line = fn.get('line')
-            
-            s= f'<a onclick="window.zd_gotoSource({line})">{method}{name}{method_end} </a>'
 
             text = ''
             look = {}
             newa = []
             for arg in args:
                 look[arg] = {'ann': anns.pop(0), 'def': defs.pop(0)}
                 a = look[arg]['def']
@@ -391,18 +389,15 @@
 
                 # sidebar.write(f'<li class="nav-item section-title mt-3">\n')
                 # sidebar.write(f' <a class="nav-link scrollto" href="#section-{klass_name}">\n')
                 # sidebar.write(f'{CLASS_ICON}{klass_name}')
                 # sidebar.write(f' </a></li>\n')
 
                 s += f'{class_href(klass_name)}\n'
-                # s += f'{keyword}class{keyword_end} <a href="{url}" target="_blank">{css_klass}{klass_name}{css_klass_end}</a>\n'
-                line = klass.get("line")
-                s += f'{keyword}class{keyword_end} <a onclick="window.zd_gotoSource({line})">{css_klass}{klass_name}{css_klass_end}</a>\n'
-                
+                s += f'{keyword}class{keyword_end} <a href="{url}" target="_blank">{css_klass}{klass_name}{css_klass_end}</a>\n'
                 if klass.get('base'):
                     params = ", ".join([f"{css_arg}{base}{css_arg_end}\n" for base in klass["base"]])
                     s += f'({params})'
                     s += ':'
                 s += format_docstring(klass.get("docs"))
 
                 # sidebar.write(f'<ul class="section-items list-unstyled nav flex-column pb3">')
```

### Comparing `orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/plugin.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,45 @@
 from orbit_component_base.src.orbit_plugin import PluginBase
-from orbit_component_base.src.orbit_decorators import Sentry
+from orbit_component_base.src.orbit_decorators import navGuard, apiSentry
 from orbit_component_zerodocs.schema.Cache import CacheCollection
 from orbit_component_zerodocs.schema.APIs import APIsCollection
 from orbit_component_zerodocs.schema.Project import ProjectCollection
-from orbit_component_base.schema.OrbitPermissions import PermissionsCollection
 from loguru import logger as log
 
-COMPONENT_NAMESPACE = 'zerodocs'
-
-
-def check_permission (session, name, args):
-    log.warning(f'name={name} host={session.get("host_id")} nsp={COMPONENT_NAMESPACE} args={str(args)}')
-    key = f'{name}|default'
-    if key in session.get('permission_cache', []):
-        return True
-    if 'permission_cache' not in session:
-        session['permission_cache'] = set()
-    if PermissionsCollection(args[1]).check(session.get("host_id"), COMPONENT_NAMESPACE, name, 'default'):
-        session['permission_cache'].add(key)
-        return True
-    log.debug(f'Permission denied, user={session.get("host_id")} namespace={COMPONENT_NAMESPACE} name={name}')
-    return False
-
 
 class Plugin (PluginBase):
 
-    NAMESPACE = COMPONENT_NAMESPACE
+    NAMESPACE = 'zerodocs'
     COLLECTIONS = [
         CacheCollection,
         APIsCollection,
         ProjectCollection
     ]
 
-    @Sentry()
+    @navGuard
     async def on_cache_fetch (self, sid, params, force=False):
         return await CacheCollection(sid).fetch(params, force)
 
-    @Sentry()
+    @navGuard
     async def on_get_project_id (self, sid, params):
         return await CacheCollection(sid).get_project_id(params)
 
-    @Sentry()
+    @navGuard
     async def on_get_api_remote (self, sid, provider, api, branch, path):
         return APIsCollection(sid).get_api_remote(provider, api, branch, path)
 
-    @Sentry(check_permission)
+    @apiSentry(['admin'])
     async def on_cache_put (self, sid, old_data, new_data):
         return await CacheCollection(sid).put(old_data, new_data)
 
-    @Sentry(check_permission)
+    @apiSentry(['admin'])
     async def on_project_put (self, sid, params):
         return await ProjectCollection(sid).put(params)
 
-    @Sentry(check_permission)
+    @apiSentry(['admin'])
     async def on_project_remove (self, sid, params):
         try:
             await ProjectCollection(sid).remove(params)
             await CacheCollection(sid).remove(params)
             return {'ok': True}
         except Exception as e:
             log.exception(e)
```

### Comparing `orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/APIs.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/APIs.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/Cache.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         try:
             project = ProjectTable().from_params(doc)
             doc._project_id = project._project_id
             head = await doc.head()
             if head:
                 etag = head.get('Etag')
                 if etag == doc._etag and not doc._refresh:
+                    # log.debug(f'Serving "{doc._path}" from cache based on Etag')
                     return
                 log.warning(f"Check did an update, new etag={etag}, old={doc._etag}")
                 doc.update({'etag': etag, 'refresh': False})
                 text = await doc.fetch()
                 return await self.update(doc, text)
             else:
                 log.error(f'Unable to load file: {doc.doc}')
@@ -254,12 +255,12 @@
     def get_ids(cls, session, params, transaction=None):
         ids, data = [], []
         limit = Doc(params.get('filter'))
         for result in cls().filter(index_name='by_root', lower=limit):
             doc = result.doc
             if doc._root != limit._root:
                 break
-            # doc._key = f'{doc._branch}|{doc._key}'
+            doc._key = f'{doc._branch}|{doc._key}'
             session.append(params, result.oid.decode(), ids, data, doc, strip=cls.table_strip)
         session.update(ids, params)
         return {'ok': True, 'ids': ids, 'data': data}
```

### Comparing `orbit_component_zerodocs-1.0.12/orbit_component_zerodocs/schema/Project.py` & `orbit_component_zerodocs-1.0.9/orbit_component_zerodocs/schema/Project.py`

 * *Files identical despite different names*

### Comparing `orbit_component_zerodocs-1.0.12/pyproject.toml` & `orbit_component_zerodocs-1.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-zerodocs"
-version = "1.0.12"
+version = "1.0.9"
 description = "Orbit Component for inline documentation"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_zerodocs"}]
 classifiers = [
@@ -22,21 +22,21 @@
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-zerodocs"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-zerodocs/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-orbit-database = ">=1.0"
-orbit-component-base = ">=1.0"
+orbit-database = "^0.99.91"
 loguru = "^0.7.0"
 pygments = "^2.15.1"
 bs4 = "^0.0.1"
 cmarkgfm = "^2022.10.27"
 python-gitlab = "^3.14.0"
+orbit-component-base = "^0.99.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `orbit_component_zerodocs-1.0.12/PKG-INFO` & `orbit_component_zerodocs-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-zerodocs
-Version: 1.0.12
+Version: 1.0.9
 Summary: Orbit Component for inline documentation
 Home-page: https://gitlab.com/madpenguin/orbit-component-zerodocs
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: cmarkgfm (>=2022.10.27,<2023.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: orbit-component-base (>=1.0)
-Requires-Dist: orbit-database (>=1.0)
+Requires-Dist: orbit-component-base (>=0.99.9,<0.100.0)
+Requires-Dist: orbit-database (>=0.99.91,<0.100.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-zerodocs
 Description-Content-Type: text/markdown
 
 # Orbit Component :: ZeroDocs
```

