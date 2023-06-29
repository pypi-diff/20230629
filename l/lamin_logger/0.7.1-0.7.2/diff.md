# Comparing `tmp/lamin_logger-0.7.1.tar.gz` & `tmp/lamin_logger-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.1.tar` & `lamin_logger-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.1/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.1/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.1/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.1/docs/api.md
--rw-r--r--   0        0        0     4471 2023-06-22 14:21:14.438600 lamin_logger-0.7.1/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.1/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.1/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.1/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-22 14:21:07.142843 lamin_logger-0.7.1/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.1/lamin_logger/_core.py
--rw-r--r--   0        0        0     3828 2023-06-22 14:19:30.502828 lamin_logger-0.7.1/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.1/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.1/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7160 2023-06-22 14:19:30.503212 lamin_logger-0.7.1/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.1/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.1/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.1/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.1/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.1/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.1/tests/test_lookup.py
--rw-r--r--   0        0        0     5769 2023-06-22 14:19:30.503907 lamin_logger-0.7.1/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.1/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.2/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.2/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.2/docs/api.md
+-rw-r--r--   0        0        0     4471 2023-06-22 14:21:14.438600 lamin_logger-0.7.2/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.2/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.2/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.2/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-29 16:03:54.672354 lamin_logger-0.7.2/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.2/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.2/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.2/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.2/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7160 2023-06-22 14:19:30.503212 lamin_logger-0.7.2/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.2/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.2/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.2/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.2/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.2/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.2/tests/test_lookup.py
+-rw-r--r--   0        0        0     5769 2023-06-22 14:19:30.503907 lamin_logger-0.7.2/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.2/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.2/PKG-INFO
```

### Comparing `lamin_logger-0.7.1/.github/workflows/build.yml` & `lamin_logger-0.7.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/.gitignore` & `lamin_logger-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/.pre-commit-config.yaml` & `lamin_logger-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/LICENSE` & `lamin_logger-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/docs/changelog.md` & `lamin_logger-0.7.2/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/docs/quickstart.ipynb` & `lamin_logger-0.7.2/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_core.py` & `lamin_logger-0.7.2/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_inspect.py` & `lamin_logger-0.7.2/lamin_logger/_inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,18 +90,18 @@
     frac_unmapped = round(len(unmapped) / n_unique_terms * 100, 1)
     frac_mapped = 100 - frac_unmapped
 
     if logging:
         if n_empty > 0:
             logger.warning(
                 f"Received {n_unique_terms} unique terms, {n_empty} empty/duplicated"
-                " terms are ignored."
+                " terms are ignored"
             )
-        logger.success(f"{len(mapped)} terms ({frac_mapped}%) are mapped.")
-        logger.warning(f"{len(unmapped)} terms ({frac_unmapped}%) are not mapped.")
+        logger.success(f"{len(mapped)} terms ({frac_mapped}%) are mapped")
+        logger.warning(f"{len(unmapped)} terms ({frac_unmapped}%) are not mapped")
 
     if return_df:
         return mapped_df
     else:
         mapping: Dict[str, List[str]] = {}
         mapping["mapped"] = mapped
         mapping["not_mapped"] = unmapped
```

### Comparing `lamin_logger-0.7.1/lamin_logger/_logger.py` & `lamin_logger-0.7.2/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_lookup.py` & `lamin_logger-0.7.2/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.2/lamin_logger/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_python_version.py` & `lamin_logger-0.7.2/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/lamin_logger/_search.py` & `lamin_logger-0.7.2/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/pyproject.toml` & `lamin_logger-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/tests/test_inspect.py` & `lamin_logger-0.7.2/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/tests/test_lookup.py` & `lamin_logger-0.7.2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/tests/test_map_synonyms.py` & `lamin_logger-0.7.2/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/tests/test_search.py` & `lamin_logger-0.7.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.1/PKG-INFO` & `lamin_logger-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.1
+Version: 0.7.2
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

