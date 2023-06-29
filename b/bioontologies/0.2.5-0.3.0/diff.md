# Comparing `tmp/bioontologies-0.2.5.tar.gz` & `tmp/bioontologies-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioontologies-0.2.5.tar", last modified: Thu Mar 30 10:18:31 2023, max compression
+gzip compressed data, was "bioontologies-0.3.0.tar", last modified: Thu Jun 29 10:00:21 2023, max compression
```

## Comparing `bioontologies-0.2.5.tar` & `bioontologies-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.235634 bioontologies-0.2.5/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-04-28 07:50:12.000000 bioontologies-0.2.5/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      342 2022-04-29 11:08:00.000000 bioontologies-0.2.5/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-03-30 10:18:31.235803 bioontologies-0.2.5/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     6660 2022-04-29 09:27:24.000000 bioontologies-0.2.5/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.211085 bioontologies-0.2.5/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.217812 bioontologies-0.2.5/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      246 2022-04-28 07:50:12.000000 bioontologies-0.2.5/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7039 2023-03-30 10:18:30.000000 bioontologies-0.2.5/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1780 2022-04-28 08:25:25.000000 bioontologies-0.2.5/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      548 2022-04-28 07:50:12.000000 bioontologies-0.2.5/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2022-04-29 12:14:06.000000 bioontologies-0.2.5/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-04-28 07:50:12.000000 bioontologies-0.2.5/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2632 2023-03-30 10:18:31.236675 bioontologies-0.2.5/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.211779 bioontologies-0.2.5/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.224947 bioontologies-0.2.5/src/bioontologies/
--rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-03-30 10:15:39.000000 bioontologies-0.2.5/src/bioontologies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      330 2022-04-28 07:50:12.000000 bioontologies-0.2.5/src/bioontologies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4996 2022-08-16 12:32:09.000000 bioontologies-0.2.5/src/bioontologies/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2801 2023-03-30 10:15:39.000000 bioontologies-0.2.5/src/bioontologies/gilda_utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    20492 2023-02-13 19:55:50.000000 bioontologies-0.2.5/src/bioontologies/obograph.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:50:12.000000 bioontologies-0.2.5/src/bioontologies/py.typed
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.229925 bioontologies-0.2.5/src/bioontologies/relations/
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2022-09-08 10:32:28.000000 bioontologies-0.2.5/src/bioontologies/relations/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2788 2022-09-27 22:41:57.000000 bioontologies-0.2.5/src/bioontologies/relations/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   108493 2022-09-27 20:50:14.000000 bioontologies-0.2.5/src/bioontologies/relations/data.json
--rw-r--r--   0 cthoyt     (501) staff       (20)    15132 2023-03-30 10:10:25.000000 bioontologies-0.2.5/src/bioontologies/robot.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.233661 bioontologies-0.2.5/src/bioontologies/upgrade/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2022-09-27 20:53:02.000000 bioontologies-0.2.5/src/bioontologies/upgrade/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5893 2023-02-01 14:50:57.000000 bioontologies-0.2.5/src/bioontologies/upgrade/data.tsv
--rw-r--r--   0 cthoyt     (501) staff       (20)      814 2022-09-09 14:23:13.000000 bioontologies-0.2.5/src/bioontologies/upgrade/import_debio.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1033 2023-03-30 10:18:30.000000 bioontologies-0.2.5/src/bioontologies/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.228129 bioontologies-0.2.5/src/bioontologies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)      950 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       57 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:56:41.000000 bioontologies-0.2.5/src/bioontologies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      195 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       14 2023-03-30 10:18:31.000000 bioontologies-0.2.5/src/bioontologies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-03-30 10:18:31.234995 bioontologies-0.2.5/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       63 2022-04-28 07:50:12.000000 bioontologies-0.2.5/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      903 2022-06-06 11:57:54.000000 bioontologies-0.2.5/tests/test_api.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.980429 bioontologies-0.3.0/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-04-28 07:50:12.000000 bioontologies-0.3.0/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      342 2022-04-29 11:08:00.000000 bioontologies-0.3.0/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-06-29 10:00:21.980575 bioontologies-0.3.0/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6660 2022-04-29 09:27:24.000000 bioontologies-0.3.0/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.956660 bioontologies-0.3.0/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.962445 bioontologies-0.3.0/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      246 2022-04-28 07:50:12.000000 bioontologies-0.3.0/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7050 2023-06-29 10:00:21.000000 bioontologies-0.3.0/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1780 2022-04-28 08:25:25.000000 bioontologies-0.3.0/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      548 2022-04-28 07:50:12.000000 bioontologies-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2022-04-29 12:14:06.000000 bioontologies-0.3.0/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-04-28 07:50:12.000000 bioontologies-0.3.0/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2645 2023-06-29 10:00:21.981571 bioontologies-0.3.0/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.957141 bioontologies-0.3.0/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.969795 bioontologies-0.3.0/src/bioontologies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      383 2023-06-21 09:33:32.000000 bioontologies-0.3.0/src/bioontologies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      330 2022-04-28 07:50:12.000000 bioontologies-0.3.0/src/bioontologies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3192 2023-06-14 12:47:47.000000 bioontologies-0.3.0/src/bioontologies/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      963 2023-06-21 11:30:52.000000 bioontologies-0.3.0/src/bioontologies/constants.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3317 2023-06-26 22:54:32.000000 bioontologies-0.3.0/src/bioontologies/gilda_utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    34494 2023-06-29 09:15:08.000000 bioontologies-0.3.0/src/bioontologies/obograph.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:50:12.000000 bioontologies-0.3.0/src/bioontologies/py.typed
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.974474 bioontologies-0.3.0/src/bioontologies/relations/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      189 2023-06-27 10:44:19.000000 bioontologies-0.3.0/src/bioontologies/relations/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5242 2023-06-29 09:22:44.000000 bioontologies-0.3.0/src/bioontologies/relations/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    96122 2023-06-29 08:55:57.000000 bioontologies-0.3.0/src/bioontologies/relations/data.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)    15567 2023-06-29 08:50:06.000000 bioontologies-0.3.0/src/bioontologies/robot.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.977536 bioontologies-0.3.0/src/bioontologies/upgrade/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1592 2023-05-16 11:21:41.000000 bioontologies-0.3.0/src/bioontologies/upgrade/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9556 2023-06-27 07:35:18.000000 bioontologies-0.3.0/src/bioontologies/upgrade/data.tsv
+-rw-r--r--   0 cthoyt     (501) staff       (20)      814 2022-09-09 14:23:13.000000 bioontologies-0.3.0/src/bioontologies/upgrade/import_debio.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1033 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.972414 bioontologies-0.3.0/src/bioontologies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8050 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1005 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       57 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-04-28 07:56:41.000000 bioontologies-0.3.0/src/bioontologies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      206 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       14 2023-06-29 10:00:21.000000 bioontologies-0.3.0/src/bioontologies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-06-29 10:00:21.979595 bioontologies-0.3.0/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       63 2022-04-28 07:50:12.000000 bioontologies-0.3.0/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      903 2022-06-06 11:57:54.000000 bioontologies-0.3.0/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      760 2023-06-29 09:16:38.000000 bioontologies-0.3.0/tests/test_relations.py
```

### Comparing `bioontologies-0.2.5/LICENSE` & `bioontologies-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioontologies-0.2.5/PKG-INFO` & `bioontologies-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioontologies
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools for biomedical ontologies.
 Home-page: https://github.com/biopragmatics/bioontologies
 Download-URL: https://github.com/biopragmatics/bioontologies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioontologies Version: 0.2.5 Summary: Tools for
