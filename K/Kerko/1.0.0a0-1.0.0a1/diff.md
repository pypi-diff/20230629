# Comparing `tmp/Kerko-1.0.0a0.tar.gz` & `tmp/Kerko-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kerko-1.0.0a0.tar", last modified: Tue Jun 27 00:18:43 2023, max compression
+gzip compressed data, was "Kerko-1.0.0a1.tar", last modified: Thu Jun 29 21:20:35 2023, max compression
```

## Comparing `Kerko-1.0.0a0.tar` & `Kerko-1.0.0a1.tar`

### file list

```diff
@@ -1,216 +1,219 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/
--rw-rw-r--   0 david     (1000) david     (1000)    28770 2023-06-27 00:15:39.000000 Kerko-1.0.0a0/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)    35149 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/LICENSE.txt
--rw-rw-r--   0 david     (1000) david     (1000)      215 2023-06-27 00:18:19.000000 Kerko-1.0.0a0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    43335 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    12613 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/babel.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/docs/
--rw-rw-r--   0 david     (1000) david     (1000)     2777 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/background.md
--rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/changelog.md
--rw-rw-r--   0 david     (1000) david     (1000)     7272 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/config-basics.md
--rw-rw-r--   0 david     (1000) david     (1000)    23335 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/config-params.md
--rw-rw-r--   0 david     (1000) david     (1000)     4040 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/contributing.md
--rw-rw-r--   0 david     (1000) david     (1000)      885 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/deployment.md
--rw-rw-r--   0 david     (1000) david     (1000)    14801 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/getting-started.md
--rw-rw-r--   0 david     (1000) david     (1000)    18067 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/index.md
--rw-rw-r--   0 david     (1000) david     (1000)     3351 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/localization.md
--rw-rw-r--   0 david     (1000) david     (1000)     6988 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/recipes.md
--rw-rw-r--   0 david     (1000) david     (1000)     4500 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/synchronization.md
--rw-rw-r--   0 david     (1000) david     (1000)     1479 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/docs/troubleshooting.md
--rw-rw-r--   0 david     (1000) david     (1000)     2193 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/mkdocs.yml
--rw-rw-r--   0 david     (1000) david     (1000)      629 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     3392 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     1336 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/Kerko.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    43335 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     9072 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       39 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      507 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        6 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/Kerko.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)      962 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     6433 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)     6795 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/codecs.py
--rw-rw-r--   0 david     (1000) david     (1000)    36095 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/composer.py
--rw-rw-r--   0 david     (1000) david     (1000)    11600 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/config_helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     7623 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/criteria.py
--rw-rw-r--   0 david     (1000) david     (1000)     4747 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)    18790 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/default_config.toml
--rw-rw-r--   0 david     (1000) david     (1000)     1294 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    26611 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/extractors.py
--rw-rw-r--   0 david     (1000) david     (1000)      511 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/forms.py
--rw-rw-r--   0 david     (1000) david     (1000)     2123 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/jinja2.py
--rw-rw-r--   0 david     (1000) david     (1000)     1674 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/renderers.py
--rw-rw-r--   0 david     (1000) david     (1000)    12863 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/searcher.py
--rw-rw-r--   0 david     (1000) david     (1000)      836 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/shortcuts.py
--rw-rw-r--   0 david     (1000) david     (1000)    27160 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/specs.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/static/kerko/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/static/kerko/css/
--rw-rw-r--   0 david     (1000) david     (1000)     2027 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/css/styles.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/static/kerko/js/
--rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/item.js
--rw-rw-r--   0 david     (1000) david     (1000)     1289 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/open_in_zotero.js
--rw-rw-r--   0 david     (1000) david     (1000)     1369 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/print.js
--rw-rw-r--   0 david     (1000) david     (1000)     2259 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/static/kerko/js/search.js
--rw-rw-r--   0 david     (1000) david     (1000)     2564 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/storage.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.591897 Kerko-1.0.0a0/src/kerko/sync/
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4103 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/attachments.py
--rw-rw-r--   0 david     (1000) david     (1000)     5301 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)     3829 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/index.py
--rw-rw-r--   0 david     (1000) david     (1000)    11723 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/sync/zotero.py
--rw-rw-r--   0 david     (1000) david     (1000)     3035 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/tags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/templates/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)      155 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_attributes.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_badges.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1234 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_collapse.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      375 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      560 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_field.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6610 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_facets.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1464 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_item-relations.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_navbar_brand.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      280 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_navbar_items.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     3908 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_pager.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     4013 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_preferences.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-form.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    10118 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-help.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      578 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-metas.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     5479 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_search-result.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/_sorter.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     4282 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/atom.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     2184 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/base.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    20615 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6640 2023-06-26 23:55:07.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/layout.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/search-item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    13015 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      348 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/sitemap.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      325 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/templates/kerko/sitemap_index.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/text.py
--rw-rw-r--   0 david     (1000) david     (1000)     2579 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/transformers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/de/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    18452 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    26381 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.po
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/fr/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    22918 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    33607 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.po
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.587897 Kerko-1.0.0a0/src/kerko/translations/pt/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/
--rw-rw-r--   0 david     (1000) david     (1000)    20867 2023-06-27 00:18:43.000000 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    30605 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.po
--rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/tree.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/views/
--rw-rw-r--   0 david     (1000) david     (1000)       52 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2329 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/breadbox.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/src/kerko/views/item/
--rw-rw-r--   0 david     (1000) david     (1000)     1361 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1660 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/creators.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/facets.py
--rw-rw-r--   0 david     (1000) david     (1000)     4160 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     2937 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/item/relations.py
--rw-rw-r--   0 david     (1000) david     (1000)     2399 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/pager.py
--rw-rw-r--   0 david     (1000) david     (1000)    17274 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/routes.py
--rw-rw-r--   0 david     (1000) david     (1000)    11280 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/search.py
--rw-rw-r--   0 david     (1000) david     (1000)      690 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/src/kerko/views/sorter.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/tests/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.595897 Kerko-1.0.0a0/tests/integration_testing/
--rw-rw-r--   0 david     (1000) david     (1000)     1649 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/README.md
--rw-rw-r--   0 david     (1000) david     (1000)    10620 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-27 00:18:43.603897 Kerko-1.0.0a0/tests/integration_testing/api_responses/
--rw-rw-r--   0 david     (1000) david     (1000)     1071 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/collections.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/fulltext.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)      329 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
--rw-rw-r--   0 david     (1000) david     (1000)      498 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
--rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      336 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)       88 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)      347 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)      265 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
--rw-rw-r--   0 david     (1000) david     (1000)      259 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      337 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      421 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)     1574 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)     1251 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      803 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1637 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_book.json
--rw-rw-r--   0 david     (1000) david     (1000)     1706 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)     1128 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_case.json
--rw-rw-r--   0 david     (1000) david     (1000)     1423 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)     1718 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)     1047 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      649 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_email.json
--rw-rw-r--   0 david     (1000) david     (1000)     1722 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1284 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      808 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1338 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      645 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1050 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)     1711 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)     1471 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_map.json
--rw-rw-r--   0 david     (1000) david     (1000)     1402 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_note.json
--rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      906 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1560 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      872 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1430 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_report.json
--rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)     1265 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1576 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      809 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypes.json
--rw-rw-r--   0 david     (1000) david     (1000)    42561 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/items.json
--rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/items_versions.json
--rwxrwxr-x   0 david     (1000) david     (1000)     2577 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/integration_testing/api_responses/update.bash
--rw-rw-r--   0 david     (1000) david     (1000)     8683 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_atom_feed.py
--rw-rw-r--   0 david     (1000) david     (1000)     5321 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_config.py
--rw-rw-r--   0 david     (1000) david     (1000)    13271 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)    16760 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_item_meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     4919 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_pager.py
--rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_sitemap.py
--rw-rw-r--   0 david     (1000) david     (1000)     1863 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_sync.py
--rw-rw-r--   0 david     (1000) david     (1000)     8126 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tests/test_tags.py
--rw-rw-r--   0 david     (1000) david     (1000)      640 2023-06-26 22:51:54.000000 Kerko-1.0.0a0/tox.ini
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/
+-rw-rw-r--   0 david     (1000) david     (1000)    30568 2023-06-29 21:13:54.000000 Kerko-1.0.0a1/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35149 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/LICENSE.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      215 2023-06-27 00:18:19.000000 Kerko-1.0.0a1/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)    45279 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    12761 2023-06-29 02:32:04.000000 Kerko-1.0.0a1/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/babel.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     3085 2023-06-28 13:58:59.000000 Kerko-1.0.0a1/docs/about.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/docs/assets/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/docs/assets/images/
+-rw-rw-r--   0 david     (1000) david     (1000)   118374 2023-06-29 00:25:36.000000 Kerko-1.0.0a1/docs/assets/images/kerko-zotero-mapping.png
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/changelog.md
+-rw-rw-r--   0 david     (1000) david     (1000)     7656 2023-06-28 22:32:39.000000 Kerko-1.0.0a1/docs/config-basics.md
+-rw-rw-r--   0 david     (1000) david     (1000)    29022 2023-06-29 13:44:46.000000 Kerko-1.0.0a1/docs/config-params.md
+-rw-rw-r--   0 david     (1000) david     (1000)     4040 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/contributing.md
+-rw-rw-r--   0 david     (1000) david     (1000)      885 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/deployment.md
+-rw-rw-r--   0 david     (1000) david     (1000)    14801 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/getting-started.md
+-rw-rw-r--   0 david     (1000) david     (1000)    18059 2023-06-29 02:31:46.000000 Kerko-1.0.0a1/docs/index.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3351 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/localization.md
+-rw-rw-r--   0 david     (1000) david     (1000)    11858 2023-06-29 13:33:33.000000 Kerko-1.0.0a1/docs/recipes.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5410 2023-06-28 17:36:03.000000 Kerko-1.0.0a1/docs/synchronization.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2646 2023-06-28 23:08:58.000000 Kerko-1.0.0a1/docs/troubleshooting.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2216 2023-06-29 12:28:30.000000 Kerko-1.0.0a1/mkdocs.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      629 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     3407 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     1336 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/Kerko.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    45279 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     9111 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       39 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      522 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        6 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      962 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7810 2023-06-29 20:49:30.000000 Kerko-1.0.0a1/src/kerko/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6795 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/codecs.py
+-rw-rw-r--   0 david     (1000) david     (1000)    36005 2023-06-27 19:41:10.000000 Kerko-1.0.0a1/src/kerko/composer.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11971 2023-06-28 21:41:17.000000 Kerko-1.0.0a1/src/kerko/config_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7621 2023-06-27 20:14:00.000000 Kerko-1.0.0a1/src/kerko/criteria.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4747 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18342 2023-06-28 18:38:21.000000 Kerko-1.0.0a1/src/kerko/default_config.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1294 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    26611 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/extractors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/forms.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2123 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/jinja2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1674 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/renderers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12863 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/searcher.py
+-rw-rw-r--   0 david     (1000) david     (1000)      836 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/shortcuts.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27169 2023-06-27 19:33:34.000000 Kerko-1.0.0a1/src/kerko/specs.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/static/kerko/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/kerko/static/kerko/css/
+-rw-rw-r--   0 david     (1000) david     (1000)     2027 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/css/styles.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.661548 Kerko-1.0.0a1/src/kerko/static/kerko/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/item.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1289 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/open_in_zotero.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1369 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/print.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2259 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/search.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2564 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/storage.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.661548 Kerko-1.0.0a1/src/kerko/sync/
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/sync/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4139 2023-06-27 18:19:44.000000 Kerko-1.0.0a1/src/kerko/sync/attachments.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5330 2023-06-27 18:19:02.000000 Kerko-1.0.0a1/src/kerko/sync/cache.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3852 2023-06-27 18:19:02.000000 Kerko-1.0.0a1/src/kerko/sync/index.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11723 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/sync/zotero.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3035 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/tags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/templates/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      155 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_attributes.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_badges.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1234 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_collapse.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      375 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      560 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_field.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     6610 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facets.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1464 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_item-relations.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_navbar_brand.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      280 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_navbar_items.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     3908 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_pager.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4013 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_preferences.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-form.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    10118 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-help.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      578 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-metas.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     5479 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-result.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_sorter.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4282 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/atom.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     2184 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/base.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    20525 2023-06-27 19:54:48.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     6640 2023-06-26 23:55:07.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/layout.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/search-item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    12963 2023-06-27 20:14:43.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      348 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/sitemap.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      325 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/sitemap_index.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2579 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/transformers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/de/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    18452 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    26381 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/fr/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    22918 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    33607 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/pt/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/
+-rw-rw-r--   0 david     (1000) david     (1000)    20867 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    30605 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.po
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/tree.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       52 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2329 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/breadbox.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/views/item/
+-rw-rw-r--   0 david     (1000) david     (1000)     1361 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1660 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/creators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/facets.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4160 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2937 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/relations.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2399 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17134 2023-06-27 19:55:17.000000 Kerko-1.0.0a1/src/kerko/views/routes.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11265 2023-06-27 19:55:24.000000 Kerko-1.0.0a1/src/kerko/views/search.py
+-rw-rw-r--   0 david     (1000) david     (1000)      690 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/sorter.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/tests/integration_testing/
+-rw-rw-r--   0 david     (1000) david     (1000)     1649 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10620 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/tests/integration_testing/api_responses/
+-rw-rw-r--   0 david     (1000) david     (1000)     1071 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/collections.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/fulltext.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)      329 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)      498 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      336 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)       88 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)      347 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)      265 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)      259 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      337 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      421 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1574 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1251 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      803 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1637 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1706 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1128 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1423 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1718 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1047 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      649 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1722 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1284 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      808 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1338 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      645 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1050 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1711 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1471 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1402 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      906 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1560 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      872 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1430 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1265 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1576 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      809 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypes.json
+-rw-rw-r--   0 david     (1000) david     (1000)    42561 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/items.json
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/items_versions.json
+-rwxrwxr-x   0 david     (1000) david     (1000)     2577 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/update.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     8683 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_atom_feed.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5321 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_config.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13271 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16760 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_item_meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4919 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_sitemap.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1863 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_sync.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8126 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_tags.py
+-rw-rw-r--   0 david     (1000) david     (1000)      640 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tox.ini
```

### Comparing `Kerko-1.0.0a0/CHANGELOG.md` & `Kerko-1.0.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,63 @@
 # Changelog
 
