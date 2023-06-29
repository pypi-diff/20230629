# Comparing `tmp/mkdocs-toc-md-0.0.7.tar.gz` & `tmp/mkdocs-toc-md-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-toc-md-0.0.7.tar", last modified: Sun May 28 09:49:19 2023, max compression
+gzip compressed data, was "mkdocs-toc-md-0.0.8.tar", last modified: Thu Jun 29 12:03:11 2023, max compression
```

## Comparing `mkdocs-toc-md-0.0.7.tar` & `mkdocs-toc-md-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.316244 mkdocs-toc-md-0.0.7/
--rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     6610 2023-05-28 09:49:19.311237 mkdocs-toc-md-0.0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6140 2023-05-28 08:31:10.000000 mkdocs-toc-md-0.0.7/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.101448 mkdocs-toc-md-0.0.7/mkdocs_toc_md/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2527 2023-05-28 06:03:42.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/hook.py
--rwxrwxrwx   0 root         (0) root         (0)     2350 2023-05-28 07:35:59.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/objects.py
--rwxrwxrwx   0 root         (0) root         (0)    12621 2023-05-28 09:34:39.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/plugin.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.284231 mkdocs-toc-md-0.0.7/mkdocs_toc_md/template/
--rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-09 12:50:24.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/template/toc.md.j2
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.250235 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     6610 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      392 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-28 09:49:19.317236 mkdocs-toc-md-0.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1300 2023-05-28 09:41:53.000000 mkdocs-toc-md-0.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 12:03:11.718265 mkdocs-toc-md-0.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     6610 2023-06-29 12:03:11.714265 mkdocs-toc-md-0.0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6140 2023-05-28 08:31:10.000000 mkdocs-toc-md-0.0.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 12:03:11.484897 mkdocs-toc-md-0.0.8/mkdocs_toc_md/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2527 2023-05-28 06:03:42.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md/hook.py
+-rwxrwxrwx   0 root         (0) root         (0)     2524 2023-06-11 02:34:03.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md/objects.py
+-rwxrwxrwx   0 root         (0) root         (0)    13593 2023-06-24 12:57:23.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md/plugin.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 12:03:11.682264 mkdocs-toc-md-0.0.8/mkdocs_toc_md/template/
+-rwxrwxrwx   0 root         (0) root         (0)      379 2023-06-24 12:51:33.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md/template/toc.md.j2
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 12:03:11.645178 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6610 2023-06-29 12:03:10.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      392 2023-06-29 12:03:11.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-29 12:03:10.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-29 12:03:10.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-06-29 12:03:10.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-06-29 12:03:10.000000 mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-29 12:03:11.720268 mkdocs-toc-md-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1300 2023-06-29 12:02:04.000000 mkdocs-toc-md-0.0.8/setup.py
```

### Comparing `mkdocs-toc-md-0.0.7/LICENSE` & `mkdocs-toc-md-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-toc-md-0.0.7/PKG-INFO` & `mkdocs-toc-md-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-toc-md
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate a table of contents markdown file
 Home-page: https://github.com/try0/mkdocs-toc-md
 Author: Ryo Tsunoda
 Author-email: try0.development@gmail.com
 License: MIT
 Keywords: mkdocs plugin toc generator
 Platform: UNKNOWN
```

### Comparing `mkdocs-toc-md-0.0.7/README.md` & `mkdocs-toc-md-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-toc-md-0.0.7/mkdocs_toc_md/hook.py` & `mkdocs-toc-md-0.0.8/mkdocs_toc_md/hook.py`

 * *Files identical despite different names*

### Comparing `mkdocs-toc-md-0.0.7/mkdocs_toc_md/objects.py` & `mkdocs-toc-md-0.0.8/mkdocs_toc_md/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,26 @@
     page_title = None
     page_description = None
     toc_headers = []
 
 
 class TocItem:
     """ headers """
-    src_level = 1
+    src_level = 0
+    level = 1
     text = None
     description = None
     url = None
     metadata = dict()
 
     def get_md_header_prefix(self) -> str:
         """ Gets level as markdown header. """
 
