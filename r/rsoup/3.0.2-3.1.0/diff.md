# Comparing `tmp/rsoup-3.0.2.tar.gz` & `tmp/rsoup-3.1.0.tar.gz`

## Comparing `rsoup-3.0.2.tar` & `rsoup-3.1.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 rsoup-3.0.2/Cargo.toml
--rw-r--r--   0     1001      123     1863 2023-06-04 21:27:22.000000 rsoup-3.0.2/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     1815 2023-06-04 21:27:22.000000 rsoup-3.0.2/.gitignore
--rw-r--r--   0     1001      123     1064 2023-06-04 21:27:22.000000 rsoup-3.0.2/LICENSE
--rw-r--r--   0     1001      123      118 2023-06-04 21:27:22.000000 rsoup-3.0.2/README.md
--rw-r--r--   0     1001      123     3490 2023-06-04 21:27:22.000000 rsoup-3.0.2/benches/context_recursive_extractor_benchmark.rs
--rw-r--r--   0     1001      123     1830 2023-06-04 21:27:22.000000 rsoup-3.0.2/benches/get_text.rs
--rw-r--r--   0     1001      123      827 2023-06-04 21:27:22.000000 rsoup-3.0.2/pyproject.toml
--rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/__init__.py
--rw-r--r--   0     1001      123     4233 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/core.pyi
--rw-r--r--   0     1001      123      586 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/exceptions.py
--rw-r--r--   0     1001      123      561 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/fetch_tables.py
--rw-r--r--   0     1001      123    15212 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/context_extractor.py
--rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/__init__.py
--rw-r--r--   0     1001      123     3091 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/context.py
--rw-r--r--   0     1001      123     9840 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/html_table.py
--rw-r--r--   0     1001      123    11141 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/table_extractor.py
--rw-r--r--   0     1001      123        4 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/.gitignore
--rw-r--r--   0     1001      123      722 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/gen_data.py
--rw-r--r--   0     1001      123     1528 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/test_table_extractor.py
--rw-r--r--   0     1001      123     1072 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/error.rs
--rw-r--r--   0     1001      123    25491 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/context_v1.rs
--rw-r--r--   0     1001      123      615 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/mod.rs
--rw-r--r--   0     1001      123    10224 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/table.rs
--rw-r--r--   0     1001      123    11019 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_rich_text.rs
--rw-r--r--   0     1001      123     3477 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_text_v1.rs
--rw-r--r--   0     1001      123     2691 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_text_v2.rs
--rw-r--r--   0     1001      123     3595 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/line.rs
--rw-r--r--   0     1001      123     1302 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/mod.rs
--rw-r--r--   0     1001      123      848 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/lib.rs
--rw-r--r--   0     1001      123     1042 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/mod.rs
--rw-r--r--   0     1001      123      404 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/range_iter.rs
--rw-r--r--   0     1001      123     5634 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/recursive_iter.rs
--rw-r--r--   0     1001      123     3474 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/iterator.rs
--rw-r--r--   0     1001      123       39 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/mod.rs
--rw-r--r--   0     1001      123     6158 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/simple_tree.rs
--rw-r--r--   0     1001      123     1600 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/url_converter.rs
--rw-r--r--   0     1001      123     4651 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/content_hierarchy.rs
--rw-r--r--   0     1001      123       61 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/mod.rs
--rw-r--r--   0     1001      123    13378 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/rich_text.rs
--rw-r--r--   0     1001      123     1824 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/cell.rs
--rw-r--r--   0     1001      123     2926 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/cell_iter.rs
--rw-r--r--   0     1001      123      158 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/mod.rs
--rw-r--r--   0     1001      123     2036 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/row.rs
--rw-r--r--   0     1001      123      591 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/row_iter.rs
--rw-r--r--   0     1001      123    13112 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/table.rs
--rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/__init__.py
--rw-r--r--   0     1001      123      639 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/conftest.py
--rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/__init__.py
--rw-r--r--   0     1001      123       79 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/mod.rs
--rw-r--r--   0     1001      123     3639 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_context_extractor.rs
--rw-r--r--   0     1001      123     3052 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_table_extractor.py
--rw-r--r--   0     1001      123     1389 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_table_extractor.rs
--rw-r--r--   0     1001      123     3573 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_text_extractor.rs
--rw-r--r--   0     1001      123      511 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/main.rs
--rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/__init__.py
--rw-r--r--   0     1001      123       20 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/mod.rs
--rw-r--r--   0     1001      123     1889 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/test_table.rs
--rw-r--r--   0     1001      123      867 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/test_table_pickle.py
--rw-r--r--   0     1001      123    38251 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/list_highest_mountains.html
--rw-r--r--   0     1001      123      326 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/one-level.html
--rw-r--r--   0     1001      123      568 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/three-level.html
--rw-r--r--   0     1001      123     4917 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/table.html
--rw-r--r--   0     1001      123     1327 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/text.html
--rw-r--r--   0     1001      123     2648 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/table_span.html
--rw-r--r--   0     1001      123    77654 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
--rw-r--r--   0     1001      123   381850 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
--rw-r--r--   0     1001      123    53084 2023-06-04 21:27:22.000000 rsoup-3.0.2/Cargo.lock
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 rsoup-3.1.0/Cargo.toml
+-rw-r--r--   0     1001      123     1856 2023-06-29 19:20:59.000000 rsoup-3.1.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1815 2023-06-29 19:20:59.000000 rsoup-3.1.0/.gitignore
+-rw-r--r--   0     1001      123     1064 2023-06-29 19:20:59.000000 rsoup-3.1.0/LICENSE
+-rw-r--r--   0     1001      123      118 2023-06-29 19:20:59.000000 rsoup-3.1.0/README.md
+-rw-r--r--   0     1001      123     3490 2023-06-29 19:20:59.000000 rsoup-3.1.0/benches/context_recursive_extractor_benchmark.rs
+-rw-r--r--   0     1001      123     1830 2023-06-29 19:20:59.000000 rsoup-3.1.0/benches/get_text.rs
+-rw-r--r--   0     1001      123      827 2023-06-29 19:20:59.000000 rsoup-3.1.0/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/__init__.py
+-rw-r--r--   0     1001      123     5477 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/core.pyi
+-rw-r--r--   0     1001      123      586 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/exceptions.py
+-rw-r--r--   0     1001      123      561 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/fetch_tables.py
+-rw-r--r--   0     1001      123    15212 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/context_extractor.py
+-rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/__init__.py
+-rw-r--r--   0     1001      123     3091 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/context.py
+-rw-r--r--   0     1001      123     9840 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/html_table.py
+-rw-r--r--   0     1001      123    11141 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/table_extractor.py
+-rw-r--r--   0     1001      123        4 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/.gitignore
+-rw-r--r--   0     1001      123      722 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/gen_data.py
+-rw-r--r--   0     1001      123     1528 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/test_table_extractor.py
+-rw-r--r--   0     1001      123     1072 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/error.rs
+-rw-r--r--   0     1001      123    25491 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/context_v1.rs
+-rw-r--r--   0     1001      123     4879 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/elementrefview.rs
+-rw-r--r--   0     1001      123     1069 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/mod.rs
+-rw-r--r--   0     1001      123    10224 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/table.rs
+-rw-r--r--   0     1001      123    11019 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_rich_text.rs
+-rw-r--r--   0     1001      123     3477 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_text_v1.rs
+-rw-r--r--   0     1001      123     2691 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_text_v2.rs
+-rw-r--r--   0     1001      123     3595 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/line.rs
+-rw-r--r--   0     1001      123     1302 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/mod.rs
+-rw-r--r--   0     1001      123      848 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/lib.rs
+-rw-r--r--   0     1001      123     1042 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/mod.rs
+-rw-r--r--   0     1001      123      404 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/range_iter.rs
+-rw-r--r--   0     1001      123     5634 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/recursive_iter.rs
+-rw-r--r--   0     1001      123     3474 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/iterator.rs
+-rw-r--r--   0     1001      123       39 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/mod.rs
+-rw-r--r--   0     1001      123     6158 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/simple_tree.rs
+-rw-r--r--   0     1001      123     1600 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/url_converter.rs
+-rw-r--r--   0     1001      123     4651 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/content_hierarchy.rs
+-rw-r--r--   0     1001      123       61 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/mod.rs
+-rw-r--r--   0     1001      123    13378 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/rich_text.rs
+-rw-r--r--   0     1001      123     1824 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/cell.rs
+-rw-r--r--   0     1001      123     2926 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/cell_iter.rs
+-rw-r--r--   0     1001      123      158 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/mod.rs
+-rw-r--r--   0     1001      123     2036 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/row.rs
+-rw-r--r--   0     1001      123      591 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/row_iter.rs
+-rw-r--r--   0     1001      123    13112 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/table.rs
+-rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/__init__.py
+-rw-r--r--   0     1001      123      639 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/conftest.py
+-rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/__init__.py
+-rw-r--r--   0     1001      123       79 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/mod.rs
+-rw-r--r--   0     1001      123     3639 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_context_extractor.rs
+-rw-r--r--   0     1001      123     3052 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_table_extractor.py
+-rw-r--r--   0     1001      123     1389 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_table_extractor.rs
+-rw-r--r--   0     1001      123     3573 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_text_extractor.rs
+-rw-r--r--   0     1001      123      511 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/main.rs
+-rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/__init__.py
+-rw-r--r--   0     1001      123       20 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/mod.rs
+-rw-r--r--   0     1001      123     1889 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/test_table.rs
+-rw-r--r--   0     1001      123      867 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/test_table_pickle.py
+-rw-r--r--   0     1001      123    38251 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/list_highest_mountains.html
+-rw-r--r--   0     1001      123      326 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/one-level.html
+-rw-r--r--   0     1001      123      568 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/three-level.html
+-rw-r--r--   0     1001      123     4917 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/table.html
+-rw-r--r--   0     1001      123     1327 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/text.html
+-rw-r--r--   0     1001      123     2648 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/table_span.html
+-rw-r--r--   0     1001      123    77654 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
+-rw-r--r--   0     1001      123   381850 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
+-rw-r--r--   0     1001      123    41375 2023-06-29 19:20:59.000000 rsoup-3.1.0/Cargo.lock
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.1.0/PKG-INFO
```

### Comparing `rsoup-3.0.2/Cargo.toml` & `rsoup-3.1.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 [package]
 name = "rsoup"