+Metadata-Version: 2.1 Name: bioontologies Version: 0.3.0 Summary: Tools for
 biomedical ontologies. Home-page: https://github.com/biopragmatics/
 bioontologies Download-URL: https://github.com/biopragmatics/bioontologies/
 releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer:
 Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-
 URL: Bug Tracker, https://github.com/biopragmatics/bioontologies/issues
 Project-URL: Source Code, https://github.com/biopragmatics/bioontologies
 Keywords: snekpack,cookiecutter,ontologies,OBO Foundry,knowledge
```

### Comparing `bioontologies-0.2.5/README.md` & `bioontologies-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bioontologies-0.2.5/docs/source/conf.py` & `bioontologies-0.3.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "bioontologies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.2.5"
+release = "0.3.0"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -224,15 +224,15 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
+    "python": ("https://docs.python.org/3", None),
 }
 
 autoclass_content = "both"
 
 # Don't sort alphabetically, explained at:
 # https://stackoverflow.com/questions/37209921/python-how-not-to-sort-sphinx-output-in-alphabetical-order
 autodoc_member_order = "bysource"
```

### Comparing `bioontologies-0.2.5/docs/source/index.rst` & `bioontologies-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bioontologies-0.2.5/docs/source/installation.rst` & `bioontologies-0.3.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bioontologies-0.2.5/setup.cfg` & `bioontologies-0.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = bioontologies
-version = 0.2.5
+version = 0.3.0
 description = Tools for biomedical ontologies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioontologies
 download_url = https://github.com/biopragmatics/bioontologies/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioontologies/issues
 	Source Code = https://github.com/biopragmatics/bioontologies
 author = Charles Tapley Hoyt
 author_email = cthoyt@gmail.com
 maintainer = Charles Tapley Hoyt
 maintainer_email = cthoyt@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 1 - Planning
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Framework :: Pytest
@@ -40,19 +40,20 @@
 	biology
 	systems biology
 	networks biology
 
 [options]
 install_requires = 
 	bioregistry>=0.6.13