-        prefix = '#'
-        for num in range(self.src_level):
+        prefix = ''
+        for num in range(self.level):
             prefix += '#'
         return prefix
 
     def get_text_as_md_header(self) -> str:
         """ Gets text as markdown header. """
 
         prefix = self.get_md_header_prefix()
@@ -73,7 +74,13 @@
         if self.url:
             return '1. [' + self.text + '](' + self.url + ')'
 
         return '1. ' + self.text
 
     def has_description(self) -> bool:
         return self.description is not None
+
+    def get_src_level_as_string(self) -> str:
+        return str(self.src_level)
+    
+    def get_level_as_string(self) -> str:
+        return str(self.level)
```

### Comparing `mkdocs-toc-md-0.0.7/mkdocs_toc_md/plugin.py` & `mkdocs-toc-md-0.0.8/mkdocs_toc_md/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from pathlib import Path
 import sys
 import logging
 import os
 import re
+from typing import TYPE_CHECKING, Any, Iterator, List, Mapping, Optional, Type, TypeVar, Union
 from mkdocs import plugins
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from mkdocs.structure.pages import Page
-from mkdocs.structure.nav import Navigation
+from mkdocs.structure.nav import Navigation, Section, Link
 from mkdocs_toc_md.objects import TocConfig, TocItem, TocPageData
 from mkdocs_toc_md.hook import TocExtendModule
 from bs4 import BeautifulSoup
 from jinja2 import Environment, FileSystemLoader
 try:
     from mkdocs.plugins import event_priority
 except ImportError:
@@ -60,20 +61,36 @@
         self.i18n_plugin = None
         if self.config['integrate_mkdocs_static_i18n'] and 'i18n' in config['plugins']:
             self.i18n_plugin = config['plugins']['i18n']
 
         self.hook = TocExtendModule(self.toc_config)
 
     def on_serve(self, server, config, builder):
-        TocExtendModule.watch_file(server, builder)
+        # for dev
+        try:
+            TocExtendModule.watch_file(server, builder)
 
-    def on_nav(self, nav, config, files):
+            if 'output_path' in self.config:
+                output_path = self.config['output_path']
+                if self.i18n_plugin:
+                    for lang in self.i18n_plugin.i18n_navs:
+                        output_path_i18n = re.sub('md$', lang + '.md', output_path)
+                        if os.path.exists(output_path_i18n):
+                            server.watch(output_path_i18n, builder)
+                else:
+                    if os.path.exists(output_path):
+                        server.watch(output_path, builder)
+        except Exception as e:
+            self.logger.error('toc-md: Failed watch files', e)
+
+    def on_nav(self, nav: Navigation, config, files):
         # keep navigations
         self.nav = nav
 
+
     def on_post_page(self, output_content, page, config):
         # remove navigation items
         pattern = self.config['remove_navigation_page_pattern']
         if pattern:
             remove_navigation_page_re = re.compile(pattern)
             if remove_navigation_page_re.match(page.file.src_path):
                 self.logger.info("toc-md: Remove toc")
@@ -115,98 +132,128 @@
                     self.output(config, nav, lang, "")
 
         else:
             # default
 
             self.output(config, self.nav, "", "")
 
