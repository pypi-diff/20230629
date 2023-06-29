# Comparing `tmp/fold_core-0.1.8.tar.gz` & `tmp/fold_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.8.tar", max compression
+gzip compressed data, was "fold_core-0.1.9.tar", max compression
```

## Comparing `fold_core-0.1.8.tar` & `fold_core-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,77 @@
--rw-r--r--   0        0        0     3870 2023-05-03 13:32:34.739451 fold_core-0.1.8/LICENSE
--rw-r--r--   0        0        0    10102 2023-05-03 13:32:34.739451 fold_core-0.1.8/README.md
--rw-r--r--   0        0        0     3957 2023-05-03 13:32:34.771452 fold_core-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      474 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/__init__.py
--rw-r--r--   0        0        0     6351 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/base.py
--rw-r--r--   0        0        0      570 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10456 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/common.py
--rw-r--r--   0        0        0     6402 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2291 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6449 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     3419 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/optimize.py
--rw-r--r--   0        0        0     4850 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3326 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2231 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/select.py
--rw-r--r--   0        0        0     5056 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/__init__.py
--rw-r--r--   0        0        0      975 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1439 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0     1264 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/checks.py
--rw-r--r--   0        0        0    11691 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/common.py
--rw-r--r--   0        0        0     7138 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2886 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/global.py
--rw-r--r--   0        0        0      852 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/inference.py
--rw-r--r--   0        0        0     2993 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/memory.py
--rw-r--r--   0        0        0     6387 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/types.py
--rw-r--r--   0        0        0      756 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/update.py
--rw-r--r--   0        0        0     2243 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/loop/wrap.py
--rw-r--r--   0        0        0      381 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3219 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/random.py
--rw-r--r--   0        0        0     5346 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/splitters.py
--rw-r--r--   0        0        0     1003 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6213 2023-05-03 13:32:34.771452 fold_core-0.1.8/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8689 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4879 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     5479 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6765 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5866 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     8447 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3836 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/scaling.py
--rw-r--r--   0        0        0     5013 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4530 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2216 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/checks.py
--rw-r--r--   0        0        0      638 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/dataframe.py
--rw-r--r--   0        0        0     2240 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/list.py
--rw-r--r--   0        0        0     4783 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-05-03 13:32:34.775452 fold_core-0.1.8/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12990 1970-01-01 00:00:00.000000 fold_core-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-05-24 08:05:30.377016 fold_core-0.1.9/LICENSE
+-rw-r--r--   0        0        0    10102 2023-05-24 08:05:30.377016 fold_core-0.1.9/README.md
+-rw-r--r--   0        0        0     4135 2023-05-24 08:05:30.413017 fold_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/__init__.py
+-rw-r--r--   0        0        0      329 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/base/__init__.py
+-rw-r--r--   0        0        0     8702 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/base/classes.py
+-rw-r--r--   0        0        0     1862 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/base/utils.py
+-rw-r--r--   0        0        0      570 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10879 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     6123 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2292 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6280 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     5419 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/optimize.py
+-rw-r--r--   0        0        0     4880 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3335 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     3183 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4976 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/composites/target.py
+-rw-r--r--   0        0        0     5428 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/__init__.py
+-rw-r--r--   0        0        0      541 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/base.py
+-rw-r--r--   0        0        0       56 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/filters/__init__.py
+-rw-r--r--   0        0        0      240 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/filters/everynth.py
+-rw-r--r--   0        0        0      177 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/filters/no.py
+-rw-r--r--   0        0        0       47 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/labeling/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/events/labeling/fixed.py
+-rw-r--r--   0        0        0      426 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1134 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     1519 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backend/pathos.py
+-rw-r--r--   0        0        0     2577 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1489 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     1546 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backend/thread.py
+-rw-r--r--   0        0        0     2938 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0     1386 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/checks.py
+-rw-r--r--   0        0        0    13411 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/common.py
+-rw-r--r--   0        0        0    10281 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2870 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/global.py
+-rw-r--r--   0        0        0      935 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/inference.py
+-rw-r--r--   0        0        0     4188 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/memory.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/process/__init__.py
+-rw-r--r--   0        0        0     2228 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/process/process_inner_loop.py
+-rw-r--r--   0        0        0     3704 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/process/process_minibatch.py
+-rw-r--r--   0        0        0     5888 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1870 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/types.py
+-rw-r--r--   0        0        0      948 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/updateing.py
+-rw-r--r--   0        0        0     1737 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/utils.py
+-rw-r--r--   0        0        0     2043 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/loop/wrap.py
+-rw-r--r--   0        0        0      381 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     4246 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/base.py
+-rw-r--r--   0        0        0     1918 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     5073 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2697 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/random.py
+-rw-r--r--   0        0        0     5326 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/py.typed
+-rw-r--r--   0        0        0     8172 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/splitters.py
+-rw-r--r--   0        0        0     1003 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6927 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8709 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     5146 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     9387 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      862 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6722 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     6262 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     9445 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3820 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/scaling.py
+-rw-r--r--   0        0        0     6377 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      965 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4402 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/transformations/window.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/__init__.py
+-rw-r--r--   0        0        0     3229 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     1561 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/dataframe.py
+-rw-r--r--   0        0        0     1872 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0      455 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/enums.py
+-rw-r--r--   0        0        0      255 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/forward.py
+-rw-r--r--   0        0        0      194 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/functional.py
+-rw-r--r--   0        0        0     2764 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/list.py
+-rw-r--r--   0        0        0     4958 2023-05-24 08:05:30.413017 fold_core-0.1.9/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     2002 2023-05-24 08:05:30.417017 fold_core-0.1.9/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    12903 1970-01-01 00:00:00.000000 fold_core-0.1.9/PKG-INFO
```

### Comparing `fold_core-0.1.8/LICENSE` & `fold_core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.8/README.md` & `fold_core-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.8/pyproject.toml` & `fold_core-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.8"
+version = "0.1.9"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -30,36 +30,40 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 pandas = ">=1.2"
 numpy = ">=1.16"
 scikit-learn = ">=0.22"
 tqdm = ">=4.0"
 iteration_utilities = ">=0.11"
+typing_extensions = ">=4.4.0"
 
 black = {version = "~=22.12.0", optional = true}
 flake8 = {version = "~=4.0.1", optional = true}
 isort = {version = "~=5.10.1", optional = true}
 pre-commit = {version = "~=2.20.0", optional = true}
 pytest = {version = "~=7.1.2", optional = true}
 pytest-cov = {version = ">=4.0", optional = true}
 imbalanced-learn = {version = ">=0.7.0", optional = true}
 holidays = {version = ">=0.10", optional = true}
-krisi = {version = "~=0.0.8", optional = true}
+krisi = {version = "~=1.0.1", optional = true}
 mkdocs = {version = ">=1.2", optional = true}
 mkdocs-material = {version = ">=9.0.0", optional = true}
 mkdocstrings-python = {version = ">=0.9.0", optional = true}
 mkdocs-include-markdown-plugin = {version = ">=4.0", optional = true}
 mkdocs-autorefs = {version = ">=0.4", optional = true}
 mkdocs-jupyter = {version = ">=0.22", optional = true}
 image = {version = ">=1.5.33", optional = true}
 mkdocs-gallery = {version = ">=0.7", optional = true}
 mkdocs-glightbox = {version = "<=0.3.2", optional = true}
 ray = {version = ">=1.4", optional = true}
 fold-models = {version = "~=0.1.2", optional = true}
 fold-wrappers = {version = "~=0.1", optional = true}
+p_tqdm = {version = ">=1.3", optional = true}
+statsmodels = {version = ">=0.12.1", optional = true}
+
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold"
 Issues = "https://github.com/dream-faster/fold/issues"
 Source = "https://github.com/dream-faster/fold"
 
 [tool.poetry.extras]
@@ -70,14 +74,15 @@
   "pre-commit",
 ]
 tests = [
   "pytest",
   "pytest-cov",
   "imbalanced-learn",
   "holidays",
+  "statsmodels",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings-python",
   "mkdocs-include-markdown-plugin",
   "mkdocs-autorefs",
   "mkdocs-jupyter",
@@ -88,16 +93,19 @@
 ray = ["ray"]
 all = [
   "ray",
   "holidays",
   "krisi",
   "fold-core",
   "fold-wrappers",
+  "p_tqdm",
+  "statsmodels",
 ]
 
+
 [tool.hatch.envs.quality]
 dependencies = [
   ".[quality]"
 ]
 detached = true
 
 [tool.hatch.envs.quality.scripts]
@@ -128,15 +136,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.8"
+current_version = "0.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.8/src/fold/composites/__init__.py` & `fold_core-0.1.9/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.8/src/fold/composites/columns.py` & `fold_core-0.1.9/src/fold/composites/columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Callable, List, Optional, Tuple
 
 import pandas as pd
 
-from ..base import Composite, Pipeline, Pipelines, T
+from ..base import Composite, Extras, Pipeline, Pipelines, T, get_concatenated_names
 from ..utils.checks import all_have_probabilities
 from ..utils.list import unique, wrap_in_double_list_if_needed
-from .common import get_concatenated_names
 
 
 class EnsembleEachColumn(Composite):
     """
     Train a pipeline for each column in the data, then ensemble their results.
 
     Parameters
@@ -27,60 +26,65 @@
     --------
         >>> from fold.loop import train_backtest
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import EnsembleEachColumn
         >>> from sklearn.ensemble import RandomForestRegressor
         >>> from fold.utils.tests import generate_sine_wave_data
         >>> X, y  = generate_sine_wave_data()
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = EnsembleEachColumn(RandomForestRegressor())
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
     """
 
     properties = Composite.Properties()
     pipelines_already_cloned = False
 
-    def __init__(self, pipeline: Pipeline) -> None:
+    def __init__(self, pipeline: Pipeline, name: Optional[str] = None) -> None:
         self.pipelines: Pipelines = wrap_in_double_list_if_needed(pipeline)
-        self.name = "PerColumnEnsemble-" + get_concatenated_names(self.pipelines)
+        self.name = name or "PerColumnEnsemble-" + get_concatenated_names(
+            self.pipelines
+        )
 
     @classmethod
     def from_cloned_instance(
-        cls, pipeline: Pipeline, pipelines_already_cloned: bool
+        cls, pipeline: Pipeline, pipelines_already_cloned: bool, name: Optional[str]
     ) -> EnsembleEachColumn:
         instance = cls(pipeline=pipeline)
         instance.pipelines_already_cloned = pipelines_already_cloned
+        instance.name = name
         return instance
 
     def before_fit(self, X: pd.DataFrame) -> None:
         if not self.pipelines_already_cloned:
             self.pipelines = [deepcopy(self.pipelines) for _ in X.columns]
             self.pipelines_already_cloned = True
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, pd.Series]:
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
         X = X.iloc[:, index].to_frame()
-        return X, y
+        return X, y, extras
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         return postprocess_results(results, self.name)
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipelines
 
-    def clone(self, clone_child_transformations: Callable) -> EnsembleEachColumn:
+    def clone(self, clone_children: Callable) -> EnsembleEachColumn:
         clone = EnsembleEachColumn.from_cloned_instance(
-            pipeline=clone_child_transformations(self.pipelines),
+            pipeline=clone_children(self.pipelines),
             pipelines_already_cloned=self.pipelines_already_cloned,
+            name=self.name,
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
 
 
 class TransformEachColumn(Composite):
     """
     Apply a single pipeline to each column, separately.
 
@@ -101,32 +105,34 @@
         >>> X.head()
                                sine  sine_plus_1
         2021-12-31 07:20:00  0.0000       1.0000
         2021-12-31 07:21:00  0.0126       1.0126
         2021-12-31 07:22:00  0.0251       1.0251
         2021-12-31 07:23:00  0.0377       1.0377
         2021-12-31 07:24:00  0.0502       1.0502
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = TransformEachColumn(lambda x: x + 1.0)
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
         >>> preds.head()
                                sine  sine_plus_1
         2021-12-31 15:40:00  1.0000       2.0000
         2021-12-31 15:41:00  1.0126       2.0126
         2021-12-31 15:42:00  1.0251       2.0251
         2021-12-31 15:43:00  1.0377       2.0377
         2021-12-31 15:44:00  1.0502       2.0502
     """
 
     properties = Composite.Properties()
     pipeline_already_cloned = False
 
-    def __init__(self, pipeline: Pipeline) -> None:
+    def __init__(self, pipeline: Pipeline, name: Optional[str] = None) -> None:
         self.pipeline = wrap_in_double_list_if_needed(pipeline)
-        self.name = "PerColumnTransform-" + get_concatenated_names(self.pipeline)
+        self.name = name or "PerColumnTransform-" + get_concatenated_names(
+            self.pipeline
+        )
 
     @classmethod
     def from_cloned_instance(
         cls, pipeline: Pipeline, pipeline_already_cloned: bool
     ) -> TransformEachColumn:
         instance = cls(pipeline=pipeline)
         instance.pipeline_already_cloned = pipeline_already_cloned
@@ -134,32 +140,33 @@
 
     def before_fit(self, X: pd.DataFrame) -> None:
         if not self.pipeline_already_cloned:
             self.pipeline = [deepcopy(self.pipeline) for _ in X.columns]
             self.pipeline_already_cloned = True
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, T]:
-        return X.iloc[:, index].to_frame(), y
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
+        return (X.iloc[:, index].to_frame(), y, extras)
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         return pd.concat(results, axis="columns")
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipeline
 
-    def clone(self, clone_child_transformations: Callable) -> TransformEachColumn:
+    def clone(self, clone_children: Callable) -> TransformEachColumn:
         clone = TransformEachColumn.from_cloned_instance(
-            pipeline=clone_child_transformations(self.pipeline),
+            pipeline=clone_children(self.pipeline),
             pipeline_already_cloned=self.pipeline_already_cloned,
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
 
 
 class SkipNA(Composite):
     """
     Skips rows with NaN values in the input data.
     In the output, rows with NaNs are returned as is, all other rows transformed.
@@ -180,49 +187,56 @@
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import ModelResiduals
         >>> from sklearn.ensemble import RandomForestClassifier
         >>> from imblearn.under_sampling import RandomUnderSampler
         >>> from fold.utils.tests import generate_zeros_and_ones
         >>> X, y  = generate_zeros_and_ones()
         >>> X[1:100] = np.nan
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = SkipNA(
         ...     pipeline=RandomForestClassifier(),
         ... )
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
     """
 
     properties = Composite.Properties()
+    original_index: Optional[pd.Index] = None
 
-    def __init__(self, pipeline: Pipeline) -> None:
+    def __init__(self, pipeline: Pipeline, name: Optional[str] = None) -> None:
         self.pipeline = wrap_in_double_list_if_needed(pipeline)
-        self.name = "SkipNA-" + get_concatenated_names(self.pipeline)
+        self.name = name or "SkipNA-" + get_concatenated_names(self.pipeline)
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, T]:
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
         self.original_index = X.index.copy()
         self.isna = X.isna().any(axis=1)