-	curies>=0.3.0
+	curies>=0.5.5
 	requests
 	pydantic
 	typing_extensions
 	pystow
+	pandas
 zip_safe = false
 include_package_data = True
 python_requires = >=3.7
 packages = find:
 package_dir = 
 	= src
 
@@ -60,15 +61,15 @@
 where = src
 
 [options.extras_require]
 tests = 
 	pytest
 	coverage
 docs = 
-	sphinx
+	sphinx<7.0
 	sphinx-rtd-theme
 	sphinx-click
 	sphinx-autodoc-typehints
 	sphinx_automodapi
 	m2r2
 
 [options.entry_points]
```

### Comparing `bioontologies-0.2.5/src/bioontologies/gilda_utils.py` & `bioontologies-0.3.0/src/bioontologies/gilda_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .robot import get_obograph_by_prefix
 
 if TYPE_CHECKING:
     import gilda.term
 
 __all__ = [
     "get_gilda_terms",
+    "gilda_from_graph",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def get_gilda_terms(prefix: str, **kwargs: Any) -> Iterable["gilda.term.Term"]:
     """Get gilda terms for the given namespace.
@@ -54,45 +55,56 @@
         scored_matches = grounder.ground("comirna")
     """
     parse_results = get_obograph_by_prefix(prefix, **kwargs)
     if parse_results.graph_document is None:
         return
     for graph in parse_results.graph_document.graphs:
         graph.standardize(prefix=prefix)
-        yield from _gilda_from_graph(prefix, graph)
+        yield from gilda_from_graph(prefix, graph)
 
 
-def _gilda_from_graph(prefix: str, graph: Graph) -> Iterable["gilda.term.Term"]:
+def gilda_from_graph(prefix: str, graph: Graph) -> Iterable["gilda.term.Term"]:
+    """Get Gilda terms from a given graph."""
     import gilda.term
     from gilda.process import normalize
 
     species = {}
     for edge in graph.edges:
-        s, p, o = edge.parse_curies()
-        if s[0] == prefix and p == ("ro", "0002162") and o[0] == "ncbitaxon":
-            species[s[1]] = o[1]
+        if not edge.standardized:
+            edge.standardize()
+        if (
+            edge.subject
+            and edge.subject.prefix == prefix
+            and edge.predicate
+            and edge.predicate.pair == ("ro", "0002162")
+            and edge.object
+            and edge.object.prefix == "ncbitaxon"
+        ):
+            species[edge.subject.identifier] = edge.object.identifier
     for node in tqdm(graph.nodes, leave=False):
-        name = node.lbl
-        if not name:
+        if not node.name or node.reference is None:
             continue
-        organism = species.get(node.luid)
+        if node.reference.prefix != prefix:
+            # Don't add references from other namespaces
+            continue
+        organism = species.get(node.reference.identifier)
         yield gilda.term.Term(
-            norm_text=normalize(name),
-            text=name,
+            norm_text=normalize(node.name),
+            text=node.name,
             db=prefix,
-            id=node.luid,
-            entry_name=name,
+            id=node.reference.identifier,
+            entry_name=node.name,
             status="name",
             source=prefix,
             organism=organism,
         )
         for synonym in node.synonyms:
             yield gilda.term.Term(
-                norm_text=normalize(synonym.val),
-                text=synonym.val,
+                norm_text=normalize(synonym.value),
+                text=synonym.value,
                 db=prefix,
-                id=node.luid,
-                entry_name=name,
+                id=node.reference.identifier,
+                entry_name=node.name,
                 status="synonym",
                 source=prefix,
                 organism=organism,
             )
```

### Comparing `bioontologies-0.2.5/src/bioontologies/robot.py` & `bioontologies-0.3.0/src/bioontologies/robot.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
 from subprocess import check_output
 from typing import List, Optional, Union
 
 import bioregistry
+import pystow
 import requests
 from pystow.utils import download, name_from_url
 from typing_extensions import Literal
 
 from .obograph import Graph, GraphDocument
 
 __all__ = [
@@ -36,35 +37,29 @@
     "get_obograph_by_prefix",
     "get_obograph_by_iri",
     "get_obograph_by_path",
 ]
 
 logger = logging.getLogger(__name__)
 
+LATEST = "1.9.4"
+ROBOT_URL = f"https://github.com/ontodev/robot/releases/download/v{LATEST}/robot.jar"
+ROBOT_MODULE = pystow.module("robot")
+ROBOT_PATH = ROBOT_MODULE.ensure(url=ROBOT_URL)
+ROBOT_COMMAND = ["java", "-jar", str(ROBOT_PATH)]
+
 
 def is_available() -> bool:
     """Check if ROBOT is available."""
     # suggested in https://stackoverflow.com/questions/11210104/check-if-a-program-exists-from-a-python-script
     from shutil import which
 
     return which("robot") is not None
 
 
-CANONICAL = {
-    "apollosv": "http://purl.obolibrary.org/obo/apollo_sv.owl",
-    "cheminf": "http://semanticchemistry.github.io/semanticchemistry/ontology/cheminf.owl",
-    "dideo": "http://purl.obolibrary.org/obo/dideo/release/2022-06-14/dideo.owl",
-    "micro": "http://purl.obolibrary.org/obo/MicrO.owl",
-    "ogsf": "http://purl.obolibrary.org/obo/ogsf-merged.owl",
-    "mfomd": "http://purl.obolibrary.org/obo/MF.owl",
-    "one": "http://purl.obolibrary.org/obo/ONE",
-    "ons": "https://raw.githubusercontent.com/enpadasi/Ontology-for-Nutritional-Studies/master/ons.owl",
-}
-
-
 @dataclass
 class ParseResults:
     """A dataclass containing an OBO Graph JSON and text output from ROBOT."""
 
     graph_document: Optional[GraphDocument]
     messages: List[str] = dataclasses.field(default_factory=list)
     iri: Optional[str] = None
@@ -78,54 +73,61 @@
             rv = rv.standardize()
         return rv
 
     def guess(self, prefix: str) -> Graph:
         """Guess the right graph."""
         if self.graph_document is None:
             raise ValueError("no graph document")
-        graphs = self.graph_document.graphs
-        if 1 == len(graphs):
-            return graphs[0]
-        id_to_graph = {graph.id: graph for graph in graphs}
-        standard_id = f"http://purl.obolibrary.org/obo/{prefix.lower()}.owl"
-        if standard_id in id_to_graph:
-            return id_to_graph[standard_id]
-        if prefix in CANONICAL and CANONICAL[prefix] in id_to_graph:
-            return id_to_graph[CANONICAL[prefix]]
-        raise ValueError(f"Several graphs in {prefix}: {sorted(id_to_graph)}")
+        return self.graph_document.guess(prefix)
 
     def guess_version(self, prefix: str) -> Optional[str]:
         """Guess the version."""
         try:
             graph = self.guess(prefix)
         except ValueError:
             return None
         else:
             return graph.version or graph.version_iri
 
+    def write(self, path: Union[str, Path]) -> None:
+        """Write the graph document to a file in JSON."""
+        if not self.graph_document:
+            raise ValueError
+        path = Path(path)
+        path.write_text(
+            self.graph_document.json(
+                indent=2, sort_keys=True, exclude_unset=True, exclude_none=True
+            )
+        )
+
 
 def get_obograph_by_iri(
     iri: str,
 ) -> ParseResults:
     """Get an ontology by its OBO Graph JSON iri."""
     res_json = requests.get(iri).json()
-    graph_document = GraphDocument(**res_json)
+    correct_raw_json(res_json)
+    graph_document = GraphDocument.parse_obj(res_json)
     return ParseResults(graph_document=graph_document, iri=iri)
 
 
 def get_obograph_by_path(path: Union[str, Path], *, iri: Optional[str] = None) -> ParseResults:
     """Get an ontology by its OBO Graph JSON file path."""
     res_json = json.loads(Path(path).resolve().read_text())
-    graph_document = GraphDocument(**res_json)
+    correct_raw_json(res_json)
+    graph_document = GraphDocument.parse_obj(res_json)
     if iri is None:
         if graph_document.graphs and len(graph_document.graphs) == 1:
             iri = graph_document.graphs[0].id
     return ParseResults(graph_document=graph_document, iri=iri)
 
 
+GETTER_MESSAGES = []
+
+
 def get_obograph_by_prefix(
     prefix: str,
     *,
     json_path: Union[None, str, Path] = None,
     cache: bool = False,
     check: bool = True,
 ) -> ParseResults:
@@ -135,17 +137,18 @@
 
     messages = []
     json_iri = bioregistry.get_json_download(prefix)
 
     if json_iri is not None:
         try:
             parse_results = get_obograph_by_iri(json_iri)
-        except (IOError, ValueError):
-            msg = f"could not parse JSON for {prefix} from {json_iri}"
+        except (IOError, ValueError, TypeError) as e:
+            msg = f"[{prefix}] could not parse JSON from {json_iri}: {e}"
             messages.append(msg)
+            GETTER_MESSAGES.append(msg)
             logger.warning(msg)
         else:
             return parse_results
 
     owl_iri = bioregistry.get_owl_download(prefix)
     obo_iri = bioregistry.get_obo_download(prefix)
 
@@ -160,16 +163,17 @@
                     download(iri, path=path)
                     parse_results = convert_to_obograph_local(
                         path, json_path=json_path, from_iri=iri, check=check
                     )
             else:
                 parse_results = convert_to_obograph_remote(iri, json_path=json_path, check=check)
         except subprocess.CalledProcessError:
-            msg = f"could not parse {label} for {prefix} from {iri}"
+            msg = f"[{prefix}] could not parse {label} from {iri}"
             messages.append(msg)
+            GETTER_MESSAGES.append(msg)
             logger.warning(msg)
             continue
         else:
             # stick all messages before
             parse_results.messages = [*messages, *parse_results.messages]
             return parse_results
 
@@ -306,38 +310,55 @@
                 raise ValueError(f"{input_path} only graph is missing id")
         else:
             missing = [i for i, graph in enumerate(graphs_raw) if "id" not in graph]
             if missing:
                 raise ValueError(f"{input_path} graphs missing IDs: {missing}")
 
         correct_raw_json(graph_document_raw)
-
-        graph_document = GraphDocument(**graph_document_raw)
+        graph_document = GraphDocument.parse_obj(graph_document_raw)
         return ParseResults(
             graph_document=graph_document,
             messages=messages,
             iri=input_path if input_is_iri else None,  # type:ignore
         )
 
 
 def correct_raw_json(graph_document_raw) -> None:
     """Correct issues in raw graph documents, in place."""
-    # clean broken content
     for graph in graph_document_raw["graphs"]:
+        _clean_raw_meta(graph)
         for node in graph["nodes"]:
-            meta = node.get("meta")
-            if not meta:
-                continue
-            basic_property_values = meta.get("basicPropertyValues")
-            if basic_property_values:
-                meta["basicPropertyValues"] = [
-                    basic_property_value
-                    for basic_property_value in basic_property_values
-                    if basic_property_value.get("pred") and basic_property_value.get("val")
-                ]
+            _clean_raw_meta(node)
+    return graph_document_raw
+
+
+def _clean_raw_meta(element):
+    meta = element.get("meta")
+    if not meta:
+        return
+    basic_property_values = meta.get("basicPropertyValues")
+    if basic_property_values:
+        meta["basicPropertyValues"] = [
+            basic_property_value
+            for basic_property_value in basic_property_values
+            if basic_property_value.get("pred") and basic_property_value.get("val")
+        ]
+
+    definition = meta.get("definition")
+    if definition is not None and not definition.get("val"):
+        del meta["definition"]
+
+    xrefs = meta.get("xrefs")
+    if xrefs:
+        meta["xrefs"] = [xref for xref in xrefs if xref.get("val")]
+
+    # What's the point of a synonym with an empty value? Nothing!
+    synonyms = meta.get("synonyms")
+    if synonyms:
+        meta["synonyms"] = [synonym for synonym in synonyms if synonym.get("val")]
 
 
 #: Prefixes that denote remote resources
 PROTOCOLS = {
     "https://",
     "http://",
     "ftp://",
@@ -388,23 +409,23 @@
         Extra positional arguments to pass in the command line
     :return: Output from standard out from running ROBOT
     """
     if input_flag is None:
         input_flag = "-I" if _is_remote(input_path) else "-i"
     if merge:
         args = [
-            "robot",
+            *ROBOT_COMMAND,
             "merge",
             input_flag,
             str(input_path),
             "convert",
         ]
     else:
         args = [
-            "robot",
+            *ROBOT_COMMAND,
             "convert",
             input_flag,
             str(input_path),
         ]
     args.extend(("-o", str(output_path)))
     if extra_args:
         args.extend(extra_args)
@@ -414,7 +435,13 @@
         args.extend(("--format", fmt))
     logger.debug("Running shell command: %s", args)
     ret = check_output(  # noqa:S603
         args,
         cwd=os.path.dirname(__file__),
     )
     return ret.decode()
+
+
+def write_getter_warnings(path: Union[str, Path]) -> None:
+    """Write warned unparsable."""
+    path = Path(path).resolve()
+    path.write_text("\n".join(GETTER_MESSAGES))
```

### Comparing `bioontologies-0.2.5/src/bioontologies/upgrade/import_debio.py` & `bioontologies-0.3.0/src/bioontologies/upgrade/import_debio.py`

 * *Files identical despite different names*

### Comparing `bioontologies-0.2.5/src/bioontologies/version.py` & `bioontologies-0.3.0/src/bioontologies/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.2.5"
+VERSION = "0.3.0"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`bioontologies` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioontologies-0.2.5/src/bioontologies.egg-info/PKG-INFO` & `bioontologies-0.3.0/src/bioontologies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioontologies
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools for biomedical ontologies.
 Home-page: https://github.com/biopragmatics/bioontologies
 Download-URL: https://github.com/biopragmatics/bioontologies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioontologies Version: 0.2.5 Summary: Tools for
+Metadata-Version: 2.1 Name: bioontologies Version: 0.3.0 Summary: Tools for
 biomedical ontologies. Home-page: https://github.com/biopragmatics/
 bioontologies Download-URL: https://github.com/biopragmatics/bioontologies/
 releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer:
 Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT Project-
 URL: Bug Tracker, https://github.com/biopragmatics/bioontologies/issues
 Project-URL: Source Code, https://github.com/biopragmatics/bioontologies
 Keywords: snekpack,cookiecutter,ontologies,OBO Foundry,knowledge
```

### Comparing `bioontologies-0.2.5/src/bioontologies.egg-info/SOURCES.txt` & `bioontologies-0.3.0/src/bioontologies.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/usage.rst
 src/bioontologies/__init__.py
 src/bioontologies/__main__.py
 src/bioontologies/cli.py
+src/bioontologies/constants.py
 src/bioontologies/gilda_utils.py
 src/bioontologies/obograph.py
 src/bioontologies/py.typed
 src/bioontologies/robot.py
 src/bioontologies/version.py
 src/bioontologies.egg-info/PKG-INFO
 src/bioontologies.egg-info/SOURCES.txt
@@ -26,8 +27,9 @@
 src/bioontologies/relations/__init__.py
 src/bioontologies/relations/api.py
 src/bioontologies/relations/data.json
 src/bioontologies/upgrade/__init__.py
 src/bioontologies/upgrade/data.tsv
 src/bioontologies/upgrade/import_debio.py
 tests/__init__.py
-tests/test_api.py
+tests/test_api.py
+tests/test_relations.py
```

### Comparing `bioontologies-0.2.5/tests/test_api.py` & `bioontologies-0.3.0/tests/test_api.py`

 * *Files identical despite different names*

