# Comparing `tmp/pyyaml-include-1.3.1b1.tar.gz` & `tmp/pyyaml-include-1.3b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyaml-include-1.3.1b1.tar", last modified: Thu Feb  2 00:58:37 2023, max compression
+gzip compressed data, was "pyyaml-include-1.3b4.tar", last modified: Sun Apr 24 04:00:46 2022, max compression
```

## Comparing `pyyaml-include-1.3.1b1.tar` & `pyyaml-include-1.3b4.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.692078 pyyaml-include-1.3.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.680078 pyyaml-include-1.3.1b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.684078 pyyaml-include-1.3.1b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/.pep8
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-02-02 00:58:37.692078 pyyaml-include-1.3.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.684078 pyyaml-include-1.3.1b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/yamlinclude.constructor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/yamlinclude.readers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/yamlinclude.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/docs/yamlinclude.version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.684078 pyyaml-include-1.3.1b1/requires/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/requires/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/requires/dist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-02 00:58:37.692078 pyyaml-include-1.3.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.684078 pyyaml-include-1.3.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.688078 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.688078 pyyaml-include-1.3.1b1/src/yamlinclude/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/src/yamlinclude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/src/yamlinclude/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/src/yamlinclude/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-02 00:58:37.000000 pyyaml-include-1.3.1b1/src/yamlinclude/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.688078 pyyaml-include-1.3.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.688078 pyyaml-include-1.3.1b1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 00:58:37.688078 pyyaml-include-1.3.1b1/tests/data/include.d/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/1.j2
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/1.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/1.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/2.j2
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/2.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/2.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/include.d/2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/data/zh_cn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/test_custome_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-02-02 00:58:23.000000 pyyaml-include-1.3.1b1/tests/test_relative_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.570032 pyyaml-include-1.3b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.570032 pyyaml-include-1.3b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.pep8
+-rw-r--r--   0 runner    (1001) docker     (121)    18074 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.574033 pyyaml-include-1.3b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6422 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/yamlinclude.constructor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/yamlinclude.readers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/yamlinclude.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/docs/yamlinclude.version.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.574033 pyyaml-include-1.3b4/requires/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/requires/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/requires/dist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.570032 pyyaml-include-1.3b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.574033 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-04-24 04:00:45.000000 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-04-24 04:00:46.000000 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-24 04:00:45.000000 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-24 04:00:46.000000 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-24 04:00:46.000000 pyyaml-include-1.3b4/src/pyyaml_include.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.574033 pyyaml-include-1.3b4/src/yamlinclude/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/src/yamlinclude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/src/yamlinclude/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/src/yamlinclude/readers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-24 04:00:45.000000 pyyaml-include-1.3b4/src/yamlinclude/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/_internel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-24 04:00:46.578033 pyyaml-include-1.3b4/tests/data/include.d/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/1.j2
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/1.json
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/1.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/2.j2
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/2.json
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/2.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/include.d/2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/data/zh_cn.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/test_custome_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11333 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-04-24 04:00:30.000000 pyyaml-include-1.3b4/tests/test_multi.py
```

### Comparing `pyyaml-include-1.3.1b1/.github/workflows/python-package.yml` & `pyyaml-include-1.3b4/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
           fi
           echo ::set-output name=version::${PEP440_VERSION}
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
     steps:
       - name: Checkout
         uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `pyyaml-include-1.3.1b1/.gitignore` & `pyyaml-include-1.3b4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/CHANGELOG.md` & `pyyaml-include-1.3b4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 # Changelog
 
-## 1.3.1b1
-
-Date: 2023-02-02
-
-- New:
-  - relative include for pure python PyYAML
-
-## 1.3
+## 1.3 beta4
 
 Date: 2022-04-24
 
 - New:
   - PyYAML 6.0 supported
 
-- Misc:
-  - Better CI processes
-
 ## 1.2
 
 Date: 2019-02-03
 
 - New:
   - non YAML file including
 
 - Misc:
   - adjust docs
   - add pip and conda configure file of development environment
 
 - Fix:
-  - add `PlainTextReader` into `__all__` list of `readers` module
+  - add `PlainTextReader` into `__all__` list of `reders` module
 
 ## 1.1
 
 Date: 2019-03-18
 
 - Change:
   - Update PyYAML to 5.*
```