-version = "2.0.0"
+version = "2.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rsoup"
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 anyhow = { version = "1.0.59", features = ["backtrace"] }
 base64 = "0.13.0"
 criterion = "0.3.6"
 ego-tree = "0.6.2"
 hashbrown = { version = "0.12.3", features = ["serde"] }
-html5ever = "0.26.0"
 lazy_static = "1.4.0"
 phf = { version = "0.11.0", features = ["macros"] }
 postcard = { version = "1.0.1", features = ["alloc"] }
 pyo3 = { version = "0.16.3", features = ["anyhow", "hashbrown", "serde"] } 
 regex = "1.6.0"
-scraper = "0.13.0"
-selectors = "0.23.0"
+scraper = "0.17.1"
 serde = "1.0.143"
 serde_json = { version = "1.0.83", features = ["preserve_order"] }
 smallvec = "1.9.0"
-soup = "0.5.1"
 thiserror = "1.0.32"
 url = "2.2.2"
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
```

### Comparing `rsoup-3.0.2/.github/workflows/ci.yml` & `rsoup-3.1.0/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   pull_request:
 
 jobs:
   build:
     strategy:
       matrix:
         python: ["3.8", "3.9", "3.10", "3.11"]
-        platform: ["ubuntu-latest", "macos-latest", "windows-latest"]
+        platform: ["ubuntu-22.04", "macos-12", "windows-2022"]
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
```

### Comparing `rsoup-3.0.2/.gitignore` & `rsoup-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/LICENSE` & `rsoup-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/benches/context_recursive_extractor_benchmark.rs` & `rsoup-3.1.0/benches/context_recursive_extractor_benchmark.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/benches/get_text.rs` & `rsoup-3.1.0/benches/get_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/pyproject.toml` & `rsoup-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rsoup"
-version = "3.0.2"
+version = "3.1.0"
 authors = [
   { name = "Binh Vu", email = "binh@toan2.com" },
 ]
 description = "A library for web scraper that handles text correctly and is very fast (Rust backend)"
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `rsoup-3.0.2/rsoup/core.pyi` & `rsoup-3.1.0/rsoup/core.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,150 @@
-from typing import Dict, Iterator, List, Optional, Tuple
+from __future__ import annotations
+
+from typing import Iterator, Optional
 
 class Document:
     def __init__(self, url: str, doc: str): ...
+    def select(self, query: str) -> list[ElementRefView]: ...
 
 class ContextExtractor:
     def __init__(
         self,
-        ignored_tags: Optional[List[str]] = None,
-        discard_tags: Optional[List[str]] = None,
-        same_content_level_elements: Optional[List[str]] = None,
-        header_elements: Optional[List[str]] = None,
+        ignored_tags: Optional[list[str]] = None,
+        discard_tags: Optional[list[str]] = None,
+        same_content_level_elements: Optional[list[str]] = None,
+        header_elements: Optional[list[str]] = None,
         only_keep_inline_tags: bool = True,
     ): ...
 
 class TableExtractor:
     def __init__(
         self,
         *,
         context_extractor: ContextExtractor,
-        ignored_tags: Optional[List[str]] = None,
-        discard_tags: Optional[List[str]] = None,
+        ignored_tags: Optional[list[str]] = None,
+        discard_tags: Optional[list[str]] = None,
         only_keep_inline_tags: bool = True,
     ) -> None: ...
     def extract(
         self,
         url: str,
         doc: str,
         auto_span: bool = True,
         auto_pad: bool = True,
         extract_context: bool = True,
-    ) -> List[Table]: ...
+    ) -> list[Table]: ...
 
 class Table:
     id: str
     url: str
     caption: str
 
     def __init__(
         self,
         id: str,
         url: str,
         caption: str,
-        attrs: Dict[str, str],
-        context: List[ContentHierarchy],
-        rows: List[Row],
+        attrs: dict[str, str],
+        context: list[ContentHierarchy],
+        rows: list[Row],
     ) -> None: ...
     @property
-    def attrs(self) -> Dict[str, str]: ...
+    def attrs(self) -> dict[str, str]: ...
     @property
-    def context(self) -> List[ContentHierarchy]: ...
+    def context(self) -> list[ContentHierarchy]: ...
     @property
-    def rows(self) -> List[Row]: ...
+    def rows(self) -> list[Row]: ...
     def span(self) -> Table: ...
     def pad(self) -> Optional[Table]: ...
     def n_rows(self) -> int: ...
-    def shape(self) -> Tuple[int, int]: ...
+    def shape(self) -> tuple[int, int]: ...
     def get_row(self, ri: int) -> Row: ...
     def get_cell(self, ri: int, ci: int) -> Cell: ...
     def iter_cells(self) -> Iterator[Cell]: ...
-    def enumerate_cells(self) -> Iterator[Tuple[int, int, Cell]]: ...
+    def enumerate_cells(self) -> Iterator[tuple[int, int, Cell]]: ...
     def iter_rows(self) -> Iterator[Row]: ...
     def to_bytes(self) -> bytes: ...
     @staticmethod
     def from_bytes(dat: bytes) -> Table: ...
     def to_json(self) -> str: ...
     @staticmethod
     def from_json(dat: str) -> Table: ...
     def to_base64(self) -> str: ...
     @staticmethod
     def from_base64(dat: str) -> Table: ...
     def to_dict(self) -> dict: ...
-    def to_list(self) -> List[List[str]]: ...
+    def to_list(self) -> list[list[str]]: ...
 
 class Row:
-    def __init__(self, cells: List[Cell], attrs: Dict[str, str]) -> None: ...
+    def __init__(self, cells: list[Cell], attrs: dict[str, str]) -> None: ...
     @property
-    def cells(self) -> List[Cell]: ...
+    def cells(self) -> list[Cell]: ...
     @property
-    def attrs(self) -> Dict[str, str]: ...
+    def attrs(self) -> dict[str, str]: ...
     def get_cell(self, ci: int) -> Cell: ...
     def iter_cells(self) -> Iterator[Cell]: ...
     def to_dict(self) -> dict: ...
-    def to_list(self) -> List[str]: ...
+    def to_list(self) -> list[str]: ...
 
 class Cell:
     is_header: bool
     rowspan: int
     colspan: int
     value: RichText
 
     def __init__(
         self, is_header: bool, rowspan: int, colspan: int, value: RichText
     ) -> None: ...
     @property
-    def attrs(self) -> Dict[str, str]: ...
+    def attrs(self) -> dict[str, str]: ...
     def to_dict(self) -> dict: ...
 
 class ContentHierarchy:
     level: int
     heading: RichText
 
     @property
-    def content_before(self) -> List[RichText]: ...
+    def content_before(self) -> list[RichText]: ...
     @property
-    def content_after(self) -> List[RichText]: ...
+    def content_after(self) -> list[RichText]: ...
     def to_dict(self) -> dict: ...
     @staticmethod
     def from_dict(c: dict) -> ContentHierarchy: ...
 
+class ElementRefView:
+    def select(self, query: str) -> list[ElementRefView]: ...
+    def name(self) -> str: ...
+    def id(self) -> str: ...
+    def attr(self, name: str) -> str: ...
+    def attrs(self) -> Iterator[tuple[str, str]]: ...
+    def classes(self) -> list[str]: ...
+    def has_class(self, cls: str, case_sensitive: bool = True) -> bool: ...
+    def html(self) -> str: ...
+    def inner_html(self) -> str: ...
+    def get_text(self) -> str: ...
+    def get_rich_text(self, cfg: RichTextConfig) -> RichText: ...
+
+class RichTextConfig:
+    def __init__(
+        self,
+        ignored_tags: list[str],
+        only_inline_tags: bool,
+        discard_tags: list[str],
+        keep_tags: list[str],
+    ) -> None:
+        """
+        Arguments:
+            ignored_tags: tags to be ignored and not include in the trace (its text is stilled captured but the element containing the text is not stored and thus, cannot be traced back)
+            only_inline_tags: whether to only keep inline tags
+            discard_tags: tags to be discarded (its text is not captured)
+            keep_tags: tags to be kept (its text is captured)
+        """
+        ...
+
 class RichText:
     @staticmethod
     def from_str(text: str) -> RichText: ...
     @property
     def text(self) -> str: ...
     def len(self) -> int: ...
     def iter_element_id(self) -> Iterator[int]: ...
@@ -129,13 +162,13 @@
     @property
     def tag(self) -> str: ...
     @property
     def start(self) -> int: ...
     @property
     def end(self) -> int: ...
     @property
-    def attrs(self) -> Dict[str, str]: ...
+    def attrs(self) -> dict[str, str]: ...
     def get_attr(self, name: str) -> str: ...
     def has_attr(self, name: str) -> bool: ...
     def to_dict(self) -> dict: ...
     @staticmethod
     def from_dict(c: dict) -> RichTextElement: ...
```