+    def create_toc_items(self, toc_items, nav_item: Union[Page, Section, Link], config, lang, nav_item_depth):
+
+        if nav_item.is_link and not nav_item.is_page:
+            # no page file
+            return
+        
+        if nav_item.is_section and not nav_item.is_page:
+            # no page file
+            if self.config['shift_header'] and not self.config['shift_header'] == 'none':
+                # consider nav hierarchy
+                nav_item_depth += 1
+
+            for child_item in nav_item.children:
+                self.create_toc_items(toc_items, child_item, config, lang, nav_item_depth)
+            return
+
+        # page file
+
+        page = nav_item
+        if 'output_path' in self.config:
+            output_path = self.config['output_path']
+            if page.file.src_path == output_path:
+                return
+
+        ignore = self.ignore_re and self.ignore_re.match(
+            page.file.src_path)
+        if ignore:
+            return
+
+        soup = BeautifulSoup(
+            page.content, self.config['beautiful_soup_parser'])
+
+        # extract page description
+        toc_description = ''
+        if 'pickup_description_meta' in self.config:
+            if self.config['pickup_description_meta']:
+                description_elm = soup.find(
+                    'meta', attrs={'name': 'description'})
+                if description_elm is not None:
+                    toc_description += description_elm['content']
+
+        if 'pickup_description_class' in self.config:
+            if self.config['pickup_description_class']:
+                description_elm = soup.find(
+                    True, class_=self.toc_description_class)
+                if description_elm is not None:
+                    toc_description += description_elm.text
+
+        if 'toc_md_description' in page.meta:
+            toc_description += page.meta['toc_md_description']
+
+        # create TocItem
+        src_elements = []
+        if self.use_extend_module('find_src_elements'):
+            # user impl
+            src_elements = self.hook.find_src_elements(soup, page)
+        else:
+            # default
+            src_elements = soup.find_all(self.header_names)
+
+        if self.use_extend_module('create_toc_items'):
+            # user impl
+            items = self.hook.create_toc_items(
+                page, toc_description, src_elements)
+            toc_items.extend(items)
+        else:
+            # default
+            for elm in src_elements:
+
+                toc_header = TocItem()
+                if elm.find('a', attrs={'class', 'headerlink'}):
+                    elm.a.extract()
+
+                toc_header.text = elm.text
+                toc_header.url = page.file.src_path + '#' + elm.get('id')
+
+                if elm.name == 'h1':
+                    toc_header.src_level = 1
+                    if toc_description:
+                        toc_header.description = toc_description
+                elif elm.name == 'h2':
+                    toc_header.src_level = 2
+                elif elm.name == 'h3':
+                    toc_header.src_level = 3
+                elif elm.name == 'h4':
+                    toc_header.src_level = 4
+                elif elm.name == 'h5':
+                    toc_header.src_level = 5
+                elif elm.name == 'h6':
+                    toc_header.src_level = 6
+
+                toc_header.level = (toc_header.src_level + nav_item_depth)
+
+                if self.config['shift_header'] and not self.config['shift_header'] == 'none':
+                    index_re = re.compile('.*(index.' + lang + '.md$|index.md$)')
+                    if self.config['shift_header'] == 'after_h1':
+                        if index_re.match(page.file.src_path):
+                            toc_header.level -= 1
+                    elif self.config['shift_header'] == 'after_h1_of_index':
+                        if index_re.match(page.file.src_path) and toc_header.src_level == 1:
+                            toc_header.level -= 1
+
+                if self.use_extend_module('on_create_toc_item'):
+                    # user hook
+                    self.hook.on_create_toc_item(toc_header, elm, page)
+                toc_items.append(toc_header)
+
     def output(self, config, nav, lang, folder):
 
         # Pickup headers
         toc_headers = []
