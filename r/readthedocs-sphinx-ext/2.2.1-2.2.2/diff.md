# Comparing `tmp/readthedocs-sphinx-ext-2.2.1.tar.gz` & `tmp/readthedocs-sphinx-ext-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readthedocs-sphinx-ext-2.2.1.tar", last modified: Tue Jun  6 20:54:02 2023, max compression
+gzip compressed data, was "readthedocs-sphinx-ext-2.2.2.tar", last modified: Thu Jun 29 20:31:36 2023, max compression
```

## Comparing `readthedocs-sphinx-ext-2.2.1.tar` & `readthedocs-sphinx-ext-2.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1083 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/LICENSE
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      250 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/MANIFEST.in
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/PKG-INFO
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1162 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/README.rst
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.734692 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/__init__.py
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.735692 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1166 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/readthedocs-insert.html.tmpl
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2400 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/embed.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2140 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/external_version_warning.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)    14982 2023-06-06 20:44:42.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/readthedocs.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      576 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/template-meta.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2215 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_ext/versionwarning.py
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.738692 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/PKG-INFO
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      855 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/SOURCES.txt
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)        1 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/dependency_links.txt
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)       31 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/requires.txt
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)       16 2023-06-06 20:54:02.000000 readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/top_level.txt
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)       67 2023-06-06 20:54:02.747692 readthedocs-sphinx-ext-2.2.1/setup.cfg
--rwxr-xr-x   0 stsewd    (1000) stsewd    (1000)      728 2023-06-06 20:49:35.000000 readthedocs-sphinx-ext-2.2.1/setup.py
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.740692 readthedocs-sphinx-ext-2.2.1/tests/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/__init__.py
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.741692 readthedocs-sphinx-ext-2.2.1/tests/pr-example/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      760 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pr-example/conf.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pr-example/index.rst
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.743692 readthedocs-sphinx-ext-2.2.1/tests/pyexample/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      762 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/conf.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)       95 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/escape' this js.rst
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample/index.rst
-drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-06 20:54:02.745692 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      582 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/conf.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/index.rst
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)     4521 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/test_integration.py
--rw-r--r--   0 stsewd    (1000) stsewd    (1000)      768 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.1/tests/util.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.956331 readthedocs-sphinx-ext-2.2.2/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1083 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/LICENSE
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      250 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/MANIFEST.in
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-29 20:31:36.956331 readthedocs-sphinx-ext-2.2.2/PKG-INFO
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1162 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/README.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.945331 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/__init__.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.946331 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/_templates/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1166 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/_templates/readthedocs-insert.html.tmpl
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2400 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/embed.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2140 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/external_version_warning.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)    12983 2023-06-29 20:27:57.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/readthedocs.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      576 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/template-meta.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     2215 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_ext/versionwarning.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.949331 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     1443 2023-06-29 20:31:36.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/PKG-INFO
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      855 2023-06-29 20:31:36.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        1 2023-06-29 20:31:36.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       31 2023-06-29 20:31:36.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/requires.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       16 2023-06-29 20:31:36.000000 readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/top_level.txt
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       67 2023-06-29 20:31:36.958331 readthedocs-sphinx-ext-2.2.2/setup.cfg
+-rwxr-xr-x   0 stsewd    (1000) stsewd    (1000)      728 2023-06-29 20:30:52.000000 readthedocs-sphinx-ext-2.2.2/setup.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.951331 readthedocs-sphinx-ext-2.2.2/tests/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)        0 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/__init__.py
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.953331 readthedocs-sphinx-ext-2.2.2/tests/pr-example/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      760 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pr-example/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pr-example/index.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.954331 readthedocs-sphinx-ext-2.2.2/tests/pyexample/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      762 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pyexample/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)       95 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pyexample/escape' this js.rst
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pyexample/index.rst
+drwxr-xr-x   0 stsewd    (1000) stsewd    (1000)        0 2023-06-29 20:31:36.956331 readthedocs-sphinx-ext-2.2.2/tests/pyexample-json/
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      582 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pyexample-json/conf.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      315 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/pyexample-json/index.rst
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)     4035 2023-06-29 20:27:57.000000 readthedocs-sphinx-ext-2.2.2/tests/test_integration.py
+-rw-r--r--   0 stsewd    (1000) stsewd    (1000)      768 2023-01-04 18:52:06.000000 readthedocs-sphinx-ext-2.2.2/tests/util.py
```

### Comparing `readthedocs-sphinx-ext-2.2.1/LICENSE` & `readthedocs-sphinx-ext-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/PKG-INFO` & `readthedocs-sphinx-ext-2.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthedocs-sphinx-ext
-Version: 2.2.1
+Version: 2.2.2
 Summary: Sphinx extension for Read the Docs overrides
 Home-page: http://github.com/readthedocs/readthedocs-sphinx-ext
 Author: Read the Docs, Inc
 Author-email: dev@readthedocs.com
 License: MIT
 License-File: LICENSE
```

### Comparing `readthedocs-sphinx-ext-2.2.1/README.rst` & `readthedocs-sphinx-ext-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/_templates/readthedocs-insert.html.tmpl` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/_templates/readthedocs-insert.html.tmpl`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/embed.py` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/embed.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/external_version_warning.py` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/external_version_warning.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/readthedocs.py` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/readthedocs.py`

 * *Files 15% similar despite different names*

