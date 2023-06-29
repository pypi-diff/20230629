# Comparing `tmp/domdf_sphinx_theme-23.0.0.tar.gz` & `tmp/domdf_sphinx_theme-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domdf_sphinx_theme-23.0.0.tar", last modified: Thu Jan 19 16:50:07 2023, max compression
+gzip compressed data, was "domdf_sphinx_theme-23.0.1.tar", last modified: Thu Jun 29 15:57:20 2023, max compression
```

## Comparing `domdf_sphinx_theme-23.0.0.tar` & `domdf_sphinx_theme-23.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-01-19 16:50:07.987980 domdf_sphinx_theme-23.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-01-19 16:50:07.979979 domdf_sphinx_theme-23.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5228 2023-01-19 16:50:07.987980 domdf_sphinx_theme-23.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-01-19 16:50:07.987980 domdf_sphinx_theme-23.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-01-19 16:50:07.987980 domdf_sphinx_theme-23.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-01-19 16:49:36.047546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (122)     8589 2023-01-19 16:49:36.043546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-01-19 16:49:36.047546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/versions.html
--rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-01-19 16:49:36.043546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-01-19 16:49:36.043546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     9611 2023-01-19 16:49:36.047546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (122)   133453 2023-01-19 16:49:36.047546 domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/static/css/domdf_sphinx_theme.css
+-rw-r--r--   0 runner    (1001) docker     (122)     5228 2023-06-29 15:57:20.945562 domdf_sphinx_theme-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-06-29 15:57:20.945562 domdf_sphinx_theme-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-29 15:57:20.945562 domdf_sphinx_theme-23.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-29 15:57:20.937562 domdf_sphinx_theme-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-29 15:57:20.945562 domdf_sphinx_theme-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/versions.html
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)   133453 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/static/css/domdf_sphinx_theme.css
+-rw-r--r--   0 runner    (1001) docker     (122)     9611 2023-06-29 15:56:45.681387 domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/static/js/theme.js
```

### Comparing `domdf_sphinx_theme-23.0.0/PKG-INFO` & `domdf_sphinx_theme-23.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: domdf-sphinx-theme
-Version: 23.0.0
+Version: 23.0.1
 Summary: Customised 'sphinx_rtd_theme' used by my Python projects.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,sphinx,sphinx-theme
 Home-page: https://github.com/domdfcoding/domdf_sphinx_theme
 Project-URL: Issue Tracker, https://github.com/domdfcoding/domdf_sphinx_theme/issues
 Project-URL: Source Code, https://github.com/domdfcoding/domdf_sphinx_theme
-Project-URL: Documentation, https://domdf_sphinx_theme.readthedocs.io/en/latest
+Project-URL: Documentation, https://domdf-sphinx-theme.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
@@ -67,16 +67,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/domdf_sphinx_theme/latest?logo=read-the-docs
-	:target: https://domdf_sphinx_theme.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/domdf-sphinx-theme/latest?logo=read-the-docs
+	:target: https://domdf-sphinx-theme.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/domdf_sphinx_theme/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/domdf_sphinx_theme/workflows/Linux/badge.svg
@@ -126,15 +126,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_sphinx_theme
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_sphinx_theme
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_sphinx_theme/v23.0.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_sphinx_theme/v23.0.1
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_sphinx_theme
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/commit/master
 	:alt: GitHub last commit
```

### Comparing `domdf_sphinx_theme-23.0.0/LICENSE` & `domdf_sphinx_theme-23.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domdf_sphinx_theme-23.0.0/pyproject.toml` & `domdf_sphinx_theme-23.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "domdf_sphinx_theme"
-version = "23.0.0"
+version = "23.0.1"
 description = "Customised 'sphinx_rtd_theme' used by my Python projects."
 readme = "README.rst"
 keywords = [ "documentation", "sphinx", "sphinx-theme",]
 dynamic = []
 dependencies = [ "docutils>=0.16", "sphinx>=3.0.4", "sphinx-rtd-theme<1.1,>0.4",]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -43,15 +43,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/domdfcoding/domdf_sphinx_theme"
 "Issue Tracker" = "https://github.com/domdfcoding/domdf_sphinx_theme/issues"
 "Source Code" = "https://github.com/domdfcoding/domdf_sphinx_theme"
-Documentation = "https://domdf_sphinx_theme.readthedocs.io/en/latest"
+Documentation = "https://domdf-sphinx-theme.readthedocs.io/en/latest"
 
 [tool.importcheck]
 always = [ "domdf_sphinx_theme",]
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `domdf_sphinx_theme-23.0.0/README.rst` & `domdf_sphinx_theme-23.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/domdf_sphinx_theme/latest?logo=read-the-docs
-	:target: https://domdf_sphinx_theme.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/domdf-sphinx-theme/latest?logo=read-the-docs
+	:target: https://domdf-sphinx-theme.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/domdf_sphinx_theme/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/domdf_sphinx_theme/workflows/Linux/badge.svg
@@ -84,15 +84,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_sphinx_theme
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_sphinx_theme
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_sphinx_theme/v23.0.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_sphinx_theme/v23.0.1
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_sphinx_theme
 	:target: https://github.com/domdfcoding/domdf_sphinx_theme/commit/master
 	:alt: GitHub last commit
```

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/layout.html` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   {% endif %}
   {# CANONICAL URL #}
   {% if theme_canonical_url %}
     <link rel="canonical" href="{{ theme_canonical_url }}{{ pagename }}.html"/>
   {% endif %}
 
   {# JAVASCRIPTS #}
+  {%- block scripts %}
 <!--  <script type="text/javascript" src="{{ pathto('_static/js/modernizr.min.js', 1) }}"></script>-->
   {%- if not embedded %}
   {# XXX Sphinx 1.8.0 made this an external js-file, quick fix until we refactor the template to inherert more blocks directly from sphinx #}
     {% if sphinx_version >= "1.8.0" %}
       <script type="text/javascript" id="documentation_options" data-url_root="{{ pathto('', 1) }}" src="{{ pathto('_static/documentation_options.js', 1) }}"></script>
       {%- for scriptfile in script_files %}
         {{ js_tag(scriptfile) }}
@@ -204,14 +205,15 @@
   {% include "versions.html" %}
 
   <script type="text/javascript">
       jQuery(function () {
           SphinxRtdTheme.Navigation.enable({{ 'true' if theme_sticky_navigation|tobool else 'false' }});
       });
   </script>
+  {%- endblock %}
 
   {# Do not conflict with RTD insertion of analytics script #}
   {% if not READTHEDOCS %}
     {% if theme_analytics_id %}
     <!-- Theme Analytics -->
     <script>
     (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
```

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/versions.html` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/versions.html`

 * *Files identical despite different names*

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/__init__.py` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from docutils.nodes import Element  # type: ignore
 from sphinx import addnodes
 from sphinx.application import Sphinx
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "23.0.0"
+__version__: str = "23.0.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __version_full__ = __version__
 
 __all__ = ["setup", "HTML5Translator"]
 
 logger = logging.getLogger(__name__)
```

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/footer.html` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/footer.html`

 * *Files identical despite different names*

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/static/js/theme.js` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `domdf_sphinx_theme-23.0.0/domdf_sphinx_theme/static/css/domdf_sphinx_theme.css` & `domdf_sphinx_theme-23.0.1/domdf_sphinx_theme/static/css/domdf_sphinx_theme.css`

 * *Files identical despite different names*