-        return X[~self.isna], y[~self.isna] if y is not None else None
+        return (
+            X[~self.isna],
+            y[~self.isna] if y is not None else None,
+            extras.loc(~self.isna),
+        )
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         results = [result.reindex(self.original_index) for result in results]
         return pd.concat(results, axis="columns")
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipeline
 
-    def clone(self, clone_child_transformations: Callable) -> SkipNA:
+    def clone(self, clone_children: Callable) -> SkipNA:
         clone = SkipNA(
-            pipeline=clone_child_transformations(self.pipeline),
+            pipeline=clone_children(self.pipeline),
         )
         clone.properties = self.properties
+        clone.original_index = self.original_index
+        clone.name = self.name
         return clone
 
 
 def postprocess_results(
     results: List[pd.DataFrame],
     name: str,
 ) -> pd.DataFrame:
```

### Comparing `fold_core-0.1.8/src/fold/composites/concat.py` & `fold_core-0.1.9/src/fold/composites/concat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from enum import Enum
 from typing import Callable, List, Optional, Union
 
 import pandas as pd
 
-from ..base import Composite, Pipelines, Transformations
+from ..base import Composite, Pipelines, Transformations, get_concatenated_names
 from ..transformations.columns import SelectColumns
 from ..transformations.dev import Identity
+from ..utils.enums import ParsableEnum
 from ..utils.list import (
     flatten,
     has_intersection,
     keep_only_duplicates,
     wrap_in_double_list_if_needed,
     wrap_in_list,
 )
-from .common import get_concatenated_names
 
 
-class ResolutionStrategy(Enum):
+class ResolutionStrategy(ParsableEnum):
     """
     Parameters
     ----------
     first : str
         Only keep the first (leftmost) duplicate column(s).
     last : str
         Only keep the last (rightmost) duplicate column(s).
@@ -33,24 +32,14 @@
         Keep both duplicate columns.
     """
 
     first = "first"
     last = "last"
     both = "both"
 
-    @staticmethod
-    def from_str(value: Union[str, ResolutionStrategy]) -> ResolutionStrategy:
-        if isinstance(value, ResolutionStrategy):
-            return value
-        for strategy in ResolutionStrategy:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown ResolutionStrategy: {value}")
-
 
 class Concat(Composite):
     """
     Concatenates the results of multiple pipelines.
 
     Parameters
     ----------
@@ -63,15 +52,15 @@
     Examples
     --------
         >>> from fold.loop import train_backtest
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import Concat
         >>> from fold.utils.tests import generate_sine_wave_data
         >>> X, y  = generate_sine_wave_data()
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = Concat([
         ...     lambda X: X.assign(sine_plus_1=X["sine"] + 1),
         ...     lambda X: X.assign(sine_plus_2=X["sine"] + 2),
         ... ])
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
         >>> preds.head()
                              sine_plus_1  sine_plus_2    sine
@@ -85,18 +74,19 @@
     ResolutionStrategy = ResolutionStrategy
     properties = Composite.Properties()
 
     def __init__(
         self,
         pipelines: Pipelines,
         if_duplicate_keep: Union[ResolutionStrategy, str] = ResolutionStrategy.first,
+        name: Optional[str] = None,
     ) -> None:
         self.pipelines = pipelines
         self.if_duplicate_keep = ResolutionStrategy.from_str(if_duplicate_keep)
-        self.name = "Concat-" + get_concatenated_names(pipelines)
+        self.name = name or "Concat-" + get_concatenated_names(pipelines)
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         columns = flatten([result.columns.to_list() for result in results])
         duplicates = keep_only_duplicates(columns)
         if len(duplicates) == 0:
@@ -118,23 +108,24 @@
             else:
                 raise ValueError(
                     f"ResolutionStrategy is not valid: {self.if_duplicate_keep}"
                 )
         else:
             return pd.concat(results, axis="columns")
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipelines
 
-    def clone(self, clone_child_transformations: Callable) -> Concat:
+    def clone(self, clone_children: Callable) -> Concat:
         clone = Concat(
-            pipelines=clone_child_transformations(self.pipelines),
+            pipelines=clone_children(self.pipelines),
             if_duplicate_keep=self.if_duplicate_keep,
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
 
 
 class Pipeline(Composite):
     """
     An optional wrappers that is equivalent to using a single array for the transformations.
     It executes the transformations sequentially, in the order they are provided.
@@ -145,41 +136,42 @@
     pipeline : Pipeline
         A list of transformations or models to be applied to the data.
 
     """
 
     properties = Composite.Properties(primary_only_single_pipeline=True)
 
-    def __init__(
-        self,
-        pipeline: "Pipeline",
-    ) -> None:
+    def __init__(self, pipeline: Pipeline, name: Optional[str] = None) -> None:
         self.pipeline = wrap_in_double_list_if_needed(pipeline)
-        self.name = "Pipeline-" + get_concatenated_names(pipeline)
+        self.name = name or "Pipeline-" + get_concatenated_names(pipeline)
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         return results[0]
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipeline
 
-    def clone(self, clone_child_transformations: Callable) -> Pipeline:
-        clone = Pipeline(pipeline=clone_child_transformations(self.pipeline))
+    def clone(self, clone_children: Callable) -> Pipeline:
+        clone = Pipeline(pipeline=clone_children(self.pipeline))
         clone.properties = self.properties
+        clone.name = self.name
         return clone
 
 
 def TransformColumn(
-    columns: Union[List[str], str], pipeline: Transformations
+    columns: Union[List[str], str],
+    pipeline: Transformations,
+    name: Optional[str] = None,
 ) -> Composite:
     """
     Transforms a single or multiple columns using the given pipeline.
     """
     return Concat(
         [
             [SelectColumns(columns)] + wrap_in_list(pipeline),
             Identity(),
         ],
         if_duplicate_keep=ResolutionStrategy.first,
+        name=name,
     )
```

### Comparing `fold_core-0.1.8/src/fold/composites/ensemble.py` & `fold_core-0.1.9/src/fold/composites/ensemble.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 from __future__ import annotations
 
 from typing import Callable, List, Optional
 
 import pandas as pd
 
-from ..base import Composite, Pipelines
+from ..base import Composite, Pipelines, get_concatenated_names
 from .columns import postprocess_results
-from .common import get_concatenated_names
 
 
 class Ensemble(Composite):
     """
     Ensemble (average) the results of multiple pipelines.
 
     Parameters
@@ -26,15 +25,15 @@
     --------
         >>> from fold.loop import train_backtest
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import Ensemble
         >>> from fold.models import DummyRegressor
         >>> from fold.utils.tests import generate_sine_wave_data
         >>> X, y  = generate_sine_wave_data()
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = Ensemble([
         ...     DummyRegressor(0.1),
         ...     DummyRegressor(0.9),
         ... ])
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
         >>> preds.squeeze().head()
         2021-12-31 15:40:00    0.5
@@ -43,25 +42,26 @@
         2021-12-31 15:43:00    0.5
         2021-12-31 15:44:00    0.5
         Freq: T, Name: predictions_Ensemble-DummyRegressor-DummyRegressor, dtype: float64
     """
 
     properties = Composite.Properties()
 
-    def __init__(self, pipelines: Pipelines) -> None:
+    def __init__(self, pipelines: Pipelines, name: Optional[str] = None) -> None:
         self.pipelines = pipelines
-        self.name = "Ensemble-" + get_concatenated_names(pipelines)
+        self.name = name or "Ensemble-" + get_concatenated_names(pipelines)
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         return postprocess_results(results, self.name)
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipelines
 
-    def clone(self, clone_child_transformations: Callable) -> Ensemble:
+    def clone(self, clone_children: Callable) -> Ensemble:
         clone = Ensemble(
-            pipelines=clone_child_transformations(self.pipelines),
+            pipelines=clone_children(self.pipelines),
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
```

### Comparing `fold_core-0.1.8/src/fold/composites/metalabeling.py` & `fold_core-0.1.9/src/fold/composites/metalabeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from fold.composites.common import get_concatenated_names
-from fold.utils.checks import get_prediction_column
-from fold.utils.list import wrap_in_double_list_if_needed
-
-from ..base import Composite, Pipeline, Pipelines, T
+from ..base import Composite, Pipeline, Pipelines, T, get_concatenated_names
+from ..utils.checks import get_prediction_column
+from ..utils.list import wrap_in_double_list_if_needed
 
 
 class MetaLabeling(Composite):
     """
     MetaLabeling takes a primary pipeline and a meta pipeline.
     The primary pipeline is used to predict the target variable.
     The meta pipeline is used to predict whether the primary model's prediction's are correct (a binary classification problem).
@@ -76,22 +74,25 @@
 
     def __init__(
         self,
         primary: Pipeline,
         meta: Pipeline,
         positive_class: Union[int, float],
         primary_output_included: bool = False,
+        name: Optional[str] = None,
     ) -> None:
         self.primary = wrap_in_double_list_if_needed(primary)
         self.meta = wrap_in_double_list_if_needed(meta)
         self.positive_class = (
             int(positive_class) if isinstance(positive_class, float) else positive_class
         )
         self.primary_output_included = primary_output_included
-        self.name = "MetaLabeling-" + get_concatenated_names(self.primary + self.meta)
+        self.name = name or "MetaLabeling-" + get_concatenated_names(
+            self.primary + self.meta
+        )
 
     def preprocess_secondary(
         self,
         X: pd.DataFrame,
         y: T,
         results_primary: List[pd.DataFrame],
         index: int,
@@ -102,19 +103,14 @@
             if self.primary_output_included
             else X
         )
         predictions = get_prediction_column(results_primary[0])
         y = y.astype(int) == predictions.astype(int)
         return X, y
 
-    def postprocess_result_primary(
-        self, results: List[pd.DataFrame], y: Optional[pd.Series]
-    ) -> pd.DataFrame:
-        raise NotImplementedError
-
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
         in_sample: bool,
     ) -> pd.DataFrame:
@@ -144,30 +140,31 @@
         dc = {
             col: f"probabilities_{self.name}_" + col.split("_")[-1]
             for col in meta_probabilities.columns
         }
         meta_probabilities = meta_probabilities.rename(columns=dc)
         return pd.concat([result, meta_probabilities], axis="columns")
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.primary
 