### Comparing `pyyaml-include-1.3.1b1/LICENSE` & `pyyaml-include-1.3b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/PKG-INFO` & `pyyaml-include-1.3b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 1.3.1b1
+Version: 1.3b4
 Summary: Extending PyYAML with a custom constructor for including YAML files within YAML files
 Home-page: https://github.com/tanbro/pyyaml-include
 Author: liu xue yan
 Author-email: liu_xue_yan@foxmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: yaml,PyYAML,include
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
@@ -180,44 +181,34 @@
 
 * Liu Xue Yan (<liu_xue_yan@foxmail.com>)
 
   [![liu_xue_yan@foxmail.com](https://www.gravatar.com/avatar/049d2fae1fd2df6439e87d1383d0276b)](mailto:liu_xue_yan@foxmail.com)
 
 # Changelog
 
-## 1.3.1b1
-
-Date: 2023-02-02
-
-- New:
-  - relative include for pure python PyYAML
-
-## 1.3
+## 1.3 beta4
 
 Date: 2022-04-24
 
 - New:
   - PyYAML 6.0 supported
 
-- Misc:
-  - Better CI processes
-
 ## 1.2
 
 Date: 2019-02-03
 
 - New:
   - non YAML file including
 
 - Misc:
   - adjust docs
   - add pip and conda configure file of development environment
 
 - Fix:
-  - add `PlainTextReader` into `__all__` list of `readers` module
+  - add `PlainTextReader` into `__all__` list of `reders` module
 
 ## 1.1
 
 Date: 2019-03-18
 
 - Change:
   - Update PyYAML to 5.*
@@ -284,7 +275,9 @@
   - Rename module file `include.py` to `constructor.py`
 
   - Rename class data member `DEFAULT_TAG` to `TAG`
 
 ## 1.0
 
 Date: 2018-06-08
+
+
```

### Comparing `pyyaml-include-1.3.1b1/README.md` & `pyyaml-include-1.3b4/README.md`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/docs/CHANGELOG.md` & `pyyaml-include-1.3b4/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 # Changelog
 
-## 1.3.1b1
-
-Date: 2023-02-02
-
-- New:
-  - relative include for pure python PyYAML
-
-## 1.3
+## 1.3 beta4
 
 Date: 2022-04-24
 
 - New:
   - PyYAML 6.0 supported
 
-- Misc:
-  - Better CI processes
-
 ## 1.2
 
 Date: 2019-02-03
 
 - New:
   - non YAML file including
 
 - Misc:
   - adjust docs
   - add pip and conda configure file of development environment
 
 - Fix:
-  - add `PlainTextReader` into `__all__` list of `readers` module
+  - add `PlainTextReader` into `__all__` list of `reders` module
 
 ## 1.1
 
 Date: 2019-03-18
 
 - Change:
   - Update PyYAML to 5.*
```

### Comparing `pyyaml-include-1.3.1b1/docs/Makefile` & `pyyaml-include-1.3b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/docs/README.md` & `pyyaml-include-1.3b4/docs/README.md`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/docs/conf.py` & `pyyaml-include-1.3b4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/docs/index.rst` & `pyyaml-include-1.3b4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/docs/make.bat` & `pyyaml-include-1.3b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/setup.cfg` & `pyyaml-include-1.3b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/PKG-INFO` & `pyyaml-include-1.3b4/src/pyyaml_include.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyyaml-include
-Version: 1.3.1b1
+Version: 1.3b4
 Summary: Extending PyYAML with a custom constructor for including YAML files within YAML files
 Home-page: https://github.com/tanbro/pyyaml-include
 Author: liu xue yan
 Author-email: liu_xue_yan@foxmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: yaml,PyYAML,include
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
@@ -180,44 +181,34 @@
 
 * Liu Xue Yan (<liu_xue_yan@foxmail.com>)
 
   [![liu_xue_yan@foxmail.com](https://www.gravatar.com/avatar/049d2fae1fd2df6439e87d1383d0276b)](mailto:liu_xue_yan@foxmail.com)
 
 # Changelog
 
-## 1.3.1b1
-
-Date: 2023-02-02
-
-- New:
-  - relative include for pure python PyYAML
-
-## 1.3
+## 1.3 beta4
 
 Date: 2022-04-24
 
 - New:
   - PyYAML 6.0 supported
 
-- Misc:
-  - Better CI processes
-
 ## 1.2
 
 Date: 2019-02-03
 
 - New:
   - non YAML file including
 
 - Misc:
   - adjust docs
   - add pip and conda configure file of development environment
 
 - Fix:
-  - add `PlainTextReader` into `__all__` list of `readers` module
+  - add `PlainTextReader` into `__all__` list of `reders` module
 
 ## 1.1
 
 Date: 2019-03-18
 
 - Change:
   - Update PyYAML to 5.*
@@ -284,7 +275,9 @@
   - Rename module file `include.py` to `constructor.py`
 
   - Rename class data member `DEFAULT_TAG` to `TAG`
 
 ## 1.0
 
 Date: 2018-06-08
+
+
```

### Comparing `pyyaml-include-1.3.1b1/src/pyyaml_include.egg-info/SOURCES.txt` & `pyyaml-include-1.3b4/src/pyyaml_include.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 .coveragerc
 .flake8
 .gitignore
 .pep8
+.pylintrc
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 README.md
 bandit.yml
+environment.yml
 pyproject.toml
+pytest.ini
 readthedocs.yml
 setup.cfg
+setup.py
 .github/workflows/python-package.yml
 docs/AUTHORS.md
 docs/CHANGELOG.md
 docs/Makefile
 docs/README.md
 docs/conf.py
 docs/index.rst
@@ -32,20 +36,19 @@
 src/pyyaml_include.egg-info/requires.txt
 src/pyyaml_include.egg-info/top_level.txt
 src/yamlinclude/__init__.py
 src/yamlinclude/constructor.py
 src/yamlinclude/readers.py
 src/yamlinclude/version.py
 tests/__init__.py
-tests/_internal.py
+tests/_internel.py
 tests/test_base_dir.py
 tests/test_custome_reader.py
 tests/test_loader.py
 tests/test_multi.py
-tests/test_relative_dir.py
 tests/data/0.yaml
 tests/data/zh_cn.yaml
 tests/data/include.d/1.j2
 tests/data/include.d/1.json
 tests/data/include.d/1.toml
 tests/data/include.d/1.txt
 tests/data/include.d/1.yaml
```

### Comparing `pyyaml-include-1.3.1b1/src/yamlinclude/constructor.py` & `pyyaml-include-1.3b4/src/yamlinclude/constructor.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,34 +4,26 @@
 Include YAML files within YAML
 """
 
 import os.path
 import re
 from glob import iglob
 from sys import version_info
-from typing import Optional, Pattern, Sequence, Tuple, Type
+from typing import Optional, Pattern, Sequence, Tuple
 
 import yaml
 
 from .readers import Reader, get_reader_class_by_name, get_reader_class_by_path
 
 __all__ = ['YamlIncludeConstructor']
 
 PYTHON_MAYOR_MINOR = '{0[0]}.{0[1]}'.format(version_info)
 
 WILDCARDS_REGEX = re.compile(r'^.*(\*|\?|\[!?.+]).*$')
 
-class YamlIncludeException(Exception):
-    pass
-
-class YamlIncludeFileTypeException(YamlIncludeException, TypeError):
-    pass
-
-class YamlIncludeLibYamlException(YamlIncludeException, ValueError):
-    pass
 
 class YamlIncludeConstructor:
     """The `include constructor` for PyYAML Loaders
 
     Call :meth:`add_to_loader_class` or :meth:`yaml.Loader.add_constructor` to add it into loader.
 
     In YAML files, use ``!include`` to load other YAML files as below::
@@ -47,39 +39,32 @@
     DEFAULT_ENCODING = 'utf-8'
     DEFAULT_TAG_NAME = '!include'
 
     def __init__(
             self,
             base_dir: str = '',
             encoding: str = '',
-            reader_map: Optional[Sequence[Tuple[Pattern, Reader]]] = None,
-            relative: bool = False,
+            reader_map: Optional[Sequence[Tuple[Pattern, Reader]]] = None
     ):
         """
         :param str base_dir: Base directory where search including YAML files
 
             :default: ``""``:  include YAML files from current working directory.
 
         :param str encoding: Encoding of the YAML files
 
             :default: ``""``:  Not specified
 
         :param Collection reader_map: A collection of `(path-pattern, reader-class)` tuple
 
             :default: ``None``: set :data:`readers.READER_TABLE` as default readers map
-
-        :param bool relative: Use the yaml files location for relative includes
-
-            :default: ``False``:  include YAML files from current working directory.
-
         """
         self._base_dir = base_dir
         self._encoding = encoding
         self._reader_map = reader_map
-        self._relative = relative
 
     def __call__(self, loader, node):
         args = []
         kwargs = {}
         if isinstance(node, yaml.nodes.ScalarNode):  # type: ignore
             args = [loader.construct_scalar(node)]
         elif isinstance(node, yaml.nodes.SequenceNode):  # type: ignore
@@ -119,15 +104,16 @@
             loader,
             pathname: str,
             recursive: bool = False,
             encoding: str = '',
             reader: str = ''
     ):  # pylint:disable=too-many-arguments
         """Once add the constructor to PyYAML loader class,
-        the loader will invoke this function to include other YAML files when parsing a ``"!include"`` tag.
+        Loader will use this function to include other YAML files
+        on parsing ``"!include"`` tag
 
         :param loader: Instance of PyYAML's loader class
         :param str pathname: pathname can be either absolute (like `/usr/src/Python-1.5/*.yml`)
             or relative (like `../../Tools/*/*.yml`), and can contain shell-style wildcards
 
         :param bool recursive: If recursive is true, the pattern ``"**"`` will match any files and zero
             or more directories and subdirectories.
@@ -155,25 +141,14 @@
 
         .. warning:: It's called by :mod:`yaml`. Do NOT call it yourself.
         """
         if not encoding:
             encoding = self._encoding or self.DEFAULT_ENCODING
         if self._base_dir:
             pathname = os.path.join(self._base_dir, pathname)
-        elif self._relative:
-            if loader.__module__ == "yaml.cyaml":
-                raise YamlIncludeLibYamlException(
-                    f"Relative import not supported for libyaml based loaders, please set the `base_dir` manually"
-                )
-            loader_name = loader.name # dirty hack to enable mocking
-            if loader_name in [ "<unicode string>" ,"<byte string>", "<file>" ]:
-                raise YamlIncludeFileTypeException(
-                    f"Relative include only supported for regular files, got {loader.name} instead."
-                    )
-            pathname = os.path.join(os.path.dirname(loader.name), pathname)
         reader_clz = None
         if reader:
             reader_clz = get_reader_class_by_name(reader)
         if re.match(WILDCARDS_REGEX, pathname):
             result = []
             iterable = iglob(pathname, recursive=recursive)
             for path in filter(os.path.isfile, iterable):
@@ -190,16 +165,16 @@
         reader_clz = get_reader_class_by_path(path, self._reader_map)
         reader_obj = reader_clz(path, encoding=encoding, loader_class=type(loader))
         return reader_obj()
 
     @classmethod
     def add_to_loader_class(
             cls,
-            loader_class: Optional[Type] = None,
-            tag: Optional[str] = None,
+            loader_class=None,
+            tag: str = None,
             **kwargs
     ):
         """
         Create an instance of the constructor, and add it to the YAML `Loader` class
 
         :param loader_class: The `Loader` **class** add constructor to.
```

### Comparing `pyyaml-include-1.3.1b1/src/yamlinclude/readers.py` & `pyyaml-include-1.3b4/src/yamlinclude/readers.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/tests/_internal.py` & `pyyaml-include-1.3b4/tests/_internel.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/tests/test_base_dir.py` & `pyyaml-include-1.3b4/tests/test_base_dir.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import unittest
 from io import StringIO
 from textwrap import dedent
 
 import yaml
 
 from yamlinclude import YamlIncludeConstructor
-from ._internal import PYTHON_VERSION_MAYOR_MINOR, YAML_LOADERS, YAML1, YAML2
+from ._internel import PYTHON_VERSION_MAYOR_MINOR, YAML_LOADERS, YAML1, YAML2
 
 
 class BaseDirTestCase(unittest.TestCase):
 
     def setUp(self):
         for loader_cls in YAML_LOADERS:
             YamlIncludeConstructor.add_to_loader_class(loader_cls, base_dir=os.path.join('tests', 'data'))
```

### Comparing `pyyaml-include-1.3.1b1/tests/test_custome_reader.py` & `pyyaml-include-1.3b4/tests/test_custome_reader.py`

 * *Files identical despite different names*

### Comparing `pyyaml-include-1.3.1b1/tests/test_loader.py` & `pyyaml-include-1.3b4/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import unittest
 from io import StringIO
 
 import yaml
 
 from yamlinclude import YamlIncludeConstructor
-from ._internal import PYTHON_VERSION_MAYOR_MINOR, YAML_LOADERS, YAML1, YAML2
+from ._internel import PYTHON_VERSION_MAYOR_MINOR, YAML_LOADERS, YAML1, YAML2
 
 
 class DefaultLoaderTestCase(unittest.TestCase):
 
     def setUp(self):
         YamlIncludeConstructor.add_to_loader_class()
```

### Comparing `pyyaml-include-1.3.1b1/tests/test_multi.py` & `pyyaml-include-1.3b4/tests/test_multi.py`

 * *Files identical despite different names*

