# Comparing `tmp/kilvin-0.3.tar.gz` & `tmp/kilvin-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilvin-0.3.tar", last modified: Thu Mar 23 16:40:26 2023, max compression
+gzip compressed data, was "kilvin-0.4.tar", last modified: Thu Jun 29 07:56:41 2023, max compression
```

## Comparing `kilvin-0.3.tar` & `kilvin-0.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1093 2023-03-03 07:41:50.000000 kilvin-0.3/LICENSE
--rw-r--r--   0 shanu     (1000) shanu     (1000)     6142 2023-03-23 16:40:26.940958 kilvin-0.3/PKG-INFO
--rw-r--r--   0 shanu     (1000) shanu     (1000)     5630 2023-03-23 16:35:38.000000 kilvin-0.3/README.md
--rw-r--r--   0 shanu     (1000) shanu     (1000)      923 2023-03-23 16:39:37.000000 kilvin-0.3/pyproject.toml
--rw-r--r--   0 shanu     (1000) shanu     (1000)       38 2023-03-23 16:40:26.940958 kilvin-0.3/setup.cfg
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/src/
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/src/kilvin/
--rw-r--r--   0 shanu     (1000) shanu     (1000)       20 2023-03-23 16:39:29.000000 kilvin-0.3/src/kilvin/__init__.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1275 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/__main__.py
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/src/kilvin/cmds/
--rw-r--r--   0 shanu     (1000) shanu     (1000)        0 2023-02-18 23:23:37.000000 kilvin-0.3/src/kilvin/cmds/__init__.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     3801 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/cmds/build.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)      667 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/cmds/init.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1007 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/cmds/new.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1281 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/configs.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)      405 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/log.py
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/src/kilvin/render/
--rw-r--r--   0 shanu     (1000) shanu     (1000)        0 2023-02-18 23:23:37.000000 kilvin-0.3/src/kilvin/render/__init__.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1411 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/render/feed.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     1408 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/render/page.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)     3153 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/render/renderer.py
--rw-r--r--   0 shanu     (1000) shanu     (1000)      919 2023-03-23 16:35:38.000000 kilvin-0.3/src/kilvin/utils.py
-drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-03-23 16:40:26.940958 kilvin-0.3/src/kilvin.egg-info/
--rw-r--r--   0 shanu     (1000) shanu     (1000)     6142 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/PKG-INFO
--rw-r--r--   0 shanu     (1000) shanu     (1000)      556 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/SOURCES.txt
--rw-r--r--   0 shanu     (1000) shanu     (1000)        1 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/dependency_links.txt
--rw-r--r--   0 shanu     (1000) shanu     (1000)       48 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/entry_points.txt
--rw-r--r--   0 shanu     (1000) shanu     (1000)      102 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/requires.txt
--rw-r--r--   0 shanu     (1000) shanu     (1000)        7 2023-03-23 16:40:26.000000 kilvin-0.3/src/kilvin.egg-info/top_level.txt
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.046975 kilvin-0.4/
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1093 2023-03-03 07:41:50.000000 kilvin-0.4/LICENSE
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     6142 2023-06-29 07:56:41.046975 kilvin-0.4/PKG-INFO
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     5630 2023-03-25 14:16:29.000000 kilvin-0.4/README.md
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      912 2023-06-29 07:56:09.000000 kilvin-0.4/pyproject.toml
+-rw-r--r--   0 shanu     (1000) shanu     (1000)       38 2023-06-29 07:56:41.046975 kilvin-0.4/setup.cfg
+-rw-r--r--   0 shanu     (1000) shanu     (1000)       38 2023-06-29 07:17:58.000000 kilvin-0.4/setup.py
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.042975 kilvin-0.4/src/
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.042975 kilvin-0.4/src/kilvin/
+-rw-r--r--   0 shanu     (1000) shanu     (1000)       20 2023-06-29 07:39:20.000000 kilvin-0.4/src/kilvin/__init__.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1114 2023-03-26 18:59:38.000000 kilvin-0.4/src/kilvin/__main__.py
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.046975 kilvin-0.4/src/kilvin/cmds/
+-rw-r--r--   0 shanu     (1000) shanu     (1000)        0 2023-02-18 23:23:37.000000 kilvin-0.4/src/kilvin/cmds/__init__.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     3937 2023-04-01 01:25:44.000000 kilvin-0.4/src/kilvin/cmds/build.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      667 2023-03-23 16:35:38.000000 kilvin-0.4/src/kilvin/cmds/init.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1007 2023-03-23 16:35:38.000000 kilvin-0.4/src/kilvin/cmds/new.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      837 2023-03-26 22:40:23.000000 kilvin-0.4/src/kilvin/cmds/server.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1264 2023-03-28 10:55:31.000000 kilvin-0.4/src/kilvin/configs.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      382 2023-03-27 21:10:24.000000 kilvin-0.4/src/kilvin/log.py
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.046975 kilvin-0.4/src/kilvin/render/
+-rw-r--r--   0 shanu     (1000) shanu     (1000)        0 2023-02-18 23:23:37.000000 kilvin-0.4/src/kilvin/render/__init__.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     3297 2023-03-27 21:10:24.000000 kilvin-0.4/src/kilvin/render/builder.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1406 2023-03-27 21:10:24.000000 kilvin-0.4/src/kilvin/render/feed.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     1357 2023-03-27 21:10:24.000000 kilvin-0.4/src/kilvin/render/page.py
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      919 2023-03-23 16:35:38.000000 kilvin-0.4/src/kilvin/utils.py
+drwxr-xr-x   0 shanu     (1000) shanu     (1000)        0 2023-06-29 07:56:41.046975 kilvin-0.4/src/kilvin.egg-info/
+-rw-r--r--   0 shanu     (1000) shanu     (1000)     6142 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/PKG-INFO
+-rw-r--r--   0 shanu     (1000) shanu     (1000)      590 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/SOURCES.txt
+-rw-r--r--   0 shanu     (1000) shanu     (1000)        1 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/dependency_links.txt
+-rw-r--r--   0 shanu     (1000) shanu     (1000)       48 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/entry_points.txt
+-rw-r--r--   0 shanu     (1000) shanu     (1000)       98 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/requires.txt
+-rw-r--r--   0 shanu     (1000) shanu     (1000)        7 2023-06-29 07:56:41.000000 kilvin-0.4/src/kilvin.egg-info/top_level.txt
```

### Comparing `kilvin-0.3/LICENSE` & `kilvin-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kilvin-0.3/PKG-INFO` & `kilvin-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilvin
-Version: 0.3
+Version: 0.4
 Summary: A minimal static site generator.
 Author-email: Pratham Singh <prathms007@gmail.com>
 Project-URL: Homepage, https://github.com/shanukun/kilvin
 Project-URL: Bug Tracker, https://github.com/shanukun/kilvin/issues
 Keywords: static site generator,markdow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kilvin-0.3/README.md` & `kilvin-0.4/README.md`

 * *Files identical despite different names*

### Comparing `kilvin-0.3/pyproject.toml` & `kilvin-0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kilvin"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="Pratham Singh", email="prathms007@gmail.com" },
 ]
 description = "A minimal static site generator."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 keywords = ["static site generator", "markdow"]
 dependencies = [
-    "markdown",
+    "markdown==3.4.3",
     "Jinja2",
     "tomli",
     "python-frontmatter",
-    "livereload",
     "click",
 ]
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/shanukun/kilvin"
```

### Comparing `kilvin-0.3/src/kilvin/__main__.py` & `kilvin-0.4/src/kilvin/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import pathlib
-import sys
 
 import click