-    def get_child_transformations_secondary(
+    def get_children_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.meta
 
-    def clone(self, clone_child_transformations: Callable) -> MetaLabeling:
+    def clone(self, clone_children: Callable) -> MetaLabeling:
         clone = MetaLabeling(
-            primary=clone_child_transformations(self.primary),
-            meta=clone_child_transformations(self.meta),
+            primary=clone_children(self.primary),
+            meta=clone_children(self.meta),
             positive_class=self.positive_class,
             primary_output_included=self.primary_output_included,
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
 
 
 def get_int_class(input: str) -> int:
     if input.endswith(".0"):
         return int(float(input[:-2]))
     elif input == "True":
```

### Comparing `fold_core-0.1.8/src/fold/composites/residual.py` & `fold_core-0.1.9/src/fold/composites/residual.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple
 
 import pandas as pd
 
-from fold.composites.common import get_concatenated_names
-from fold.utils.checks import get_prediction_column
-from fold.utils.list import wrap_in_double_list_if_needed
-
-from ..base import Composite, Pipeline, Pipelines, T
+from ..base import Composite, Extras, Pipeline, Pipelines, T, get_concatenated_names
+from ..utils.checks import get_prediction_column
+from ..utils.list import wrap_in_double_list_if_needed
 
 
 class ModelResiduals(Composite):
     """
     This is a composite that combines two pipelines:
     * The primary pipeline is used to predict the target variable.
     * The meta pipeline is used to predict the primary pipeline's residual (or, error).
@@ -45,15 +43,15 @@
         >>> from fold.loop import train_backtest
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import ModelResiduals
         >>> from sklearn.ensemble import RandomForestRegressor
         >>> from sklearn.linear_model import LinearRegression
         >>> from fold.utils.tests import generate_sine_wave_data
         >>> X, y  = generate_sine_wave_data()
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = ModelResiduals(
         ...     primary=LinearRegression(),
         ...     meta=RandomForestRegressor(),
         ... )
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
     References
@@ -70,24 +68,27 @@
     )
 
     def __init__(
         self,
         primary: Pipeline,
         meta: Pipeline,
         primary_output_included: bool = False,
+        name: Optional[str] = None,
     ) -> None:
         self.primary = wrap_in_double_list_if_needed(primary)
         self.meta = wrap_in_double_list_if_needed(meta)
         self.primary_output_included = primary_output_included
-        self.name = "Hybrid-" + get_concatenated_names(self.primary + self.meta)
+        self.name = name or "ModelResidual-" + get_concatenated_names(
+            self.primary + self.meta
+        )
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, T]:
-        return X, y
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
+        return X, y, extras
 
     def preprocess_secondary(
         self,
         X: pd.DataFrame,
         y: T,
         results_primary: List[pd.DataFrame],
         index: int,
@@ -119,23 +120,24 @@
 
         return (
             (primary_predictions + residual_predictions)
             .rename(f"predictions_{self.name}")
             .to_frame()
         )
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.primary
 
-    def get_child_transformations_secondary(
+    def get_children_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.meta
 
-    def clone(self, clone_child_transformations: Callable) -> ModelResiduals:
+    def clone(self, clone_children: Callable) -> ModelResiduals:
         clone = ModelResiduals(
-            primary=clone_child_transformations(self.primary),
-            meta=clone_child_transformations(self.meta),
+            primary=clone_children(self.primary),
+            meta=clone_children(self.meta),
             primary_output_included=self.primary_output_included,
         )
+        clone.name = self.name
         clone.properties = self.properties
         return clone
```

### Comparing `fold_core-0.1.8/src/fold/composites/sample.py` & `fold_core-0.1.9/src/fold/composites/sample.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 
 from __future__ import annotations
 
 from typing import Any, Callable, List, Optional, Tuple
 
 import pandas as pd
 
-from fold.composites.common import get_concatenated_names
-from fold.utils.list import wrap_in_double_list_if_needed
-
-from ..base import Composite, Pipeline, Pipelines, T
+from ..base import Composite, Extras, Pipeline, Pipelines, T, get_concatenated_names
+from ..utils.list import wrap_in_double_list_if_needed
 
 
 class Sample(Composite):
     """
     Sample data with an imbalanced-learn sampler instance during training.
     No sampling is done during inference or backtesting.
 
@@ -34,15 +32,15 @@
         >>> from fold.loop import train_backtest
         >>> from fold.splitters import SlidingWindowSplitter
         >>> from fold.composites import ModelResiduals
         >>> from sklearn.ensemble import RandomForestClassifier
         >>> from imblearn.under_sampling import RandomUnderSampler
         >>> from fold.utils.tests import generate_zeros_and_ones_skewed
         >>> X, y  = generate_zeros_and_ones_skewed()
-        >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+        >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
         >>> pipeline = Sample(
         ...     sampler=RandomUnderSampler(),
         ...     pipeline=RandomForestClassifier(),
         ... )
         >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
 
@@ -53,44 +51,46 @@
 
     properties = Composite.Properties(
         primary_requires_predictions=False,
         primary_only_single_pipeline=True,
     )
 
     def __init__(
-        self,
-        sampler: Any,
-        pipeline: Pipeline,
+        self, sampler: Any, pipeline: Pipeline, name: Optional[str] = None
     ) -> None:
         self.sampler = sampler
+
         self.pipeline = wrap_in_double_list_if_needed(pipeline)
-        self.name = f"Sample-{sampler.__class__.__name__}-{get_concatenated_names(self.pipeline)}"
+        self.name = (
+            name
+            or f"Sample-{sampler.__class__.__name__}-{get_concatenated_names(self.pipeline)}"
+        )
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, T]:
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
         if fit:
             X_resampled, y_resampled = self.sampler.fit_resample(X, y)
             X_resampled.columns = X.columns
-            X_resampled.index = X.index[: len(X_resampled)]
             if y is not None:
                 y_resampled.name = y.name
-                y_resampled.index = y.index[: len(y_resampled)]
-            return X_resampled, y_resampled
+            extras_resampled = extras.iloc(self.sampler.sample_indices_)
+            return X_resampled, y_resampled, extras_resampled
         else:
-            return X, y
+            return X, y, extras
 
     def postprocess_result_primary(
         self, results: List[pd.DataFrame], y: Optional[pd.Series]
     ) -> pd.DataFrame:
         return results[0]
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.pipeline
 
-    def clone(self, clone_child_transformations: Callable) -> Sample:
+    def clone(self, clone_children: Callable) -> Sample:
         clone = Sample(
             sampler=self.sampler,
-            pipeline=clone_child_transformations(self.pipeline),
+            pipeline=clone_children(self.pipeline),
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
```

### Comparing `fold_core-0.1.8/src/fold/composites/target.py` & `fold_core-0.1.9/src/fold/composites/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Composite, InvertibleTransformation, Pipeline, Pipelines, T
+from ..base import (
+    Composite,
+    Extras,
+    InvertibleTransformation,
+    Pipeline,
+    Pipelines,
+    T,
+    get_concatenated_names,
+)
 from ..utils.checks import get_prediction_column, get_prediction_column_name
 from ..utils.dataframe import to_series
 from ..utils.list import wrap_in_double_list_if_needed
-from .common import get_concatenated_names
 
 
 class TransformTarget(Composite):
     """
     Transforms the target within the context of the wrapped Pipeline.
     `wrapped_pipeline` will be applied to the input data, where the target (`y`) is already transformed.
     `y_pipeline` will be applied to the target column.
@@ -40,15 +47,15 @@
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.composites import ModelResiduals
     >>> from sklearn.linear_model import LinearRegression
     >>> from fold.transformations import Difference
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = TransformTarget(
     ...     wrapped_pipeline=LinearRegression(),
     ...     y_pipeline=Difference(),
     ... )
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
     ```
@@ -60,38 +67,35 @@
     )
 
     def __init__(
         self,
         wrapped_pipeline: Pipeline,
         y_pipeline: Union[List[InvertibleTransformation], InvertibleTransformation],
         invert_wrapped_output: bool = True,
+        name: Optional[str] = None,
     ) -> None:
         self.wrapped_pipeline = wrap_in_double_list_if_needed(wrapped_pipeline)
         self.y_pipeline = wrap_in_double_list_if_needed(y_pipeline)
-        self.name = "TransformTarget-" + get_concatenated_names(
+        self.invert_wrapped_output = invert_wrapped_output
+        self.name = name or "TransformTarget-" + get_concatenated_names(
             self.wrapped_pipeline + self.y_pipeline
         )
-        self.invert_wrapped_output = invert_wrapped_output
 
     def preprocess_primary(
-        self, X: pd.DataFrame, index: int, y: T, fit: bool
-    ) -> Tuple[pd.DataFrame, T]:
+        self, X: pd.DataFrame, index: int, y: T, extras: Extras, fit: bool
+    ) -> Tuple[pd.DataFrame, T, Extras]:
         # TransformTarget's primary transformation transforms `y`, not `X`.
         if y is None:
             return (
                 pd.DataFrame(),
                 None,
+                extras,
             )  # at inference time, `y` will be None, and we don't need to use primary transformations at all, so we return a dummy DataFrame.
         else:
-            return y.to_frame(), None
-
-    def postprocess_result_primary(
-        self, results: List[pd.DataFrame], y: Optional[pd.Series]
-    ) -> pd.DataFrame:
-        raise NotImplementedError
+            return y.to_frame(), None, extras
 
     def preprocess_secondary(
         self,
         X: pd.DataFrame,
         y: T,
         results_primary: List[pd.DataFrame],
         index: int,
@@ -111,23 +115,24 @@
         predictions = get_prediction_column(secondary_results[0])
         for transformation in reversed(self.y_pipeline[0]):
             predictions = transformation.inverse_transform(predictions, in_sample)
         results = secondary_results[0]
         results[get_prediction_column_name(results)] = to_series(predictions)
         return results
 
-    def get_child_transformations_primary(self) -> Pipelines:
+    def get_children_primary(self) -> Pipelines:
         return self.y_pipeline
 
-    def get_child_transformations_secondary(
+    def get_children_secondary(
         self,
     ) -> Optional[Pipelines]:
         return self.wrapped_pipeline
 
-    def clone(self, clone_child_transformations: Callable) -> TransformTarget:
+    def clone(self, clone_children: Callable) -> TransformTarget:
         clone = TransformTarget(
-            wrapped_pipeline=clone_child_transformations(self.wrapped_pipeline),
-            y_pipeline=clone_child_transformations(self.y_pipeline),
+            wrapped_pipeline=clone_children(self.wrapped_pipeline),
+            y_pipeline=clone_children(self.y_pipeline),
             invert_wrapped_output=self.invert_wrapped_output,
         )
         clone.properties = self.properties
+        clone.name = self.name
         return clone
```

### Comparing `fold_core-0.1.8/src/fold/loop/backend/__init__.py` & `fold_core-0.1.9/src/fold/loop/backend/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
     process_child_transformations: Callable
     train_transformations: Callable
 
 
 def get_backend_dependent_functions(backend: Backend) -> BackendDependentFunctions:
     if backend == Backend.ray:
         from .ray import process_child_transformations, train_transformations
-
-        return BackendDependentFunctions(
-            process_child_transformations,
-            train_transformations,
-        )
     elif backend == Backend.no:
         from .sequential import process_child_transformations, train_transformations
+    elif backend == Backend.pathos:
+        from .pathos import process_child_transformations, train_transformations
+    elif backend == Backend.thread:
+        from .thread import process_child_transformations, train_transformations
+    else:
+        raise ValueError(f"Backend {backend} not supported.")
 
-        return BackendDependentFunctions(
-            process_child_transformations,
-            train_transformations,
-        )
+    return BackendDependentFunctions(
+        process_child_transformations,
+        train_transformations,
+    )
```

### Comparing `fold_core-0.1.8/src/fold/loop/backend/ray.py` & `fold_core-0.1.9/src/fold/loop/backend/sequential.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from typing import Callable, List, Optional
 
 import pandas as pd
-import ray
+from tqdm.auto import tqdm
 
-from ...base import Composite, Transformations
+from ...base import Artifact, Composite, Transformations, X
 from ...splitters import Fold
 from ..types import Backend, Stage
 
 
 def train_transformations(
     func: Callable,
     transformations: Transformations,
@@ -18,50 +18,40 @@
     y: pd.Series,
     sample_weights: Optional[pd.Series],
     splits: List[Fold],
     never_update: bool,
     backend: Backend,
     silent: bool,
 ):
-    func = ray.remote(func)
-    X = ray.put(X)
-    y = ray.put(y)
-    return ray.get(
-        [
-            func.remote(
-                X, y, sample_weights, transformations, split, never_update, backend
-            )
-            for split in splits
-        ]
-    )
+    return [
+        func(X, y, sample_weights, transformations, split, never_update, backend)
+        for split in tqdm(splits, disable=silent)
+    ]
 
 
 def process_child_transformations(
     func: Callable,
     list_of_child_transformations_with_index: List,
     composite: Composite,
-    X: pd.DataFrame,
+    X: X,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
+    artifacts: Artifact,
     stage: Stage,
     backend: Backend,
     results_primary: Optional[List[pd.DataFrame]],
 ):
-    func = ray.remote(func)
-    X = ray.put(X)
-    y = ray.put(y)
-    return ray.get(
-        [
-            func.remote(
-                composite,
-                index,
-                child_transformation,
-                X,
-                y,
-                sample_weights,
-                stage,
-                backend,
-                results_primary,
-            )
-            for index, child_transformation in list_of_child_transformations_with_index
-        ]
-    )
+    return [
+        func(
+            composite,
+            index,
+            child_transformation,
+            X,
+            y,
+            sample_weights,
+            artifacts,
+            stage,
+            backend,
+            results_primary,
+        )
+        for index, child_transformation in list_of_child_transformations_with_index
+    ]
```

### Comparing `fold_core-0.1.8/src/fold/loop/backend/sequential.py` & `fold_core-0.1.9/src/fold/loop/backend/thread.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from typing import Callable, List, Optional
 
 import pandas as pd
-from tqdm.auto import tqdm
+from tqdm.contrib.concurrent import thread_map
 
-from ...base import Composite, Transformations
+from ...base import Artifact, Composite, Transformations, X
 from ...splitters import Fold
 from ..types import Backend, Stage
 
 
 def train_transformations(
     func: Callable,
     transformations: Transformations,
@@ -18,38 +18,43 @@
     y: pd.Series,
     sample_weights: Optional[pd.Series],
     splits: List[Fold],
     never_update: bool,
     backend: Backend,
     silent: bool,
 ):
-    return [
-        func(X, y, sample_weights, transformations, split, never_update, backend)
-        for split in tqdm(splits, disable=silent)
-    ]
+    return thread_map(
+        lambda split: func(
+            X, y, sample_weights, transformations, split, never_update, backend
+        ),
+        splits,
+        disable=silent,
+    )
 
 
 def process_child_transformations(
     func: Callable,
     list_of_child_transformations_with_index: List,
     composite: Composite,
-    X: pd.DataFrame,
+    X: X,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
+    artifacts: Artifact,
     stage: Stage,
     backend: Backend,
     results_primary: Optional[List[pd.DataFrame]],
 ):
     return [
         func(
             composite,
             index,
             child_transformation,
             X,
             y,
             sample_weights,
+            artifacts,
             stage,
             backend,
             results_primary,
         )
         for index, child_transformation in list_of_child_transformations_with_index
     ]
```

### Comparing `fold_core-0.1.8/src/fold/loop/checks.py` & `fold_core-0.1.9/src/fold/loop/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 
 
 from logging import warn
 from typing import Optional, Tuple
 
 import pandas as pd
 
+from ..base.classes import Extras
 from ..utils.trim import trim_initial_nans
 
 
 def check_types(
     X: Optional[pd.DataFrame], y: pd.Series
 ) -> Tuple[pd.DataFrame, pd.Series]:
     if X is None:
-        X = pd.DataFrame(0, index=y.index, columns=["X_not_available"])
+        X = pd.DataFrame(
+            pd.arrays.SparseArray(0), index=y.index, columns=["X_not_available"]
+        )
     else:
         assert isinstance(X, pd.DataFrame), "X must be a pandas DataFrame."
     assert isinstance(y, pd.Series), "y must be a pandas Series."
 
-    X_trimmed, _ = trim_initial_nans(X, y)
+    X_trimmed, _, _ = trim_initial_nans(X, y, Extras())
     if len(X_trimmed) < len(X):
         warn(
-            f"Detected initial NaNs in X ({ len(X) - len(X_trimmed) } instances), that'll be trimmed internally. Please trim your data before passing it to the model."
+            f"Detected initial NaNs in X ({ len(X) - len(X_trimmed) } instances),"
+            " that'll be trimmed internally. Please trim your data before passing it"
+            " to the model."
         )
     return X, y
 
 
 def check_types_multi_series(data: pd.DataFrame):
     assert isinstance(data, pd.DataFrame), "data must be a pandas DataFrame."
     assert "y" in data.columns, "data must have a column `y`."
```

### Comparing `fold_core-0.1.8/src/fold/loop/encase.py` & `fold_core-0.1.9/src/fold/loop/encase.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 
 import importlib.util
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Union
 
 import pandas as pd
 from sklearn.metrics import mean_squared_error
 
-from ..base import OutOfSamplePredictions, Pipeline, TrainedPipelines
+from ..base import Artifact, OutOfSamplePredictions, Pipeline, TrainedPipelines
 from ..splitters import Splitter
+from ..utils.checks import (
+    all_have_probabilities,
+    get_prediction_column,
+    get_probabilities_columns,
+)
+from ..utils.dataframe import concat_on_index
 from .backtesting import backtest
 from .training import train
-from .types import Backend, TrainMethod
+from .types import Backend, EventDataFrame, TrainMethod
 
 if TYPE_CHECKING:
     from krisi import ScoreCard
 
 
 def backtest_score(
     trained_pipelines: TrainedPipelines,
     X: Optional[pd.DataFrame],
     y: pd.Series,
     splitter: Splitter,
     backend: Union[str, Backend] = Backend.no,
     sample_weights: Optional[pd.Series] = None,
+    events: Optional[EventDataFrame] = None,
     silent: bool = False,
+    return_artifacts: bool = False,
     krisi_args: Optional[Dict[str, Any]] = None,
     evaluation_func: Callable = mean_squared_error,
-) -> Tuple[Union["ScoreCard", Dict[str, float]], OutOfSamplePredictions]:
+) -> Union[
+    Tuple[Union["ScoreCard", Dict[str, float]], OutOfSamplePredictions],
+    Tuple[Union["ScoreCard", Dict[str, float]], OutOfSamplePredictions, Artifact],
+]:
     """
     Run backtest then scoring.
     If [`krisi`](https://github.com/dream-faster/krisi) is installed it will use it to generate a ScoreCard,
     otherwise it will run the `evaluation_func` passed in.
 
     Parameters
     ----------
@@ -43,66 +54,98 @@
         Endogenous Data (Target).
     splitter: Splitter
         Defines how the folds should be constructed.
     backend: str, Backend = Backend.no
         The library/service to use for parallelization / distributed computing, by default `no`.
     sample_weights: Optional[pd.Series] = None
         Weights assigned to each sample/timestamp, that are passed into models that support it, by default None.
+    events: EventDataFrame, optional = None
+        Events that should be passed into the pipeline, by default None.
     silent: bool = False
         Wether the pipeline should print to the console, by default False.
+    return_artifacts: bool = False
+        Whether to return the artifacts of the training process, by default False.
     krisi_args: Optional[Dict[str, Any]] = None
         Arguments that will be passed into `krisi` score function, by default None.
     evaluation_func: Callable = mean_squared_error
         Function to evaluate with if `krisi` is not available, by default `mean_squared_error`.
 
 
     Returns
     -------
     "ScoreCard", Dict[str, float]
         A ScoreCard if `krisi` is available, else the result of the `evaluation_func` in a dict
     OutOfSamplePredictions
         Predictions for all folds, concatenated.
     """
 
-    pred = backtest(
+    pred, artifacts = backtest(
         trained_pipelines,
         X,
         y,
         splitter,
-        backend,
-        sample_weights,
-        silent,
-        mutate=False,
+        backend=backend,
+        sample_weights=sample_weights,
+        events=events,
+        silent=silent,
+        return_artifacts=True,
+    )
+
+    probabilities = (
+        get_probabilities_columns(pred) if all_have_probabilities([pred]) else None
     )
+    pred_point = get_prediction_column(pred)
+
+    if artifacts is not None and "label" in artifacts.columns:
+        y = artifacts["label"].reindex(pred.index).dropna()
+        pred_point = pred_point.dropna()
+        probabilities = probabilities.dropna()
+
+    if len(y) != len(pred_point):
+        if probabilities is not None:
+            probabilities = probabilities[: len(y)]
+        pred_point = pred_point[: len(y)]
 
     if importlib.util.find_spec("krisi") is not None:
         from krisi import score
 
         scorecard = score(
-            y[pred.index],
-            pred.squeeze(),
+            y=y[pred_point.index],
+            predictions=pred_point,
+            probabilities=probabilities,
             **(krisi_args if krisi_args is not None else {}),
         )
     else:
+        pred_point = get_prediction_column(pred)
         scorecard = {
-            "mean_squared_error": evaluation_func(y[pred.index], pred.squeeze())
+            evaluation_func.__class__.__name__: evaluation_func(
+                y[pred_point.index], pred_point.squeeze()
+            )
         }
-    return scorecard, pred
+    if return_artifacts:
+        return scorecard, pred, artifacts
+    else:
+        return scorecard, pred
 
 
 def train_backtest(
     pipeline: Pipeline,
     X: Optional[pd.DataFrame],
     y: pd.Series,
     splitter: Splitter,
     backend: Union[Backend, str] = Backend.no,
     sample_weights: Optional[pd.Series] = None,
+    events: Optional[EventDataFrame] = None,
     train_method: Union[TrainMethod, str] = TrainMethod.parallel,
     silent: bool = False,
-) -> Tuple[OutOfSamplePredictions, TrainedPipelines]:
+    return_artifacts: bool = False,
+) -> Union[
+    Tuple[OutOfSamplePredictions, TrainedPipelines],
+    Tuple[OutOfSamplePredictions, TrainedPipelines, Artifact],
+]:
     """
     Run train and backtest.
 
     Parameters
     ----------
     pipeline: Pipeline
         The pipeline to be fitted.
@@ -112,58 +155,90 @@
         Endogenous Data (Target).
     splitter: Splitter
         Defines how the folds should be constructed.
     backend: str, Backend = Backend.no
         The library/service to use for parallelization / distributed computing, by default `no`.
     sample_weights: Optional[pd.Series] = None
         Weights assigned to each sample/timestamp, that are passed into models that support it, by default None.
+    events: EventDataFrame, optional = None
+        Events that should be passed into the pipeline, by default None.
     train_method: TrainMethod, str = TrainMethod.parallel
         The training methodology, by default `parallel`.
     silent: bool = False
         Wether the pipeline should print to the console, by default False.
+    return_artifacts: bool = False
+        Whether to return the artifacts of the process, by default False.
 
     Returns
     -------
     OutOfSamplePredictions
         Predictions for all folds, concatenated.
     TrainedPipelines
         The fitted pipelines, for all folds.
     """
-    trained_pipelines = train(
-        pipeline, X, y, splitter, sample_weights, train_method, backend, silent
+    trained_pipelines, train_artifacts = train(
+        pipeline,
+        X,
+        y,
+        splitter,
+        sample_weights,
+        events=events,
+        train_method=train_method,
+        backend=backend,
+        silent=silent,
+        return_artifacts=True,
     )
 
-    pred = backtest(
+    pred, backtest_artifacts = backtest(
         trained_pipelines,
         X,
         y,
         splitter,
-        backend,
-        sample_weights,
-        silent,
+        backend=backend,
+        sample_weights=sample_weights,
+        events=events,
+        silent=silent,
+        return_artifacts=True,
     )
 
-    return pred, trained_pipelines
+    if return_artifacts:
+        return (
+            pred,
+            trained_pipelines,
+            concat_on_index([train_artifacts, backtest_artifacts]),
+        )
+    else:
+        return pred, trained_pipelines
 
 
 def train_evaluate(
     pipeline: Pipeline,
     X: Optional[pd.DataFrame],
     y: pd.Series,
     splitter: Splitter,
     backend: Backend = Backend.no,
     sample_weights: Optional[pd.Series] = None,
+    events: Optional[EventDataFrame] = None,
     train_method: Union[TrainMethod, str] = TrainMethod.parallel,
     silent: bool = False,
+    return_artifacts: bool = False,
     krisi_args: Optional[Dict[str, Any]] = None,
     evaluation_func: Callable = mean_squared_error,
-) -> Tuple[
-    Union["ScoreCard", Dict[str, float]],
-    OutOfSamplePredictions,
-    TrainedPipelines,
+) -> Union[
+    Tuple[
+        Union["ScoreCard", Dict[str, float]],
+        OutOfSamplePredictions,
+        TrainedPipelines,
+    ],
+    Tuple[
+        Union["ScoreCard", Dict[str, float]],
+        OutOfSamplePredictions,
+        TrainedPipelines,
+        Artifact,
+    ],
 ]:
     """
     Run train, backtest then run scoring.
     If [`krisi`](https://github.com/dream-faster/krisi) is installed it will use it to generate a ScoreCard,
     otherwise it will run the `evaluation_func` passed in.
 
     Parameters
@@ -176,14 +251,16 @@
         Endogenous Data (Target).
     splitter: Splitter
         Defines how the folds should be constructed.
     backend: str, Backend = Backend.no
         The library/service to use for parallelization / distributed computing, by default `no`.
     sample_weights: pd.Series, optional = None
         Weights assigned to each sample/timestamp, that are passed into models that support it, by default None.
+    events: EventDataFrame, optional = None
+        Events that should be passed into the pipeline, by default None.
     train_method: TrainMethod, str = TrainMethod.parallel
         The training methodology, by default `parallel`.
     silent: bool = False
         Wether the pipeline should print to the console, by default False.
     krisi_args: Dict[str, Any], optional = None
         Arguments that will be passed into `krisi` score function, by default None.
     evaluation_func: Callable = mean_squared_error
@@ -194,24 +271,43 @@
     "ScoreCard", Dict[str, float]
         A ScoreCard if `krisi` is available, else the result of the `evaluation_func` in a dict
     OutOfSamplePredictions
         Predictions for all folds, concatenated.
     TrainedPipelines
         The fitted pipelines, for all folds.
     """
-    trained_pipelines = train(
-        pipeline, X, y, splitter, sample_weights, train_method, backend, silent
+    trained_pipelines, train_artifacts = train(
+        pipeline,
+        X,
+        y,
+        splitter,
+        sample_weights,
+        events=events,
+        train_method=train_method,
+        backend=backend,
+        silent=silent,
+        return_artifacts=True,
     )
 
-    scorecard, pred = backtest_score(
+    scorecard, pred, backtest_artifacts = backtest_score(
         trained_pipelines,
         X,
         y,
         splitter,
-        backend,
-        sample_weights,
-        silent,
-        krisi_args,
-        evaluation_func,
+        backend=backend,
+        sample_weights=sample_weights,
+        events=events,
+        silent=silent,
+        return_artifacts=True,
+        krisi_args=krisi_args,
+        evaluation_func=evaluation_func,
     )
 
-    return scorecard, pred, trained_pipelines
+    if return_artifacts:
+        return (
+            scorecard,
+            pred,
+            trained_pipelines,
+            concat_on_index([train_artifacts, backtest_artifacts]),
+        )
+    else:
+        return scorecard, pred, trained_pipelines
```

### Comparing `fold_core-0.1.8/src/fold/loop/global.py` & `fold_core-0.1.9/src/fold/loop/global.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pandas as pd
 
 from ..base import Pipeline, TrainedPipelines
 from ..splitters import Splitter
 from ..utils.list import wrap_in_list
 from .checks import check_types_multi_series
-from .training import _process_pipeline_window
+from .training import _train_on_window
 from .types import Backend
 from .wrap import wrap_transformation_if_needed
 
 
 def _train_global(
     pipeline: Pipeline,
     data: pd.DataFrame,
@@ -44,15 +44,15 @@
     processed_pipeline = pipeline
 
     # TODO:
     #  - initial_fit probably needs to be done on the concatenated data, as some Transformations we can't update, and Optimizers need to select the correct configuration on not just a single time series, but on the whole.
     #  - global models are only possible with tabular models, we should throw an exception if one is passed in that we don't support
     for split in splits:
         for X, y, sample_weights in __get_X_y_from_data(data):
-            processed_id, processed_pipeline = _process_pipeline_window(
+            processed_id, processed_pipeline = _train_on_window(
                 processed_pipeline, X, y, sample_weights, split, True, backend, silent
             )
         processed_idx.append(processed_id)
         processed_pipelines.append(processed_pipeline)
 
     return [
         pd.Series(
```

### Comparing `fold_core-0.1.8/src/fold/loop/inference.py` & `fold_core-0.1.9/src/fold/loop/inference.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import pandas as pd
 
-from ..base import DeployablePipeline, OutOfSamplePredictions
+from ..base import DeployablePipeline, Extras, OutOfSamplePredictions
 from .common import recursively_transform
 from .types import Backend, Stage
 
 
 def infer(
     pipeline: DeployablePipeline,
     X: Optional[pd.DataFrame],
@@ -18,11 +18,17 @@
     If X is None it will predict one step ahead.
     """
     if X is None:
         X = pd.DataFrame([0], columns=[0])
     else:
         assert type(X) is pd.DataFrame, "X must be a pandas DataFrame."
 
-    results = recursively_transform(
-        X, None, None, pipeline, stage=Stage.infer, backend=Backend.no
+    _, results, _ = recursively_transform(
+        X,
+        None,
+        Extras(),
+        pd.DataFrame(),
+        pipeline,
+        stage=Stage.infer,
+        backend=Backend.no,
     )
     return results
```

### Comparing `fold_core-0.1.8/src/fold/loop/update.py` & `fold_core-0.1.9/src/fold/loop/updateing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from typing import Optional
 
 import pandas as pd
 
-from ..base import DeployablePipeline
+from ..base import DeployablePipeline, EventDataFrame, Extras
 from .checks import check_types
 from .common import deepcopy_pipelines, recursively_transform
 from .types import Backend, Stage
 
 
 def update(
     pipeline: DeployablePipeline,
     X: Optional[pd.DataFrame],
     y: pd.Series,
     sample_weights: Optional[pd.Series] = None,
+    events: Optional[EventDataFrame] = None,
 ) -> DeployablePipeline:
     """
     Update a set of Transformations with new data.
     Returns a new set of Transformations, does not mutate the original.
     """
     X, y = check_types(X, y)
+    extras = Extras(events=events, sample_weights=sample_weights)
 
     transformations = deepcopy_pipelines(pipeline)
     _ = recursively_transform(
-        X, y, sample_weights, transformations, stage=Stage.update, backend=Backend.no
+        X,
+        y,
+        extras,
+        pd.DataFrame(),
+        transformations,
+        stage=Stage.update,
+        backend=Backend.no,
     )
     return transformations
```

### Comparing `fold_core-0.1.8/src/fold/loop/wrap.py` & `fold_core-0.1.9/src/fold/loop/wrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 
 
 from importlib.util import find_spec
 from typing import Callable, List
 
 from sklearn.base import ClassifierMixin, RegressorMixin, TransformerMixin
 from sklearn.feature_selection import SelectorMixin
-from sklearn.pipeline import Pipeline as SKLearnPipeline
 
-from fold.models.sklearn import (
-    WrapSKLearnClassifier,
-    WrapSKLearnPipeline,
-    WrapSKLearnRegressor,
-)
+from fold.models.sklearn import WrapSKLearnClassifier, WrapSKLearnRegressor
 from fold.transformations.sklearn import (
     WrapSKLearnFeatureSelector,
     WrapSKLearnTransformation,
 )
 
 from ..base import Composite, Optimizer, Pipeline, Transformation
 from ..transformations.function import WrapFunction
@@ -33,16 +28,14 @@
         return WrapSKLearnClassifier.from_model(transformation)
     elif isinstance(transformation, Callable):
         return WrapFunction(transformation, None)
     elif isinstance(transformation, SelectorMixin):
         return WrapSKLearnFeatureSelector.from_model(transformation)
     elif isinstance(transformation, TransformerMixin):
         return WrapSKLearnTransformation.from_model(transformation)
-    elif isinstance(transformation, SKLearnPipeline):
-        return WrapSKLearnPipeline(transformation)
     elif isinstance(transformation, Composite):
         return transformation.clone(wrap_transformation_if_needed)
     elif isinstance(transformation, Optimizer):
         return transformation.clone(wrap_transformation_if_needed)
     elif isinstance(transformation, Transformation):
         return transformation
     elif find_spec("fold_wrappers") is not None:
```

### Comparing `fold_core-0.1.8/src/fold/models/base.py` & `fold_core-0.1.9/src/fold/models/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from abc import abstractmethod
-from typing import Union
+from typing import Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-from ..base import Transformation
+from fold.utils.checks import (
+    get_classes_from_probabilies_column_names,
+    get_probabilities_column_names,
+    has_probabilities,
+)
+
+from ..base import Artifact, Transformation
 
 
 class Model(Transformation):
     @abstractmethod
     def predict(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
         """
         Predictions for exclusively out-of-sample data, the model has never seen before.
@@ -21,19 +27,24 @@
     @abstractmethod
     def predict_in_sample(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
         """
         Predictions for in-sample, already seen data.
         """
         raise NotImplementedError
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if in_sample:
-            return postpostprocess_prediction(self.predict_in_sample(X), self.name)
+            return (
+                postpostprocess_output(self.predict_in_sample(X), self.name),
+                None,
+            )
         else:
-            return postpostprocess_prediction(self.predict(X), self.name)
+            return postpostprocess_output(self.predict(X), self.name), None
 
 
 class TimeSeriesModel(Transformation):
     """
     Convenience class, for models that have access to past `y` values.
     """
 
@@ -53,45 +64,65 @@
         self, X: pd.DataFrame, past_y: pd.Series
     ) -> Union[pd.Series, pd.DataFrame]:
         """
         Predictions for in-sample, already seen data.
         """
         raise NotImplementedError
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if in_sample:
-            return postpostprocess_prediction(
-                self.predict_in_sample(X, self._state.memory_y.shift(1)), self.name
+            return (
+                postpostprocess_output(
+                    self.predict_in_sample(X, self._state.memory_y.shift(1)), self.name
+                ),
+                None,
             )
         else:
-            return postpostprocess_prediction(
-                self.predict(
-                    X[-(self.properties.memory_size + 1) : None],
-                    pd.Series(
-                        np.concatenate(
-                            [
-                                np.ones((1,)) * np.nan,
-                                self._state.memory_y[
-                                    -self.properties.memory_size : None
-                                ],
-                            ]
+            return (
+                postpostprocess_output(
+                    self.predict(
+                        X[-(self.properties.memory_size + 1) : None],
+                        pd.Series(
+                            np.concatenate(
+                                [
+                                    np.ones((1,)) * np.nan,
+                                    self._state.memory_y[
+                                        -self.properties.memory_size : None
+                                    ],
+                                ]
+                            ),
+                            index=X.index,
                         ),
-                        index=X.index,
                     ),
+                    self.name,
                 ),
-                self.name,
+                None,
             )
 
 
-def postpostprocess_prediction(
+def postpostprocess_output(
     dataframe_or_series: Union[pd.DataFrame, pd.Series], name: str
 ) -> pd.DataFrame:
     if isinstance(dataframe_or_series, pd.Series):
         return dataframe_or_series.rename(f"predictions_{name}").to_frame()
     elif isinstance(dataframe_or_series, pd.DataFrame):
         if len(dataframe_or_series.columns) == 1:
             dataframe_or_series.columns = [f"predictions_{name}"]
-        return dataframe_or_series
+            return dataframe_or_series
+        elif has_probabilities(dataframe_or_series):
+            # Sort probabilities columns if necessary
+            prob_columns = get_probabilities_column_names(dataframe_or_series)
+            prob_columns_sorted = sorted(
+                get_classes_from_probabilies_column_names(prob_columns)
+            )
+            if prob_columns == prob_columns_sorted:
+                return dataframe_or_series
+            else:
+                return dataframe_or_series.sort_index(axis="columns")
+        else:
+            return dataframe_or_series
     else:
         raise ValueError(
             f"Expected dataframe or series, got {type(dataframe_or_series)} instead."
         )
```

### Comparing `fold_core-0.1.8/src/fold/models/baseline.py` & `fold_core-0.1.9/src/fold/models/baseline.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.models import Naive
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = Naive()
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> pd.concat([preds, y[preds.index]], axis=1).head()
                          predictions_Naive    sine
     2021-12-31 15:40:00            -0.0000  0.0126
     2021-12-31 15:41:00             0.0126  0.0251
     2021-12-31 15:42:00             0.0251  0.0377
```

### Comparing `fold_core-0.1.8/src/fold/models/dummy.py` & `fold_core-0.1.9/src/fold/models/dummy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import List, Union
+from typing import List, Optional, Union
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Transformation, Tunable, fit_noop
 from .base import Model
 
 
-class DummyClassifier(Model):
+class DummyClassifier(Model, Tunable):
     """
     A model that predicts a predefined class with predefined probabilities.
 
     Parameters
     ----------
     predicted_value : float, int
         The class to predict.
@@ -26,15 +26,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.models import DummyClassifier
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = DummyClassifier(1, [0, 1], [0.5, 0.5])
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                          predictions_DummyClassifier  ...  probabilities_DummyClassifier_1
     2021-12-31 15:40:00                            1  ...                              0.5
     2021-12-31 15:41:00                            1  ...                              0.5
     2021-12-31 15:42:00                            1  ...                              0.5
@@ -43,25 +43,29 @@
     <BLANKLINE>
     [5 rows x 3 columns]
 
     ```
     """
 
     properties = Transformation.Properties(requires_X=False)
-    name = "DummyClassifier"
+    name = ""
 
     def __init__(
         self,
         predicted_value: Union[float, int],
         all_classes: List[int],
         predicted_probabilities: List[float],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         self.predicted_value = predicted_value
         self.all_classes = all_classes
         self.predicted_probabilities = predicted_probabilities
+        self.params_to_try = params_to_try
+        self.name = name or "DummyClassifier"
 
     def predict(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
         predictions = pd.Series(
             [self.predicted_value] * len(X),
             index=X.index,
             name="predictions_DummyClassifier",
         )
@@ -78,16 +82,24 @@
 
         return pd.concat([predictions] + probabilities, axis="columns")
 
     predict_in_sample = predict
     fit = fit_noop
     update = fit
 
+    def get_params(self) -> dict:
+        return dict(
+            predicted_value=self.predicted_value,
+            all_classes=self.all_classes,
+            predicted_probabilities=self.predicted_probabilities,
+            name=self.name,
+        )
+
 
-class DummyRegressor(Model):
+class DummyRegressor(Model, Tunable):
     """
     A model that predicts a predefined value.
 
     Parameters
     ----------
     predicted_value : float
         The value to predict.
@@ -96,15 +108,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.models import DummyRegressor
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = DummyRegressor(0.1)
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                          predictions_DummyRegressor
     2021-12-31 15:40:00                         0.1
     2021-12-31 15:41:00                         0.1
     2021-12-31 15:42:00                         0.1
@@ -113,19 +125,29 @@
 
     ```
     """
 
     properties = Transformation.Properties(requires_X=False)
     name = "DummyRegressor"
 
-    def __init__(self, predicted_value: float) -> None:
+    def __init__(
+        self,
+        predicted_value: float,
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
+    ) -> None:
         self.predicted_value = predicted_value
+        self.params_to_try = params_to_try
+        self.name = name or self.name
 
     def predict(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
         return pd.Series(
             [self.predicted_value] * len(X),
             index=X.index,
         )
 
     predict_in_sample = predict
     fit = fit_noop
     update = fit
+
+    def get_params(self) -> dict:
+        return dict(predicted_value=self.predicted_value, name=self.name)
```

### Comparing `fold_core-0.1.8/src/fold/models/random.py` & `fold_core-0.1.9/src/fold/models/random.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from random import choices
-from typing import List, Union
+from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from ..base import Transformation, fit_noop
 from .base import Model
 
@@ -28,44 +28,58 @@
     ```pycon
     >>> import numpy as np
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.models import RandomClassifier
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> np.random.seed(42)
-    >>> pipeline = RandomClassifier([0,1], 0.5)
+    >>> pipeline = RandomClassifier([0,1], [0.5, 0.5])
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
 
     ```
     """
 
     properties = Transformation.Properties(requires_X=False)
     name = "RandomClassifier"
 
-    def __init__(self, all_classes: List[int], probability_mean: float = 0.5) -> None:
+    def __init__(
+        self, all_classes: List[int], probability_mean: Optional[List[float]] = None
+    ) -> None:
         self.all_classes = all_classes
-        self.probability_mean = probability_mean
+        if probability_mean is not None:
+            assert len(probability_mean) == len(all_classes)
+        self.probability_mean = (
+            [1 / len(all_classes) for _ in range(len(all_classes))]
+            if probability_mean is None
+            else probability_mean
+        )
 
     fit = fit_noop
 
     def predict(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
         predictions = pd.Series(
             choices(population=self.all_classes, k=len(X)),
             index=X.index,
             name="predictions_RandomClassifier",
         )
-        probabilities = [
-            pd.Series(
-                np.random.normal(self.probability_mean, 0.1, len(X)).clip(0, 1),
-                index=X.index,
-                name=f"probabilities_RandomClassifier_{associated_class}",
-            )
-            for associated_class in self.all_classes
-        ]
+        probabilities = pd.concat(
+            [
+                pd.Series(
+                    np.random.normal(prob_mean, 0.1, len(X)).clip(0, 1),
+                    index=X.index,
+                    name=f"probabilities_RandomClassifier_{associated_class}",
+                )
+                for associated_class, prob_mean in zip(
+                    self.all_classes, self.probability_mean
+                )
+            ],
+            axis="columns",
+        )
+        probabilities = probabilities.div(probabilities.sum(axis=1), axis=0)
 
-        return pd.concat([predictions] + probabilities, axis="columns")
+        return pd.concat([predictions, probabilities], axis="columns")
 
     predict_in_sample = predict
 
     update = fit
```

### Comparing `fold_core-0.1.8/src/fold/splitters.py` & `fold_core-0.1.9/src/fold/splitters.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,59 +39,65 @@
     Creates folds with a sliding window.
     The folds are created by moving the train and test windows forward by a fixed step size.
     See [the documentation](https://dream-faster.github.io/fold/concepts/splitters/) for more details.
 
     Parameters
     ----------
 
-    initial_train_window : int, float
-        The initial training window size. If a float, it is interpreted as a fraction of the total length of the data.
+    train_window : int, float
+        The training window size. If a float, it is interpreted as a fraction of the total length of the data.
     step : int, float
         The step size of the sliding window. If a float, it is interpreted as a fraction of the total length of the data.
     embargo : int, optional
         The gap between the train and the test window, by default 0.
     start : int, optional
         The start index of the first fold, by default 0.
     end : int, optional
         The end index of the last fold, by default None.
+    merge_threshold: float, optional, default 0.01
+        The percentage threshold for merging the last fold with the previous one if it is too small.
     """
 
     def __init__(
         self,
-        initial_train_window: Union[
+        train_window: Union[
             int, float
         ],  # this is what you don't out of sample get predictions for
         step: Union[int, float],
         embargo: int = 0,
         start: int = 0,
         end: Optional[int] = None,
+        merge_threshold: float = 0.01,
     ) -> None:
-        self.window_size = initial_train_window
+        self.window_size = train_window
         self.step = step
         self.embargo = embargo
         self.start = start
         self.end = end
+        self.merge_threshold = merge_threshold
 
     def splits(self, length: int) -> List[Fold]:
+        merge_threshold = int(length * self.merge_threshold)
         end = self.end if self.end is not None else length
         window_size = translate_float_if_needed(self.window_size, length)
         step = translate_float_if_needed(self.step, length)
-        return [
+        folds = [
             Fold(
                 order=order,
                 model_index=index,
                 train_window_start=index - window_size,
                 train_window_end=index - self.embargo,
                 update_window_start=0,  # SlidingWindowSplitter is incompatible with sequential updates
                 update_window_end=0,
                 test_window_start=index,
                 test_window_end=min(end, index + step),
             )
             for order, index in enumerate(range(self.start + window_size, end, step))
         ]
+        return merge_last_fold_if_too_small(folds, merge_threshold)
 
 
 class ExpandingWindowSplitter(Splitter):
     """
     Creates folds with an expanding window.
     The folds are created by moving the end of the train and test windows forward by a fixed step size,
     while keeping the training window's start fixed.
@@ -106,51 +112,57 @@
         The step size of the sliding window. If a float, it is interpreted as a fraction of the total length of the data.
     embargo : int, optional
         The gap between the train and the test window, by default 0.
     start : int, optional
         The start index of the first fold, by default 0.
     end : int, optional
         The end index of the last fold, by default None.
+    merge_threshold: float, optional, default 0.01
+        The percentage threshold for merging the last fold with the previous one if it is too small.
     """
 
     def __init__(
         self,
         initial_train_window: Union[
             int, float
         ],  # this is what you don't out of sample get predictions for
         step: Union[int, float],
         embargo: int = 0,
         start: int = 0,
         end: Optional[int] = None,
+        merge_threshold: float = 0.01,
     ) -> None:
         self.window_size = initial_train_window
         self.step = step
         self.embargo = embargo
         self.start = start
         self.end = end
+        self.merge_threshold = merge_threshold
 
     def splits(self, length: int) -> List[Fold]:
+        merge_threshold = int(length * self.merge_threshold)
         end = self.end if self.end is not None else length
         window_size = translate_float_if_needed(self.window_size, length)
         step = translate_float_if_needed(self.step, length)
 
-        return [
+        folds = [
             Fold(
                 order=order,
                 model_index=index,
                 train_window_start=self.start,
                 train_window_end=index - self.embargo,
                 update_window_start=index
                 - step,  # the length of the update window is the step size, see documentation
                 update_window_end=index - self.embargo,
                 test_window_start=index,
                 test_window_end=min(end, index + step),
             )
             for order, index in enumerate(range(self.start + window_size, end, step))
         ]
+        return merge_last_fold_if_too_small(folds, merge_threshold)
 
 
 class SingleWindowSplitter(Splitter):
     """
     Creates a single fold with a fixed train and test window.
     See [the documentation](https://dream-faster.github.io/fold/concepts/splitters/) for more details.
 
@@ -183,7 +195,26 @@
                 train_window_end=window_size - self.embargo,
                 update_window_start=0,
                 update_window_end=0,  # SingleWindowSplitter is incompatible with sequantial updating
                 test_window_start=window_size,
                 test_window_end=length,
             ),
         ]
+
+
+def merge_last_fold_if_too_small(splits: List[Fold], threshold: int) -> List[Fold]:
+    last_fold = splits[-1]
+    if last_fold.test_window_end - last_fold.test_window_start > threshold:
+        return splits
+
+    previous_fold = splits[-2]
+    merged_fold = Fold(
+        order=previous_fold.order,
+        model_index=previous_fold.model_index,
+        train_window_start=previous_fold.train_window_start,
+        train_window_end=previous_fold.train_window_end,
+        update_window_start=previous_fold.update_window_start,
+        update_window_end=previous_fold.update_window_end,
+        test_window_start=previous_fold.test_window_start,
+        test_window_end=last_fold.test_window_end,
+    )
+    return splits[:-2] + [merged_fold]
```

### Comparing `fold_core-0.1.8/src/fold/transformations/__init__.py` & `fold_core-0.1.9/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.8/src/fold/transformations/columns.py` & `fold_core-0.1.9/src/fold/transformations/columns.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from typing import List, Union
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Transformation, Tunable, fit_noop
+from ..base import Artifact, Transformation, Tunable, fit_noop
 from ..utils.checks import check_get_columns
 from ..utils.list import wrap_in_list
 
 
 class SelectColumns(Transformation, Tunable):
     """
     Selects a single or multiple columns, drops the rest.
@@ -23,26 +23,34 @@
         The column or columns to select (dropping the rest).
 
 
     """
 
     properties = Transformation.Properties(requires_X=True)
 
-    def __init__(self, columns: Union[List[str], str]) -> None:
+    def __init__(
+        self,
+        columns: Union[List[str], str],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
+    ) -> None:
         self.columns: List[str] = wrap_in_list(columns)
-        self.name = f"SelectColumns-{columns}"
+        self.params_to_try = params_to_try
+        self.name = name or f"SelectColumns-{columns}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X[self.columns]
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return X[self.columns], None
 
     fit = fit_noop
     update = fit
 
     def get_params(self) -> dict:
-        return {"columns": self.columns}
+        return dict(columns=self.columns, name=self.name)
 
 
 class DropColumns(Transformation, Tunable):
     """
     Drops a single or multiple columns.
 
     Parameters
@@ -51,26 +59,34 @@
     columns : List[str], str
         The column or columns to drop.
 
     """
 
     properties = Transformation.Properties(requires_X=True)
 
-    def __init__(self, columns: Union[List[str], str]) -> None:
+    def __init__(
+        self,
+        columns: Union[List[str], str],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
+    ) -> None:
         self.columns = wrap_in_list(columns)
-        self.name = f"DropColumns-{columns}"
+        self.params_to_try = params_to_try
+        self.name = name or f"DropColumns-{columns}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X.drop(columns=check_get_columns(self.columns, X))
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return X.drop(columns=check_get_columns(self.columns, X)), None
 
     fit = fit_noop
     update = fit
 
     def get_params(self) -> dict:
-        return {"columns": self.columns}
+        return {"columns": self.columns, "name": self.name}
 
 
 class RenameColumns(Transformation):
     """
     Renames columns.
 
     Parameters
@@ -84,15 +100,15 @@
 
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import RenameColumns
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = RenameColumns({"sine": "sine_renamed"})
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                          sine_renamed
     2021-12-31 15:40:00       -0.0000
     2021-12-31 15:41:00        0.0126
     2021-12-31 15:42:00        0.0251
@@ -104,16 +120,18 @@
 
     properties = Transformation.Properties(requires_X=True)
 
     def __init__(self, columns_mapper: dict) -> None:
         self.columns_mapper = columns_mapper
         self.name = "RenameColumns"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X.rename(columns=self.columns_mapper)
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return X.rename(columns=self.columns_mapper), None
 
     fit = fit_noop
     update = fit
 
 
 class OnlyPredictions(Transformation):
     """
@@ -124,15 +142,15 @@
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import OnlyProbabilities
     >>> from fold.models.dummy import DummyClassifier
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = [DummyClassifier(1, [0, 1], [0.5, 0.5]), OnlyPredictions()]
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                          predictions_DummyClassifier
     2021-12-31 15:40:00                            1
     2021-12-31 15:41:00                            1
     2021-12-31 15:42:00                            1
@@ -143,17 +161,22 @@
     """
 
     properties = Transformation.Properties(requires_X=True)
 
     def __init__(self) -> None:
         self.name = "OnlyPredictions"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X.drop(
-            columns=[col for col in X.columns if not col.startswith("predictions_")]
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return (
+            X.drop(
+                columns=[col for col in X.columns if not col.startswith("predictions_")]
+            ),
+            None,
         )
 
     fit = fit_noop
     update = fit
 
 
 class OnlyProbabilities(Transformation):
@@ -165,15 +188,15 @@
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import OnlyProbabilities
     >>> from fold.models.dummy import DummyClassifier
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = [DummyClassifier(1, [0, 1], [0.5, 0.5]), OnlyProbabilities()]
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                          probabilities_DummyClassifier_0  probabilities_DummyClassifier_1
     2021-12-31 15:40:00                              0.5                              0.5
     2021-12-31 15:41:00                              0.5                              0.5
     2021-12-31 15:42:00                              0.5                              0.5
@@ -184,14 +207,21 @@
     """
 
     properties = Transformation.Properties(requires_X=True)
 
     def __init__(self) -> None:
         self.name = "OnlyProbabilities"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X.drop(
-            columns=[col for col in X.columns if not col.startswith("probabilities_")]
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return (
+            X.drop(
+                columns=[
+                    col for col in X.columns if not col.startswith("probabilities_")
+                ]
+            ),
+            None,
         )
 
     fit = fit_noop
     update = fit
```

### Comparing `fold_core-0.1.8/src/fold/transformations/date.py` & `fold_core-0.1.9/src/fold/transformations/date.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from enum import Enum
-from typing import Callable, List, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import SingleFunctionTransformation, Transformation, Tunable, fit_noop
+from ..base import (
+    Artifact,
+    SingleFunctionTransformation,
+    Transformation,
+    Tunable,
+    fit_noop,
+)
+from ..utils.enums import ParsableEnum
 from ..utils.list import wrap_in_list
 
 
-class DateTimeFeature(Enum):
+class DateTimeFeature(ParsableEnum):
     second = "second"
     minute = "minute"
     hour = "hour"
     day_of_week = "day_of_week"
     day_of_month = "day_of_month"
     day_of_year = "day_of_year"
     week = "week"
     week_of_year = "week_of_year"
     month = "month"
     quarter = "quarter"
     year = "year"
 
-    @staticmethod
-    def from_str(value: Union[str, DateTimeFeature]) -> DateTimeFeature:
-        if isinstance(value, DateTimeFeature):
-            return value
-        for strategy in DateTimeFeature:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown DateTimeFeature: {value}")
-
 
 class AddDateTimeFeatures(Transformation, Tunable):
     """
     Adds (potentially multiple) date/time features to the input, as additional columns.
     The name of the new column will be the name of the DateTimeFeature passed in.
     Values are returned as integers, so the 59th minute of the hour will be `59`, and year 2022 will be `2022`.
 
@@ -52,38 +48,47 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddDateTimeFeatures
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="min")
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddDateTimeFeatures(["minute"])
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                            sine  minute
     2021-12-31 15:40:00 -0.0000      40
     2021-12-31 15:41:00  0.0126      41
     2021-12-31 15:42:00  0.0251      42
     2021-12-31 15:43:00  0.0377      43
     2021-12-31 15:44:00  0.0502      44
 
     ```
     """
 
     properties = Transformation.Properties(requires_X=False)
-    name = "AddDateTimeFeatures"
 
     def __init__(
         self,
         features: List[Union[DateTimeFeature, str]],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         self.features = [DateTimeFeature(f) for f in wrap_in_list(features)]
-
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+        self.name = (
+            name
+            if name is not None
+            else f"AddDateTimeFeatures-{'-'.join([i.value for i in self.features])}"
+        )
+        self.params_to_try = params_to_try
+
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         X_datetime = pd.DataFrame([], index=X.index)
         for feature in self.features:
             if feature == DateTimeFeature.second:
                 X_datetime[feature.value] = X.index.second
             elif feature == DateTimeFeature.minute:
                 X_datetime[feature.value] = X.index.minute
             elif feature == DateTimeFeature.hour:
@@ -105,36 +110,36 @@
                 X_datetime[feature.value] = X.index.month
             elif feature == DateTimeFeature.quarter:
                 X_datetime[feature.value] = X.index.quarter
             elif feature == DateTimeFeature.year:
                 X_datetime[feature.value] = X.index.year
             else:
                 raise ValueError(f"Unsupported feature: {feature}")
-        return pd.concat([X, X_datetime], axis="columns")
+        return pd.concat([X, X_datetime], axis="columns"), None
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"features": self.features}
+        return {"features": self.features, "name": self.name}
 
 
 class AddSecond(SingleFunctionTransformation):
     """
     Adds "second" features to the input, as an additional column.
 
     Examples
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddSecond
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="S")
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddSecond()
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                            sine  second
     2021-12-31 23:51:40 -0.0000      40
     2021-12-31 23:51:41  0.0126      41
     2021-12-31 23:51:42  0.0251      42
@@ -158,15 +163,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddMinute
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="min")
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddMinute()
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                            sine  minute
     2021-12-31 15:40:00 -0.0000      40
     2021-12-31 15:41:00  0.0126      41
     2021-12-31 15:42:00  0.0251      42
```

### Comparing `fold_core-0.1.8/src/fold/transformations/dev.py` & `fold_core-0.1.9/src/fold/transformations/dev.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from inspect import getfullargspec
-from typing import Callable, Optional
+from typing import Callable, Optional, Tuple
 
 import pandas as pd
 
-from ..base import InvertibleTransformation, Transformation, fit_noop
+from ..base import Artifact, InvertibleTransformation, Transformation, fit_noop
 
 
 class Breakpoint(Transformation):
     """
     A transformation that stops execution at the specified point.
     """
 
@@ -28,39 +28,43 @@
         self.stop_at_transform = stop_at_transform
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         if self.stop_at_fit:
             breakpoint()
 
     def update(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         if self.stop_at_update:
             breakpoint()
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if self.stop_at_transform:
             breakpoint()
-        return X
+        return X, None
 
 
 class Identity(InvertibleTransformation):
     properties = Transformation.Properties(requires_X=False)
     name = "Identity"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return X, None
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return X
 
     fit = fit_noop
     update = fit
 
@@ -88,15 +92,15 @@
         self.inverse_transform_func = inverse_transform_func
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         self.no_of_calls_fit += 1
         argspec = getfullargspec(self.fit_func)
         if len(argspec.args) == 1:
             self.fit_func(X)
         elif len(argspec.args) == 2:
             self.fit_func(X, y)
         elif len(argspec.args) == 3:
@@ -108,15 +112,15 @@
             )
 
     def update(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         self.no_of_calls_update += 1
         if self.update_func is None:
             return
         argspec = getfullargspec(self.update_func)
         if len(argspec.args) == 1:
             self.update_func(X)
         elif len(argspec.args) == 2:
@@ -125,23 +129,25 @@
             self.update_func(X, y, sample_weights)
         else:
             raise ValueError(
                 "update_func must accept between 1 and 3 arguments, "
                 f"but {len(argspec.args)} were given."
             )
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if in_sample:
             self.no_of_calls_transform_insample += 1
         else:
             self.no_of_calls_transform_outofsample += 1
         return_value = self.transform_func(X)
         if return_value is None:
-            return X
-        return return_value
+            return X, None
+        return return_value, None
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         self.no_of_calls_inverse_transform += 1
         if self.inverse_transform_func is not None:
             return self.inverse_transform_func(X)
         return X
 
@@ -155,12 +161,14 @@
     properties = Transformation.Properties(
         requires_X=False,
         mode=Transformation.Properties.Mode.online,
         memory_size=0,
         _internal_supports_minibatch_backtesting=True,
     )
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return self._state.memory_y.to_frame()
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return self._state.memory_y.to_frame(), None
 
     fit = fit_noop
     update = fit
```

### Comparing `fold_core-0.1.8/src/fold/transformations/function.py` & `fold_core-0.1.9/src/fold/transformations/function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import Callable, Optional
+from typing import Callable, Optional, Tuple
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Artifact, Transformation, fit_noop
 
 
 class WrapFunction(Transformation):
     """
     Wraps and arbitrary function that will run at inference.
     """
 
     def __init__(self, func: Callable, past_window_size: Optional[int]) -> None:
         self.func = func
         self.name = func.__name__
         self.properties = Transformation.Properties(
             requires_X=True, memory_size=past_window_size
         )
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return self.func(X)
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return self.func(X), None
 
     fit = fit_noop
     update = fit
```

### Comparing `fold_core-0.1.8/src/fold/transformations/holidays.py` & `fold_core-0.1.9/src/fold/transformations/holidays.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
+from __future__ import annotations
 
 from datetime import date
-from enum import Enum
-from typing import List, Union
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Transformation, Tunable, fit_noop
+from ..base import Artifact, Transformation, Tunable, fit_noop
+from ..utils.enums import ParsableEnum
 from ..utils.list import swap_tuples, wrap_in_list
 
 
-class LabelingMethod(Enum):
+class LabelingMethod(ParsableEnum):
     """
     Parameters
     ----------
     holiday_binary: string
         * Workdays = 0
         * National Holidays = 1
     weekday_weekend_holiday: string
@@ -33,24 +34,14 @@
     """
 
     holiday_binary = "holiday_binary"
     weekday_weekend_holiday = "weekday_weekend_holiday"
     weekday_weekend_uniqueholiday = "weekday_weekend_uniqueholiday"
     weekday_weekend_uniqueholiday_string = "weekday_weekend_uniqueholiday_string"
 
-    @staticmethod
-    def from_str(value: Union[str, "LabelingMethod"]) -> "LabelingMethod":
-        if isinstance(value, LabelingMethod):
-            return value
-        for strategy in LabelingMethod:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown HolidayType: {value}")
-
 
 class AddHolidayFeatures(Transformation, Tunable):
     """
     Adds holiday features for given region(s) as new column(s).
     It uses the pattern "holiday_{country_code}" for naming the columns.
 
 
@@ -69,19 +60,20 @@
 
     properties = Transformation.Properties(requires_X=False)
 
     def __init__(
         self,
         country_codes: Union[List[str], str],
         labeling: Union[str, LabelingMethod] = LabelingMethod.weekday_weekend_holiday,
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         self.country_codes = [
             country_code.upper() for country_code in wrap_in_list(country_codes)
         ]
-        self.name = f"AddHolidayFeatures-{self.country_codes}"
         self.labeling = LabelingMethod.from_str(labeling)
         from holidays import country_holidays, list_supported_countries
 
         all_supported_countries = list_supported_countries()
 
         assert all(
             [
@@ -105,35 +97,39 @@
                         ),
                         start=1,
                     )
                 )
             )
             for country_code in self.country_codes
         ]
+        self.params_to_try = params_to_try
+        self.name = name or f"AddHolidayFeatures-{self.country_codes}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if self.labeling == LabelingMethod.holiday_binary:
             holidays = _get_holidays(
                 X.index, self.country_codes, self.holiday_to_int_maps, encode=True
             )
             holidays[holidays != 0] = 1
 
-            return pd.concat([X, holidays], axis="columns")
+            return pd.concat([X, holidays], axis="columns"), None
         elif self.labeling == LabelingMethod.weekday_weekend_holiday:
             holidays = _get_holidays(
                 X.index, self.country_codes, self.holiday_to_int_maps, encode=True
             )
 
             # All values that are (bigger than 0 or a string) are holidays, but we don't want to differentiate between them
             holidays[holidays != 0] = 2
 
             holidays[holidays == 0] = holidays[holidays == 0].add(
                 _get_weekends(X.index), axis="index"
             )
-            return pd.concat([X, holidays], axis="columns")
+            return pd.concat([X, holidays], axis="columns"), None
         elif (
             self.labeling == LabelingMethod.weekday_weekend_uniqueholiday
             or self.labeling == LabelingMethod.weekday_weekend_uniqueholiday_string
         ):
             holidays = _get_holidays(
                 X.index,
                 self.country_codes,
@@ -141,25 +137,26 @@
                 encode=self.labeling == LabelingMethod.weekday_weekend_uniqueholiday,
             )
 
             weekends = _get_weekends(X.index)
             holidays[holidays == 0] = holidays[holidays == 0].add(
                 weekends, axis="index"
             )
-            return pd.concat([X, holidays], axis="columns")
+            return pd.concat([X, holidays], axis="columns"), None
         else:
             raise ValueError(f"Unknown HolidayType: {self.labeling}")
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
         return {
             "country_codes": self.country_codes,
             "labeling": self.labeling,
+            "name": self.name,
         }
 
 
 def _get_weekends(dates: pd.DatetimeIndex) -> pd.Series:
     return pd.Series((dates.weekday > 4).astype(int), index=dates)
```

### Comparing `fold_core-0.1.8/src/fold/transformations/lags.py` & `fold_core-0.1.9/src/fold/transformations/lags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import List, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
 from fold.utils.checks import is_X_available
 
-from ..base import Transformation, Tunable, fit_noop
+from ..base import Artifact, Transformation, Tunable, fit_noop
 from ..utils.list import flatten, transform_range_to_list, wrap_in_list
 
 
 class AddLagsY(Transformation, Tunable):
     """
     Adds past values of `y`.
 
@@ -24,62 +24,69 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddLagsY
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> _, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddLagsY([1,2,3])
     >>> preds, trained_pipeline = train_backtest(pipeline, None, y, splitter)
     >>> preds.head()
                          y_lag_1  y_lag_2  y_lag_3
     2021-12-31 15:40:00  -0.0000  -0.0126  -0.0251
     2021-12-31 15:41:00   0.0126  -0.0000  -0.0126
     2021-12-31 15:42:00   0.0251   0.0126  -0.0000
     2021-12-31 15:43:00   0.0377   0.0251   0.0126
     2021-12-31 15:44:00   0.0502   0.0377   0.0251
 
     ```
     """
 
-    def __init__(self, lags: Union[List[int], range]) -> None:
+    def __init__(
+        self,
+        lags: Union[List[int], range],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
+    ) -> None:
         if not isinstance(lags, range) and not isinstance(lags, List):
             raise ValueError("lags must be a range or a List")
         self.lags = sorted(transform_range_to_list(lags))
-        self.name = f"AddLagsY-{self.lags}"
         self.properties = Transformation.Properties(
             requires_X=False,
             mode=Transformation.Properties.Mode.online,
             memory_size=max(self.lags),
             _internal_supports_minibatch_backtesting=True,
         )
+        self.params_to_try = params_to_try
+        self.name = name or f"AddLagsY-{self.lags}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         lags = pd.DataFrame([], index=X.index)
 
-        if in_sample:
-            for lag in self.lags:
-                lags[f"y_lag_{lag}"] = self._state.memory_y.shift(lag)[-len(X) :]
-        else:
-            past_y = self._state.memory_y.reindex(X.index)
-            for lag in self.lags:
-                lags[f"y_lag_{lag}"] = past_y.shift(lag)[-len(X) :]
-
+        past_y = (
+            self._state.memory_y if in_sample else self._state.memory_y.reindex(X.index)
+        )
+        lags = pd.concat(
+            [past_y.shift(lag)[-len(X) :].rename(f"y_lag_{lag}") for lag in self.lags],
+            axis="columns",
+        )
         if is_X_available(X):
-            return pd.concat([X, lags], axis="columns")
+            return pd.concat([X, lags], axis="columns"), None
         else:
             # If X is just an DataFrame with zeros, then just return the lags
-            return lags
+            return lags, None
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"lags": self.lags}
+        return {"lags": self.lags, "name": self.name}
 
 
 class AddLagsX(Transformation, Tunable):
     """
     Adds past values of `X` for the desired column(s).
 
     Parameters
@@ -91,15 +98,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddLagsX
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddLagsX([("sine", 1), ("sine", [2,3])])
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                            sine  sine_lag_1  sine_lag_2  sine_lag_3
     2021-12-31 15:40:00 -0.0000     -0.0126     -0.0251     -0.0377
     2021-12-31 15:41:00  0.0126     -0.0000     -0.0126     -0.0251
     2021-12-31 15:42:00  0.0251      0.0126     -0.0000     -0.0126
@@ -108,17 +115,21 @@
 
     ```
     """
 
     ColumnAndLag = Tuple[str, Union[int, List[int]]]
 
     def __init__(
-        self, columns_and_lags: Union[List[ColumnAndLag], ColumnAndLag]
+        self,
+        columns_and_lags: Union[List[ColumnAndLag], ColumnAndLag],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         self.columns_and_lags = wrap_in_list(columns_and_lags)
+        self.params_to_try = params_to_try
 
         def check_and_transform_if_needed(
             column_and_lag: AddLagsX.ColumnAndLag,
         ) -> AddLagsX.ColumnAndLag:
             column, lags = column_and_lag
             if (
                 not isinstance(lags, int)
@@ -130,31 +141,33 @@
                 transform_range_to_list([lags] if isinstance(lags, int) else lags)
             )
             return column, lags
 
         self.columns_and_lags = list(
             map(check_and_transform_if_needed, self.columns_and_lags)
         )
-        self.name = f"AddLagsX-{self.columns_and_lags}"
         self.properties = Transformation.Properties(
             requires_X=True,
             memory_size=max(flatten([l for _, l in self.columns_and_lags])),
         )
+        self.name = name or f"AddLagsX-{self.columns_and_lags}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         X_lagged = pd.DataFrame([], index=X.index)
         for column, lags in self.columns_and_lags:
             for lag in lags:
                 if column == "all":
                     X_lagged = pd.concat(
                         [X_lagged, X.shift(lag)[-len(X) :].add_suffix(f"_lag_{lag}")],
                         axis="columns",
                     )
                 else:
                     X_lagged[f"{column}_lag_{lag}"] = X[column].shift(lag)[-len(X) :]
-        return pd.concat([X, X_lagged], axis="columns")
+        return pd.concat([X, X_lagged], axis="columns"), None
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"columns_and_lags": self.columns_and_lags}
+        return {"columns_and_lags": self.columns_and_lags, "name": self.name}
```

### Comparing `fold_core-0.1.8/src/fold/transformations/math.py` & `fold_core-0.1.9/src/fold/transformations/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import Dict, Optional, Union
+from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-from fold.base import InvertibleTransformation, Tunable, fit_noop
+from ..base import Artifact, InvertibleTransformation, Tunable, fit_noop
 
 
 class TakeLog(InvertibleTransformation, Tunable):
     """
     Takes the logarithm of the data.
 
     Parameters
@@ -23,15 +23,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import TakeLog
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="min")
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = TakeLog()
     >>> X["sine"].head()
     2021-12-31 07:20:00    0.0000
     2021-12-31 07:21:00    0.0126
     2021-12-31 07:22:00    0.0251
     2021-12-31 07:23:00    0.0377
     2021-12-31 07:24:00    0.0502
@@ -44,32 +44,46 @@
     2021-12-31 15:43:00   -3.278095
     2021-12-31 15:44:00   -2.991740
     Freq: T, Name: sine, dtype: float64
 
     ```
     """
 
-    name = "TakeLog"
     properties = InvertibleTransformation.Properties(requires_X=True)
 
     def __init__(
         self,
         base: Union[int, str] = "e",
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         if base not in ["e", np.e, "10", 10, "2", 2]:
             raise ValueError("base should be either 'e', np.e, '10', 10, '2', 2.")
         self.base = base
+        self.params_to_try = params_to_try
+        self.name = name or f"TakeLog-{self.base}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if self.base == "e" or self.base == np.e:
-            return pd.DataFrame(np.log(X.values), columns=X.columns, index=X.index)
+            return (
+                pd.DataFrame(np.log(X.values), columns=X.columns, index=X.index),
+                None,
+            )
         elif self.base == "10" or self.base == 10:
-            return pd.DataFrame(np.log10(X.values), columns=X.columns, index=X.index)
+            return (
+                pd.DataFrame(np.log10(X.values), columns=X.columns, index=X.index),
+                None,
+            )
         elif self.base == "2" or self.base == 2:
-            return pd.DataFrame(np.log2(X.values), columns=X.columns, index=X.index)
+            return (
+                pd.DataFrame(np.log2(X.values), columns=X.columns, index=X.index),
+                None,
+            )
         else:
             raise ValueError(f"Invalid base: {self.base}")
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         if self.base == "e" or self.base == np.e:
             return pd.Series(np.exp(X.values), index=X.index)
         elif self.base == "10" or self.base == 10:
@@ -79,15 +93,15 @@
         else:
             raise ValueError(f"Invalid base: {self.base}")
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"base": self.base}
+        return {"base": self.base, "name": self.name}
 
 
 class AddConstant(InvertibleTransformation, Tunable):
 
     """
     Adds a constant to the data.
 
@@ -100,15 +114,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddConstant
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="min")
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddConstant(1.0)
     >>> X["sine"].head()
     2021-12-31 07:20:00    0.0000
     2021-12-31 07:21:00    0.0126
     2021-12-31 07:22:00    0.0251
     2021-12-31 07:23:00    0.0377
     2021-12-31 07:24:00    0.0502
@@ -121,52 +135,60 @@
     2021-12-31 15:43:00    1.0377
     2021-12-31 15:44:00    1.0502
     Freq: T, Name: sine, dtype: float64
 
     ```
     """
 
-    name = "AddConstant"
     properties = InvertibleTransformation.Properties(requires_X=True)
 
     def __init__(
         self,
         constant: Union[int, float, Dict[str, Union[float, int]]],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         if not isinstance(constant, (int, float, dict)):
             raise ValueError(
                 "constant can be only integer, float or a dictionary of integers or"
                 " floats"
             )
 
         self.constant = constant
+        self.params_to_try = params_to_try
+        self.name = name or "AddConstant"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         if isinstance(self.constant, dict):
             transformed_columns = X[list(self.constant.keys())] + pd.Series(
                 self.constant
             )
-            return pd.concat(
-                [X.drop(columns=self.constant.keys()), transformed_columns],
-                axis="columns",
+            return (
+                pd.concat(
+                    [X.drop(columns=self.constant.keys()), transformed_columns],
+                    axis="columns",
+                ),
+                None,
             )
         else:
-            return X + self.constant
+            return X + self.constant, None
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         constant = self.constant
         if constant is dict:
             constant = next(iter(constant.values()))
         return X - constant
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"constant": self.constant}
+        return {"constant": self.constant, "name": self.name}
 
 
 class TurnPositive(InvertibleTransformation):
     """
     Adds a constant to the data, varying by column, so that all values are positive.
     It identifies the constant during training, and applies it during inference (and backtesting).
     Therefore there's no guarantee that the data will be positive during inference (and backtesting).
@@ -178,15 +200,15 @@
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import TurnPositive
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data(freq="min")
     >>> X, y  = X - 1, y - 1
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = TurnPositive()
     >>> X["sine"].head()
     2021-12-31 07:20:00   -1.0000
     2021-12-31 07:21:00   -0.9874
     2021-12-31 07:22:00   -0.9749
     2021-12-31 07:23:00   -0.9623
     2021-12-31 07:24:00   -0.9498
@@ -207,47 +229,60 @@
     properties = InvertibleTransformation.Properties(requires_X=True)
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         min_values = X.min(axis=0)
         self.constant = dict(min_values[min_values <= 0].abs() + 1)
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         transformed_columns = X[list(self.constant.keys())] + pd.Series(self.constant)
-        return pd.concat(
-            [X.drop(columns=self.constant.keys()), transformed_columns],
-            axis="columns",
+        return (
+            pd.concat(
+                [X.drop(columns=self.constant.keys()), transformed_columns],
+                axis="columns",
+            ),
+            None,
         )
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return X - next(iter(self.constant.values()))
 
     update = fit_noop
 
 
 class MultiplyBy(InvertibleTransformation, Tunable):
     """
     Multiplies the data by a constant.
     """
 
-    name = "MultiplyBy"
     properties = InvertibleTransformation.Properties(requires_X=True)
     constant: float
 
-    def __init__(self, constant: float) -> None:
+    def __init__(
+        self,
+        constant: float,
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
+    ) -> None:
         self.constant = constant
+        self.params_to_try = params_to_try
+        self.name = name or f"MultiplyBy-{constant}"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return X * self.constant
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return X * self.constant, None
 
     def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return X / self.constant
 
     fit = fit_noop
     update = fit_noop
 
     def get_params(self) -> dict:
-        return {"constant": self.constant}
+        return {"constant": self.constant, "name": self.name}
```

### Comparing `fold_core-0.1.8/src/fold/transformations/scaling.py` & `fold_core-0.1.9/src/fold/transformations/scaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import StandardScaler
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = StandardScaler()
     >>> X["sine"].head()
     2021-12-31 07:20:00    0.0000
     2021-12-31 07:21:00    0.0126
     2021-12-31 07:22:00    0.0251
     2021-12-31 07:23:00    0.0377
     2021-12-31 07:24:00    0.0502
@@ -75,15 +75,15 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import MinMaxScaler
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = MinMaxScaler()
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> X["sine"].loc[preds.index].head()
     2021-12-31 15:40:00   -0.0000
     2021-12-31 15:41:00    0.0126
     2021-12-31 15:42:00    0.0251
     2021-12-31 15:43:00    0.0377
```

### Comparing `fold_core-0.1.8/src/fold/transformations/update.py` & `fold_core-0.1.9/src/fold/transformations/update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import Optional
+from typing import Optional, Tuple
 
 import pandas as pd
 
-from ..base import Transformation, fit_noop
+from ..base import Artifact, Transformation, fit_noop
 
 
 class DontUpdate(Transformation):
     properties = Transformation.Properties(requires_X=False)
 
     def __init__(self, transformation: Transformation) -> None:
         self.transformation = transformation
         self.name = f"DontUpdate-{transformation.name}"
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
-    ) -> None:
+    ) -> Optional[Artifact]:
         self.transformation.fit(X, y, sample_weights)
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
-        return self.transformation.transform(X, in_sample)
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
+        return self.transformation.transform(X, in_sample), None
 
     update = fit_noop
```

### Comparing `fold_core-0.1.8/src/fold/transformations/window.py` & `fold_core-0.1.9/src/fold/transformations/window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from enum import Enum
-from typing import Callable, List, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Transformation, Tunable, fit_noop
+from ..base import Artifact, Transformation, Tunable, fit_noop
+from ..utils.enums import ParsableEnum
 from ..utils.list import wrap_in_list
 
 
-class PredefinedFunction(Enum):
+class PredefinedFunction(ParsableEnum):
     mean = "mean"
     sum = "sum"
     median = "median"
     std = "std"
     var = "var"
     kurt = "kurt"
     min = "min"
     max = "max"
     corr = "corr"
     cov = "cov"
     skew = "skew"
     sem = "sem"
 
-    @staticmethod
-    def from_str(value: Union[str, PredefinedFunction]) -> PredefinedFunction:
-        if isinstance(value, PredefinedFunction):
-            return value
-        for strategy in PredefinedFunction:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown PredefinedFunction: {value}")
-
 
 ColumnOrColumns = Union[str, List[str]]
 FunctionOrPredefined = Union[Callable, PredefinedFunction, str]
 ColumnWindowFunction = Tuple[ColumnOrColumns, int, FunctionOrPredefined]
 
 
 class AddWindowFeatures(Transformation, Tunable):
@@ -59,33 +49,33 @@
     --------
     ```pycon
     >>> from fold.loop import train_backtest
     >>> from fold.splitters import SlidingWindowSplitter
     >>> from fold.transformations import AddWindowFeatures
     >>> from fold.utils.tests import generate_sine_wave_data
     >>> X, y  = generate_sine_wave_data()
-    >>> splitter = SlidingWindowSplitter(initial_train_window=0.5, step=0.2)
+    >>> splitter = SlidingWindowSplitter(train_window=0.5, step=0.2)
     >>> pipeline = AddWindowFeatures(("sine", 10, "mean"))
     >>> preds, trained_pipeline = train_backtest(pipeline, X, y, splitter)
     >>> preds.head()
                            sine  sine_10_mean
     2021-12-31 15:40:00 -0.0000      -0.05649
     2021-12-31 15:41:00  0.0126      -0.04394
     2021-12-31 15:42:00  0.0251      -0.03139
     2021-12-31 15:43:00  0.0377      -0.01883
     2021-12-31 15:44:00  0.0502      -0.00628
 
     ```
     """
 
-    name = "AddWindowFeatures"
-
     def __init__(
         self,
         column_window_func: Union[ColumnWindowFunction, List[ColumnWindowFunction]],
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> None:
         self.column_window_func = [
             (
                 wrap_in_list(column),
                 window,
                 function
                 if isinstance(function, Callable)
@@ -93,16 +83,20 @@
             )
             for column, window, function in wrap_in_list(column_window_func)
         ]
         max_memory = max([window for _, window, _ in self.column_window_func])
         self.properties = Transformation.Properties(
             requires_X=True, memory_size=max_memory
         )
+        self.params_to_try = params_to_try
+        self.name = name or "AddWindowFeatures"
 
-    def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
+    def transform(
+        self, X: pd.DataFrame, in_sample: bool
+    ) -> Tuple[pd.DataFrame, Optional[Artifact]]:
         X_function_applied = pd.DataFrame([], index=X.index)
         for columns, window, function in self.column_window_func:
             if isinstance(function, PredefinedFunction):
                 function = getattr(pd.core.window.rolling.Rolling, function.value)
             function_name = (
                 function.__name__ if function.__name__ != "<lambda>" else "transformed"
             )
@@ -117,14 +111,14 @@
                     axis="columns",
                 )
             else:
                 for col in columns:
                     X_function_applied[f"{col}_{window}_{function_name}"] = function(
                         X[col].rolling(window)
                     )
-        return pd.concat([X, X_function_applied], axis="columns")
+        return pd.concat([X, X_function_applied], axis="columns"), None
 
     fit = fit_noop
     update = fit
 
     def get_params(self) -> dict:
-        return {"column_window_func": self.column_window_func}
+        return {"column_window_func": self.column_window_func, "name": self.name}
```

### Comparing `fold_core-0.1.8/src/fold/utils/checks.py` & `fold_core-0.1.9/src/fold/utils/checks.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,18 +34,46 @@
             or len(df.columns) == 0
             or (len(df.columns) == 1 and df.isna().sum()[0] == len(df))
             for df in results
         ]
     )
 
 
+def has_probabilities(df: pd.DataFrame) -> bool:
+    """
+    Check if all the DataFrames have probabilities columns,
+    or if their values are all NaN, indicating an empty DataFrame
+    being passed around, as SkipNA filtered out all data.
+    """
+    return (
+        any([True for col in df.columns if str(col).startswith("probabilities_")])
+        or len(df.columns) == 0
+        or (len(df.columns) == 1 and df.isna().sum()[0] == len(df))
+    )
+
+
 def get_prediction_column(input: pd.DataFrame) -> pd.Series:
     return to_series(input[get_prediction_column_name(input)])
 
 
+def get_probabilities_columns(input: pd.DataFrame) -> pd.DataFrame:
+    return input[get_probabilities_column_names(input)]
+
+
+def get_probabilities_column_names(input: pd.DataFrame) -> List[str]:
+    candidates = [col for col in input.columns if str(col).startswith("probabilities_")]
+    if len(candidates) == 0:
+        raise ValueError(f"Could not find any probabilities column in {input.columns}.")
+    return candidates
+
+
+def get_classes_from_probabilies_column_names(columns: List[str]) -> List[str]:
+    return [col.split("_")[-1] for col in columns]
+
+
 def get_prediction_column_name(input: pd.DataFrame) -> str:
     candidates = [col for col in input.columns if col.startswith("predictions_")]
     if len(candidates) == 0:
         if len(input.columns) == 1:
             return input.columns[0]
         else:
             raise ValueError(f"Could not find a predictions column in {input.columns}.")
```

### Comparing `fold_core-0.1.8/src/fold/utils/dataset.py` & `fold_core-0.1.9/src/fold/utils/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from __future__ import annotations
 
-from enum import Enum
 from typing import Optional, Tuple, Union
 
 import pandas as pd
 
+from .enums import ParsableEnum
+
 
 def load_dataset(
     dataset_name: str,
     base_path: str = "https://raw.githubusercontent.com/dream-faster/datasets/main/datasets",
 ) -> pd.DataFrame:
     return pd.read_csv(f"{base_path}/{dataset_name}.csv", parse_dates=True, index_col=0)
 
 
-class DeduplicationStrategy(Enum):
+class DeduplicationStrategy(ParsableEnum):
     first = "first"
     last = "last"
 
-    @staticmethod
-    def from_str(value: Union[str, DeduplicationStrategy]) -> DeduplicationStrategy:
-        if isinstance(value, DeduplicationStrategy):
-            return value
-        for strategy in DeduplicationStrategy:
-            if strategy.value == value:
-                return strategy
-        else:
-            raise ValueError(f"Unknown DeduplicationStrategy: {value}")
-
 
 def __process_dataset(
     df: pd.DataFrame,
     target_col: str,
     resample: Optional[str] = None,
     deduplication_strategy: Optional[Union[DeduplicationStrategy, str]] = None,
     shorten: Optional[int] = None,
```

### Comparing `fold_core-0.1.8/src/fold/utils/list.py` & `fold_core-0.1.9/src/fold/utils/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 import collections
 from collections.abc import Iterable
-from typing import List, Tuple, TypeVar, Union
+from typing import Dict, List, Optional, Tuple, TypeVar, Union
 
 from iteration_utilities import unique_everseen
 
 T = TypeVar("T")
 
 
 def wrap_in_list(input: Union[T, List[T]]) -> List[T]:
@@ -52,7 +52,43 @@
 
 def unique(input: List) -> List:
     return unique_everseen(input)
 
 
 def swap_tuples(input: List[Tuple]) -> List[Tuple]:
     return [(b, a) for a, b in input]
+
+
+def filter_none(input: List) -> List:
+    return [x for x in input if x is not None]
+
+
+def empty_if_none(input: Union[List, None]) -> List:
+    return [] if input is None else input
+
+
+def to_hierachical_dict(flat_dict: dict, length_of_uuid4: int = 36) -> dict:
+    hierarchy = {}
+    for key, value in flat_dict.items():
+        unraveled_obj_key = key[:length_of_uuid4]
+        unraveled_param_key = key[length_of_uuid4 + 1 :]
+        if unraveled_obj_key not in hierarchy:
+            hierarchy[unraveled_obj_key] = {}
+        hierarchy[unraveled_obj_key][unraveled_param_key] = value
+    return hierarchy
+
+
+def to_hierachical_dict_arbitrary_depth(flat_dict: dict, separator: str = ".") -> dict:
+    hierarchy = {}
+    for key, value in flat_dict.items():
+        current_dict = hierarchy
+        parts = key.split(separator)
+        for part in parts[:-1]:
+            if part not in current_dict:
+                current_dict[part] = {}
+            current_dict = current_dict[part]
+        current_dict[parts[-1]] = value
+    return hierarchy
+
+
+def ensure_dict(dictionary: Optional[Dict]) -> dict:
+    return {} if dictionary is None else dictionary
```

### Comparing `fold_core-0.1.8/src/fold/utils/tests.py` & `fold_core-0.1.9/src/fold/utils/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,44 +106,50 @@
 
 def tuneability_test(
     instance: Transformation,
     different_params: dict,
     init_function: Optional[Callable] = None,
     classification: bool = False,
     tolerance: Optional[float] = None,
+    modify_X_func: Optional[Callable] = None,
 ):
     """
     Used to test the general structure and implementation of get_params() and clone_with_params() methods.
     the kwargs are used to set the parameters of the transformation, which should be different to the init parameters of the `instance`.
     """
     assert isinstance(instance, Tunable)
+    assert instance.id is not None
 
     params = instance.get_params()
     different_instance = (
         instance.__class__(**different_params)
         if init_function is None
         else init_function(**different_params)
     )
 
     X, y = (
         generate_zeros_and_ones(length=500)
         if classification
         else generate_sine_wave_data(length=500)
     )
+    if modify_X_func is not None:
+        X = modify_X_func(X)
     splitter = SingleWindowSplitter(train_window=0.5)
     preds_orig, _ = train_backtest(instance, X, y, splitter)
     preds_different, _ = train_backtest(different_instance, X, y, splitter)
     assert not preds_orig.equals(
         preds_different
     ), "The output of the two instances with different parameters should be different"
 
-    reconstructed_instance = different_instance.clone_with_params(**params)
+    reconstructed_instance = different_instance.clone_with_params(params)
 
     preds_reconstructed, _ = train_backtest(reconstructed_instance, X, y, splitter)
     if tolerance is None:
-        assert preds_orig.equals(
-            preds_reconstructed
-        ), "The output of the two instances with different parameters should be the same"
+        assert preds_orig.equals(preds_reconstructed), (
+            "The output of the two instances with different parameters should be the"
+            " same"
+        )
     else:
-        assert np.isclose(
-            preds_orig, preds_reconstructed, atol=tolerance
-        ).all(), "The output of the two instances with different parameters should be the close"
+        assert np.isclose(preds_orig, preds_reconstructed, atol=tolerance).all(), (
+            "The output of the two instances with the same parameters should be the"
+            " close"
+        )
```

### Comparing `fold_core-0.1.8/src/fold/utils/trim.py` & `fold_core-0.1.9/src/fold/utils/trim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
-from typing import Tuple, Union
+from typing import Optional, Tuple, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
+from ..base import Extras
 
-def trim_initial_nans(X: pd.DataFrame, y: pd.Series) -> Tuple[pd.DataFrame, pd.Series]:
+T = TypeVar("T", pd.Series, Optional[pd.Series])
+
+
+def trim_initial_nans(
+    X: pd.DataFrame, y: pd.Series, extras: Extras
+) -> Tuple[pd.DataFrame, pd.Series, Extras]:
     # Optimize for speed, if the first value is not NaN, we can save all the subsequent computation
     if not X.iloc[0].isna().any() and (y is None or not np.isnan(y.iloc[0])):
-        return X, y
+        return X, y, extras
     first_valid_index_X = get_first_valid_index(X)
     first_valid_index_y = get_first_valid_index(y)
     if first_valid_index_X is None or first_valid_index_y is None:
-        return pd.DataFrame(), pd.Series()
+        return (
+            pd.DataFrame(),
+            pd.Series(dtype="float64"),
+            Extras(),
+        )
     first_valid_index = max(first_valid_index_X, first_valid_index_y)
-    return X.iloc[first_valid_index:], y.iloc[first_valid_index:]
+    return (
+        X.iloc[first_valid_index:],
+        y.iloc[first_valid_index:],
+        extras.iloc(slice(first_valid_index, None)),
+    )
 
 
 def trim_initial_nans_single(X: pd.DataFrame) -> pd.DataFrame:
     # Optimize for speed, if the first value is not NaN, we can save all the subsequent computation
     if not X.iloc[0].isna().any():
         return X
     first_valid_index = get_first_valid_index(X)
```

### Comparing `fold_core-0.1.8/PKG-INFO` & `fold_core-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
@@ -12,19 +12,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: quality
 Provides-Extra: ray
 Provides-Extra: tests
@@ -33,31 +28,34 @@
 Requires-Dist: fold-models (>=0.1.2,<0.2.0)
 Requires-Dist: fold-wrappers (>=0.1,<1.0) ; extra == "all"
 Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "all"
 Requires-Dist: image (>=1.5.33) ; extra == "docs"
 Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests"
 Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
 Requires-Dist: iteration_utilities (>=0.11)
-Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "all"
+Requires-Dist: krisi (>=1.0.1,<1.1.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.2)
 Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs"
 Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
 Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
 Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=9.0.0) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.16)
+Requires-Dist: p_tqdm (>=1.3) ; extra == "all"
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality"
 Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests"
 Requires-Dist: pytest-cov (>=4.0) ; extra == "tests"
 Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "all"
 Requires-Dist: scikit-learn (>=0.22)
+Requires-Dist: statsmodels (>=0.12.1) ; extra == "tests" or extra == "all"
 Requires-Dist: tqdm (>=4.0)
+Requires-Dist: typing_extensions (>=4.4.0)
 Description-Content-Type: text/markdown
 
 <!-- # fold -->
 
 <p align="center" style="display:flex; width:100%; align-items:center; justify-content:center;">
   <a style="margin:2px" href="https://dream-faster.github.io/fold/"><img alt="Docs" src="https://img.shields.io/github/actions/workflow/status/dream-faster/fold/docs.yaml?logo=readthedocs"></a>
   <a style="margin:2px" href="https://codecov.io/gh/dream-faster/fold" ><img src="https://codecov.io/gh/dream-faster/fold/branch/main/graph/badge.svg?token=Z7I2XSF188"/></a>
```

#### html2text {}

```diff
@@ -1,46 +1,44 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.8 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.9 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Provides-Extra: all Provides-Extra: docs Provides-Extra: quality Provides-
-Extra: ray Provides-Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ;
-extra == "quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
-Requires-Dist: fold-models (>=0.1.2,<0.2.0) Requires-Dist: fold-wrappers
-(>=0.1,<1.0) ; extra == "all" Requires-Dist: holidays (>=0.10) ; extra ==
-"tests" or extra == "all" Requires-Dist: image (>=1.5.33) ; extra == "docs"
-Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests" Requires-Dist:
-isort (>=5.10.1,<5.11.0) ; extra == "quality" Requires-Dist:
-iteration_utilities (>=0.11) Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra ==
-"all" Requires-Dist: mkdocs (>=1.2) Requires-Dist: mkdocs-autorefs (>=0.4) ;
-extra == "docs" Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
-Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra == "docs" Requires-Dist:
-mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs" Requires-Dist: mkdocs-
-jupyter (>=0.22) ; extra == "docs" Requires-Dist: mkdocs-material (>=9.0.0) ;
-extra == "docs" Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
-Requires-Dist: numpy (>=1.16) Requires-Dist: pandas (>=1.2) Requires-Dist: pre-
+Programming Language :: Python :: Implementation :: CPython Classifier:
+Programming Language :: Python :: Implementation :: PyPy Provides-Extra: all
+Provides-Extra: docs Provides-Extra: quality Provides-Extra: ray Provides-
+Extra: tests Requires-Dist: black (>=22.12.0,<22.13.0) ; extra == "quality"
+Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality" Requires-Dist:
+fold-models (>=0.1.2,<0.2.0) Requires-Dist: fold-wrappers (>=0.1,<1.0) ; extra
+== "all" Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "all"
+Requires-Dist: image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-
+learn (>=0.7.0) ; extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ;
+extra == "quality" Requires-Dist: iteration_utilities (>=0.11) Requires-Dist:
+krisi (>=1.0.1,<1.1.0) ; extra == "all" Requires-Dist: mkdocs (>=1.2) Requires-
+Dist: mkdocs-autorefs (>=0.4) ; extra == "docs" Requires-Dist: mkdocs-gallery
+(>=0.7) ; extra == "docs" Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra ==
+"docs" Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
+Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs" Requires-Dist: mkdocs-
+material (>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-python
+(>=0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist: p_tqdm
+(>=1.3) ; extra == "all" Requires-Dist: pandas (>=1.2) Requires-Dist: pre-
 commit (>=2.20.0,<2.21.0) ; extra == "quality" Requires-Dist: pytest
 (>=7.1.2,<7.2.0) ; extra == "tests" Requires-Dist: pytest-cov (>=4.0) ; extra
 == "tests" Requires-Dist: ray (>=1.4) ; extra == "ray" or extra == "all"
-Requires-Dist: scikit-learn (>=0.22) Requires-Dist: tqdm (>=4.0) Description-
-Content-Type: text/markdown
+Requires-Dist: scikit-learn (>=0.22) Requires-Dist: statsmodels (>=0.12.1) ;
+extra == "tests" or extra == "all" Requires-Dist: tqdm (>=4.0) Requires-Dist:
+typing_extensions (>=4.4.0) Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                       ****
                      Fast Adaptive Time Series ML Engine
```

