# Comparing `tmp/ape-avalanche-0.6.2.tar.gz` & `tmp/ape-avalanche-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-avalanche-0.6.2.tar", last modified: Tue Apr 11 14:20:59 2023, max compression
+gzip compressed data, was "ape-avalanche-0.6.3.tar", last modified: Thu Jun 29 21:07:20 2023, max compression
```

## Comparing `ape-avalanche-0.6.2.tar` & `ape-avalanche-0.6.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/ape_avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/ape_avalanche.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/ape_avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/ape_avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/ape_avalanche/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/ape_avalanche/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/ape_avalanche.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 21:07:20.000000 ape-avalanche-0.6.3/ape_avalanche.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 21:07:20.743914 ape-avalanche-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:07:20.739914 ape-avalanche-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-29 21:06:18.000000 ape-avalanche-0.6.3/tests/test_provider.py
```

### Comparing `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-avalanche-0.6.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.github/release-drafter.yml` & `ape-avalanche-0.6.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.github/workflows/codeql.yaml` & `ape-avalanche-0.6.3/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.github/workflows/commitlint.yaml` & `ape-avalanche-0.6.3/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[dev]
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-avalanche-0.6.2/.github/workflows/prtitle.yaml` & `ape-avalanche-0.6.3/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-avalanche-0.6.2/.github/workflows/publish.yaml` & `ape-avalanche-0.6.3/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-avalanche-0.6.2/.github/workflows/test.yaml` & `ape-avalanche-0.6.3/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
@@ -90,14 +90,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-avalanche-0.6.2/.gitignore` & `ape-avalanche-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/.pre-commit-config.yaml` & `ape-avalanche-0.6.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
-        additional_dependencies: [types-setuptools]
+        additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.14
     hooks:
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
```

### Comparing `ape-avalanche-0.6.2/CONTRIBUTING.md` & `ape-avalanche-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/LICENSE` & `ape-avalanche-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/PKG-INFO` & `ape-avalanche-0.6.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 Metadata-Version: 2.1
 Name: ape-avalanche
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-avalanche: Ape Ecosystem Plugin for Avalanche
 Home-page: https://github.com/ApeWorX/ape-avalanche
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Avalanche (C-Chain) support in Ape
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install avalanche
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: avalanche
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-avalanche
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-avalanche.git
-        cd ape-avalanche
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Avalanche ecosystem:
-        
-        ```bash
-        ape console --network avalanche:mainnet
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Avalanche (C-Chain) support in Ape
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install avalanche
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: avalanche
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-avalanche
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-avalanche.git
+cd ape-avalanche
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Avalanche ecosystem:
+
+```bash
+ape console --network avalanche:mainnet
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-avalanche-0.6.2/README.md` & `ape-avalanche-0.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Avalanche (C-Chain) support in Ape
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-avalanche-0.6.2/ape_avalanche/__init__.py` & `ape-avalanche-0.6.3/ape_avalanche/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/ape_avalanche/ecosystem.py` & `ape-avalanche-0.6.3/ape_avalanche/ecosystem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from typing import Optional
 
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME
+from ape.utils import DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT
 from ape_ethereum.ecosystem import Ethereum, NetworkConfig
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (43114, 43114),
     "fuji": (43113, 43113),
 }
 
 
 def _create_network_config(
-    required_confirmations: int = 1, block_time: int = 2, **kwargs
+    required_confirmations: int = 1, block_time: int = 3, **kwargs
 ) -> NetworkConfig:
     return NetworkConfig(
         required_confirmations=required_confirmations, block_time=block_time, **kwargs
     )
 
 
-def _create_local_config(default_provider: Optional[str] = None) -> NetworkConfig:
+def _create_local_config(default_provider: Optional[str] = None, **kwargs) -> NetworkConfig:
     return _create_network_config(
-        required_confirmations=0, block_time=0, default_provider=default_provider
+        required_confirmations=0,
+        default_provider=default_provider,
+        transaction_acceptance_timeout=DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT,
+        gas_limit="max",
+        **kwargs,
     )
 
 
 class AvalancheConfig(PluginConfig):
     mainnet: NetworkConfig = _create_network_config()
     mainnet_fork: NetworkConfig = _create_local_config()
     fuji: NetworkConfig = _create_network_config()
     fuji_fork: NetworkConfig = _create_local_config()
-    local: NetworkConfig = NetworkConfig(default_provider="test")
+    local: NetworkConfig = _create_local_config(default_provider="test")
     default_network: str = LOCAL_NETWORK_NAME
 
 
 class Avalanche(Ethereum):
     @property
     def config(self) -> AvalancheConfig:  # type: ignore
         return self.config_manager.get_config("avalanche")  # type: ignore
```

### Comparing `ape-avalanche-0.6.2/ape_avalanche.egg-info/PKG-INFO` & `ape-avalanche-0.6.3/ape_avalanche.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 Metadata-Version: 2.1
 Name: ape-avalanche
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-avalanche: Ape Ecosystem Plugin for Avalanche
 Home-page: https://github.com/ApeWorX/ape-avalanche
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Avalanche (C-Chain) support in Ape
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install avalanche
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: avalanche
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-avalanche
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-avalanche.git
-        cd ape-avalanche
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Avalanche ecosystem:
-        
-        ```bash
-        ape console --network avalanche:mainnet
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Avalanche (C-Chain) support in Ape
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install avalanche
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: avalanche
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-avalanche
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-avalanche.git
+cd ape-avalanche
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Avalanche ecosystem:
+
+```bash
+ape console --network avalanche:mainnet
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-avalanche-0.6.2/ape_avalanche.egg-info/SOURCES.txt` & `ape-avalanche-0.6.3/ape_avalanche.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 ape_avalanche.egg-info/SOURCES.txt
 ape_avalanche.egg-info/dependency_links.txt
 ape_avalanche.egg-info/not-zip-safe
 ape_avalanche.egg-info/requires.txt
 ape_avalanche.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_ecosystem.py
 tests/test_integration.py
 tests/test_provider.py
```

### Comparing `ape-avalanche-0.6.2/ape_avalanche.egg-info/requires.txt` & `ape-avalanche-0.6.3/ape_avalanche.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.2/pyproject.toml` & `ape-avalanche-0.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=51.1.1", "wheel", "setuptools_scm[toml]>=5.0"]
 
 [tool.mypy]
 exclude = "build/"
+plugins = ["pydantic.mypy"]
 
 [tool.setuptools_scm]
 write_to = "ape_avalanche/version.py"
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -n auto
     -p no:ape_test
     --cov-branch
```

### Comparing `ape-avalanche-0.6.2/setup.py` & `ape-avalanche-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,9 +74,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-avalanche-0.6.2/tests/test_integration.py` & `ape-avalanche-0.6.3/tests/test_integration.py`

 * *Files identical despite different names*