```diff
@@ -269,75 +269,14 @@
         with codecs.open(searchtools_file, 'w', encoding='utf-8') as outfile:
             data = replacement_regex.sub(replacement_text, data)
             outfile.write(data)
     else:
         log.warning('Missing searchtools: {}'.format(searchtools_file))
 
 
-def dump_sphinx_data(app, exception):
-    """
-    Dump data that is only in memory during Sphinx build.
-    This is mostly used for search indexing.
-
-    This includes:
-
-    * `paths`: A mapping of HTML Filename -> RST file
-    * `pages`: A mapping of HTML Filename -> Sphinx Page name
-    * `titles`: A mapping of HTML Filename -> Page Title
-    * `types`: A mapping of Sphinx Domain type slugs -> human-readable name for that type
-
-    """
-    if app.builder.name not in JSON_BUILDERS or exception:
-        return
-    try:
-        types = {}
-        titles = {}
-        paths = {}
-        pages = {}
-
-        for domain_name, domain_obj in app.env.domains.items():
-            for type_name, type_obj in domain_obj.object_types.items():
-                key = "{}:{}".format(domain_name, type_name)
-                types[key] = str(type_obj.lname)
-
-        for page, title in app.env.titles.items():
-            page_uri = app.builder.get_target_uri(page)
-            titles[page_uri] = title.astext()
-            paths[page_uri] = app.env.doc2path(page, base=None)
-            pages[page_uri] = page
-
-        to_dump = {
-            'types': types,
-            'titles': titles,
-            'paths': paths,
-            'pages': pages,
-        }
-
-        # We need to get the output directory where the docs are built
-        # _build/json.
-        build_json = os.path.abspath(
-            os.path.join(app.outdir, '..', 'json')
-        )
-        outjson = os.path.join(build_json, 'readthedocs-sphinx-domain-names.json')
-        with open(outjson, 'w+') as json_file:
-            json.dump(to_dump, json_file, indent=4)
-    except TypeError:
-        log.exception(
-            'Fail to encode JSON for object names'
-        )
-    except IOError:
-        log.exception(
-            'Fail to save JSON for object names'
-        )
-    except Exception:
-        log.exception(
-            'Failure in JSON search dump for object names'
-        )
-
-
 def dump_telemetry(app, config):
     # We need to get the output directory where the docs are built
     # _build/json.
     build_json = os.path.abspath(
         os.path.join(app.outdir, '..', 'json')
     )
     outjson = os.path.join(build_json, 'telemetry.json')
@@ -409,15 +348,14 @@
 
 
 def setup(app):
     app.add_builder(ReadtheDocsSingleFileHTMLBuilderLocalMedia)
     app.connect('html-page-context', update_body)
     app.connect('html-page-context', generate_json_artifacts)
     app.connect('build-finished', remove_search_init)
-    app.connect('build-finished', dump_sphinx_data)
 
     if sphinx.version_info >= (1, 8, 0):
         # `config-inited` event was introduced in Sphinx 1.8
         app.connect('config-inited', dump_telemetry)
 
     # Embed
     app.add_directive('readthedocs-embed', EmbedDirective)
```

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/template-meta.py` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/template-meta.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_ext/versionwarning.py` & `readthedocs-sphinx-ext-2.2.2/readthedocs_ext/versionwarning.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/PKG-INFO` & `readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readthedocs-sphinx-ext
-Version: 2.2.1
+Version: 2.2.2
 Summary: Sphinx extension for Read the Docs overrides
 Home-page: http://github.com/readthedocs/readthedocs-sphinx-ext
 Author: Read the Docs, Inc
 Author-email: dev@readthedocs.com
 License: MIT
 License-File: LICENSE
```

### Comparing `readthedocs-sphinx-ext-2.2.1/readthedocs_sphinx_ext.egg-info/SOURCES.txt` & `readthedocs-sphinx-ext-2.2.2/readthedocs_sphinx_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/setup.py` & `readthedocs-sphinx-ext-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 setup(
     name='readthedocs-sphinx-ext',
-    version='2.2.1',
+    version='2.2.2',
     author='Read the Docs, Inc',
     author_email='dev@readthedocs.com',
     url='http://github.com/readthedocs/readthedocs-sphinx-ext',
     license='MIT',
     description='Sphinx extension for Read the Docs overrides',
     install_requires=['requests', 'Jinja2>=2.9', 'packaging'],
     package_dir={'': '.'},
```

### Comparing `readthedocs-sphinx-ext-2.2.1/tests/pr-example/conf.py` & `readthedocs-sphinx-ext-2.2.2/tests/pr-example/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/tests/pyexample/conf.py` & `readthedocs-sphinx-ext-2.2.2/tests/pyexample/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/tests/pyexample-json/conf.py` & `readthedocs-sphinx-ext-2.2.2/tests/pyexample-json/conf.py`

 * *Files identical despite different names*

### Comparing `readthedocs-sphinx-ext-2.2.1/tests/test_integration.py` & `readthedocs-sphinx-ext-2.2.2/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,30 +68,14 @@
             '_build/json/index.fjson',
             [
                 'current_page_name', 'title', 'body',
                 'toc', 'sourcename', 'page_source_suffix',
             ],
         )
 
-    def test_generate_json_domain_artifacts(self):
-        self._run_test(
-            'pyexample-json',
-            '_build/json/readthedocs-sphinx-domain-names.json',
-            [
-                # types
-                '"js:class": "class"',
-                # pages
-                '"index.html": "index"',
-                # paths
-                '"index.html": "index.rst"',
-                # titles
-                '"index.html": "Welcome to pyexample',
-            ],
-        )
-
     def test_escape_js_vars(self):
         with build_output('pyexample', '_build/html/escape\' this js.html',
                           builder='html') as data:
             self.assertNotIn('escape \' this js', data)
             self.assertIn('escape\\u0027 this js', data)
 
         with build_output('pyexample', '_build/html/index.html', builder='html') as data:
```

### Comparing `readthedocs-sphinx-ext-2.2.1/tests/util.py` & `readthedocs-sphinx-ext-2.2.2/tests/util.py`

 * *Files identical despite different names*