-from livereload import Server
 
 from kilvin import configs, utils
 from kilvin.cmds import build as _build
 from kilvin.cmds import init as _init
 from kilvin.cmds import new as _new
-
-
-def start_server():
-    server = Server()
-    try:
-        log.info("Serving.")
-        server.serve(root="./public")
-    except KeyboardInterrupt:
-        sys.exit(1)
+from kilvin.cmds import server as _server
 
 
 def main():
     @click.group()
     @click.version_option()
     def cli():
         """
@@ -46,10 +36,10 @@
         """Build the current project"""
         utils.clean_public()
         _build.build_proj(configs.load_config())
 
     @cli.command()
     def server():
         """Serve the current project"""
-        start_server()
+        _server.start_server()
 
     cli()
```

### Comparing `kilvin-0.3/src/kilvin/cmds/build.py` & `kilvin-0.4/src/kilvin/cmds/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 import frontmatter
 
 from kilvin import log
-from kilvin.render import renderer
+from kilvin.render import builder
 from kilvin.render.page import Page
 from kilvin.utils import copy_dir, copy_file, is_kilvin_dir, join_path
 
 DIR_CONTENT = "content"
 DIR_PUBLIC = "public"
 _INDEX = "_index.md"
 INDEX = "index.html"
@@ -83,76 +83,86 @@
         name=file_path.stem if parent else rel_path,
         rel_path=rel_path,
         html_path=html_path,
         fmatter=fmatter.metadata,
         body=fmatter.content,
         is_index=False if parent else True,
     )
-    if parent:
-        parent.insert_page(raw_page)
     return raw_page
 
 
 def process_non_md(file_path: Path):
     """
     All the files other than markdown should be directly copied to appropriate
     directory in public directory.
     """
     rel_path = get_rel_path(file_path)
     final_path = get_public_path(rel_path)
 
     copy_file(file_path, final_path)
 
 
+def handle_index_file(root_path):
+    # ./content/*/_index.md
+    index_md = join_path(root_path, _INDEX)
+
+    index_page = None
+    if index_md.exists():
+        index_page = process_md(index_md, None)
+
+    return index_page
+
+
+def handle_files(files, root_path, index_page):
+    pages = []
+    for file in files:
+        file_path = join_path(root_path, Path(file))
+
+        if not is_md(file_path):
+            process_non_md(file_path)
+        elif not is_index(file_path):
+            raw_page = process_md(file_path, index_page)
+            pages.append(raw_page)
+
+    return pages
+
+
 def find_pages():
     """
     Seek all the files in content dirs.
     """
     content_path = Path(DIR_CONTENT)
-
     pages = []
 
     prev_index = None
     for root, dirs, files in os.walk(content_path):
         # ./content/*/
         root_path = Path(root)
 
-        # ./content/*/_index.md
-        index_md = join_path(root_path, _INDEX)
+        index_page = handle_index_file(root_path)
+        sub_pages = handle_files(files, root_path, index_page)
 
-        index_page = None
-        if index_md.exists():
-            index_page = process_md(index_md, None)
+        if index_page:
+            index_page.page_list.extend(sub_pages)
+            index_page.dir_list.extend(dirs)
             pages.append(index_page)
+        else:
+            pages.extend(sub_pages)
+            index_page = prev_index
 
-        index_page = index_page if index_page else prev_index
-
-        for file in files:
-            file_path = join_path(root_path, Path(file))
-
-            if is_md(file_path) and not is_index(file_path):
-                raw_page = process_md(file_path, index_page)
-                if not index_page:
-                    pages.append(raw_page)
-            elif not is_index(file_path):
-                process_non_md(file_path)
-
-        if index_page:
-            for dir in dirs:
-                index_page.insert_dir(dir)
         prev_index = index_page
 
     return pages
 
 
 @is_kilvin_dir
 def build_proj(config):
     """
     Build the site from content and static files.
     """
 
     pages = find_pages()
-    renderer.render(pages, config)
+    builder.render(pages, config)
 
     copy_dir("./static", "./public/static")
 
     log.succ("Building finished.")
```

### Comparing `kilvin-0.3/src/kilvin/cmds/init.py` & `kilvin-0.4/src/kilvin/cmds/init.py`

 * *Files identical despite different names*

### Comparing `kilvin-0.3/src/kilvin/cmds/new.py` & `kilvin-0.4/src/kilvin/cmds/new.py`

 * *Files identical despite different names*

### Comparing `kilvin-0.3/src/kilvin/configs.py` & `kilvin-0.4/src/kilvin/configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     if is_incomplete:
         sys.exit(1)
 
 
 def load_config():
     try:
         with open("config.toml", "rb") as cf:
-            pass
             try:
                 config = tomllib.load(cf)
                 check_config(config)
                 return config
             except tomllib.TOMLDecodeError:
                 log.error("Something is wrong with the config file.")
                 sys.exit(1)
```

### Comparing `kilvin-0.3/src/kilvin/render/feed.py` & `kilvin-0.4/src/kilvin/render/feed.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime, timezone
 
 from kilvin.utils import join_path
 
 NAMESPACE = "http://www.w3.org/2005/Atom"
 
 
-def build_feed(config, sorted_pages, save_path):
+def build(config, sorted_pages, save_path):
     feed = ET.Element("feed", xmlns=NAMESPACE)
     ET.SubElement(feed, "title").text = config["title"]
     ET.SubElement(feed, "id").text = config["url"]
     ET.SubElement(feed, "url", href=config["url"])
     ET.SubElement(feed, "updated").text = datetime.now(timezone.utc).isoformat()
 
     author = ET.SubElement(feed, "author")
```

### Comparing `kilvin-0.3/src/kilvin/render/page.py` & `kilvin-0.4/src/kilvin/render/page.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,40 +25,39 @@
         return join_path("/", self.rel_path, self.name)
 
     @property
     def pages(self):
         return self.page_list
 
     @property
+    def sorted_pages(self):
+        self.page_list.sort()
+        return self.pages
+
+    @property
     def save_dir(self):
         return self.save_path.parent
 
     @property
     def template(self):
         try:
             templ = self.meta["template"]
         except KeyError:
-            log.error(f"{self.name}.md does not have a correct frontmatter.")
+            log.error(f"{self.name}.md: Invalid front matter.")
             sys.exit(1)
 
         if templ != None:
             return templ
         elif self.is_index:
             return LIST
         else:
             return SINGLE
 
     @property
     def dirs(self):
         return self.dir_list
 
-    def insert_page(self, page):
-        self.page_list.append(page)
-
-    def insert_dir(self, dir):
-        self.dir_list.append(dir)
-
     def __lt__(self, other):
         try:
             return self.meta["date"] > other.meta["date"]
         except KeyError:
             return self.url > other.url
```

### Comparing `kilvin-0.3/src/kilvin/render/renderer.py` & `kilvin-0.4/src/kilvin/render/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,96 +16,109 @@
 def is_same_path(path, other):
     CONTENT = Path("./content")
     path = CONTENT / Path(path)
     other = CONTENT / Path(other)
     return path.samefile(other)
 
 
-class Renderer:
-    """
-    Handles the rendering and saving of all markdown file with suitable context.
-    """
-
-    # Layout path in kilvin dir.
-    LAYOUT = "layouts"
-
+class KMarkdown(Markdown):
     # Extensions required for converting markdown to html.
     EXTENSIONS = [
         CodeHiliteExtension(),
         TocExtension(),
         "fenced_code",
         "footnotes",
         "md_in_html",
         "sane_lists",
         "tables",
         "abbr",
         "legacy_attrs",
     ]
+
+    def __init__(self):
+        super().__init__(extensions=self.EXTENSIONS)
+
+    def convert(self, source):
+        super().reset()
+        return super().convert(source)
+
+
+class TempEngine:
+    # Layout path in kilvin dir.
+    LAYOUT = "layouts"
     FS = jinja2.FileSystemLoader(LAYOUT)
 
-    def __init__(self, config):
-        self.config = config
-        self.md_conv = Markdown(extensions=self.EXTENSIONS)
+    def __init__(self):
         self.env = jinja2.Environment(loader=self.FS)
 
-        self.pages = defaultdict(list)
-        self.tags = []
-
     def get_template(self, templt):
         try:
             return self.env.get_template(templt)
         except TemplateNotFound:
             log.error(f"Template {templt} not found.")
             sys.exit(1)
 
-    def render_markdown(self, page):
-        html = self.md_conv.reset().convert(page.body)
-        page.body = html
-        self.tags.extend(page.meta.get("tags", ""))
-        self.pages[page.template].append(page)
+
+class Builder:
+    """
+    Handles the rendering and saving of all markdown file with suitable context.
+    """
+
+    def __init__(self, config):
+        self.config = config
+        self.conv = KMarkdown()
+        self.temp_engine = TempEngine()
+
+        self.pages = defaultdict(list)
+        self.tags = []
 
     def get_site_context(self):
         site = {}
         for key, value in self.config.items():
             site[key] = value
+
         site["tags"] = self.tags
         site["pages"] = self.pages
+
         return site
 
+    def render_markdown(self, page):
+        html = self.conv.convert(page.body)
+        page.body = html
+        self.tags.extend(page.meta.get("tags", ""))
+        self.pages[page.template].append(page)
+
+    def render_template(self, site, page, template):
+        try:
+            out = template.render(
+                site=site,
+                meta=page.meta,
+                pages=page.sorted_pages,
+                dirs=page.dirs,
+                body=page.body,
+            )
+            with open(page.save_path, "w") as f:
+                f.write(out)
+        except TemplateError as e:
+            log.error(f"{e.message}")
+            sys.exit(1)
+
+    def build_feed(self, page):
+        if page.is_index and not is_same_path(page.rel_path, "./"):
+            feed.build(self.config, page.sorted_pages, page.save_dir)
+
     def save_pages(self):
         site = self.get_site_context()
-
         for temp_name in self.pages:
-            templ = self.get_template(temp_name)
-
+            templ = self.temp_engine.get_template(temp_name)
             for page in self.pages[temp_name]:
-                sorted_pages = page.pages
-                sorted_pages.sort()
-
-                if page.is_index and not is_same_path(page.rel_path, "./"):
-                    feed.build_feed(self.config, sorted_pages, page.save_dir)
-
-                try:
-                    # TODO make template rendering part of render_markdown func.
-                    out = templ.render(
-                        site=site,
-                        meta=page.meta,
-                        pages=sorted_pages,
-                        dirs=page.dirs,
-                        body=page.body,
-                    )
-
-                    with open(page.save_path, "w") as f:
-                        f.write(out)
-
-                except TemplateError as e:
-                    log.error(f"{temp_name}: {e.message}.")
-                    sys.exit(1)
+                self.render_template(site, page, templ)
+                self.build_feed(page)
 
 
 def render(page_list, config):
-    renderer = Renderer(config)
+    builder = Builder(config)
     for page in page_list:
-        renderer.render_markdown(page)
+        builder.render_markdown(page)
         for child_page in page.pages:
-            renderer.render_markdown(child_page)
-    renderer.save_pages()
+            builder.render_markdown(child_page)
+    builder.save_pages()
```

### Comparing `kilvin-0.3/src/kilvin/utils.py` & `kilvin-0.4/src/kilvin/utils.py`

 * *Files identical despite different names*

### Comparing `kilvin-0.3/src/kilvin.egg-info/PKG-INFO` & `kilvin-0.4/src/kilvin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilvin
-Version: 0.3
+Version: 0.4
 Summary: A minimal static site generator.
 Author-email: Pratham Singh <prathms007@gmail.com>
 Project-URL: Homepage, https://github.com/shanukun/kilvin
 Project-URL: Bug Tracker, https://github.com/shanukun/kilvin/issues
 Keywords: static site generator,markdow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kilvin-0.3/src/kilvin.egg-info/SOURCES.txt` & `kilvin-0.4/src/kilvin.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 src/kilvin/__init__.py
 src/kilvin/__main__.py
 src/kilvin/configs.py
 src/kilvin/log.py
 src/kilvin/utils.py
 src/kilvin.egg-info/PKG-INFO
 src/kilvin.egg-info/SOURCES.txt
@@ -12,11 +13,12 @@
 src/kilvin.egg-info/entry_points.txt
 src/kilvin.egg-info/requires.txt
 src/kilvin.egg-info/top_level.txt
 src/kilvin/cmds/__init__.py
 src/kilvin/cmds/build.py
 src/kilvin/cmds/init.py
 src/kilvin/cmds/new.py
+src/kilvin/cmds/server.py
 src/kilvin/render/__init__.py
+src/kilvin/render/builder.py
 src/kilvin/render/feed.py
-src/kilvin/render/page.py
-src/kilvin/render/renderer.py
+src/kilvin/render/page.py
```