-For changes that might be specific to KerkoApp, please refer to the [KerkoApp
-changelog](https://github.com/whiskyechobravo/kerkoapp/blob/master/CHANGELOG.md).
+## 1.0.0alpha1 (2023-06-29)
 
+Features:
+
+- Add the `--full` option to the `sync` command line interface (CLI) command.
+
+Bug fixes:
 
-## 1.0.0alpha0
+- Fix validation pattern too restrictive for the `kerko.facets.*.collection_key`
+  configuration parameter.
+- Fix incorrect typing for the `kerko.features.download_results_max_count` and
+  `kerko.features.print_results_max_count` configuration parameters.
+
+Other changes:
+
+- Rename the default branch of the repository from 'master' to 'main'. If you
+  have cloned the repository with Git, use the following commands to rename your
+  local branch:
+
+    ```bash
+    git branch -m master main
+    git fetch origin
+    git branch -u origin/main main
+    git remote set-head origin -a
+    ```
+
+- Make the `config` CLI command show the configuration in TOML format.
+- Make the `config` CLI command hide secrets by default. Add a `--show-secrets`
+  option.
+- Improve documentation.
+
+Backwards incompatible changes:
+
+- Prevent the `clean` CLI command from cleaning everything by default. To delete
+  everything, you now have to run `flask kerko clean everything`. This may help
+  accidental deletion of the cache or the search index, which in some instances
+  can take long to rebuild.
+- Rename the following configuration parameters:
+    - `kerko.citation_formats.*` → `kerko.bib_formats.*`.
+    - `kerko.features.download_citations_link` → `kerko.features.download_results_link`
+    - `kerko.features.download_citations_max_count` → `kerko.features.download_results_max_count`
+    - `kerko.features.print_citations_link` → `kerko.features.print_results_link`
+    - `kerko.features.print_citations_max_count` → `kerko.features.print_results_max_count`
+- Rename the following views:
+    - `item_citation_download` → `item_bib_download`
+    - `search_citation_download` → `search_bib_download`
+
+
+## 1.0.0alpha0 (2023-06-26)
 
 *Warning:* Upgrading from version 0.9 or earlier will require that you adapt
-your installation and configuration (if you are using KerkoApp, make sure to
-check its changelog), then rebuild your search index. Use the following
-commands, then restart the application:
+your installation and configuration files, then rebuild your search index. Use
+the commands below, then restart the application. If you are using KerkoApp,
+make sure to check its [changelog][KerkoApp_changelog].
 
 ```bash
 flask kerko clean index
 flask kerko sync index
 ```
 
 Features:
@@ -616,7 +660,10 @@
 ## 0.3alpha1 (2019-07-17)
 
 - Fix broken links in documentation.
 
 ## 0.3alpha0 (2019-07-16)
 
 - First PyPI release.
+
+
+[KerkoApp_changelog]: https://github.com/whiskyechobravo/kerkoapp/blob/main/CHANGELOG.md
```

### Comparing `Kerko-1.0.0a0/LICENSE.txt` & `Kerko-1.0.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/PKG-INFO` & `Kerko-1.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Kerko
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
-Home-page: https://github.com/whiskyechobravo/kerko
+Home-page: https://whiskyechobravo.github.io/kerko/
 Author: David Lesieur
 Author-email: kerko@whiskyechobravo.com
 Project-URL: Documentation, https://whiskyechobravo.github.io/kerko/
 Project-URL: Code, https://github.com/whiskyechobravo/kerko
-Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/master/CHANGELOG.md
+Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/main/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/whiskyechobravo/kerko/issues
 Keywords: academia,bibliography,bibliographies,flask,search,zotero
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -198,14 +198,16 @@
   You may define such relations using Zotero's _Related_ field. Moreover, Kerko
   adds the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
   through notes. Custom applications can add more types of relations if desired.
 - **Badges**: custom applications can have icons conditionally displayed next to
   items.
 - **Responsive design**: the simple default implementation works on large
   monitors as well as on small screens. It is based on [Bootstrap].
+- **Google Analytics integration**: just provide a Google Analytics stream ID to
+  have Kerko automatically include the tracking code into its pages.
 - **Integration**: as a Flask [blueprint][Flask_blueprint], Kerko can be
   integrated into any Flask application. For a standalone application, however,
   you may simply install [KerkoApp].
 - **Customizable front-end**: applications may partly or fully replace the
   default templates, scripts and stylesheets with their own.
 - **Command line interface (CLI)**: Kerko provides commands for synchronizing or
   deleting its data.
@@ -236,15 +238,15 @@
 [Dublin_Core]: https://en.wikipedia.org/wiki/Dublin_Core
 [Flask]: https://pypi.org/project/Flask/
 [Flask_blueprint]: https://flask.palletsprojects.com/en/latest/blueprints/
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [Kerko_actions]: https://github.com/whiskyechobravo/kerko/actions
 [Kerko_documentation]: https://whiskyechobravo.github.io/kerko/
 [Kerko_pypi]: https://pypi.org/project/Kerko/
-[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/src/kerko/translations
+[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/main/src/kerko/translations
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
 [Snowball]: https://snowballstem.org/
 [TOML]: https://toml.io/
 [Twelve-factor_App]: https://12factor.net/config
 [Whoosh]: https://pypi.org/project/Whoosh/
 [XML_Sitemap]: https://www.sitemaps.org/
@@ -253,24 +255,68 @@
 [Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
 [Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
 [Zotero_schema]: https://api.zotero.org/schema
 [Zotero_styles]: https://www.zotero.org/styles/
 
 # Changelog
 
-For changes that might be specific to KerkoApp, please refer to the [KerkoApp
-changelog](https://github.com/whiskyechobravo/kerkoapp/blob/master/CHANGELOG.md).
+## 1.0.0alpha1 (2023-06-29)
 
+Features:
+
+- Add the `--full` option to the `sync` command line interface (CLI) command.
+
+Bug fixes:
 
-## 1.0.0alpha0
+- Fix validation pattern too restrictive for the `kerko.facets.*.collection_key`
+  configuration parameter.
+- Fix incorrect typing for the `kerko.features.download_results_max_count` and
+  `kerko.features.print_results_max_count` configuration parameters.
+
+Other changes:
+
+- Rename the default branch of the repository from 'master' to 'main'. If you
+  have cloned the repository with Git, use the following commands to rename your
+  local branch:
+
+    ```bash
+    git branch -m master main
+    git fetch origin
+    git branch -u origin/main main
+    git remote set-head origin -a
+    ```
+
+- Make the `config` CLI command show the configuration in TOML format.
+- Make the `config` CLI command hide secrets by default. Add a `--show-secrets`
+  option.
+- Improve documentation.
+
+Backwards incompatible changes:
+
+- Prevent the `clean` CLI command from cleaning everything by default. To delete
+  everything, you now have to run `flask kerko clean everything`. This may help
+  accidental deletion of the cache or the search index, which in some instances
+  can take long to rebuild.
+- Rename the following configuration parameters:
+    - `kerko.citation_formats.*` → `kerko.bib_formats.*`.
+    - `kerko.features.download_citations_link` → `kerko.features.download_results_link`
+    - `kerko.features.download_citations_max_count` → `kerko.features.download_results_max_count`
+    - `kerko.features.print_citations_link` → `kerko.features.print_results_link`
+    - `kerko.features.print_citations_max_count` → `kerko.features.print_results_max_count`
+- Rename the following views:
+    - `item_citation_download` → `item_bib_download`
+    - `search_citation_download` → `search_bib_download`
+
+
+## 1.0.0alpha0 (2023-06-26)
 
 *Warning:* Upgrading from version 0.9 or earlier will require that you adapt
-your installation and configuration (if you are using KerkoApp, make sure to
-check its changelog), then rebuild your search index. Use the following
-commands, then restart the application:
+your installation and configuration files, then rebuild your search index. Use
+the commands below, then restart the application. If you are using KerkoApp,
+make sure to check its [changelog][KerkoApp_changelog].
 
 ```bash
 flask kerko clean index
 flask kerko sync index
 ```
 
 Features:
@@ -873,7 +919,10 @@
 ## 0.3alpha1 (2019-07-17)
 
 - Fix broken links in documentation.
 
 ## 0.3alpha0 (2019-07-16)
 
 - First PyPI release.
+
+
+[KerkoApp_changelog]: https://github.com/whiskyechobravo/kerkoapp/blob/main/CHANGELOG.md
```

### Comparing `Kerko-1.0.0a0/README.md` & `Kerko-1.0.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
   You may define such relations using Zotero's _Related_ field. Moreover, Kerko
   adds the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
   through notes. Custom applications can add more types of relations if desired.
 - **Badges**: custom applications can have icons conditionally displayed next to
   items.
 - **Responsive design**: the simple default implementation works on large
   monitors as well as on small screens. It is based on [Bootstrap].
+- **Google Analytics integration**: just provide a Google Analytics stream ID to
+  have Kerko automatically include the tracking code into its pages.
 - **Integration**: as a Flask [blueprint][Flask_blueprint], Kerko can be
   integrated into any Flask application. For a standalone application, however,
   you may simply install [KerkoApp].
 - **Customizable front-end**: applications may partly or fully replace the
   default templates, scripts and stylesheets with their own.
 - **Command line interface (CLI)**: Kerko provides commands for synchronizing or
   deleting its data.
@@ -194,15 +196,15 @@
 [Dublin_Core]: https://en.wikipedia.org/wiki/Dublin_Core
 [Flask]: https://pypi.org/project/Flask/
 [Flask_blueprint]: https://flask.palletsprojects.com/en/latest/blueprints/
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [Kerko_actions]: https://github.com/whiskyechobravo/kerko/actions
 [Kerko_documentation]: https://whiskyechobravo.github.io/kerko/
 [Kerko_pypi]: https://pypi.org/project/Kerko/
-[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/src/kerko/translations
+[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/main/src/kerko/translations
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
 [Snowball]: https://snowballstem.org/
 [TOML]: https://toml.io/
 [Twelve-factor_App]: https://12factor.net/config
 [Whoosh]: https://pypi.org/project/Whoosh/
 [XML_Sitemap]: https://www.sitemaps.org/
```

### Comparing `Kerko-1.0.0a0/docs/background.md` & `Kerko-1.0.0a1/docs/about.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-# Project background
+# About
 
-Kerko was inspired by two prior projects:
+Kerko was inspired by prior work accomplished by [Whisky Echo
+Bravo][Whisky_Echo_Bravo] on two projects:
 
 - [Bibliographie sur l’histoire de
   Montréal](https://bibliomontreal.uqam.ca/bibliographie/), developed in 2014 by
   David Lesieur and Patrick Fournier, of Whisky Echo Bravo, for the [Laboratoire
   d'histoire et de patrimoine de Montréal](https://lhpm.uqam.ca/) (Université du
   Québec à Montréal, Canada).
 - [Bibliography on English-speaking Quebec](http://quescren.concordia.ca/),
   developed in 2017 by David Lesieur, for the [Quebec English-Speaking
   Communities Research Network
   (QUESCREN)](https://www.concordia.ca/artsci/scpa/quescren.html) (Concordia
   University, Canada).
 
-Later on, it became clear that other organizations needed a similar solution.
-However, software from the prior projects had to be rewritten so it could more
-easily be configured for different bibliographies from organizations with
-different needs. That led to Kerko, whose initial development was made possible
-through the following project:
+In 2019, [Whisky Echo Bravo][Whisky_Echo_Bravo] was asked to work on another
+similar project. That made it clear that a general solution would benefit many
+organizations. However, software from the prior projects had to be rewritten in
+order to be more adaptable to a variety of needs. That led to Kerko, whose
+initial development was made possible through the following project:
 
 - [Bibliographie francophone sur l'archivistique](https://bibliopiaf.ebsi.umontreal.ca/),
   funded by the
   [Association internationale des archives francophones (AIAF)](http://www.aiaf.org/)
   and hosted by the
   [École de bibliothéconomie et des sciences de l’information (EBSI)](https://ebsi.umontreal.ca/)
   (Université de Montréal, Canada).
 
+Since then, Kerko has continued to evolve, thanks to work by [Whisky Echo
+Bravo][Whisky_Echo_Bravo] and other contributors, often through funding provided
+by organizations needing new features or customizations of Kerko.
+
 ## Design choices
 
 Here are some of the design choices that have guided the development of Kerko so
 far:
 
-- Do not build a back-end. Let Zotero act as the "content management" system.
+- Do not build back-end software. Let Zotero manage the data.
 - Allow Kerko to integrate into richer web applications.
 - Only provide features that pertain to the exploration of a bibliography.
   Other features, even when they are common to many web sites, do not belong to
   Kerko and should be left to the applications to implement.
 - Use a lightweight framework to avoid carrying many features that are not
   needed by Kerko (Flask was selected for this reason).
 - Use pure Python dependencies to keep installation and deployment simple (Hence
   the use of Whoosh for search, for example, instead of Elasticsearch or Solr).
-- Use a classic fullstack architecture. Keep it simple and avoid asset
-  management. Some will want to replace the templates and stylesheets anyway.
+- Use a classic server-side rendering architecture. Keep it simple and avoid
+  asset management when possible.
 
 ## Etymology
 
 The name _Zotero_ reportedly derives from the Albanian word _zotëroj_, which
 means "to learn something extremely well, that is to master or acquire a skill
 in learning" (Source: Mark Dingemanse, 2008, [Etymology of
 Zotero](http://ideophone.org/zotero-etymology/)).
 
 The name _Kerko_ is a nod to Zotero as it takes a similar etymological route: it
 derives from the Albanian word _kërkoj_, which means "to ask, to request, to
 seek, to look for, to demand, to search" and seems fit to describe a search
 tool.
+
+
+[Whisky_Echo_Bravo]: https://whiskyechobravo.com/
```

### Comparing `Kerko-1.0.0a0/docs/config-basics.md` & `Kerko-1.0.0a1/docs/config-basics.md`

 * *Files 2% similar despite different names*

```diff
@@ -170,12 +170,25 @@
 from kerko.config_helpers import config_set
 config_set(app.config, "kerko.meta.title", "My Awesome Bibliography")
 ```
 
 Such assignments must be done during the initialization process. The application
 cannot change a setting while responding to a request.
 
+## Verifying the configuration
+
+With configuration parameters potentially taking values from different sources
+(default values defined by Kerko, environment variables, configuration files),
+you may sometimes want to verify the actual values taken by each parameter.
+
+The following command will show the parameters of the application and their
+values:
+
+```bash
+flask kerko config
+```
+
 
 [Flask_dotenv]: https://flask.palletsprojects.com/en/2.3.x/cli/#environment-variables-from-dotenv
 [Flask_instance_folder]: https://flask.palletsprojects.com/en/2.3.x/config/#instance-folders
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [TOML]: https://toml.io/
```

### Comparing `Kerko-1.0.0a0/docs/config-params.md` & `Kerko-1.0.0a1/docs/config-params.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,707 +1,1087 @@
 # Configuration parameters
 
 This section describes most configuration parameters available to Kerko and
-KerkoApp.
+[KerkoApp].
 
 Unless indicated otherwise, all parameters are optional and will take a default
 value if omitted from your configuration.
 
-**TODO:docs: Specify the data type of each parameter**
-
-**TODO:docs: For each parameter, specify if clean and/or sync is required**
-
-**TODO:docs: Consider referring to Kerko's `default_config.toml`, especially for viewing the default facets, fields, sorts, etc.**
-
 !!! note
 
     Flask and Flask extensions loaded by the application may provide additional
     configuration parameters that are not described in this manual. To find
     those, please refer to the documentation of the relevant package.
 
-!!! warning "Changing settings can be disruptive"
+!!! warning "Changing configuration can be disruptive"
 
-    Changing the configuration requires that you at least restart the
-    application for the change to become effective.
+    Making any change to a configuration file requires that you at least restart
+    the application afterwards for the change to become effective.
 
-    Moreover, many parameters affect the structure of the cache or the search
-    index that Kerko depends on. Changing such parameters may require that you
-    rebuild the cache or the search index. See [Useful
-    commands](synchronization.md#useful-commands) for cleaning and
-    synchronization operations.
+    Moreover, some parameters have an effect on the structure of the cache or
+    the search index that Kerko depends on. Changing such parameters may require
+    that you rebuild either. The documentation of each concerned parameters
+    indicates what actions are required after a change.
 
 !!! warning "Prefix your environment variables"
 
     KerkoApp users must prefix parameter names with `KERKOAPP_` when configuring
-    them as environment variables. However, no prefix should be used in TOML
-    files. See [Environment variables](config-basics.md#environment-variables)
-    for details on setting such variables.
+    them as environment variables. However, that prefix should be used when the
+    same parameter is set in a TOML file. See [environment variables] for
+    details on setting such variables.
+
+---
 
 ## `BABEL_DEFAULT_LOCALE`
 
-The default language of the user interface. Defaults to `'en'`.
+The default language of the user interface.
+
+Type: String <br>
+Default value: `"en"`
+
+---
 
 ## `BABEL_DEFAULT_TIMEZONE`
 
-The timezone to use for user facing times. Defaults to `'UTC'`. Any timezone
-name supported by the [pytz] package should work.
+The timezone to use for user facing times. Any timezone name supported by the
+[pytz] package should work.
+
+Type: String <br>
+Default value: `"UTC"`
+
+---
 
 ## `CONFIG_FILES`
 
 Specifies where to look for one or more TOML configuration files. The value must
 be a semicolon-separated list of file paths.
 
 The files are loaded in the specified order. The parameters from each file get
 merged into the previously known configuration. If a given parameter was already
 set, its value is overwritten by the one from the later file.
 
-The default value is `"config.toml;instance.toml;.secrets.toml"`.
-
 Paths may be absolute or relative. Relative paths are resolved from the current
 working directory. If a specified file is not found there, it is searched by
 traversing the directories upwards. If the root directory is reached and the
 file is still not found, then the same search method is reapplied, but this time
 starting from the [`INSTANCE_PATH`](#instance_path).
 
+Type: String <br>
+Default value: `"config.toml;instance.toml;.secrets.toml"`
+
 !!! warning "Environment variable only"
 
     This parameter is specific to KerkoApp and cannot be set in a TOML file. It
     can only be set as an environment variable, therefore it should actually be
-    referenced as `KERKOAPP_CONFIG_FILES` (see [Environment variables](config-basics.md#environment-variables) for details on setting such variables).
+    referenced as `KERKOAPP_CONFIG_FILES`. See [environment variables] for
+    details.
+
+---
 
 ## `DATA_PATH`
 
 The data path specifies a directory where Kerko may store its cache, search
 index, and file attachments. This may be provided as an absolute path or as a
 relative path. If a relative path is given, it will be relative to
 [`INSTANCE_PATH`](#instance_path).
 
-The default value is `kerko`.
-
 It is typically unnecessary to set both `DATA_PATH` and `INSTANCE_PATH`.
 
+Type: String <br>
+Default value: `"kerko"`
+
+---
+
 ## `INSTANCE_PATH`
 
 The instance path specifies a directory where the application may store data and
 configuration files.
 
-The default value is [determined by Flask][Flask_instance_folder]. In practice,
-the default for KerkoApp users is a directory named `instance` located at the
-same level as the `wsgi.py` file. You may set `INSTANCE_PATH` to a different
-directory, which you must provide as an **absolute path**.
-
 It is unnecessary to set `INSTANCE_PATH` if you are already setting
 [`DATA_PATH`](#data_path) as an absolute path.
 
+Type: String <br>
+Default value: [Determined by Flask][Flask instance folder]. In practice, the
+default for KerkoApp users is a directory named `instance` located at the same
+level as the `wsgi.py` file. You may set `INSTANCE_PATH` to a different
+directory, which you must provide as an **absolute path**.
+
 !!! warning "Environment variable only"
 
     This parameter is specific to KerkoApp and cannot be set in a TOML file. It
     can only be set as an environment variable, therefore it should actually be
-    referenced as `KERKOAPP_INSTANCE_PATH` (see [Environment variables](config-basics.md#environment-variables) for details on setting such variables).
+    referenced as `KERKOAPP_INSTANCE_PATH`. See [environment variables] for
+    details.
+
+---
 
 ## `LOGGING_ADDRESS`
 
+---
+
 ## `LOGGING_FORMAT`
 
+---
+
 ## `LOGGING_HANDLER`
 
+---
+
 ## `LOGGING_LEVEL`
 
 Severity of events to log. Allowed values are `"DEBUG"`, `"INFO"`, `"WARNING"`,
 `"ERROR"`, and `"CRITICAL"`.
 
-Defaults to `"DEBUG"` if the application is running in debug mode, and to
+Type: String <br>
+Default value: `"DEBUG"` if the application is running in debug mode, or
 `"WARNING"` otherwise.
 
+---
+
 ## `SECRET_KEY`
 
 This parameter is required for generating secure tokens in web forms. It should
 have a hard to guess value, and should really remain secret.
 
 This parameter is **required** and has no default value.
 
+Type: String
+
+---
+
 ## `ZOTERO_API_KEY`
 
 Your Zotero API key, as [created on
 zotero.org](https://www.zotero.org/settings/keys/new). We recommend that you
 create a read-only API key, as Kerko does not need to write to your library.
 
 This parameter is **required** and has no default value.
 
+Type: String
+
+---
+
 ## `ZOTERO_LIBRARY_ID`
 
 The identifier of the Zotero library to get data from. For a personal library
 the value is your _userID_, as found on https://www.zotero.org/settings/keys
 (you must be logged-in). For a group library this value is the _groupID_ of the
 library, as found in the URL of the library (e.g., the _groupID_ of the library
 at https://www.zotero.org/groups/2348869/kerko_demo is `"2348869"`).
 
 This parameter is **required** and has no default value.
 
+Type: String
+
+---
+
 ## `ZOTERO_LIBRARY_TYPE`
 
 The type of library to get data from, either `"user"` for a personal library, or
 `"group"` for a group library.
 
 This parameter is **required** and has no default value.
 
-## `kerko.citation_formats.*`
+Type: String
+
+---
+
+## `kerko.bib_formats.*.`
 
-Record download formats. Default formats are: `bibtex`, `ris`.
+Bibliographic record download formats, where `*` is a format key.
+
+The default formats are:
+
+- `bibtex`
+- `ris`
 
 The configuration system does not allow adding new formats.
 
 ### `enabled`
 
-Enable the format.
+Enable the format. If this is set to `false`, the format will not be available
+through any download link.
+
+Type: Boolean
+
+!!! warning "Modifies the cache and the search index"
+
+    Changing this parameter from `false` to `true` will require that you run the
+    `sync cache --full` and `sync index` commands. See [synchronization
+    commands] for details.
 
 ### `extension`
 
 File extension of the downloadable file.
 
+Type: String
+
 ### `help_text`
 
 Description of the format, to show in the help window.
 
+Type: String
+
 ### `label`
 
 Label to use in the format selector.
 
+Type: String
+
 ### `mime_type`
 
 MIME type of the downloadable format.
 
+Type: String
+
 ### `weight`
 
 Relative position of the format in lists. Formats with low weights (small
 numbers) rise above heavier ones (large numbers).
 
-## `kerko.facets.*`
+Type: Integer
+
+---
+
+## `kerko.facets.*.`
+
+Facets to provide in the search interface, where `*` is a facet key. The facet
+key is used internally by Kerko to identify the facet.
 
-Facets to provide in the search interface. Default facets are: `tag`,
-`item_type`, `year`, `link`.
+The default facets are:
+
+- `item_type`
+- `link`
+- `tag`
+- `year`
 
 You may define additional facets.
 
+!!! warning "Modifies the search index"
+
+    Changing any of the `kerko.facets.*` parameters will require that you run
+    the `clean index` and `sync index` commands. See [synchronization commands]
+    for details.
+
 ### `collection_key`
 
 Key of the Zotero collection to map the facet to. This must refer to a
 **top-level collection** containing **at least one hierarchical level of
 subcollections**. Each subcollection will be mapped to a filter under the facet,
-if it contains at least one item.
+if it contains at least one item that is not excluded through the
+[`kerko.zotero.item_include_re`](#item_include_re) or
+[`kerko.zotero.item_exclude_re`](#item_exclude_re) parameters.
 
-This parameter is only allowed when the facet's `type` is `"collection"`.
+The `collection_key` parameter is only allowed when the [`type`](#type)
+parameter is set to `"collection"`.
+
+Type: String
 
 ### `enabled`
 
 Enable the facet.
 
+Type: Boolean
+
 ### `filter_key`
 
 Key to use in URLs when filtering with the facet.
 
+Type: String
+
 ### `initial_limit`
 
 Maximum number of filters to show by default under the facet. Excess filters
 will be shown if the user clicks a "view more" button. A value of `0` means no
 limit.
 
+Type: Integer
+
 ### `initial_limit_leeway`
 
 If the number of filters under the facet exceeds `initial_limit` by this
 tolerance margin or less, all filters will be shown. A value of `0` means no
 tolerance margin.
 
+Type: Integer
+
 ### `item_view`
 
 Show the facet on item view pages.
 
+Type: Boolean
+
 ### `sort_by`
 
 List of criteria used for sorting the filters under the facet. Allowed values in
 this list are `"count"` and `"label"`.
 
+Type: Array of strings
+
 ### `sort_reverse`
 
 Reverse the sort order of the filters under the facet.
 
+Type: Boolean
+
 ### `title`
 
 Heading of the facet.
 
+Type: String
+
 ### `type`
 
 Type of facet. Determines the data source of the facet.
 
 Allowed values are:
 
 - `"collection"`: Use a Zotero collection as source.
 - `"item_type"`: Use the item type as source.
 - `"link"`: Use item URL field as source.
 - `"tag"`: Use Zotero tags as source.
 - `"year"`: Use the item year field as source.
 
+Type: String
+
 ### `weight`
 
 Relative position of the facet in lists. Facets with low weights (small numbers)
 rise above heavier ones (large numbers).
 
-## `kerko.features`
+Type: Integer
+
+---
+
+## `kerko.features.`
 
 ### `download_attachment_new_window`
 
 Open attachments in new windows. In other words: add the HTML `target="_blank"`
-attribute to attachment links. Defaults to `false`.
+attribute to attachment links.
 
-### `download_citations_link`
+Type: Boolean <br>
+Default value: `false`
 
-Provide a record download button on search results pages. Defaults to `true`.
+### `download_results_link`
 
-### `download_citations_max_count`
+Provide a record download button on search results pages.
+
+Type: Boolean <br>
+Default value: `true`
+
+### `download_results_max_count`
 
 Limit over which the record download button should be hidden from search results
-pages. Defaults to `0` (i.e. no limit).
+pages.
+
+Type: Integer <br>
+Default value: `0` (i.e., no limit)
 
 ### `open_in_zotero_app`
 
 On item pages, show a button for opening the corresponding item in the Zotero
 application (through a link using the `zotero://` protocol). If this parameter
 is set to `true`, a user will still need to first enable the button from the
 Preferences menu (which can be accessed from the footer of item pages and saves
 the user's choices in browser cookies). For the link to work, the user must also
 have the Zotero application installed, and have access to the Zotero library.
 This feature is generally only useful to library editors and might confuse other
 users, especially if your Zotero library is private. Thus you should probably
-enable this option only if there is a strong need from the editors. Defaults to
-`false`.
+enable this option only if there is a strong need from the editors.
+
+Type: Boolean <br>
+Default value: `false`
 
 ### `open_in_zotero_web`
 
 On item pages, show a button for viewing the corresponding item on zotero.org
 (through a regular hyperlink). If this parameter is set to `true`, a user will
 still need to first enable the button from the Preferences menu (which can be
 accessed from the footer of item pages and saves the user's choices in browser
 cookies). For the link to work, the user must also have access to the Zotero
 library. This feature is generally only useful to library editors and might
 confuse other users, especially if your Zotero library is private. Thus you
 should probably enable this option only if there is a strong need from the
-editors. Defaults to `false`.
+editors.
+
+Type: Boolean <br>
+Default value: `false`
 
 ### `print_item_link`
 
-Provide a print button on item pages. Defaults to `false`.
+Provide a print button on item pages.
+
+Type: Boolean <br>
+Default value: `false`
 
-### `print_citations_link`
+### `print_results_link`
 
-Provide a print button on search results pages. Defaults to `false`.
+Provide a print button on search results pages.
 
-### `print_citations_max_count`
+Type: Boolean <br>
+Default value: `false`
+
+### `print_results_max_count`
 
 Limit over which the print button should be hidden from search results pages.
-Defaults to `0` (i.e. no limit).
+
+Type: Integer <br>
+Default value: `0` (i.e., no limit)
 
 ### `relations_initial_limit`
 
-Number of related items to show above the "show more" link. Defaults to `5`.
+Number of related items to show above the "show more" link.
+
+Type: Integer <br>
+Default value: `5`
 
 ### `relations_links`
 
-Show item links in lists of related items. Defaults to `false`. Enabling this
-only has an effect if at least one of the following variables is also set to
-`true`: `kerko.features.results_attachment_links`,
+Show item links in lists of related items.
+
+Enabling this only has an effect if at least one of the following variables is
+also set to `true`: `kerko.features.results_attachment_links`,
 `kerko.features.results_url_links`.
 
+Type: Boolean <br>
+Default value: `false`
+
 ### `results_abstracts`
 
-Show abstracts on search result pages. Defaults to `false` (abstracts are
-hidden).
+Show abstracts on search result pages.
+
+Type: Boolean <br>
+Default value: `false` (i.e., hide abstracts)
 
 ### `results_abstracts_toggler`
 
 Show a button letting users show or hide abstracts on search results pages.
-Defaults to `true` (toggle is displayed).
+
+Type: Boolean <br>
+Defaults value: `true` (i.e., toggle is displayed)
 
 ### `results_abstracts_max_length`
 
 Truncate abstracts at the given length (in number of characters). If text is to
 be truncated in the middle of a word, the whole word is discarded instead.
-Truncated text is appended with an ellipsis sign ("..."). Defaults to `0`
-(abstracts get displayed in their full length, without any truncation).
+Truncated text is appended with an ellipsis sign ("...").
+
+Type: Integer <br>
+Default value: `0` (i.e., abstracts get displayed in their full length, without
+any truncation)
 
 ### `results_abstracts_max_length_leeway`
 
 If the length of an abstract only exceeds
 `kerko.features.results_abstracts_max_length` by this tolerance margin or less
-(in number of characters), it will not be truncated. Defaults to `0` (no
-tolerance margin). No effect if `results_abstracts_max_length` is set to 0 (no
+(in number of characters), it will not be truncated.
+
+This parameter has no effect if `results_abstracts_max_length` is set to `0` (no
 truncation).
 
+Type: Integer <br>
+Default value: `0` (i.e., no tolerance margin).
+
 ### `results_attachment_links`
 
-Provide links to attachments in search results. Defaults to `true`.
+Provide links to attachments in search results.
+
+Type: Boolean <br>
+Default value: `true`
 
 ### `results_url_links`
 
 Provide links to online resources in search results (for items whose URL field
-has a value). Defaults to `true`.
+has a value).
+
+Type: Boolean <br>
+Default value: `true`
 
-## `kerko.feeds`
+---
+
+## `kerko.feeds.`
 
 ### `formats`
 
-A list of syndication feed formats to publish. Defaults to `['atom']`. If set to
-an empty list, no web feed will be provided. The only supported format is
-`'atom'`.
+A list of syndication feed formats to publish.
+
+If set to an empty array, no web feed will be provided. The only supported
+format at this time is `'atom'`.
+
+Type: Array of strings <br>
+Default value: `["atom"]`
 
 ### `fields`
 
 List of fields to retrieve for each feed item (these may be used by the
 `kerko.templates.atom_feed` template). Values in this list are keys identifying
 fields defined in the `kerko_composer` object. One probably only needs to change
 the default list when overriding the template to display additional fields. Note
 that some fields from the default list may be required by Kerko, and removing
 those could cause crashes.
 
+Type: Dictionary
+
 ### `max_days`
 
 The age (in number of days) of the oldest items allowed into web feeds. The date
 field of the items is used for that purpose, and when no date is available, the
-date the item was added to Zotero is used instead. Defaults to `0` (no age
-limit). Unless your goal is to promote recent literature only, you should
-probably keep the default value. Note: Items with missing dates will be
-considered as very recent, to prevent them from being excluded from feeds. For
-the same reason, items whose date lack the month and/or the day will be
-considered as from the 12th month of the year and/or the last day of the month.
+date the item was added to Zotero is used instead.
+
+Unless your goal is to promote recent literature only, you should probably keep
+the default value.
+
+Items with missing dates will be considered as very recent, to prevent them from
+being excluded from feeds. For the same reason, items whose date lack the month
+and/or the day will be considered as from the 12th month of the year and/or the
+last day of the month.
 
-## `kerko.meta`
+Type: Integer <br>
+Default value: `0` (i.e., no age limit)
+
+---
+
+## `kerko.meta.`
 
 ### `google_analytics_id`
 
-A Google Analytics stream ID, e.g., `'G-??????????'`. This variable is optional
-and is empty by default. If set and Flask is not running in debug mode, then the
+A Google Analytics stream ID, e.g., `'G-??????????'`.
+
+If the value is not empty *and* Flask is not running in debug mode, then the
 Google Analytics tag is inserted into the pages.
 
+Type: String <br>
+Default value: `""`
+
 ### `highwirepress_tags`
 
 Embed [Highwire Press
 tags](https://scholar.google.ca/intl/en/scholar/inclusion.html#indexing) into
 the HTML of item pages. This should help search engines such as Google Scholar
 index your items more accurately, but works only with book, conference paper,
-journal article, report or thesis items. Defaults to `true` (i.e. enabled).
+journal article, report or thesis items.
+
+Type: Boolean <br>
+Default value: `true` (i.e., enabled).
 
 ### `title`
 
 The title to display in web pages.
 
-## `kerko.pagination`
+Type: String
+
+---
+
+## `kerko.pagination.`
 
 ### `page_len`
 
-The number of search results per page. Defaults to `20`.
+The number of search results per page.
+
+Type: Integer <br>
+Default value: `20`
 
 ### `pager_links`
 
-Number of pages to show in the pager (not counting the current page). Defaults
-to `4`.
+Number of pages to show in the pager (not counting the current page).
+
+Type: Integer <br>
+Default value: `4`
 
-## `kerko.scopes.*`
+---
 
-List of keyword search scopes. Scopes allow users to restrict the search to some
-fields.
+## `kerko.scopes.*.`
 
-Default scopes are:
+Keyword search scopes, where `*` is a scope key. The scope key is used
+internally by Kerko to identify the scope. Scopes allow users to restrict the
+search to some fields.
+
+The default scopes are:
 
 - `all`
 - `creator`
 - `fulltext`
 - `metadata`
 - `title`
 
 You may define additional scopes. To link fields to scopes, see
 [`kerko.search_fields.scopes`](#scopes).
 
-!!! note
-
-    Note that if `kerko.search.fulltext` is `false`, the `'metadata'` and
-    `'fulltext'` scopes are automatically disabled. **TODO:docs: Statement to verify. Not sure this still true.**
-
-!!! warning
-
-    Most fields are referring to the default scopes. If required scopes are disabled, the application may not start. **TODO:docs: Behavior to verify**
-
-!!! warning
-
-    At least one scope must remain enabled for the application to start. **TODO:docs: Behavior to verify**
-
 ### `breadbox_label`
 
 Label to use when the scope appears in the breadbox, i.e. in the list of search
 criteria.
 
 ### `enabled`
 
 Enable the scope.
 
+Type: Boolean
+
 ### `help_text`
 
 Description of the scope, to show in the help window.
 
+Type: String
+
 ### `selector_label`
 
 Label to use in the scope selector.
 
+Type: String
+
 ### `weight`
 
 Relative position of the scope in lists. Scopes with low weights (small numbers)
 rise above heavier ones (large numbers).
 
-## `kerko.search`
+Type: Integer
+
+---
+
+## `kerko.search.`
 
 ### `fulltext`
 
-Allow full-text search of PDF attachments. Defaults to `true`. To get consistent
-results, see [Ensuring full-text indexing of your attachments in
-Zotero](recipes.md#ensuring-full-text-indexing-of-your-attachments-in-zotero).
+Allow full-text search of PDF attachments.
+
+Type: Boolean <br>
+Default value: `true`
+
+!!! Tip
+
+    To get consistent results with full-text search, see [Ensuring full-text
+    indexing of your attachments in Zotero].
+
+!!! Tip
+
+    When setting `kerko.search.fulltext` to `false`, it is recommended that you
+    set `kerko.scopes.fulltext.enabled` and `kerko.scopes.metadata.enabled` to
+    `false` as well. With full-text data unavailable, the `fulltext` scope is
+    useless, and the `metadata` scope gives the same results as the `all` scope.
+
+!!! warning "Modifies the cache and the search index"
+
+    Changing this parameter will require that you run the `sync cache --full`
+    and `sync index` commands. See [synchronization commands] for details.
 
 ### `result_fields`
 
 List of item fields to retrieve for search results (most notably used by the
-`kerko.templates.search_item` template). Values in this list are keys
-identifying fields defined in the `kerko.composer.Composer` instance. One
-probably only needs to change the default list when overriding the template to
-display additional fields. Note that some fields from the default list may be
-required by Kerko, and removing those could cause crashes.
+`kerko.templates.search_item` template).
+
+Values in this list are keys identifying fields defined in the
+`kerko.composer.Composer` instance. One probably only needs to change the
+default list when overriding the template to display additional fields.
+
+Note that some fields from the default list may be required by Kerko, and
+removing those could cause crashes.
+
+Type: Array of strings <br>
+Default value: `["id", "attachments", "bib", "coins", "data", "url"]`
 
 ### `whoosh_language`
 
-The language of search requests. Defaults to `'en'`.
+The language of search requests.
 
 As of this writing, Whoosh supports the following languages: ar, da, nl, en, fi,
 fr, de, hu, it, no, pt, ro, ru, es, sv, tr. You may refer to Whoosh's source
 code to get the list of supported languages (see `whoosh.lang.languages`) and
 the list of languages that support stemming (see `whoosh.lang.has_stemmer()`).
 
-## `kerko.search_fields.*`
+Type: String <br>
+Default value: `"en"`
+
+!!! warning "Modifies the search index"
+
+    Changing this parameter will require that you run the `sync index --full`
+    command. See [synchronization commands] for details.
 
-Searchable fields. The default fields fall into different tables:
+---
+
+## `kerko.search_fields.*.`
+
+Searchable fields, where `*` is a field key. The default fields fall into
+different tables:
 
 - `core.optional.*`: These fields have limited parameters. Their only allowed
   parameters are `boost`, `enabled`, and `scopes`.
 - `core.required.*`: These fields cannot be disabled. Their only allowed
   parameters are `boost` and `scopes`.
 - `zotero.*`: These fields derive directly from Zotero item fields and allow all
   field parameters.
 
 The configuration system does not allow adding new fields.
 
+!!! warning "Modifies the search index"
+
+    Changing any of the `kerko.search_fields.*` parameters will require that you
+    run the `clean index` and `sync index` commands, except if you are just
+    disabling a field or changing its `scopes` parameter. See [synchronization
+    commands] for details.
+
 ### `analyzer`
 
 Type of analysis to apply to the field value when building the search index.
 
-Allowed values are:
+Allowed values:
 
 - `"id"`: Index the entire value of the field as one token.
 - `"name"`: Apply standard tokenization and filtering, but without stemming.
 - `"text"`: Apply standard tokenization, stemming and filtering.
 
+Type: String
+
 ### `boost`
 
 Scaling factor to apply to score when matches are found in the field.
 
+Type: Float
+
 ### `enabled`
 
 Enable the field.
 
+Type: Boolean
+
 ### `scopes`
 
 List of keyword search scopes that will exploit the field.
 
 Allowed values are determined by [`kerko.scopes`](#kerkoscopes).
 
-## `kerko.sorts.*`
+Type: Array of strings
+
+---
 
-List of search results sorting options. Default sorts are:
+## `kerko.sorts.*.`
+
+Search results sorting options, where `*` is a sort option key.
+
+The default sort options are:
 
 - `author_asc`
 - `author_desc`
 - `date_asc`
 - `date_desc`
 - `score`
 - `title_asc`
 - `title_desc`
 
-The configuration system does not allow adding new sorts.
-
-!!! warning
-
-    At least one sort must remain enabled for the application to start. **TODO:docs: Behavior to verify**
+The configuration system does not allow adding new sort options.
 
 ### `enabled`
 
 Enable the sort option.
 
+Type: Boolean
+
 ### `label`
 
 Label of the sort option.
 
+Type: String
+
 ### `weight`
 
 Relative position of the sort option in lists. Sort options with low weights
 (small numbers) rise above heavier ones (large numbers).
 
-## `kerko.templates`
+The default sort option will be the one with the lowest weight.
+
+Type: Integer
+
+!!! tip
+
+    It is recommended that `kerko.sorts.score.weight` has the smallest value of
+    all your sort options. Thus, when a keyword search is performed, sorting by
+    relevance score will be the default, and when no keywords are used in the
+    search, then the sort option with the second smallest weight will be the
+    default one.
+
+---
+
+## `kerko.templates.`
 
 ### `search`
 
 Name of the Jinja2 template to render for the search page with list of results.
-Defaults to `kerko/search.html.jinja2`.
+
+Type: String <br>
+Default value: `"kerko/search.html.jinja2"`
 
 ### `search_item`
 
 Name of the Jinja2 template to render for the search page with a single
-bibliographic record. Defaults to `kerko/search-item.html.jinja2`.
+bibliographic record.
+
+Type: String <br>
+Default value: `"kerko/search-item.html.jinja2"`
 
 ### `item`
 
 Name of the Jinja2 template to render for the bibliographic record view.
-Defaults to `kerko/item.html.jinja2`.
+
+Type: String <br>
+Default value: `"kerko/item.html.jinja2"`
 
 ### `atom_feed`
 
-Name of the Jinja2 template used to render an Atom feed. Defaults to
-`kerko/atom.xml.jinja2`.
+Name of the Jinja2 template used to render an Atom feed.
+
+Type: String <br>
+Default value: `"kerko/atom.xml.jinja2"`
 
 ### `layout`
 
 Name of the Jinja2 template that is extended by the search, search-item, and
-item templates. Defaults to `kerko/layout.html.jinja2`.
+item templates.
+
+Type: String <br>
+Default value: `"kerko/layout.html.jinja2"`
 
 ### `base`
 
-Name of the Jinja2 template that is extended by the layout template. Defaults to
-`kerko/base.html.jinja2`.
+Name of the Jinja2 template that is extended by the layout template.
+
+Type: String <br>
+Default value: `"kerko/base.html.jinja2"`
 
-## `kerko.zotero`
+---
+
+## `kerko.zotero.`
 
 ### `attachment_mime_types`
 
 List of allowed MIME types for attachments.
 
+Type: Array of strings <br>
+Default value: `["application/pdf"]`
+
+!!! warning "Modifies the attachments"
+
+    Changing this parameter will require that you run the `sync attachments`
+    command. See [synchronization commands] for details.
+
 ### `csl_style`
 
-The citation style to use for formatted references. Can be either the file name
-(without the `.csl` extension) of one of the styles in the [Zotero Styles
-Repository][Zotero_styles] (e.g., `apa`) or the URL of a remote CSL file.
-Defaults to `'apa'`.
+The citation style to use for formatted references.
+
+Allowed values are either a file name (without the `.csl` extension) found in
+the [Zotero Styles Repository] (e.g., `"apa"`) or the publicly accessible URL of
+a remote CSL file.
+
+Type: String <br>
+Default value: `"apa"`.
+
+!!! warning "Modifies the cache and the search index"
+
+    Changing this parameter will require that you run the `sync cache --full`
+    and `sync index` commands. See [synchronization commands] for details.
 
 ### `batch_size`
 
-Number of items to request on each call to the Zotero API. Defaults to `100`
-(which is the maximum currently allowed by the API).
+Number of items to request on each call to the Zotero API.
+
+Type: Integer <br>
+Default value: `100` (this is the maximum currently allowed by the Zotero API)
 
 ### `child_include_re`
 
 Regular expression to use to include children (e.g. notes, attachments) based on
 their tags. Any child which does not have a tag that matches this regular
 expression will be ignored. If this value is empty (which is the default), all
 children will be accepted unless `kerko.zotero.child_exclude_re` is set and
 causes some to be rejected.
 
+Type: String <br>
+Default value: `""`
+
+!!! warning "Modifies the search index and attachments"
+
+    Changing this parameter will require that you run the `sync index --full`
+    and `sync attachments` commands. See [synchronization commands] for details.
+
 ### `child_exclude_re`
 
 Regular expression to use to exclude children (e.g. notes, attachments) based on
 their tags. Any child that have a tag that matches this regular expression will
 be ignored. If empty, no children will be rejected unless
 `kerko.zotero.child_include_re` is set and the tags of those children do not
 match it. By default, any child having at least one tag that begins with an
 underscore character (`_`) is rejected.
 
+Type: String <br>
+Default value: `"^_"`
+
+!!! warning "Modifies the search index and attachments"
+
+    Changing this parameter will require that you run the `sync index --full`
+    and `sync attachments` commands. See [synchronization commands] for details.
+
 ### `item_include_re`
 
 Regular expression to use to include items based on their tags. Any item which
 does not have a tag that matches this regular expression will be ignored. If
 this value is empty (which is the default), all items will be accepted unless
 `kerko.zotero.item_exclude_re` is set which can cause some items to be rejected.
 
+Type: String <br>
+Default value: `""`
+
+!!! warning "Modifies the search index and attachments"
+
+    Changing this parameter will require that you run the `sync index --full`
+    and `sync attachments` commands. See [synchronization commands] for details.
+
 ### `item_exclude_re`
 
 Regular expression to use to exclude items based on their tags. Any item that
 have a tag that matches this regular expression will be excluded. If empty
 (which is the default), no items will be excluded unless
 `kerko.zotero.item_include_re` is set, in which case items that do not have any
 tag that matches it will be excluded.
 
+Type: String <br>
+Default value: `""`
+
+!!! warning "Modifies the search index and attachments"
+
+    Changing this parameter will require that you run the `sync index --full`
+    and `sync attachments` commands. See [synchronization commands] for details.
+
 ### `locale`
 
 The locale to use with Zotero API calls. This dictates the locale of Zotero item
-types, field names, creator types and citations. Defaults to `'en-US'`.
+types, field names, creator types and citations.
 Supported locales are listed at https://api.zotero.org/schema, under "locales".
 
+Type: String <br>
+Default value: `"en-US"`
+
+!!! warning "Modifies the cache and the search index"
+
+    Changing this parameter will require that you run the `sync cache --full`
+    and `sync index` commands. See [synchronization commands] for details.
+
 ### `max_attempts`
 
 Maximum number of tries after the Zotero API has returned an error or has not
-responded during indexing. Defaults to `10`.
+responded during indexing.
+
+Type: Integer <br>
+Default value: `10`
 
 ### `tag_include_re`
 
 Regular expression to use to include tags. By default, all tags are accepted.
+
 Note that record exports (downloads) always include all tags regardless of this
 parameter, which only applies to information displayed by Kerko (exports are
 generated by the Zotero API, not by Kerko).
 
+Type: String <br>
+Default value: `""`
+
+!!! warning "Modifies the search index"
+
+    Changing this parameter will require that you run the `sync index --full`
+    command. See [synchronization commands] for details.
+
 ### `tag_exclude_re`
 
 Regular expression to use to exclude tags. The default value causes any tag that
-begins with an underscore character (`_`) to be ignored by Kerko. Note that
-record exports (downloads) always include all tags regardless of this parameter,
-which only applies to information displayed by Kerko (exports are generated by
-the Zotero API, not by Kerko).
+begins with an underscore character (`_`) to be ignored by Kerko.
+
+Note that record exports (downloads) always include all tags regardless of this
+parameter, which only applies to information displayed by Kerko (exports are
+generated by the Zotero API, not by Kerko).
+
+Type: String <br>
+Default value: `"^_"`
+
+!!! warning "Modifies the search index"
+
+    Changing this parameter will require that you run the `sync index --full`
+    command. See [synchronization commands] for details.
 
 ### `wait`
 
 Time to wait (in seconds) between failed attempts to call the Zotero API.
-Defaults to `120`.
 
-## `kerkoapp.proxy_fix`
+Type: Integer <br>
+Default value: `120`
+
+---
+
+## `kerkoapp.proxy_fix.`
 
 When an application is running behind a proxy server, WSGI may see the request
 as coming from that server rather than the real client. Proxies set various
 headers to track where the request actually came from.
 
 In that case you must tell the application how many proxies set each header so
 it knows what values to trust. However, enable this ONLY if the application is
 actually running behind a proxy; it would be a security issue to trust values
 that came directly from the client rather than a proxy.
 
-Refer to [Tell Flask it is behind a proxy][Flask_proxy] for details.
+Refer to [Tell Flask it is behind a proxy][Flask proxy] for details.
+
+!!! warning
+
+    This parameter is specific to KerkoApp.
 
 ### `enabled`
 
-Enable the proxy parameters. Defaults to `false`. All other `kerkoapp.proxy_fix`
-parameters are ignored unless this is set to `true`.
+Enable the proxy parameters.
+
+All other `kerkoapp.proxy_fix` parameters are ignored unless this is set to
+`true`.
+
+Type: Boolean <br>
+Default value: `false`
 
 ### `x_for`
 
-Number of values to trust for `X-Forwarded-For`. Defaults to `1`.
+Number of values to trust for `X-Forwarded-For`.
+
+Type: Integer <br>
+Default value: `1`
 
 ### `x_proto`
 
-Number of values to trust for `X-Forwarded-Proto`. Defaults to `1`.
+Number of values to trust for `X-Forwarded-Proto`.
+
+Type: Integer <br>
+Default value: `1`
 
 ### `x_host`
 
-Number of values to trust for `X-Forwarded-Host`. Defaults to `0`.
+Number of values to trust for `X-Forwarded-Host`.
+
+Type: Integer <br>
+Default value: `0`
 
 ### `x_port`
 
-Number of values to trust for `X-Forwarded-Port`. Defaults to `0`.
+Number of values to trust for `X-Forwarded-Port`.
+
+Type: Integer <br>
+Default value: `0`
 
 ### `x_prefix`
 
-Number of values to trust for `X-Forwarded-Prefix`. Defaults to `0`.
+Number of values to trust for `X-Forwarded-Prefix`.
+
+Type: Integer <br>
+Default value: `0`
 
 
-[Flask_instance_folder]: https://flask.palletsprojects.com/en/2.3.x/config/#instance-folders
-[Flask_proxy]: https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/
-[Flask-Babel_documentation]: https://python-babel.github.io/flask-babel/
+[environment variables]: config-basics.md#environment-variables
+[Ensuring full-text indexing of your attachments in Zotero]: recipes.md#ensuring-full-text-indexing-of-your-attachments-in-zotero
+[Flask instance folder]: https://flask.palletsprojects.com/en/2.3.x/config/#instance-folders
+[Flask proxy]: https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/
+[KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [pytz]: https://pypi.org/project/pytz/
-[Zotero_styles]: https://www.zotero.org/styles/
+[synchronization commands]: synchronization.md#command-line-interface-cli
+[Zotero Styles Repository]: https://www.zotero.org/styles/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Kerko-1.0.0a0/docs/contributing.md` & `Kerko-1.0.0a1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/docs/deployment.md` & `Kerko-1.0.0a1/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/docs/getting-started.md` & `Kerko-1.0.0a1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/docs/index.md` & `Kerko-1.0.0a1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 !!! warning
 
-    **This documentation is for the development (upcoming) version of Kerko.**
-    This new version brings significant changes to installation and configuration
-    procedures.<br>
-    **If you are looking for information on Kerko 0.9 (the latest released
-    version), see the [Kerko 0.9
-    documentation](https://github.com/whiskyechobravo/kerko/blob/0.9/README.md).**
+    **This documentation is for Kerko version 1.0.x (currently alpha).** This
+    new version brings significant changes to installation and configuration
+    procedures.<br> **If you are looking for information on Kerko 0.9, see the
+    [Kerko 0.9 documentation](https://github.com/whiskyechobravo/kerko/blob/0.9/README.md).**
 
 # Introduction
 
 [Kerko] is a web application component that provides a user-friendly search and
 browsing interface for sharing a bibliography managed with the [Zotero]
 reference manager.
 
@@ -200,23 +198,24 @@
   through notes (see [
   guide](recipes.md#providing-cites-and-cited-by-relations)). Custom
   applications can add more types of relations if desired.
 - **Badges**: custom applications can have icons conditionally displayed next to
   items.
 - **Responsive design**: the simple default implementation works on large
   monitors as well as on small screens. It is based on [Bootstrap].
+- **Google Analytics integration**: just provide a Google Analytics stream ID to
+  have Kerko automatically include the tracking code into its pages.
 - **Integration**: as a Flask [blueprint][Flask_blueprint], Kerko can be
   integrated into any Flask application. For a standalone application, however,
   you may simply [install
   KerkoApp](getting-started.md#getting-started-with-kerkoapp).
 - **Customizable front-end**: applications may partly or fully replace the
   default templates, scripts and stylesheets with their own.
 - **Command line interface (CLI)**: Kerko provides commands for synchronizing or
-  deleting its data. These can be invoked through the `flask` command (see
-  [useful commands](synchronization.md#useful-commands)).
+  deleting its data.
 
 [KerkoApp] is a standalone application built around Kerko. It inherits all of
 Kerko's features and it provides a few additions of its own:
 
 - **Configuration files**: allow separation of configuration from code and
   enable the [Twelve-factor App][Twelve-factor_App] methodology. Environment
   variables and [TOML] configuration files are supported. Secrets,
@@ -293,15 +292,15 @@
 [Flask-WTF]: https://pypi.org/project/Flask-WTF/
 [FontAwesome]: https://fontawesome.com/icons
 [HighwirePress_Google]: https://scholar.google.ca/intl/en/scholar/inclusion.html#indexing
 [Jinja2]: https://pypi.org/project/Jinja2/
 [jQuery]: https://jquery.com/
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [Kerko_email]: mailto:kerko@whiskyechobravo.com
-[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/src/kerko/translations
+[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/main/src/kerko/translations
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
 [Popper.js]: https://popper.js.org/
 [Pydantic]: https://pypi.org/project/pydantic/
 [Python]: https://www.python.org/
 [Pyzotero]: https://pypi.org/project/Pyzotero/
 [Snowball]: https://snowballstem.org/
```

### Comparing `Kerko-1.0.0a0/docs/localization.md` & `Kerko-1.0.0a1/docs/localization.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/docs/recipes.md` & `Kerko-1.0.0a1/docs/recipes.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,125 @@
 # Recipes
 
-## Defining custom facets based on Zotero collections
+## Defining a custom facet based on a Zotero collection
 
-**TODO:docs: Give instructions. Mention required clean index & sync index.**
+Zotero collections can be mapped to custom facets in Kerko. With this scheme, a
+collection in the Zotero library represents a facet, and its subcollections
+correspond to values (or user-selectable filters) within the facet. Figure 1
+below illustrates such mapping, taken from the [demo library] and its
+corresponding [demo site].
+
+<figure markdown>
+![Zotero collections mapped to Kerko facets](assets/images/kerko-zotero-mapping.png){ width="600" }
+<figcaption><b>Figure 1.</b> Side-by-side comparison between the structure of collections in a
+Zotero library and the resulting faceted browsing interface in Kerko.</figcaption>
+</figure>
+
+For such mapping to work, the following conditions must be met:
+
+- The collection that is to be mapped to a facet must be a **top-level
+  collection**. In other words, it must be directly under the root of your
+  Zotero library.
+- **At least one subcollection** must be present within the chosen top-level
+  collection, and that subcollection (or one of its own subcollections) must
+  contain at least one item.
 
-```toml title="Facet configuration example"
-[kerko.facets.my_facet]
+Once your Zotero library it set up to meet those conditions, you may configure
+the facets. For the example in Figure 1, the configuration looks like this:
+
+```toml
+[kerko.facets.topic]
+enabled = true
+type = "collection"
+collection_key = "KY3BNA6T"
+filter_key = "topic"
+title = "Topic"
+weight = 110
+initial_limit = 5
+initial_limit_leeway = 2
+
+[kerko.facets.field_of_study]
 enabled = true
 type = "collection"
-collection_key = "AAAAAAAA"
-filter_key = "my_facet"
-title = "My facet"
-weight = 50
-initial_limit = 10
+collection_key = "7H2Q7L6I"
+filter_key = "field-of-study"
+title = "Field of study"
+weight = 120
+initial_limit = 5
+initial_limit_leeway = 2
+
+[kerko.facets.contribution]
+enabled = true
+type = "collection"
+collection_key = "JFQRH4X2"
+filter_key = "contribution"
+title = "Contribution"
+weight = 130
+initial_limit = 5
 initial_limit_leeway = 2
-sort_by = ["count", "label"]
-sort_reverse = false
-item_view = true
 ```
 
-Please refer to [`kerko.facets`](config-params.md#kerkofacets) for details on
-each parameter.
+For details on each parameter, please refer to the [parameters
+documentation](config-params.md#kerkofacets). However, we can highlight some
+elements:
+
+- `collection_key` is the key assigned by Zotero to identify the collection. An
+  easy way to find this key is to visit your library using Zotero's web
+  interface. Click the collection, and check its URL in your browser's address
+  bar. In our example, the URL of the "Topic" collection is
+  [https://www.zotero.org/groups/2348869/kerko_demo/collections/**KY3BNA6T**](https://www.zotero.org/groups/2348869/kerko_demo/collections/KY3BNA6T),
+  hence the use of `"KY3BNA6T"` as the collection key.
+- `filter_key` tells Kerko the key to use in URLs when a user of your Kerko site
+  selects a filter within the facet. In our example, for the "Topic" facet we
+  chose to set this parameter to `"topic"` and, consequently, the search URL
+  will look like
+  [https://demo.kerko.whiskyechobravo.com/bibliography/?**topic**=Z8LT6QZG.2ZGZH2E2](https://demo.kerko.whiskyechobravo.com/bibliography/?topic=Z8LT6QZG.2ZGZH2E2).
+- `title` is the heading that Kerko will show for the facet. If desired, you may
+  choose a title that is different from the collection's name in Zotero.
+- `weight` determines the relative position of the facet. Small numbers (low
+  weights) rise above large ones (heavier weights). This explains why, in our
+  example, Kerko displays "Topic" (weighting 110) above "Field of study" (120)
+  and "Contribution" (130).
+
+Other things to know:
+
+- After adding a new facet, you must clean and re-sync the search index. Please
+  check the documentation on [synchronization](synchronization.md), but in short
+  you have to use the following commands:
+
+    ```bash
+    flask kerko clean index
+    flask kerko sync index
+    ```
+
+- Kerko allows a facet to have any number of hierarchical sublevels (nested
+  subcollections).
+- Any new subcollection will automatically appear under the facet after a sync,
+  if it (or one of its own subcollections) contains at least one item.
+  Collection structures that contain no items will not show up in Kerko.
+- An item may belong to multiple collections in Zotero. Take advantage of that
+  capability when designing your faceted classification. Ideally, facets
+  complement each other in describing different perspectives on the same
+  objects. If you are unfamiliar with faceted classification, we highly
+  recommend this paper by William Denton (2003): [How to Make a Faceted
+  Classification and Put It On the
+  Web](https://www.miskatonic.org/library/facet-web-howto.html).
+- In Zotero, an item only needs to be assigned to the hierarchical level that is
+  most relevant for it. You do not need to also add the item to the parent
+  collections. The reason is that in Kerko a given filter automatically includes
+  the items from its corresponding subcollection and all of its subcollections.
+- You do not have to expose all of your Zotero library's top-level collections
+  to Kerko. Kerko will only use those that are given in the configuration, and
+  ignore the others. Note, however, that unless you use [item
+  inclusion](config-params.md#item_include_re) or
+  [exclusion](config-params.md#item_exclude_re) parameters, items will be
+  visible in your Kerko site regardless of the collections they belong to.
+
+Phew! We think that this is simpler to setup in practice than it looks in
+writing. Hopefully you will agree.
 
 
 ## Ensuring full-text indexing of your attachments in Zotero
 
 Kerko's full-text indexing relies on text content extracted from attachments by
 Zotero. Consequently, for Kerko's full-text search to work, you must make sure
 that full-text indexing works in Zotero first; see [Zotero's documentation on
@@ -144,9 +239,11 @@
 ```
 
 A `robots.txt` file can have multiple `Sitemap` directives, thus the Kerko
 sitemap can be specified alongside any other sitemaps you might already have.
 
 
 [Kerko]: https://github.com/whiskyechobravo/kerko
+[demo library]: https://www.zotero.org/groups/2348869/kerko_demo/items
+[demo site]: https://demo.kerko.whiskyechobravo.com
 [venv]: https://docs.python.org/3.11/tutorial/venv.html
 [XML_Sitemap]: https://www.sitemaps.org/
```

### Comparing `Kerko-1.0.0a0/docs/synchronization.md` & `Kerko-1.0.0a1/docs/synchronization.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,33 +32,25 @@
 
 !!! note
 
     The synchronization process is unidirectional, where Kerko pulls data from
     Zotero. Kerko will never try to write anything to your Zotero library.
 
 
-## Useful commands
+## Command line interface (CLI)
 
 Kerko provides an integration with the [Flask command line interface][Flask_CLI].
 The `flask` command will work with your virtual environment active.
 
 Some frequently used commands are:
 
 `flask kerko --help`
 
 : Lists all commands provided by Kerko.
 
-`flask kerko clean`
-
-: Deletes all of Kerko's data: cache, search index, attachments.
-
-`flask kerko clean --help`
-
-: Shows help about the clean command.
-
 `flask kerko sync`
 
 : Synchronizes everything: the cache (from Zotero), the search index (from the
   cache), the attachments (from files in Zotero, based on list in search index).
 
     !!! tip "Tip: Making commands more verbose"
 
@@ -68,24 +60,15 @@
 
         ```bash
         flask --debug kerko sync
         ```
 
 `flask kerko sync --help`
 
-: Shows help about the sync command:
-
-`flask kerko clean cache`
-
-: Deletes the cache. A subsequent execution of `flask kerko sync` will perform a
-  full update from Zotero, but it will not re-download all file attachments.
-
-`flask kerko clean index`
-
-: Deletes just the search index.
+: Shows help specifically about the `sync` command:
 
 `flask kerko sync index`
 
 : Synchronizes just the search index (from the cache).
 
 !!! tip "Tip: Running commands from outside the application's directory"
 
@@ -94,14 +77,50 @@
     directory, you could use Flask's `--app` command line option, or to set the
     `FLASK_APP` environment variable. For example:
 
     ```bash
     flask --app=/path/to/kerkoapp/wsgi:app kerko sync
     ```
 
+`flask kerko sync cache --full`
+
+: When possible, the synchronization process performs an incremental update of
+  just the new or changed items. Here, the `--full` option forces a full
+  synchronization of the cache, even if no or just some items have been updated
+  since the last synchronization of the cache.
+
+    This can be useful after changing certain configuration parameters.
+
+`flask kerko clean everything`
+
+: Deletes all of Kerko's data: cache, search index, attachments.
+
+`flask kerko clean --help`
+
+: Shows help about the clean command.
+
+`flask kerko clean cache`
+
+: Deletes just the cache. A subsequent execution of `flask kerko sync` will
+  perform a full update from Zotero, but it will not re-download all file
+  attachments.
+
+    This does not affect the search index. Thus, if the index was built before a
+    `clean cache`, users will still be able to access the bibliography using the
+    Kerko web interface.
+
+`flask kerko clean index`
+
+: Deletes just the search index. The bibliography will become unavailable to the
+  Kerko web interface until the index gets synchronized again.
+
+    It can be necessary to use this command after changing certain configuration
+    parameters, and you will usually want to run `flask kerko sync index`
+    immediately after.
+
 
 ## Monitoring data synchronization
 
 Kerko provides a web API endpoint that you could use to monitor data
 synchronization.
 
 In the description below, `BASE_URL` should be replaced with the protocol,
```

### Comparing `Kerko-1.0.0a0/mkdocs.yml` & `Kerko-1.0.0a1/mkdocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   - config-basics.md
   - config-params.md
   - localization.md
   - deployment.md
   - recipes.md
   - troubleshooting.md
   - contributing.md
-  - background.md
+  - about.md
   - changelog.md
 
 theme:
   name: material
   features:
     - navigation.instant
     - navigation.tracking
@@ -37,33 +37,34 @@
         name: Switch to dark mode
     - scheme: slate
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   icon:
     repo: fontawesome/brands/github
-    view: material/eye
-    edit: material/lead-pencil
+    view: material/file-eye-outline
+    edit: material/file-edit-outline
 
 plugins:
   - search
 
 repo_url: https://github.com/whiskyechobravo/kerko
 repo_name: whiskyechobravo/kerko
-edit_uri: blob/master/docs/
+edit_uri: blob/main/docs/
 
 markdown_extensions:
   # See https://squidfunk.github.io/mkdocs-material/setup/extensions/
   # Python Markdown
   - abbr
   - admonition
   - attr_list
   - def_list
   - footnotes
   - md_in_html
+  - tables
   - toc:
       permalink: true
   # Python Markdown Extensions
   - pymdownx.arithmatex:
       generic: true
   - pymdownx.betterem:
       smart_enable: all
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
 site_name: Kerko nav: - Introduction: index.md - getting-started.md -
 synchronization.md - config-basics.md - config-params.md - localization.md -
-deployment.md - recipes.md - troubleshooting.md - contributing.md -
-background.md - changelog.md theme: name: material features: -
-navigation.instant - navigation.tracking - navigation.sections -
-navigation.expand - navigation.top - navigation.footer - header.autohide -
-toc.follow - search.suggest - search.highlight - content.code.copy -
-content.action.view - content.action.edit palette: - scheme: default toggle:
-icon: material/brightness-7 name: Switch to dark mode - scheme: slate toggle:
-icon: material/brightness-4 name: Switch to light mode icon: repo: fontawesome/
-brands/github view: material/eye edit: material/lead-pencil plugins: - search
-repo_url: https://github.com/whiskyechobravo/kerko repo_name: whiskyechobravo/
-kerko edit_uri: blob/master/docs/ markdown_extensions: # See https://
-squidfunk.github.io/mkdocs-material/setup/extensions/ # Python Markdown - abbr
-- admonition - attr_list - def_list - footnotes - md_in_html - toc: permalink:
-true # Python Markdown Extensions - pymdownx.arithmatex: generic: true -
-pymdownx.betterem: smart_enable: all - pymdownx.caret - pymdownx.details -
-pymdownx.emoji: emoji_index: !!python/name:materialx.emoji.twemoji
-emoji_generator: !!python/name:materialx.emoji.to_svg - pymdownx.highlight -
-pymdownx.inlinehilite - pymdownx.keys - pymdownx.mark - pymdownx.smartsymbols -
-pymdownx.snippets: check_paths: true - pymdownx.superfences - pymdownx.tabbed:
-alternate_style: true - pymdownx.tasklist: custom_checkbox: true -
-pymdownx.tilde extra: social: - icon: fontawesome/brands/github link: https://
-github.com/whiskyechobravo/kerko name: Kerko on GitHub version: provider: mike
-copyright: Copyright © Whisky_Echo_Bravo_Services_inc.Â­
+deployment.md - recipes.md - troubleshooting.md - contributing.md - about.md -
+changelog.md theme: name: material features: - navigation.instant -
+navigation.tracking - navigation.sections - navigation.expand - navigation.top
+- navigation.footer - header.autohide - toc.follow - search.suggest -
+search.highlight - content.code.copy - content.action.view -
+content.action.edit palette: - scheme: default toggle: icon: material/
+brightness-7 name: Switch to dark mode - scheme: slate toggle: icon: material/
+brightness-4 name: Switch to light mode icon: repo: fontawesome/brands/github
+view: material/file-eye-outline edit: material/file-edit-outline plugins: -
+search repo_url: https://github.com/whiskyechobravo/kerko repo_name:
+whiskyechobravo/kerko edit_uri: blob/main/docs/ markdown_extensions: # See
+https://squidfunk.github.io/mkdocs-material/setup/extensions/ # Python Markdown
+- abbr - admonition - attr_list - def_list - footnotes - md_in_html - tables -
+toc: permalink: true # Python Markdown Extensions - pymdownx.arithmatex:
+generic: true - pymdownx.betterem: smart_enable: all - pymdownx.caret -
+pymdownx.details - pymdownx.emoji: emoji_index: !!python/name:
+materialx.emoji.twemoji emoji_generator: !!python/name:materialx.emoji.to_svg -
+pymdownx.highlight - pymdownx.inlinehilite - pymdownx.keys - pymdownx.mark -
+pymdownx.smartsymbols - pymdownx.snippets: check_paths: true -
+pymdownx.superfences - pymdownx.tabbed: alternate_style: true -
+pymdownx.tasklist: custom_checkbox: true - pymdownx.tilde extra: social: -
+icon: fontawesome/brands/github link: https://github.com/whiskyechobravo/kerko
+name: Kerko on GitHub version: provider: mike copyright: Copyright © Whisky
+Echo_Bravo_Services_inc.Â­
```

### Comparing `Kerko-1.0.0a0/pyproject.toml` & `Kerko-1.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/setup.cfg` & `Kerko-1.0.0a1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = Kerko
-version = 1.0.0alpha0
+version = 1.0.0alpha1
 author = David Lesieur
 author_email = kerko@whiskyechobravo.com
 license_files = LICENSE.txt
-url = https://github.com/whiskyechobravo/kerko
+url = https://whiskyechobravo.github.io/kerko/
 project_urls = 
 	Documentation = https://whiskyechobravo.github.io/kerko/
 	Code = https://github.com/whiskyechobravo/kerko
-	Changes = https://github.com/whiskyechobravo/kerko/blob/master/CHANGELOG.md
+	Changes = https://github.com/whiskyechobravo/kerko/blob/main/CHANGELOG.md
 	Issue tracker = https://github.com/whiskyechobravo/kerko/issues
 description = A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 keywords = academia, bibliography, bibliographies, flask, search, zotero
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -53,14 +53,15 @@
 	Flask-WTF >=0.14.2
 	Jinja2 >=3.0.1
 	pydantic >=1.10.7, <2.0
 	python-dotenv >=0.21.1
 	pytz  # Babel does not require it (since 2.12.0), but will use it if present.
 	Pyzotero >=1.4.26
 	tomli >=2.0.1
+	tomli-w >=1.0.0
 	w3lib >=1.22.0
 	Werkzeug >=2.0.1
 	Whoosh >=2.7.4
 	wrapt >=1.10.0
 	WTForms >=3.0.0
 include_package_data = True
 setup_requires =
```

### Comparing `Kerko-1.0.0a0/setup.py` & `Kerko-1.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/Kerko.egg-info/PKG-INFO` & `Kerko-1.0.0a1/src/Kerko.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Kerko
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
-Home-page: https://github.com/whiskyechobravo/kerko
+Home-page: https://whiskyechobravo.github.io/kerko/
 Author: David Lesieur
 Author-email: kerko@whiskyechobravo.com
 Project-URL: Documentation, https://whiskyechobravo.github.io/kerko/
 Project-URL: Code, https://github.com/whiskyechobravo/kerko
-Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/master/CHANGELOG.md
+Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/main/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/whiskyechobravo/kerko/issues
 Keywords: academia,bibliography,bibliographies,flask,search,zotero
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -198,14 +198,16 @@
   You may define such relations using Zotero's _Related_ field. Moreover, Kerko
   adds the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
   through notes. Custom applications can add more types of relations if desired.
 - **Badges**: custom applications can have icons conditionally displayed next to
   items.
 - **Responsive design**: the simple default implementation works on large
   monitors as well as on small screens. It is based on [Bootstrap].
+- **Google Analytics integration**: just provide a Google Analytics stream ID to
+  have Kerko automatically include the tracking code into its pages.
 - **Integration**: as a Flask [blueprint][Flask_blueprint], Kerko can be
   integrated into any Flask application. For a standalone application, however,
   you may simply install [KerkoApp].
 - **Customizable front-end**: applications may partly or fully replace the
   default templates, scripts and stylesheets with their own.
 - **Command line interface (CLI)**: Kerko provides commands for synchronizing or
   deleting its data.
@@ -236,15 +238,15 @@
 [Dublin_Core]: https://en.wikipedia.org/wiki/Dublin_Core
 [Flask]: https://pypi.org/project/Flask/
 [Flask_blueprint]: https://flask.palletsprojects.com/en/latest/blueprints/
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [Kerko_actions]: https://github.com/whiskyechobravo/kerko/actions
 [Kerko_documentation]: https://whiskyechobravo.github.io/kerko/
 [Kerko_pypi]: https://pypi.org/project/Kerko/
-[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/master/src/kerko/translations
+[Kerko_translations]: https://github.com/whiskyechobravo/kerko/tree/main/src/kerko/translations
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [KerkoApp_demo]: https://demo.kerko.whiskyechobravo.com
 [Snowball]: https://snowballstem.org/
 [TOML]: https://toml.io/
 [Twelve-factor_App]: https://12factor.net/config
 [Whoosh]: https://pypi.org/project/Whoosh/
 [XML_Sitemap]: https://www.sitemaps.org/
@@ -253,24 +255,68 @@
 [Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
 [Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
 [Zotero_schema]: https://api.zotero.org/schema
 [Zotero_styles]: https://www.zotero.org/styles/
 
 # Changelog
 
-For changes that might be specific to KerkoApp, please refer to the [KerkoApp
-changelog](https://github.com/whiskyechobravo/kerkoapp/blob/master/CHANGELOG.md).
+## 1.0.0alpha1 (2023-06-29)
 
+Features:
+
+- Add the `--full` option to the `sync` command line interface (CLI) command.
+
+Bug fixes:
 
-## 1.0.0alpha0
+- Fix validation pattern too restrictive for the `kerko.facets.*.collection_key`
+  configuration parameter.
+- Fix incorrect typing for the `kerko.features.download_results_max_count` and
+  `kerko.features.print_results_max_count` configuration parameters.
+
+Other changes:
+
+- Rename the default branch of the repository from 'master' to 'main'. If you
+  have cloned the repository with Git, use the following commands to rename your
+  local branch:
+
+    ```bash
+    git branch -m master main
+    git fetch origin
+    git branch -u origin/main main
+    git remote set-head origin -a
+    ```
+
+- Make the `config` CLI command show the configuration in TOML format.
+- Make the `config` CLI command hide secrets by default. Add a `--show-secrets`
+  option.
+- Improve documentation.
+
+Backwards incompatible changes:
+
+- Prevent the `clean` CLI command from cleaning everything by default. To delete
+  everything, you now have to run `flask kerko clean everything`. This may help
+  accidental deletion of the cache or the search index, which in some instances
+  can take long to rebuild.
+- Rename the following configuration parameters:
+    - `kerko.citation_formats.*` → `kerko.bib_formats.*`.
+    - `kerko.features.download_citations_link` → `kerko.features.download_results_link`
+    - `kerko.features.download_citations_max_count` → `kerko.features.download_results_max_count`
+    - `kerko.features.print_citations_link` → `kerko.features.print_results_link`
+    - `kerko.features.print_citations_max_count` → `kerko.features.print_results_max_count`
+- Rename the following views:
+    - `item_citation_download` → `item_bib_download`
+    - `search_citation_download` → `search_bib_download`
+
+
+## 1.0.0alpha0 (2023-06-26)
 
 *Warning:* Upgrading from version 0.9 or earlier will require that you adapt
-your installation and configuration (if you are using KerkoApp, make sure to
-check its changelog), then rebuild your search index. Use the following
-commands, then restart the application:
+your installation and configuration files, then rebuild your search index. Use
+the commands below, then restart the application. If you are using KerkoApp,
+make sure to check its [changelog][KerkoApp_changelog].
 
 ```bash
 flask kerko clean index
 flask kerko sync index
 ```
 
 Features:
@@ -873,7 +919,10 @@
 ## 0.3alpha1 (2019-07-17)
 
 - Fix broken links in documentation.
 
 ## 0.3alpha0 (2019-07-16)
 
 - First PyPI release.
+
+
+[KerkoApp_changelog]: https://github.com/whiskyechobravo/kerkoapp/blob/main/CHANGELOG.md
```

### Comparing `Kerko-1.0.0a0/src/Kerko.egg-info/SOURCES.txt` & `Kerko-1.0.0a1/src/Kerko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 README.md
 babel.cfg
 mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-docs/background.md
+docs/about.md
 docs/changelog.md
 docs/config-basics.md
 docs/config-params.md
 docs/contributing.md
 docs/deployment.md
 docs/getting-started.md
 docs/index.md
 docs/localization.md
 docs/recipes.md
 docs/synchronization.md
 docs/troubleshooting.md
+docs/assets/images/kerko-zotero-mapping.png
 src/Kerko.egg-info/PKG-INFO
 src/Kerko.egg-info/SOURCES.txt
 src/Kerko.egg-info/dependency_links.txt
 src/Kerko.egg-info/entry_points.txt
 src/Kerko.egg-info/requires.txt
 src/Kerko.egg-info/top_level.txt
 src/kerko/__init__.py
```

### Comparing `Kerko-1.0.0a0/src/kerko/__init__.py` & `Kerko-1.0.0a1/src/kerko/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/cli.py` & `Kerko-1.0.0a1/src/kerko/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pprint
 from datetime import datetime
 
 import click
+import tomli_w
 import wrapt
 from flask import current_app
 from flask.cli import with_appcontext
 
+from kerko.config_helpers import is_toml_serializable
 from kerko.storage import (SchemaError, SearchIndexError, delete_storage,
                            get_doc_count)
 from kerko.sync import zotero
 from kerko.sync.attachments import delete_attachments, sync_attachments
 from kerko.sync.cache import sync_cache
 from kerko.sync.index import sync_index
 
@@ -29,49 +31,58 @@
 
 @cli.command()
 @click.argument(
     'target',
     default='everything',
     type=click.Choice(['cache', 'index', 'attachments', 'everything'], case_sensitive=False),
 )
+@click.option(
+    '--full',
+    default=False,
+    is_flag=True,
+    flag_value=True,
+    help="When possible, the synchronization process performs an incremental "
+         "update of just the new or changed items since the last "
+         "synchronization. This option forces a full update."
+)
 @with_appcontext
 @execution_time_logger
-def sync(target):
+def sync(target, full=False):
     """
     Synchronize the cache, the search index, and/or the file attachments.
 
     By default, everything is synchronized.
     """
     try:
         if target in ['everything', 'cache']:
-            sync_cache()
+            sync_cache(full)
         if target in ['everything', 'index']:
-            sync_index()
+            sync_index(full)
         if target in ['everything', 'attachments']:
-            sync_attachments()
+            sync_attachments(full)
     except SearchIndexError as e:
         current_app.logger.error(e)
         raise click.Abort
     except SchemaError as e:
         current_app.logger.error(e)
         raise click.Abort
 
 
 @cli.command()
 @click.argument(
     'target',
-    default='everything',
     type=click.Choice(['cache', 'index', 'attachments', 'everything'], case_sensitive=False),
 )
 @with_appcontext
 def clean(target):
     """
-    Delete the cache, the search index, and/or the attachments immediately.
+    Delete the specified data.
 
-    By default, everything is cleaned.
+    Use the argument to select which data to delete, either the cache, the
+    search index, the attachments, or all of those (everything).
     """
     if target in ['everything', 'cache']:
         delete_storage('cache')
     if target in ['everything', 'index']:
         delete_storage('index')
     if target in ['everything', 'attachments']:
         delete_attachments()
@@ -99,110 +110,134 @@
     its children in a single record. The count may include items that are not
     usually displayed in search results, e.g., standalone notes or attachments.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     try:
-        pprint.pprint(get_doc_count(target))
+        click.echo(get_doc_count(target))
     except SearchIndexError as e:
         current_app.logger.error(e)
         raise click.Abort
 
 
 @cli.command()
+@click.option(
+    '--show-secrets',
+    default=False,
+    is_flag=True,
+    flag_value=True,
+    help="Secrets are hidden from the output by default. This option causes them to be revealed."
+)
 @with_appcontext
-def config():
+def config(show_secrets=False):
     """
-    Show the app's full configuration.
+    Show the configuration.
+
+    Note that unset parameters and parameters that internally have 'None' values
+    will be omitted because such values cannot be represented in TOML files.
     """
-    pprint.pprint(dict(current_app.config))
+    def copy_serializable(src: dict) -> dict:
+        dst = {}
+        for k, v in sorted(src.items()):
+            if isinstance(v, dict):
+                dst_v = copy_serializable(v)
+                if dst_v is not None:
+                    dst[k] = dst_v
+            elif is_toml_serializable(v):
+                if not show_secrets and k in ['SECRET_KEY', 'ZOTERO_API_KEY']:
+                    v = "*****"
+                dst[k] = v
+        return dst
+
+    serializable_config = copy_serializable(current_app.config)
+    click.echo(tomli_w.dumps(serializable_config))
 
 
 @cli.command()
 @click.argument('item_key')
 @with_appcontext
 def zotero_item(item_key):
     """
     Retrieve an item from the library, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
-    pprint.pprint(zotero.load_item(credentials, item_key))
+    click.echo(pprint.pformat(zotero.load_item(credentials, item_key)))
 
 
 @cli.command()
 @with_appcontext
 def zotero_item_types():
     """
     List all item types, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
-    pprint.pprint(zotero.load_item_types(credentials))
+    click.echo(pprint.pformat(zotero.load_item_types(credentials)))
 
 
 @cli.command()
 @with_appcontext
 def zotero_item_fields():
     """
     List all fields, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
-    pprint.pprint(zotero.load_item_fields(credentials))
+    click.echo(pprint.pformat(zotero.load_item_fields(credentials)))
 
 
 @cli.command()
 @click.argument('item_type')
 @with_appcontext
 def zotero_item_type_fields(item_type):
     """
     List the available fields for a given item type, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
-    pprint.pprint(zotero.load_item_type_fields(credentials, item_type))
+    click.echo(pprint.pformat(zotero.load_item_type_fields(credentials, item_type)))
 
 
 @cli.command()
 @click.argument('item_type')
 @with_appcontext
 def zotero_item_type_creator_types(item_type):
     """
     List the available creator types for a given item type, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
-    pprint.pprint(zotero.load_item_type_creator_types(credentials, item_type))
+    click.echo(pprint.pformat(zotero.load_item_type_creator_types(credentials, item_type)))
 
 
 @cli.command()
 @with_appcontext
 def zotero_top_level_collections():
     """
     List top-level collections of the library, using the Zotero API.
 
     WARNING: This command is provided for development purposes only and may be
     modified or removed from the module at any time.
     """
     credentials = zotero.init_zotero()
     collections = zotero.Collections(credentials, top_level=True)
     for c in collections:
-        print(f"{c.get('key')} {c.get('data', {}).get('name', '')}")
+        click.echo(f"{c.get('key')} {c.get('data', {}).get('name', '')}")
 
 
 def _format_elapsed_time(start_time):
     elapsed_time = int(round((datetime.now() - start_time).total_seconds()))
     elapsed_min, elapsed_sec = elapsed_time // 60, elapsed_time % 60
     s = 'Execution time:'
     if elapsed_min > 0:
```

### Comparing `Kerko-1.0.0a0/src/kerko/codecs.py` & `Kerko-1.0.0a1/src/kerko/codecs.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/composer.py` & `Kerko-1.0.0a1/src/kerko/composer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from whoosh.query import Prefix, Term
 from whoosh.support.charset import accent_map
 from whoosh.util.text import rcompile
 
 from kerko import codecs, extractors, transformers
 from kerko.config_helpers import config_get
 from kerko.datetime import iso_to_datetime, iso_to_timestamp
-from kerko.specs import (BadgeSpec, CitationFormatSpec, CollectionFacetSpec,
+from kerko.specs import (BadgeSpec, BibFormatSpec, CollectionFacetSpec,
                          FacetSpec, FieldSpec, FlatFacetSpec, RelationSpec,
                          ScopeSpec, SortSpec, TreeFacetSpec)
 
 
 class Composer:
     """
     A factory for the setting up the search elements.
@@ -65,22 +65,22 @@
             LowercaseFilter()
 
         self.schema = Schema()
         self.scopes: Dict[str, ScopeSpec] = {}
         self.fields: Dict[str, FieldSpec] = {}
         self.facets: Dict[str, FacetSpec] = {}
         self.sorts: Dict[str, SortSpec] = {}
-        self.citation_formats: Dict[str, CitationFormatSpec] = {}
+        self.bib_formats: Dict[str, BibFormatSpec] = {}
         self.relations: Dict[str, RelationSpec] = {}
         self.badges: Dict[str, BadgeSpec] = {}
         self.init_scopes(config)
         self.init_fields(config)
         self.init_facets(config)
         self.init_sorts(config)
-        self.init_citation_formats(config)
+        self.init_bib_formats(config)
         self.init_relations(config)
 
     def init_scopes(self, config: Config) -> None:
         """
         Initialize a set of `ScopeSpec` instances using config settings.
         """
         # Note: Default labels are defined here rather than in config so that they are translatable.
@@ -737,40 +737,40 @@
                                 True,
                                 False,
                                 False,
                             ],
                         )
                     )
 
-    def init_citation_formats(self, config: Config) -> None:
+    def init_bib_formats(self, config: Config) -> None:
         """
-        Initialize a set of `CitationFormatSpec` instances using config settings.
+        Initialize a set of `BibFormatSpec` instances using config settings.
 
         These rely on `FieldSpec` instances, which must have been added beforehand.
         """
-        formats_dict = config_get(config, 'kerko.citation_formats')
+        formats_dict = config_get(config, 'kerko.bib_formats')
         for format_key, format_config in formats_dict.items():
             if format_config['enabled']:
                 kwargs = {
                     k: v
                     for k, v in format_config.items() if k in ['weight', 'extension', 'mime_type']
                 }
                 if format_key == 'ris':
-                    self.add_citation_format(
-                        CitationFormatSpec(
+                    self.add_bib_format(
+                        BibFormatSpec(
                             key=format_key,
                             field=self.fields['ris'],
                             label=format_config.get('label') or _("RIS"),
                             help_text=format_config.get('help_text') or _("Recommended format for most reference management software"),
                             **kwargs,
                         )
                     )
                 elif format_key == 'bibtex':
-                    self.add_citation_format(
-                        CitationFormatSpec(
+                    self.add_bib_format(
+                        BibFormatSpec(
                             key=format_key,
                             field=self.fields['bibtex'],
                             label=format_config.get('label') or _("BibTeX"),
                             help_text=format_config.get('help_text') or _("Recommended format for BibTeX-specific software"),
                             **kwargs,
                         )
                     )
@@ -846,19 +846,19 @@
 
     def add_sort(self, sort):
         self.sorts[sort.key] = sort
 
     def remove_sort(self, key):
         del self.sorts[key]
 
-    def add_citation_format(self, citation_format):
-        self.citation_formats[citation_format.key] = citation_format
+    def add_bib_format(self, bib_format):
+        self.bib_formats[bib_format.key] = bib_format
 
-    def remove_citation_format(self, key):
-        del self.citation_formats[key]
+    def remove_bib_format(self, key):
+        del self.bib_formats[key]
 
     def add_badge(self, badge):
         self.badges[badge.key] = badge
 
     def remove_badge(self, key):
         del self.badges[key]
```

### Comparing `Kerko-1.0.0a0/src/kerko/config_helpers.py` & `Kerko-1.0.0a1/src/kerko/config_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import abc
 import pathlib
+from datetime import date, datetime, time
+from decimal import Decimal
 from typing import Any, Dict, List, Optional, Type, Union
 
 from typing_extensions import Annotated, Literal
 
 try:
     import tomllib
 except ModuleNotFoundError:
@@ -54,21 +56,21 @@
 class FeaturesModel(BaseModel):
     """Model for the kerko.features config table."""
 
     class Config:
         extra = Extra.forbid
 
     download_attachment_new_window: bool
-    download_citations_link: bool
-    download_citations_max_count: bool
+    download_results_link: bool
+    download_results_max_count: NonNegativeInt
     open_in_zotero_app: bool
     open_in_zotero_web: bool
-    print_citations_link: bool
-    print_citations_max_count: bool
     print_item_link: bool
+    print_results_link: bool
+    print_results_max_count: NonNegativeInt
     relations_links: bool
     relations_initial_limit: int = Field(ge=5)
     relations_sort: SlugStr
     results_abstracts: bool
     results_abstracts_max_length: NonNegativeInt
     results_abstracts_max_length_leeway: NonNegativeInt
     results_abstracts_toggler: bool
@@ -265,15 +267,15 @@
     title: Optional[str]
     item_view: bool = False
 
 
 class CollectionFacetModel(BaseFacetModel):
     type: Literal["collection"]
     title: str
-    collection_key: str = Field(regex=r'^[A-Z]{8}$')
+    collection_key: str = Field(regex=r'^[A-Z0-9]{8}$')
 
 
 # Note: Discriminated unions ensure that a single unambiguous error gets
 # reported when validation fails. Reference:
 # https://docs.pydantic.dev/latest/usage/types/#discriminated-unions-aka-tagged-unions
 
 FacetModelUnion = Annotated[
@@ -294,16 +296,16 @@
         extra = Extra.forbid
 
     enabled: bool = True
     weight: int = 0
     label: Optional[str]
 
 
-class CitationFormatsModel(BaseModel):
-    """Model for the kerko.citation_formats config table."""
+class BibFormatsModel(BaseModel):
+    """Model for the kerko.bib_formats config table."""
 
     class Config:
         extra = Extra.forbid
 
     enabled: bool = True
     weight: int = 0
     label: Optional[str]
@@ -337,15 +339,15 @@
     templates: TemplatesModel
     zotero: ZoteroModel
     search: SearchModel
     scopes: Dict[SlugStr, ScopesModel]
     search_fields: SearchFieldsModel
     facets: Dict[FieldNameStr, FacetModelUnion]
     sorts: Dict[SlugStr, SortsModel]
-    citation_formats: Dict[SlugStr, CitationFormatsModel]
+    bib_formats: Dict[SlugStr, BibFormatsModel]
     relations: Dict[ElementIdStr, RelationsModel]
 
 
 class ConfigModel(BaseModel):
     """Model for validating mandatory at the root config table."""
 
     # Note: This model allows extra fields since we cannot cover all variables
@@ -431,7 +433,18 @@
         elif config.get(key):
             # The parsed models are stored in the config as dicts. This way, the
             # whole configuration structure is made of dicts only, allowing
             # consistent access for any element at any depth.
             config_set(config, key, model.parse_obj(config[key]).dict())
     except ValidationError as e:
         raise RuntimeError(f"Invalid configuration. {e}") from e
+
+
+def is_toml_serializable(obj: object) -> bool:
+    """
+    Check if the given object would be serializable into a TOML file.
+
+    This only performs a shallow check of the object.
+    """
+    return isinstance(
+        obj, (bool, int, float, date, datetime, time, Decimal, str, list, tuple, dict)
+    )
```

### Comparing `Kerko-1.0.0a0/src/kerko/criteria.py` & `Kerko-1.0.0a1/src/kerko/criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             if abstracts:
                 if abstracts in ['t', '1'] and not enabled_by_default:
                     self.options['abstracts'] = 1
                 elif abstracts in ['f', '0'] and enabled_by_default:
                     self.options['abstracts'] = 0
 
     def initialize_print_preview(self, initial):
-        if config('kerko.features.print_citations_link') and initial.get('print-preview') in [
+        if config('kerko.features.print_results_link') and initial.get('print-preview') in [
             't', '1'
         ]:
             self.options['print-preview'] = 1
 
     def initialize_id(self, initial):
         if self.options.get('page-len') == 1 and initial.get('id'):
             self.options['id'] = initial.get('id')
```

### Comparing `Kerko-1.0.0a0/src/kerko/datetime.py` & `Kerko-1.0.0a1/src/kerko/datetime.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/default_config.toml` & `Kerko-1.0.0a1/src/kerko/default_config.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 popper_version = "1.16.1"
 with_jquery = true
 with_popper = true
 
 [kerko.features]
 
 download_attachment_new_window = false
-download_citations_link = true
-download_citations_max_count = 0
+download_results_link = true
+download_results_max_count = 0
 open_in_zotero_app = false
 open_in_zotero_web = false
-print_citations_link = false
-print_citations_max_count = 0
 print_item_link = false
+print_results_link = false
+print_results_max_count = 0
 relations_links = false
 relations_initial_limit = 5
 relations_sort = "author_asc"
 results_abstracts = false
 results_abstracts_max_length = 0
 results_abstracts_max_length_leeway = 0
 results_abstracts_toggler = true
@@ -61,31 +61,29 @@
 
 [kerko.zotero]
 
 batch_size = 100
 max_attempts = 10
 wait = 120  # In seconds.
 
-# Changing any of the following will require sync cache --force && sync index.
-
 csl_style = "apa"
 locale = "en-US"
 item_include_re = ''
 item_exclude_re = ''
 child_include_re = ''
 child_exclude_re = '^_'
 attachment_mime_types = ["application/pdf"]
 tag_include_re = ''
 tag_exclude_re = '^_'
 
 [kerko.search]
 
 result_fields = ["id", "attachments", "bib", "coins", "data", "url"]
-fulltext = true         # Changing this will require sync cache --force && sync index.
-whoosh_language = "en"  # Changing this will require sync index --force.
+fulltext = true
+whoosh_language = "en"
 
 [kerko.scopes]
 
     [kerko.scopes.all]
     enabled = true
     weight = 0
 
@@ -103,17 +101,14 @@
 
     [kerko.scopes.fulltext]
     enabled = true
     weight = 400
 
 [kerko.search_fields]
 
-    # Changing any search field will require clean index && sync index. Except
-    # if you are just disabling the field or changing its 'scopes' parameter.
-
     # How boost factors are applied:
     # - 200.0 for primary identifiers
     # - 40.0 for secondary identifiers
     # - 20.0 for primary titles
     # - 8.0 for secondary titles and creator names
     # - 4.0 for primary text and other names
     # - 2.0 for secondary text
@@ -744,16 +739,14 @@
     enabled = true
     scopes = ["all", "metadata"]
     analyzer = "text"
     boost = 4.0
 
 [kerko.facets]
 
-    # Changing any facet will require clean index && sync index.
-
     [kerko.facets.tag]
     enabled = true
     type = "tag"
     filter_key = "topic"
     weight = 100
     initial_limit = 0
     initial_limit_leeway = 2
@@ -818,23 +811,23 @@
     enabled = true
     weight = 30
 
     [kerko.sorts.title_desc]
     enabled = true
     weight = 31
 
-[kerko.citation_formats]
+[kerko.bib_formats]
 
-    [kerko.citation_formats.ris]
+    [kerko.bib_formats.ris]
     enabled = true
     weight = 10
     extension = "ris"
     mime_type = "application/x-research-info-systems"
 
-    [kerko.citation_formats.bibtex]
+    [kerko.bib_formats.bibtex]
     enabled = true
     weight = 20
     extension = "bib"
     mime_type = "application/x-bibtex"
 
 [kerko.relations]
```

### Comparing `Kerko-1.0.0a0/src/kerko/exceptions.py` & `Kerko-1.0.0a1/src/kerko/exceptions.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/extractors.py` & `Kerko-1.0.0a1/src/kerko/extractors.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/jinja2.py` & `Kerko-1.0.0a1/src/kerko/jinja2.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/renderers.py` & `Kerko-1.0.0a1/src/kerko/renderers.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/searcher.py` & `Kerko-1.0.0a1/src/kerko/searcher.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/shortcuts.py` & `Kerko-1.0.0a1/src/kerko/shortcuts.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/specs.py` & `Kerko-1.0.0a1/src/kerko/specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,17 +568,17 @@
 
     def get_field_keys(self):
         if self.fields:
             return [spec.key for spec in self.fields]
         return None
 
 
-class CitationFormatSpec:
+class BibFormatSpec:
     """
-    Specifies a record download format.
+    Specifies a bibliographic record download format.
 
     This is a configuration element, with no effect on the search index schema.
     """
 
     def __init__(
             self,
             key,
```

### Comparing `Kerko-1.0.0a0/src/kerko/static/kerko/css/styles.css` & `Kerko-1.0.0a1/src/kerko/static/kerko/css/styles.css`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/static/kerko/js/open_in_zotero.js` & `Kerko-1.0.0a1/src/kerko/static/kerko/js/open_in_zotero.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/static/kerko/js/print.js` & `Kerko-1.0.0a1/src/kerko/static/kerko/js/print.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/static/kerko/js/search.js` & `Kerko-1.0.0a1/src/kerko/static/kerko/js/search.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/storage.py` & `Kerko-1.0.0a1/src/kerko/storage.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/sync/attachments.py` & `Kerko-1.0.0a1/src/kerko/sync/attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             data = f.read(8192)
             if not data:
                 break
             md5_hash.update(data)
         return md5_hash.hexdigest()
 
 
-def sync_attachments():
+def sync_attachments(full=False):
     """
     Synchronize attachments from Zotero into the attachments directory.
 
     Files are requested based on item data available in the search index. Thus,
     it always makes sense to synchronize the search index beforehand.
 
     Return the number of synchronized items.
@@ -38,15 +38,16 @@
             current_app.logger.warning(f"An attachment lacks an id {context}. Skipped.")
             return
         if not attachment['data'].get('md5'):
             current_app.logger.warning(f"Attachment {attachment['id']} lacks a checksum {context}.")
         if attachment['id'] in local_files:
             local_files.remove(attachment['id'])
         filepath = attachments_dir / attachment['id']
-        if not filepath.exists() or md5_checksum(filepath) != attachment['data'].get('md5', ''):
+        if full or not filepath.exists() \
+                or md5_checksum(filepath) != attachment['data'].get('md5', ''):
             current_app.logger.debug(f"Requesting attachment {attachment['id']} {context}...")
             try:
                 # Download attachment.
                 with filepath.open('wb') as f:
                     f.write(zotero.retrieve_file(zotero_credentials, attachment['id']))
             except zotero.zotero_errors.PyZoteroError as e:
                 current_app.logger.error(
```

### Comparing `Kerko-1.0.0a0/src/kerko/sync/cache.py` & `Kerko-1.0.0a1/src/kerko/sync/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         fulltext=STORED,  # Kerko addition.
     )
     for format_ in get_formats():
         schema.add(format_, STORED)
     return schema
 
 
-def sync_cache():
+def sync_cache(full=False):
     """
     Build a cache of items retrieved from Zotero.
 
     Return the number of synchronized items.
     """
     current_app.logger.info("Starting cache sync...")
     count = 0
     zotero_credentials = zotero.init_zotero()
     library_context = zotero.request_library_context(zotero_credentials)  # TODO: Load pickle & sync collections incrementally
-    since = load_object('cache', 'version', default=0)
+    since = load_object('cache', 'version', default=0) if not full else 0
     version = zotero.last_modified_version(zotero_credentials)
 
     cache = open_index('cache', schema=get_cache_schema, auto_create=True, write=True)
     writer = cache.writer(limitmb=256)
     try:
         if config('kerko.search.fulltext'):
             fulltext_items = zotero.load_new_fulltext(zotero_credentials, since)
```

### Comparing `Kerko-1.0.0a0/src/kerko/sync/index.py` & `Kerko-1.0.0a1/src/kerko/sync/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 from kerko.shortcuts import composer, config
 from kerko.storage import (SchemaError, SearchIndexError, load_object,
                            open_index, save_object)
 from kerko.tags import TagGate
 
 
-def sync_index():
+def sync_index(full=False):
     """
     Build the search index from the local cache.
 
     Return the number of synchronized items.
     """
     current_app.logger.info("Starting index sync...")
     library_context = load_object('cache', 'library')
 
     cache = open_index('cache')
     cache_version = load_object('cache', 'version', default=0)
     if not cache_version:
         raise SearchIndexError("The cache is empty and needs to be synchronized first.")
     # FIXME: The following does not detect when just the collections have changed in the cache (with no item changes). Should check the collections_version! https://pyzotero.readthedocs.io/en/latest/#zotero.Zotero.collection_versions
-    # if load_object('index', 'version', default=0) == cache_version:
+    # if not full and load_object('index', 'version', default=0) == cache_version:
     #     current_app.logger.warning(f"The index is already up-to-date with cache version {cache_version}, nothing to do.")
     #     return 0
 
     def yield_items(parent_key):
         with cache.searcher() as searcher:
             results = searcher.search(Term('parentItem', parent_key), limit=None)
             for hit in results:
```

### Comparing `Kerko-1.0.0a0/src/kerko/sync/zotero.py` & `Kerko-1.0.0a1/src/kerko/sync/zotero.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/tags.py` & `Kerko-1.0.0a1/src/kerko/tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_badges.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_badges.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_breadbox.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_breadbox.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_collapse.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_collapse.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_facet_field.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_field.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_facets.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_facets.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_item-relations.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_item-relations.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_pager.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_pager.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_preferences.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_preferences.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-form.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-form.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-help.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-help.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-metas.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-metas.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_search-result.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-result.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/_sorter.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/_sorter.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/atom.xml.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/atom.xml.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/base.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/base.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/item.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/item.html.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -39,26 +39,26 @@
 {% macro permalink(url) -%}
     <a rel="bookmark" title="{{ _('Permanent link to this bibliographic record') }}" href="{{ url }}">{{ url }}</a>
 {%- endmacro -%}
 
 {%- block metas %}
     {{- super() }}
     <link rel="canonical" title="{{ title|escape }}" href="{{ item_url }}">
-    {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
-        <link rel="alternate" title="{{ citation_format.label|escape }}" type="{{ citation_format.mime_type|escape }}" href="{{ url_for('kerko.item_citation_download', item_id=item.id, citation_format_key=citation_format.key) }}">
+    {%- for bib_format in config.kerko_composer.get_ordered_specs('bib_formats') %}
+        <link rel="alternate" title="{{ bib_format.label|escape }}" type="{{ bib_format.mime_type|escape }}" href="{{ url_for('kerko.item_bib_download', item_id=item.id, bib_format_key=bib_format.key) }}">
     {%- endfor %}
     {%- for tag in highwirepress_tags %}
         <meta name="{{ tag[0] }}" content="{{ tag[1]|striptags|escape }}">
     {%- endfor %}
 {%- endblock metas %}
 
 {%- block content_inner %}
     <div class="mt-2 mb-4 item-content">
         {%- block item_actions %}
-            {%- if item.attachments or config.kerko.features.print_item_link or config.kerko_composer.citation_formats or config.kerko.features.open_in_zotero_app or config.kerko.features.open_in_zotero_web %}
+            {%- if item.attachments or config.kerko.features.print_item_link or config.kerko_composer.bib_formats or config.kerko.features.open_in_zotero_app or config.kerko.features.open_in_zotero_web %}
                 <div class="row my-2">
                     <div class="col-auto ml-auto text-right">
                         {%- if item.attachments|length > 1 %}
                             <div class="{% block attachment_links_wrapper_classes %}d-inline-block d-print-none mb-2{% endblock %}">
                                 <div class="dropdown">
                                     <button class="{% block attachment_links_btn_classes %}btn btn-primary dropdown-toggle{% endblock %}" type="button" id="attachment-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                         <span class="fas fa-file" aria-hidden="true"></span> {{ _('Read documents') -}}
@@ -82,26 +82,26 @@
                         {%- if config.kerko.features.print_item_link %}
                             <div class="{% block print_link_wrapper_classes %}d-none d-md-inline-block d-print-none mb-2{% endblock %}">
                                 <button id="print-link" class="{% block print_btn_classes %}btn btn-light{% endblock %}" type="button">
                                     <span class="fas fa-print" aria-hidden="true"></span> {{ _('Print this record') }}
                                 </button>
                             </div>
                         {%- endif %}
-                        {%- if config.kerko_composer.citation_formats %}
+                        {%- if config.kerko_composer.bib_formats %}
                             <div class="{% block download_link_wrapper_classes %}d-inline-block d-print-none mb-2{% endblock %}">
                                 <div class="dropdown">
                                     <button class="{% block download_btn_classes %}btn btn-light dropdown-toggle{% endblock %}" type="button" id="download-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                         <span class="fas fa-download" aria-hidden="true"></span> {% trans count=1, count_formatted='1' %}Download this record{% pluralize %}Download {{ count_formatted }} records{% endtrans -%} {# TODO: Remove pluralization after solving issue where translation is not loaded when the same message is sometimes pluralized, sometimes not. -#}
                                     </button>
                                     <div class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="download-options">
-                                        {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
-                                            <a class="dropdown-item" href="{{ url_for('kerko.item_citation_download', item_id=item.id, citation_format_key=citation_format.key) }}" rel="alternate" type="{{ citation_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=citation_format.label|escape)) }}>
-                                                {{- citation_format.label -}}
+                                        {%- for bib_format in config.kerko_composer.get_ordered_specs('bib_formats') %}
+                                            <a class="dropdown-item" href="{{ url_for('kerko.item_bib_download', item_id=item.id, bib_format_key=bib_format.key) }}" rel="alternate" type="{{ bib_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=bib_format.label|escape)) }}>
+                                                {{- bib_format.label -}}
                                             </a>
-                                            <p class="px-4 text-muted">{{ citation_format.help_text }}</p>
+                                            <p class="px-4 text-muted">{{ bib_format.help_text }}</p>
                                         {%- endfor %}
                                     </div>
                                 </div>
                             </div>
                         {%- endif %}
                         {%- if config.kerko.features.open_in_zotero_app and open_in_zotero_app_url %}
                             <div id="open-in-zotero-app" class="text-right d-inline-block d-print-none mb-2 {% if not open_in_zotero_app %}d-none-important{% endif %}">
```

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/layout.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/layout.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/search-item.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/search-item.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/templates/kerko/search.html.jinja2` & `Kerko-1.0.0a1/src/kerko/templates/kerko/search.html.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends config.kerko.templates.layout %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
 
-{%- set show_print_link = config.kerko.features.print_citations_max_count == 0 or total_count <= config.kerko.features.print_citations_max_count %}
-{%- set show_print_link = show_print_link and config.kerko.features.print_citations_link %}
-{%- set show_download_link = config.kerko.features.download_citations_max_count == 0 or total_count <= config.kerko.features.download_citations_max_count %}
-{%- set show_download_link = show_download_link and config.kerko.features.download_citations_link and config.kerko_composer.citation_formats %}
+{%- set show_print_link = config.kerko.features.print_results_max_count == 0 or total_count <= config.kerko.features.print_results_max_count %}
+{%- set show_print_link = show_print_link and config.kerko.features.print_results_link %}
+{%- set show_download_link = config.kerko.features.download_results_max_count == 0 or total_count <= config.kerko.features.download_results_max_count %}
+{%- set show_download_link = show_download_link and config.kerko.features.download_results_link and config.kerko_composer.bib_formats %}
 {%- set abstracts_toggler_title = _('Hide abstracts') if show_abstracts else _('Show abstracts') %}
 
 {%- block metas %}
     {{- super() }}
     {%- include "kerko/_search-metas.html.jinja2" %}
 {%- endblock metas %}
 
@@ -120,19 +120,19 @@
                             {%- if show_download_link %}
                                 <div class="{% block download_link_wrapper_classes %}d-inline-block d-print-none mb-1{% endblock %}">
                                     <div class="dropdown">
                                         <button class="{% block download_btn_classes %}btn btn-secondary btn-light dropdown-toggle{% endblock %}" type="button" id="download-options" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                             <span class="fas fa-download" aria-hidden="true"></span> {% trans count=total_count, count_formatted=total_count_formatted|safe %}Download this record{% pluralize %}Download {{ count_formatted }} records{% endtrans -%}
                                         </button>
                                         <div class="dropdown-menu dropdown-menu-right dropdown-width-300" aria-labelledby="download-options">
-                                            {%- for citation_format in config.kerko_composer.get_ordered_specs('citation_formats') %}
-                                                <a class="dropdown-item" href="{{ download_urls[citation_format.key] }}" rel="nofollow" type="{{ citation_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=citation_format.label|escape)) }}>
-                                                    {{- citation_format.label -}}
+                                            {%- for bib_format in config.kerko_composer.get_ordered_specs('bib_formats') %}
+                                                <a class="dropdown-item" href="{{ download_urls[bib_format.key] }}" rel="nofollow" type="{{ bib_format.mime_type|escape }}" {{ title_aria_label(_('Download in {download_option} format').format(download_option=bib_format.label|escape)) }}>
+                                                    {{- bib_format.label -}}
                                                 </a>
-                                                <p class="px-4 text-muted">{{ citation_format.help_text }}</p>
+                                                <p class="px-4 text-muted">{{ bib_format.help_text }}</p>
                                             {%- endfor %}
                                         </div>
                                     </div>
                                 </div>
                             {%- endif %}
                             {%- if atom_feed_url %}
                                 <div class="{% block atom_feed_link_wrapper_classes %}d-inline-block d-print-none mb-1{% endblock %}">
```

### Comparing `Kerko-1.0.0a0/src/kerko/text.py` & `Kerko-1.0.0a1/src/kerko/text.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/transformers.py` & `Kerko-1.0.0a1/src/kerko/transformers.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.mo`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/de/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.mo`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/fr/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.mo`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/translations/pt/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/tree.py` & `Kerko-1.0.0a1/src/kerko/tree.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/breadbox.py` & `Kerko-1.0.0a1/src/kerko/views/breadbox.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/item/__init__.py` & `Kerko-1.0.0a1/src/kerko/views/item/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/item/creators.py` & `Kerko-1.0.0a1/src/kerko/views/item/creators.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/item/facets.py` & `Kerko-1.0.0a1/src/kerko/views/item/facets.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/item/meta.py` & `Kerko-1.0.0a1/src/kerko/views/item/meta.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/item/relations.py` & `Kerko-1.0.0a1/src/kerko/views/item/relations.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/pager.py` & `Kerko-1.0.0a1/src/kerko/views/pager.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/src/kerko/views/routes.py` & `Kerko-1.0.0a1/src/kerko/views/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -308,21 +308,21 @@
         get_storage_dir('attachments'),
         item['id'],
         download_name=filename,
         mimetype=item['data'].get('contentType', 'octet-stream'),
     )
 
 
-@blueprint.route('/<path:item_id>/export/<string:citation_format_key>')
+@blueprint.route('/<path:item_id>/export/<string:bib_format_key>')
 @except_abort(SchemaError, 500)
 @except_abort(SearchIndexError, 503)
-def item_citation_download(item_id, citation_format_key):
+def item_bib_download(item_id, bib_format_key):
     """Download a record."""
-    citation_format = composer().citation_formats.get(citation_format_key)
-    if not citation_format:
+    bib_format = composer().bib_formats.get(bib_format_key)
+    if not bib_format:
         return abort(404)
 
     index = open_index('index')
     with Searcher(index) as searcher:
         # Try matching the item by id, with fallback to alternate id.
         try_id_fields = deque(['id', 'alternate_id'])
         fellback = False
@@ -335,44 +335,44 @@
             )
             if results.is_empty():
                 fellback = True  # Not found on first attempt.
                 continue
             break  # Found item, or no more id fields to try.
         if results.is_empty():
             return abort(404)
-        item = results.items(composer().select_fields(['id', citation_format.field.key]))[0]
+        item = results.items(composer().select_fields(['id', bib_format.field.key]))[0]
 
-    content = item.get(citation_format.field.key)
+    content = item.get(bib_format.field.key)
     if not content:
         return abort(404)
 
     if fellback:
         return redirect(
             url_for(
-                '.item_citation_download',
+                '.item_bib_download',
                 item_id=item['id'],
-                citation_format_key=citation_format_key
+                bib_format_key=bib_format_key
             ), 301
         )
 
     response = make_response(content)
     response.headers['Content-Disposition'] = \
-        f"attachment; filename={item['id']}.{citation_format.extension}"
+        f"attachment; filename={item['id']}.{bib_format.extension}"
     response.headers['Content-Type'] = \
-        f'{citation_format.mime_type}; charset=utf-8'
+        f'{bib_format.mime_type}; charset=utf-8'
     return response
 
 
-@blueprint.route('/export/<string:citation_format_key>/')
+@blueprint.route('/export/<string:bib_format_key>/')
 @except_abort(SchemaError, 500)
 @except_abort(SearchIndexError, 503)
-def search_citation_download(citation_format_key):
+def search_bib_download(bib_format_key):
     """Download all records resulting from a search."""
-    citation_format = composer().citation_formats.get(citation_format_key)
-    if not citation_format:
+    bib_format = composer().bib_formats.get(bib_format_key)
+    if not bib_format:
         return abort(404)
 
     criteria = create_search_criteria(request.args)
     index = open_index('index')
     with Searcher(index) as searcher:
         results = searcher.search(
             limit=None,
@@ -381,26 +381,26 @@
             reject_any={'item_type': ['note', 'attachment']},
             sort_spec=criteria.get_active_sort_spec(),
             faceting=False,
         )
         if results.is_empty():
             return abort(404)
         citations = [
-            item.get(citation_format.field.key, '') for item in
-            results.items(field_specs={citation_format.field.key: citation_format.field})
+            item.get(bib_format.field.key, '') for item in
+            results.items(field_specs={bib_format.field.key: bib_format.field})
         ]
     response = make_response(
-        citation_format.group_format.format(
-            citation_format.group_item_delimiter.join(citations)
+        bib_format.group_format.format(
+            bib_format.group_item_delimiter.join(citations)
         )
     )
     response.headers['Content-Disposition'] = \
-        f'attachment; filename=bibliography.{citation_format.extension}'  # TODO: Make filename configurable.
+        f'attachment; filename=bibliography.{bib_format.extension}'  # TODO: Make filename configurable.
     response.headers['Content-Type'] = \
-        f'{citation_format.mime_type}; charset=utf-8'
+        f'{bib_format.mime_type}; charset=utf-8'
     return response
 
 
 def get_sitemap_page_count():
     count = get_doc_count('index')
     if count:
         count = math.ceil(count / SITEMAP_URL_MAX_COUNT)
```

### Comparing `Kerko-1.0.0a0/src/kerko/views/search.py` & `Kerko-1.0.0a1/src/kerko/views/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,21 +226,21 @@
                 'page-len': 'all',
                 'print-preview': 1,
             })
         )
         context['print_preview'] = criteria.options.get('print-preview', 0)
         context['download_urls'] = {
             key: url_for(
-                '.search_citation_download',
-                citation_format_key=key,
+                '.search_bib_download',
+                bib_format_key=key,
                 **criteria.params(options={
                     'page': None,
                 })
             )
-            for key in composer().citation_formats.keys()
+            for key in composer().bib_formats.keys()
         }
         if 'atom' in config('kerko.feeds.formats'):
             context['atom_feed_url'] = url_for(
                 '.atom_feed',
                 **create_feed_criteria(initial=criteria).params(options={
                     'page': None,
                 })
```

### Comparing `Kerko-1.0.0a0/src/kerko/views/sorter.py` & `Kerko-1.0.0a1/src/kerko/views/sorter.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/README.md` & `Kerko-1.0.0a1/tests/integration_testing/README.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/__init__.py` & `Kerko-1.0.0a1/tests/integration_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/collections.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/collections.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_artwork.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_artwork.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bill.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bill.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_blogPost.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_blogPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_book.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_book.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_bookSection.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bookSection.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_case.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_case.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_document.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_document.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_email.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_email.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_film.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_film.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_forumPost.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_forumPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_hearing.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_hearing.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_interview.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_interview.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_letter.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_letter.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_manuscript.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_manuscript.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_map.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_map.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_patent.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_patent.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_podcast.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_podcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_preprint.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_preprint.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_presentation.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_presentation.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_report.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_report.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_statute.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_statute.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_thesis.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_thesis.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypeFields_webpage.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_webpage.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/itemTypes.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypes.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/items.json` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/items.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/integration_testing/api_responses/update.bash` & `Kerko-1.0.0a1/tests/integration_testing/api_responses/update.bash`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_atom_feed.py` & `Kerko-1.0.0a1/tests/test_atom_feed.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_config.py` & `Kerko-1.0.0a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_datetime.py` & `Kerko-1.0.0a1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_item_meta.py` & `Kerko-1.0.0a1/tests/test_item_meta.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_pager.py` & `Kerko-1.0.0a1/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_sitemap.py` & `Kerko-1.0.0a1/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_sync.py` & `Kerko-1.0.0a1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tests/test_tags.py` & `Kerko-1.0.0a1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a0/tox.ini` & `Kerko-1.0.0a1/tox.ini`

 * *Files identical despite different names*