### Comparing `rsoup-3.0.2/rsoup/exceptions.py` & `rsoup-3.1.0/rsoup/exceptions.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/rsoup/fetch_tables.py` & `rsoup-3.1.0/rsoup/fetch_tables.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/rsoup/python/context_extractor.py` & `rsoup-3.1.0/rsoup/python/context_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/rsoup/python/models/context.py` & `rsoup-3.1.0/rsoup/python/models/context.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/rsoup/python/models/html_table.py` & `rsoup-3.1.0/rsoup/python/models/html_table.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/rsoup/python/table_extractor.py` & `rsoup-3.1.0/rsoup/python/table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/scripts/gen_data.py` & `rsoup-3.1.0/scripts/gen_data.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/scripts/test_table_extractor.py` & `rsoup-3.1.0/scripts/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/error.rs` & `rsoup-3.1.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/context_v1.rs` & `rsoup-3.1.0/src/extractors/context_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/table.rs` & `rsoup-3.1.0/src/extractors/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/text/get_rich_text.rs` & `rsoup-3.1.0/src/extractors/text/get_rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/text/get_text_v1.rs` & `rsoup-3.1.0/src/extractors/text/get_text_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/text/get_text_v2.rs` & `rsoup-3.1.0/src/extractors/text/get_text_v2.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/text/line.rs` & `rsoup-3.1.0/src/extractors/text/line.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/extractors/text/mod.rs` & `rsoup-3.1.0/src/extractors/text/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/lib.rs` & `rsoup-3.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/misc/mod.rs` & `rsoup-3.1.0/src/misc/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/misc/recursive_iter.rs` & `rsoup-3.1.0/src/misc/recursive_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/misc/tree/iterator.rs` & `rsoup-3.1.0/src/misc/tree/iterator.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/misc/tree/simple_tree.rs` & `rsoup-3.1.0/src/misc/tree/simple_tree.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/misc/url_converter.rs` & `rsoup-3.1.0/src/misc/url_converter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/content_hierarchy.rs` & `rsoup-3.1.0/src/models/content_hierarchy.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/rich_text.rs` & `rsoup-3.1.0/src/models/rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/table/cell.rs` & `rsoup-3.1.0/src/models/table/cell.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/table/cell_iter.rs` & `rsoup-3.1.0/src/models/table/cell_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/table/row.rs` & `rsoup-3.1.0/src/models/table/row.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/table/row_iter.rs` & `rsoup-3.1.0/src/models/table/row_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/src/models/table/table.rs` & `rsoup-3.1.0/src/models/table/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/conftest.py` & `rsoup-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/extractors/test_context_extractor.rs` & `rsoup-3.1.0/tests/extractors/test_context_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/extractors/test_table_extractor.py` & `rsoup-3.1.0/tests/extractors/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/extractors/test_table_extractor.rs` & `rsoup-3.1.0/tests/extractors/test_table_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/extractors/test_text_extractor.rs` & `rsoup-3.1.0/tests/extractors/test_text_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/models/test_table.rs` & `rsoup-3.1.0/tests/models/test_table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/models/test_table_pickle.py` & `rsoup-3.1.0/tests/models/test_table_pickle.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/extractors/context/list_highest_mountains.html` & `rsoup-3.1.0/tests/resources/extractors/context/list_highest_mountains.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/extractors/context/three-level.html` & `rsoup-3.1.0/tests/resources/extractors/context/three-level.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/extractors/table.html` & `rsoup-3.1.0/tests/resources/extractors/table.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/extractors/text.html` & `rsoup-3.1.0/tests/resources/extractors/text.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/table_span.html` & `rsoup-3.1.0/tests/resources/table_span.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html` & `rsoup-3.1.0/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html` & `rsoup-3.1.0/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.2/Cargo.lock` & `rsoup-3.1.0/Cargo.lock`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,27 @@
 
 [[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
- "getrandom 0.2.7",
+ "getrandom",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
 version = "0.7.18"
@@ -64,23 +76,14 @@
  "hermit-abi",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "0.1.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0dde43e75fd43e8a1bf86103336bc699aa8d17ad1be60c76c0bdfd4828e19b78"
-dependencies = [
- "autocfg 1.1.0",
-]
-
-[[package]]
-name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "backtrace"
 version = "0.3.66"
@@ -132,14 +135,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "lazy_static",
  "memchr",
@@ -179,41 +188,26 @@
 
 [[package]]
 name = "clap"
 version = "2.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "textwrap",
  "unicode-width",
 ]
 
 [[package]]
-name = "cloudabi"
-version = "0.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddfc5b9aa5d4507acaf872de71051dfd0e309860e88966e1051e462a077aac4f"
-dependencies = [
- "bitflags",
-]
-
-[[package]]
 name = "cobs"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67ba02a97a2bd10f4b59b25c7973101c79642302776489e030cd13cdab09ed15"
 
 [[package]]
-name = "convert_case"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
-
-[[package]]
 name = "cortex-m"
 version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd20d4ac4aa86f4f75f239d59e542ef67de87cce2c282818dc6e84155d3ea126"
 dependencies = [
  "bare-metal 0.2.5",
  "bitfield",
@@ -292,15 +286,15 @@
 
 [[package]]
 name = "crossbeam-epoch"
 version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "045ebe27666471bb549370b4b0b3e51b07f56325befa4284db65fc89c02511b1"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
  "cfg-if",
  "crossbeam-utils",
  "memoffset",
  "once_cell",
  "scopeguard",
 ]
 
@@ -312,54 +306,33 @@
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "cssparser"
-version = "0.27.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "754b69d351cdc2d8ee09ae203db831e005560fc6030da058f86ad60c92a9cb0a"
-dependencies = [
- "cssparser-macros",
- "dtoa-short",
- "itoa 0.4.8",
- "matches",
- "phf 0.8.0",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
- "smallvec",
- "syn 1.0.95",
-]
-
-[[package]]
-name = "cssparser"
-version = "0.28.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1db8599a9761b371751fbf13e076fa03c6e1a78f8c5288e6ab9467f10a2322c1"
+checksum = "5b3df4f93e5fbbe73ec01ec8d3f68bba73107993a5b1e7519273c32db9b0d5be"
 dependencies = [
  "cssparser-macros",
  "dtoa-short",
- "itoa 0.4.8",
- "matches",
- "phf 0.8.0",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "itoa 1.0.3",
+ "phf 0.11.0",
  "smallvec",
- "syn 1.0.95",
 ]
 
 [[package]]
 name = "cssparser-macros"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfae75de57f2b2e85e8768c3ea840fd159c8f33e2b6522c7835b7abac81be16e"
+checksum = "13b588ba4ac1a99f7f2964d24b3d896ddc6bf847ee3855dbd4366f058cfcd331"
 dependencies = [
- "quote 1.0.18",
- "syn 1.0.95",
+ "quote",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "csv"
 version = "1.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22813a6dc45b335f9bade10bf7271dc477e81113e89eb251a0bc2a8a81c536e1"
@@ -382,18 +355,16 @@
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
- "convert_case",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
- "rustc_version 0.4.0",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "dtoa"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -437,20 +408,14 @@
 checksum = "5fc25a87fa4fd2094bffb06925852034d90a17f0d1e05197d4956d3555752191"
 dependencies = [
  "matches",
  "percent-encoding",
 ]
 
 [[package]]
-name = "fuchsia-cprng"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
-
-[[package]]
 name = "futf"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df420e2e84819663797d1ec6544b13c5be84629e7bb00dc960d6917db2987843"
 dependencies = [
  "mac",
  "new_debug_unreachable",
@@ -472,32 +437,21 @@
 checksum = "14dbbfd5c71d70241ecf9e6f13737f7b5ce823821063188d7e46c41d371eebd5"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.1.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fc3cb4d91f53b50155bdcfd23f6a4c39ae1969c2ae85982b135750cccaf5fce"
-dependencies = [
- "cfg-if",
- "libc",
- "wasi 0.9.0+wasi-snapshot-preview1",
-]
-
-[[package]]
-name = "getrandom"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4eb1a864a501629691edf6c15a593b7a51eebaa1e8468e9ddc623de7c9b58ec6"
 dependencies = [
  "cfg-if",
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22030e2c5a68ec659fde1e949a745124b48e6fa8b045b7ed5bd1fe4ccc5c4e5d"
@@ -519,15 +473,15 @@
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
- "ahash",
+ "ahash 0.7.6",
  "serde",
 ]
 
 [[package]]
 name = "heapless"
 version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -548,37 +502,23 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "html5ever"
-version = "0.22.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c213fa6a618dc1da552f54f85cba74b05d8e883c92ec4e89067736938084c26e"
-dependencies = [
- "log",
- "mac",
- "markup5ever 0.7.5",
- "proc-macro2 0.4.30",
- "quote 0.6.13",
- "syn 0.15.44",
-]
-
-[[package]]
-name = "html5ever"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bea68cab48b8459f17cf1c944c67ddc572d272d9f2b274140f223ecb1da4a3b7"
 dependencies = [
  "log",
  "mac",
- "markup5ever 0.11.0",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "markup5ever",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "idna"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -591,15 +531,15 @@
 
 [[package]]
 name = "indexmap"
 version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10a35a97730320ffe8e2d410b5d3b69279b98d2c14bdb8b70ea89ecf7888d41e"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -649,15 +589,15 @@
 
 [[package]]
 name = "lock_api"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "327fa5b6a6940e4699ec49a9beae1ea4845c6bab9314e4f84ac68742139d8c53"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -670,39 +610,23 @@
 name = "mac"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c41e0c4fef86961ac6d6f8a82609f55f31b05e4fce149ac5710e439df7619ba4"
 
 [[package]]
 name = "markup5ever"
-version = "0.7.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "897636f9850c3eef4905a5540683ed53dc9393860f0846cab2c2ddf9939862ff"
-dependencies = [
- "phf 0.7.24",
- "phf_codegen 0.7.24",
- "serde",
- "serde_derive",
- "serde_json",
- "string_cache 0.7.5",
- "string_cache_codegen 0.4.4",
- "tendril",
-]
-
-[[package]]
-name = "markup5ever"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a2629bb1404f3d34c2e921f21fd34ba00b206124c81f65c50b43b6aaefeb016"
 dependencies = [
  "log",
  "phf 0.10.1",
- "phf_codegen 0.10.0",
- "string_cache 0.8.4",
- "string_cache_codegen 0.5.2",
+ "phf_codegen",
+ "string_cache",
+ "string_cache_codegen",
  "tendril",
 ]
 
 [[package]]
 name = "matches"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -716,15 +640,15 @@
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f5c75688da582b8ffc1f1799e9db273f32133c49e048f614d22ec3256773ccc"
@@ -750,26 +674,20 @@
 [[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
-name = "nodrop"
-version = "0.1.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72ef4a56884ca558e5ddb05a1d1e7e1bfd9a68d9ed024c21704cc98872dae1bb"
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19e64526ebdee182341572e50e9ad03965aa510cd94427a4549448f285e957a1"
@@ -785,17 +703,17 @@
 checksum = "21158b2c33aa6d4561f1c0a6ea283ca92bc54802a93b263e910746d679a7eb53"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.12.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7709cef83f0c1f58f666e746a08b21e0085f7440fa6a29cc194d68aac97a4225"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
@@ -826,182 +744,90 @@
 name = "percent-encoding"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4fd5641d01c8f18a23da7b6fe29298ff4b55afcccdf78973b24cf3175fee32e"
 
 [[package]]
 name = "phf"
-version = "0.7.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3da44b85f8e8dfaec21adae67f95d93244b2ecf6ad2a692320598dcc8e6dd18"
-dependencies = [
- "phf_shared 0.7.24",
-]
-
-[[package]]
-name = "phf"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dfb61232e34fcb633f43d12c58f83c1df82962dcdfa565a4e866ffc17dafe12"
-dependencies = [
- "phf_macros 0.8.0",
- "phf_shared 0.8.0",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "phf"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
 dependencies = [
  "phf_shared 0.10.0",
 ]
 
 [[package]]
 name = "phf"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4724fa946c8d1e7cd881bd3dbee63ce32fc1e9e191e35786b3dc1320a3f68131"
 dependencies = [
- "phf_macros 0.11.0",
+ "phf_macros",
  "phf_shared 0.11.0",
 ]
 
 [[package]]
 name = "phf_codegen"
-version = "0.7.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b03e85129e324ad4166b06b2c7491ae27fe3ec353af72e72cd1654c7225d517e"
-dependencies = [
- "phf_generator 0.7.24",
- "phf_shared 0.7.24",
-]
-
-[[package]]
-name = "phf_codegen"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cbffee61585b0411840d3ece935cce9cb6321f01c45477d30066498cd5e1a815"
-dependencies = [
- "phf_generator 0.8.0",
- "phf_shared 0.8.0",
-]
-
-[[package]]
-name = "phf_codegen"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb1c3a8bc4dd4e5cfce29b44ffc14bedd2ee294559a294e2a4d4c9e9a6a13cd"
 dependencies = [
  "phf_generator 0.10.0",
  "phf_shared 0.10.0",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.7.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09364cc93c159b8b06b1f4dd8a4398984503483891b0c26b867cf431fb132662"
-dependencies = [
- "phf_shared 0.7.24",
- "rand 0.6.5",
-]
-
-[[package]]
-name = "phf_generator"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17367f0cc86f2d25802b2c26ee58a7b23faeccf78a396094c13dced0d0182526"
-dependencies = [
- "phf_shared 0.8.0",
- "rand 0.7.3",
-]
-
-[[package]]
-name = "phf_generator"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d5285893bb5eb82e6aaf5d59ee909a06a16737a8970984dd7746ba9283498d6"
 dependencies = [
  "phf_shared 0.10.0",
- "rand 0.8.5",
+ "rand",
 ]
 
 [[package]]
 name = "phf_generator"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b450720b6f75cfbfabc195814bd3765f337a4f9a83186f8537297cac12f6705"
 dependencies = [
  "phf_shared 0.11.0",
- "rand 0.8.5",
-]
-
-[[package]]
-name = "phf_macros"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6fde18ff429ffc8fe78e2bf7f8b7a5a5a6e2a8b58bc5a9ac69198bbda9189c"
-dependencies = [
- "phf_generator 0.8.0",
- "phf_shared 0.8.0",
- "proc-macro-hack",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
- "syn 1.0.95",
+ "rand",
 ]
 
 [[package]]
 name = "phf_macros"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd94351ac44e70e56b59883e15029a5135f902a8a3020f9c18d580a420e526aa"
 dependencies = [
  "phf_generator 0.11.0",
  "phf_shared 0.11.0",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.7.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "234f71a15de2288bcb7e3b6515828d22af7ec8598ee6d24c3b526fa0a80b67a0"
-dependencies = [
- "siphasher 0.2.3",
-]
-
-[[package]]
-name = "phf_shared"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c00cf8b9eafe68dde5e9eaa2cef8ee84a9336a47d566ec55ca16589633b65af7"
-dependencies = [
- "siphasher 0.3.10",
-]
-
-[[package]]
-name = "phf_shared"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
 dependencies = [
- "siphasher 0.3.10",
+ "siphasher",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9dd5609d4b2df87167f908a32e1b146ce309c16cf35df76bc11f440b756048e4"
 dependencies = [
- "siphasher 0.3.10",
+ "siphasher",
 ]
 
 [[package]]
 name = "plotters"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9428003b84df1496fb9d6eeee9c5f8145cb41ca375eb0dad204328888832811f"
@@ -1048,33 +874,18 @@
 [[package]]
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbf0c48bc1d91375ae5c3cd81e3722dff1abcf81a30960240640d223f59fe0e5"
-
-[[package]]
-name = "proc-macro2"
-version = "0.4.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf3d2011ab5c909338f7887f4fc896d35932e29146c12c8d01da6b22a80ba759"
-dependencies = [
- "unicode-xid",
-]
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.39"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c54b25569025b7fc9651de43004ae593a75ad88543b17178aa5e1b9c4f15f56f"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.16.5"
@@ -1116,243 +927,77 @@
 
 [[package]]
 name = "pyo3-macros"
 version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "284fc4485bfbcc9850a6d661d627783f18d19c2ab55880b021671c4ba83e90f7"
 dependencies = [
- "proc-macro2 1.0.39",
+ "proc-macro2",
  "pyo3-macros-backend",
- "quote 1.0.18",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bda0f58f73f5c5429693c96ed57f7abdb38fdfc28ae06da4101a257adb7faf"
 dependencies = [
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "quote"
-version = "0.6.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ce23b6b870e8f94f81fb0a363d65d86675884b34a09043c81e5562f11c1f8e1"
-dependencies = [
- "proc-macro2 0.4.30",
-]
-
-[[package]]
-name = "quote"
-version = "1.0.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1feb54ed693b93a84e14094943b84b7c4eae204c512b7ccb95ab0c66d278ad1"
-dependencies = [
- "proc-macro2 1.0.39",
-]
-
-[[package]]
-name = "rand"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d71dacdc3c88c1fde3885a3be3fbab9f35724e6ce99467f7d9c5026132184ca"
-dependencies = [
- "autocfg 0.1.8",
- "libc",
- "rand_chacha 0.1.1",
- "rand_core 0.4.2",
- "rand_hc 0.1.0",
- "rand_isaac",
- "rand_jitter",
- "rand_os",
- "rand_pcg 0.1.2",
- "rand_xorshift",
- "winapi",
-]
-
-[[package]]
-name = "rand"
-version = "0.7.3"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a6b1679d49b24bbfe0c803429aa1874472f50d9b363131f0e89fc356b544d03"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
- "getrandom 0.1.16",
- "libc",
- "rand_chacha 0.2.2",
- "rand_core 0.5.1",
- "rand_hc 0.2.0",
- "rand_pcg 0.2.1",
+ "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
- "rand_chacha 0.3.1",
- "rand_core 0.6.3",
-]
-
-[[package]]
-name = "rand_chacha"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "556d3a1ca6600bfcbab7c7c91ccb085ac7fbbcd70e008a98742e7847f4f7bcef"
-dependencies = [
- "autocfg 0.1.8",
- "rand_core 0.3.1",
-]
-
-[[package]]
-name = "rand_chacha"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4c8ed856279c9737206bf725bf36935d8666ead7aa69b52be55af369d193402"
-dependencies = [
- "ppv-lite86",
- "rand_core 0.5.1",
+ "rand_chacha",
+ "rand_core",
 ]
 
 [[package]]
 name = "rand_chacha"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
 dependencies = [
  "ppv-lite86",
- "rand_core 0.6.3",
-]
-
-[[package]]
-name = "rand_core"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a6fdeb83b075e8266dcc8762c22776f6877a63111121f5f8c7411e5be7eed4b"
-dependencies = [
- "rand_core 0.4.2",
-]
-
-[[package]]
-name = "rand_core"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c33a3c44ca05fa6f1807d8e6743f3824e8509beca625669633be0acbdf509dc"
-
-[[package]]
-name = "rand_core"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90bde5296fc891b0cef12a6d03ddccc162ce7b2aff54160af9338f8d40df6d19"
-dependencies = [
- "getrandom 0.1.16",
+ "rand_core",
 ]
 
 [[package]]
 name = "rand_core"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d34f1408f55294453790c48b2f1ebbb1c5b4b7563eb1f418bcfcfdbb06ebb4e7"
 dependencies = [
- "getrandom 0.2.7",
-]
-
-[[package]]
-name = "rand_hc"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b40677c7be09ae76218dc623efbf7b18e34bced3f38883af07bb75630a21bc4"
-dependencies = [
- "rand_core 0.3.1",
-]
-
-[[package]]
-name = "rand_hc"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
-dependencies = [
- "rand_core 0.5.1",
-]
-
-[[package]]
-name = "rand_isaac"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ded997c9d5f13925be2a6fd7e66bf1872597f759fd9dd93513dd7e92e5a5ee08"
-dependencies = [
- "rand_core 0.3.1",
-]
-
-[[package]]
-name = "rand_jitter"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1166d5c91dc97b88d1decc3285bb0a99ed84b05cfd0bc2341bdf2d43fc41e39b"
-dependencies = [
- "libc",
- "rand_core 0.4.2",
- "winapi",
-]
-
-[[package]]
-name = "rand_os"
-version = "0.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b75f676a1e053fc562eafbb47838d67c84801e38fc1ba459e8f180deabd5071"
-dependencies = [
- "cloudabi",
- "fuchsia-cprng",
- "libc",
- "rand_core 0.4.2",
- "rdrand",
- "winapi",
-]
-
-[[package]]
-name = "rand_pcg"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abf9b09b01790cfe0364f52bf32995ea3c39f4d2dd011eac241d2914146d0b44"
-dependencies = [
- "autocfg 0.1.8",
- "rand_core 0.4.2",
-]
-
-[[package]]
-name = "rand_pcg"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16abd0c1b639e9eb4d7c50c0b8100b0d0f849be2349829c740fe8e6eb4816429"
-dependencies = [
- "rand_core 0.5.1",
-]
-
-[[package]]
-name = "rand_xorshift"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cbf7e9e623549b0e21f6e97cf8ecf247c1a8fd2e8a992ae265314300b2455d5c"
-dependencies = [
- "rand_core 0.3.1",
+ "getrandom",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd99e5772ead8baa5215278c9b15bf92087709e9c1b2d1f97cdb5a183c933a7d"
 dependencies = [
- "autocfg 1.1.0",
+ "autocfg",
  "crossbeam-deque",
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1363,29 +1008,20 @@
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
-name = "rdrand"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "678054eb77286b51581ba43620cc911abf02758c91f93f479767aed0f90458b2"
-dependencies = [
- "rand_core 0.3.1",
-]
-
-[[package]]
 name = "redox_syscall"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62f25bc4c7e55e0b0b7a1d43fb893f4fa1361d0abe38b9ce4f323c2adfe6ef42"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c4eb3267174b8c6c2f654116623910a0fef09c4753f8dd83db29c48a0df988b"
@@ -1426,33 +1062,30 @@
 dependencies = [
  "lazy_static",
  "regex",
 ]
 
 [[package]]
 name = "rsoup"
-version = "2.0.0"
+version = "2.1.0"
 dependencies = [
  "anyhow",
  "base64",
  "criterion",
  "ego-tree",
  "hashbrown",
- "html5ever 0.26.0",
  "lazy_static",
  "phf 0.11.0",
  "postcard",
  "pyo3",
  "regex",
  "scraper",
- "selectors 0.23.0",
  "serde",
  "serde_json",
  "smallvec",
- "soup",
  "thiserror",
  "url",
 ]
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.21"
@@ -1496,61 +1129,43 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scraper"
-version = "0.13.0"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5684396b456f3eb69ceeb34d1b5cb1a2f6acf7ca4452131efa3ba0ee2c2d0a70"
+checksum = "c95a930e03325234c18c7071fd2b60118307e025d6fff3e12745ffbf63a3d29c"
 dependencies = [
- "cssparser 0.27.2",
+ "ahash 0.8.3",
+ "cssparser",
  "ego-tree",
  "getopts",
- "html5ever 0.26.0",
- "matches",
- "selectors 0.22.0",
+ "html5ever",
+ "once_cell",
+ "selectors",
  "smallvec",
  "tendril",
 ]
 
 [[package]]
 name = "selectors"
-version = "0.22.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df320f1889ac4ba6bc0cdc9c9af7af4bd64bb927bccdf32d81140dc1f9be12fe"
+checksum = "4eb30575f3638fc8f6815f448d50cb1a2e255b0897985c8c59f4d37b72a07b06"
 dependencies = [
- "bitflags",
- "cssparser 0.27.2",
+ "bitflags 2.3.3",
+ "cssparser",
  "derive_more",
  "fxhash",
  "log",
- "matches",
- "phf 0.8.0",
- "phf_codegen 0.8.0",
- "precomputed-hash",
- "servo_arc",
- "smallvec",
- "thin-slice",
-]
-
-[[package]]
-name = "selectors"
-version = "0.23.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fdea87c686be721aab36607728047801ee21561bfdbd6bf0da7ace2536d5879f"
-dependencies = [
- "bitflags",
- "cssparser 0.28.1",
- "derive_more",
- "fxhash",
- "log",
- "phf 0.8.0",
- "phf_codegen 0.8.0",
+ "new_debug_unreachable",
+ "phf 0.10.1",
+ "phf_codegen",
  "precomputed-hash",
  "servo_arc",
  "smallvec",
 ]
 
 [[package]]
 name = "semver"
@@ -1594,16 +1209,16 @@
 
 [[package]]
 name = "serde_derive"
 version = "1.0.143"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3d8e8de557aee63c26b85b947f5e59b690d0454c753f3adeb5cd7835ab88391"
 dependencies = [
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1613,49 +1228,32 @@
  "itoa 1.0.3",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "servo_arc"
-version = "0.1.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d98238b800e0d1576d8b6e3de32827c2d74bee68bb97748dcf5071fb53965432"
+checksum = "d036d71a959e00c77a63538b90a6c2390969f9772b096ea837205c6bd0491a44"
 dependencies = [
- "nodrop",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "siphasher"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b8de496cf83d4ed58b6be86c3a275b8602f6ffe98d3024a869e124147a9a3ac"
-
-[[package]]
-name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "smallvec"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
-
-[[package]]
-name = "soup"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa5a5d21523f4b7a17ad04eaf534360fc908879f53f3341918cbec2fee9cfe14"
-dependencies = [
- "html5ever 0.22.5",
- "regex",
-]
+checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f6002a767bff9e83f8eeecf883ecb8011875a21ae8da43bffb817a57e78cc09"
 dependencies = [
@@ -1666,91 +1264,57 @@
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
 name = "string_cache"
-version = "0.7.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89c058a82f9fd69b1becf8c274f412281038877c553182f1d02eb027045a2d67"
-dependencies = [
- "lazy_static",
- "new_debug_unreachable",
- "phf_shared 0.7.24",
- "precomputed-hash",
- "serde",
- "string_cache_codegen 0.4.4",
- "string_cache_shared",
-]
-
-[[package]]
-name = "string_cache"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "213494b7a2b503146286049378ce02b482200519accc31872ee8be91fa820a08"
 dependencies = [
  "new_debug_unreachable",
  "once_cell",
  "parking_lot",
  "phf_shared 0.10.0",
  "precomputed-hash",
  "serde",
 ]
 
 [[package]]
 name = "string_cache_codegen"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0f45ed1b65bf9a4bf2f7b7dc59212d1926e9eaf00fa998988e420fd124467c6"
-dependencies = [
- "phf_generator 0.7.24",
- "phf_shared 0.7.24",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
- "string_cache_shared",
-]
-
-[[package]]
-name = "string_cache_codegen"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bb30289b722be4ff74a408c3cc27edeaad656e06cb1fe8fa9231fa59c728988"
 dependencies = [
  "phf_generator 0.10.0",
  "phf_shared 0.10.0",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
 ]
 
 [[package]]
-name = "string_cache_shared"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1884d1bc09741d466d9b14e6d37ac89d6909cbcac41dd9ae982d4d063bbedfc"
-
-[[package]]
 name = "syn"
-version = "0.15.44"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ca4b3b69a77cbe1ffc9e198781b7acb0c7365a883670e8f1c1bc66fba79a5c5"
+checksum = "fbaf6116ab8924f39d52792136fb74fd60a80194cf1b1c6ffa6453eef1c3f942"
 dependencies = [
- "proc-macro2 0.4.30",
- "quote 0.6.13",
- "unicode-xid",
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.95"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbaf6116ab8924f39d52792136fb74fd60a80194cf1b1c6ffa6453eef1c3f942"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1773,36 +1337,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
-name = "thin-slice"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaa81235c7058867fa8c0e7314f33dcce9c215f535d1913822a2b3f5e289f3c"
-
-[[package]]
 name = "thiserror"
 version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5f6586b7f764adc0231f4c79be7b920e766bb2f3e51b3661cdb263828f19994"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
 version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12bafc5b54507e0149cdf1b145a5d80ab80a90bcd9275df43d4fff68460f6c21"
 dependencies = [
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1851,20 +1409,14 @@
 [[package]]
 name = "unicode-width"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ed742d4ea2bd1176e236172c8429aaf54486e7ac098db29ffe6529e0ce50973"
 
 [[package]]
-name = "unicode-xid"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc72304796d0818e357ead4e000d19c9c174ab23dc11093ac919054d20a6a7fc"
-
-[[package]]
 name = "unindent"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52fee519a3e570f7df377a06a1a7775cdbfb7aa460be7e08de2b1f0e69973a44"
 
 [[package]]
 name = "url"
@@ -1920,20 +1472,14 @@
  "same-file",
  "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
-version = "0.9.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
-
-[[package]]
-name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
 version = "0.2.82"
@@ -1949,38 +1495,38 @@
 version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "662cd44805586bd52971b9586b1df85cdbbd9112e4ef4d8f41559c334dc6ac3f"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b260f13d3012071dfb1512849c033b1925038373aea48ced3012c09df952c602"
 dependencies = [
- "quote 1.0.18",
+ "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
 version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5be8e654bdd9b79216c2929ab90721aa82faf65c48cdf08bdc4e7f51357b80da"
 dependencies = [
- "proc-macro2 1.0.39",
- "quote 1.0.18",
+ "proc-macro2",
+ "quote",
  "syn 1.0.95",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
```

### Comparing `rsoup-3.0.2/PKG-INFO` & `rsoup-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsoup
-Version: 3.0.2
+Version: 3.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: html5lib >=1.1.0, <2.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
```