-        for page in nav.pages:
-            if 'output_path' in self.config:
-                output_path = self.config['output_path']
-                if page.file.src_path == output_path:
-                    continue
-
-            ignore = self.ignore_re and self.ignore_re.match(
-                page.file.src_path)
-            if ignore:
-                continue
-
-            soup = BeautifulSoup(
-                page.content, self.config['beautiful_soup_parser'])
-
-            # extract page description
-            toc_description = ''
-            if 'pickup_description_meta' in self.config:
-                if self.config['pickup_description_meta']:
-                    description_elm = soup.find(
-                        'meta', attrs={'name': 'description'})
-                    if description_elm is not None:
-                        toc_description += description_elm['content']
-
-            if 'pickup_description_class' in self.config:
-                if self.config['pickup_description_class']:
-                    description_elm = soup.find(
-                        True, class_=self.toc_description_class)
-                    if description_elm is not None:
-                        toc_description += description_elm.text
-
-            if 'toc_md_description' in page.meta:
-                toc_description += page.meta['toc_md_description']
-
-            # create TocItem
-            src_elements = []
-            if self.use_extend_module('find_src_elements'):
-                # user impl
-                src_elements = self.hook.find_src_elements(soup, page)
-            else:
-                # default
-                src_elements = soup.find_all(self.header_names)
-
-            if self.use_extend_module('create_toc_items'):
-                # user impl
-                items = self.hook.create_toc_items(
-                    page, toc_description, src_elements)
-                toc_headers.extend(items)
-            else:
-                # default
-                for elm in src_elements:
-
-                    toc_header = TocItem()
-                    if elm.find('a', attrs={'class', 'headerlink'}):
-                        elm.a.extract()
-
-                    toc_header.text = elm.text
-                    toc_header.url = page.file.src_path + '#' + elm.get('id')
-
-                    if elm.name == 'h1':
-                        toc_header.src_level = 1
-                        if toc_description:
-                            toc_header.description = toc_description
-                    elif elm.name == 'h2':
-                        toc_header.src_level = 2
-                    elif elm.name == 'h3':
-                        toc_header.src_level = 3
-                    elif elm.name == 'h4':
-                        toc_header.src_level = 4
-                    elif elm.name == 'h5':
-                        toc_header.src_level = 5
-                    elif elm.name == 'h6':
-                        toc_header.src_level = 6
-
-                    if self.config['shift_header'] and not self.config['shift_header'] == 'none':
-                        self.shift_header(toc_header, page, lang)
-
-                    if self.use_extend_module('on_create_toc_item'):
-                        # user hook
-                        self.hook.on_create_toc_item(toc_header, elm, page)
-                    toc_headers.append(toc_header)
+        nav_item_depth = 1
+        for nav_item in nav.items:
+            self.create_toc_items(toc_headers, nav_item, config, lang, nav_item_depth)
 
         if self.use_extend_module('on_before_output'):
             # user hook
             self.hook.on_before_output(nav, toc_headers)
 
         # create template arg
         template_param = TocPageData()
@@ -282,30 +329,8 @@
                 if self.is_build_command:
                     self.logger.warning(
                         'toc-md: Command line contains [build]. You may need to build again to render toc md as html.')
 
     def use_extend_module(self, name) -> bool:
         return 'extend_module' in self.config and self.config['extend_module'] and self.hook.can_call(name)
 
-    def shift_header(self, item: TocItem, page: Page, lang):
-
-        if page.file.src_path.count(os.sep) <= 0:
-            # skip root
-            return
 
-        index_re = re.compile('.*(index.' + lang + '.md$|index.md$)')
-        hasindex = False
-        for path in os.listdir(Path(page.file.abs_src_path).parent):
-            if index_re.match(path):
-                hasindex = True
-                break
-
-        if self.config['shift_header'] == 'after_index':
-            if hasindex and not index_re.match(page.file.src_path):
-                item.src_level += 1
-
-        if self.config['shift_header'] == 'after_h1_of_index':
-            if hasindex and (not index_re.match(page.file.src_path)):
-                item.src_level += 1
-            elif index_re.match(page.file.src_path) and item.src_level > 1:
-                item.src_level += 1
-
```

### Comparing `mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/PKG-INFO` & `mkdocs-toc-md-0.0.8/mkdocs_toc_md.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-toc-md
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate a table of contents markdown file
 Home-page: https://github.com/try0/mkdocs-toc-md
 Author: Ryo Tsunoda
 Author-email: try0.development@gmail.com
 License: MIT
 Keywords: mkdocs plugin toc generator
 Platform: UNKNOWN
```

### Comparing `mkdocs-toc-md-0.0.7/setup.py` & `mkdocs-toc-md-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # python setup.py develop
 # python setup.py sdist bdist_wheel
 # twine check dist/mkdocs-toc-md-x.x.x.tar.gz
 # twine upload --repository pypi dist/*
 setup(
     name='mkdocs-toc-md',
-    version='0.0.7',
+    version='0.0.8',
     description='Generate a table of contents markdown file',
     long_description=io.open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs plugin toc generator',
     author='Ryo Tsunoda',
     author_email='try0.development@gmail.com',
     url='https://github.com/try0/mkdocs-toc-md',
```

