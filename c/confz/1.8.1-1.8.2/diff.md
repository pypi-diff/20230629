# Comparing `tmp/confz-1.8.1.tar.gz` & `tmp/confz-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confz-1.8.1.tar", max compression
+gzip compressed data, was "confz-1.8.2.tar", max compression
```

## Comparing `confz-1.8.1.tar` & `confz-1.8.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1064 2022-12-22 17:24:32.044307 confz-1.8.1/LICENSE
--rw-r--r--   0        0        0     8288 2022-12-22 17:24:32.044307 confz-1.8.1/README.md
--rw-r--r--   0        0        0      488 2022-12-22 17:24:32.044307 confz-1.8.1/confz/__init__.py
--rw-r--r--   0        0        0     3281 2022-12-22 17:24:32.044307 confz-1.8.1/confz/change.py
--rw-r--r--   0        0        0     3859 2022-12-22 17:24:32.044307 confz-1.8.1/confz/confz.py
--rw-r--r--   0        0        0     4811 2022-12-22 17:24:32.044307 confz-1.8.1/confz/confz_source.py
--rw-r--r--   0        0        0      372 2022-12-22 17:24:32.044307 confz-1.8.1/confz/exceptions.py
--rw-r--r--   0        0        0      148 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/__init__.py
--rw-r--r--   0        0        0     1065 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/cl_arg_loader.py
--rw-r--r--   0        0        0      296 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/data_loader.py
--rw-r--r--   0        0        0     2716 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/env_loader.py
--rw-r--r--   0        0        0     5432 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/file_loader.py
--rw-r--r--   0        0        0     3113 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/loader.py
--rw-r--r--   0        0        0     1190 2022-12-22 17:24:32.044307 confz-1.8.1/confz/loaders/register.py
--rw-r--r--   0        0        0        0 2022-12-22 17:24:32.044307 confz-1.8.1/confz/py.typed
--rw-r--r--   0        0        0     1585 2022-12-22 17:24:32.044307 confz-1.8.1/confz/validate.py
--rw-r--r--   0        0        0     1992 2022-12-22 17:24:32.044307 confz-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     9293 1970-01-01 00:00:00.000000 confz-1.8.1/setup.py
--rw-r--r--   0        0        0     9710 1970-01-01 00:00:00.000000 confz-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-29 11:43:37.180638 confz-1.8.2/LICENSE
+-rw-r--r--   0        0        0     8288 2023-06-29 11:43:37.180638 confz-1.8.2/README.md
+-rw-r--r--   0        0        0      488 2023-06-29 11:43:37.180638 confz-1.8.2/confz/__init__.py
+-rw-r--r--   0        0        0     3281 2023-06-29 11:43:37.180638 confz-1.8.2/confz/change.py
+-rw-r--r--   0        0        0     3859 2023-06-29 11:43:37.180638 confz-1.8.2/confz/confz.py
+-rw-r--r--   0        0        0     4811 2023-06-29 11:43:37.180638 confz-1.8.2/confz/confz_source.py
+-rw-r--r--   0        0        0      372 2023-06-29 11:43:37.180638 confz-1.8.2/confz/exceptions.py
+-rw-r--r--   0        0        0      148 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/__init__.py
+-rw-r--r--   0        0        0     1065 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/cl_arg_loader.py
+-rw-r--r--   0        0        0      296 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/data_loader.py
+-rw-r--r--   0        0        0     2716 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/env_loader.py
+-rw-r--r--   0        0        0     5432 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/file_loader.py
+-rw-r--r--   0        0        0     3113 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/loader.py
+-rw-r--r--   0        0        0     1190 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/register.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:43:37.180638 confz-1.8.2/confz/py.typed
+-rw-r--r--   0        0        0     1585 2023-06-29 11:43:37.180638 confz-1.8.2/confz/validate.py
+-rw-r--r--   0        0        0     1990 2023-06-29 11:43:37.184638 confz-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 confz-1.8.2/PKG-INFO
```

### Comparing `confz-1.8.1/LICENSE` & `confz-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/README.md` & `confz-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/change.py` & `confz-1.8.2/confz/change.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/confz.py` & `confz-1.8.2/confz/confz.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/confz_source.py` & `confz-1.8.2/confz/confz_source.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/loaders/cl_arg_loader.py` & `confz-1.8.2/confz/loaders/cl_arg_loader.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/loaders/env_loader.py` & `confz-1.8.2/confz/loaders/env_loader.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/loaders/file_loader.py` & `confz-1.8.2/confz/loaders/file_loader.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/loaders/loader.py` & `confz-1.8.2/confz/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/loaders/register.py` & `confz-1.8.2/confz/loaders/register.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/confz/validate.py` & `confz-1.8.2/confz/validate.py`

 * *Files identical despite different names*

### Comparing `confz-1.8.1/pyproject.toml` & `confz-1.8.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confz"
-version = "1.8.1"
+version = "1.8.2"
 description = "ConfZ is a configuration management library for Python based on pydantic."
 license = "MIT"
 authors = ["Zühlke"]
 readme = "README.md"
 homepage = "https://github.com/Zuehlke/ConfZ"
 repository = "https://github.com/Zuehlke/ConfZ"
 documentation = "https://confz.readthedocs.io"
@@ -22,24 +22,24 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 pydantic = "^1.9.0"
 PyYAML = ">=5.4.1, <7.0.0"
-python-dotenv = ">=0.19.2, <0.22.0"
+python-dotenv = ">=0.19.2, <2.0.0"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 Sphinx = "^5.3.0"
 pytest-cov = "^4.0.0"
-pytest-asyncio = "^0.20.1"
-black = {extras = ["d"], version = "^22.10.0"}
-mypy = "^0.991"
+pytest-asyncio = "^0.21.0"
+black = {extras = ["d"], version = "^23.3.0"}
+mypy = "^1.4.1"
 pylint = "^2.15.5"
 types-PyYAML = "^6.0.12"
 types-toml = "^0.10.8"
 
 [tool.black]
 # Use default black configuration
```

### Comparing `confz-1.8.1/setup.py` & `confz-1.8.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,237 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: confz
+Version: 1.8.2
+Summary: ConfZ is a configuration management library for Python based on pydantic.
+Home-page: https://github.com/Zuehlke/ConfZ
+License: MIT
+Keywords: Configuration Management,Config Management
+Author: Zühlke
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: python-dotenv (>=0.19.2,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://confz.readthedocs.io
+Project-URL: Repository, https://github.com/Zuehlke/ConfZ
+Description-Content-Type: text/markdown
 
-packages = \
-['confz', 'confz.loaders']
+# ConfZ – Pydantic Config Management
 
-package_data = \
-{'': ['*']}
+[![test](https://github.com/Zuehlke/ConfZ/actions/workflows/test.yml/badge.svg)](https://github.com/Zuehlke/ConfZ/actions/workflows/test.yml)
+[![documentation](https://readthedocs.org/projects/confz/badge/?version=latest)](https://confz.readthedocs.io/en/latest/)
+[![coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)](https://github.com/Zuehlke/ConfZ/actions/workflows/coverage.yml)  <!-- hard-code because can not merge if below 100 -->
+[![python](https://img.shields.io/pypi/pyversions/confz)](https://pypi.org/project/confz/)
+[![pypi](https://img.shields.io/pypi/v/confz)](https://pypi.org/project/confz/)
 
-install_requires = \
-['PyYAML>=5.4.1,<7.0.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'python-dotenv>=0.19.2,<0.22.0',
- 'toml>=0.10.2,<0.11.0']
-
-setup_kwargs = {
-    'name': 'confz',
-    'version': '1.8.1',
-    'description': 'ConfZ is a configuration management library for Python based on pydantic.',
-    'long_description': '# ConfZ – Pydantic Config Management\n\n[![test](https://github.com/Zuehlke/ConfZ/actions/workflows/test.yml/badge.svg)](https://github.com/Zuehlke/ConfZ/actions/workflows/test.yml)\n[![documentation](https://readthedocs.org/projects/confz/badge/?version=latest)](https://confz.readthedocs.io/en/latest/)\n[![coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)](https://github.com/Zuehlke/ConfZ/actions/workflows/coverage.yml)  <!-- hard-code because can not merge if below 100 -->\n[![python](https://img.shields.io/pypi/pyversions/confz)](https://pypi.org/project/confz/)\n[![pypi](https://img.shields.io/pypi/v/confz)](https://pypi.org/project/confz/)\n\n`ConfZ` is a configuration management library for Python based on [pydantic](https://pydantic-docs.helpmanual.io/).\nIt easily allows you to\n\n* load your configuration from config files, environment variables, command line arguments and more\n* transform the loaded data into a desired format and validate it\n* access the results as Python dataclass-like objects with full IDE support\n\nIt furthermore supports you in common use cases like:\n\n* Multiple environments\n* Singleton with lazy loading\n* Config changes for unit tests\n* Custom config sources\n\n\n## :package: Installation\n\n`ConfZ` is on [PyPI](https://pypi.org/project/confz/) and can be installed with pip:\n\n```shell\npip install confz\n```\n\n\n## :rocket: Quick Start\n\nThe first step of using `ConfZ` is to declare your config classes and sources, for example in `config.py`:\n\n```python\nfrom pathlib import Path\n\nfrom confz import ConfZ, ConfZFileSource\nfrom pydantic import SecretStr, AnyUrl\n\nclass DBConfig(ConfZ):\n    user: str\n    password: SecretStr\n\nclass APIConfig(ConfZ):\n    host: AnyUrl\n    port: int\n    db: DBConfig\n\n    CONFIG_SOURCES = ConfZFileSource(file=\'/path/to/config.yml\')\n```\n\nThanks to [pydantic](https://pydantic-docs.helpmanual.io/), you can use a wide variety of\n[field types](https://pydantic-docs.helpmanual.io/usage/types/) and\n[validators](https://pydantic-docs.helpmanual.io/usage/validators/).\n\nFrom now on, in any other file, you can access your config directly:\n\n```python\nfrom config import APIConfig\n\nprint(f"Serving API at {APIConfig().host}, port {APIConfig().port}.")\n```\n\nAs can be seen, the config does neither have to be loaded explicitly, nor instantiated globally. `ConfZ` automatically\nloads your config as defined in `CONFIG_SOURCES` the first time you access it. Thanks to its singleton mechanism, this\nhappens the first time only, afterwards you get back a cached,\n[immutable](https://pydantic-docs.helpmanual.io/usage/models/#faux-immutability) instance, behaving like any other\n_pydantic_ instance.\n\n```python\nassert APIConfig() is APIConfig()   # true because of singleton mechanism\nAPIConfig().port = 1234             # raises an error because of immutability\nAPIConfig().json()                  # call pydantic\'s method to get a json representation\n```\n\n**Note:** While the implicit and hidden loading of your config might be surprising and feel a bit like Python magic at\nfirst, it allows you to reduce a lot of boilerplate. Instead of having to load your config explicitly and then passing\nit down to all code layers that need it, you can directly access it from anywhere by just importing your config class\nand accessing for example `APIConfig().db.user` directly.\n\n### More Config Sources\n\n`ConfZ` is highly flexible in defining the source of your config. Do you have multiple environments? No Problem:\n\n```python\nfrom pathlib import Path\n\nfrom confz import ConfZ, ConfZFileSource\n\nclass MyConfig(ConfZ):\n    ...\n    CONFIG_SOURCES = ConfZFileSource(\n        folder=\'/path/to/config/folder\',\n        file_from_env=\'ENVIRONMENT\'\n    )\n```\n\nYour config file can now be defined in the environment variable `ENVIRONMENT` and is relative to `folder`.\n\nYou can also provide a list as config source and read for example from environment variables including a .env file and\nfrom command line arguments:\n\n```python\nfrom pathlib import Path\nfrom confz import ConfZ, ConfZEnvSource, ConfZCLArgSource\n\nclass MyConfig(ConfZ):\n    ...\n    CONFIG_SOURCES = [\n        ConfZEnvSource(allow_all=True, file=".env.local"),\n        ConfZCLArgSource(prefix=\'conf_\')\n    ]\n```\n\n`ConfZ` now tries to populate your config either from environment variables having the same name as your attributes or\nby reading command line arguments that start with `conf_`. Recursive models are supported too, for example if you want\nto control the user-name in the API above, you can either set the environment variable `DB.USER` or pass the command\nline argument `--conf_db.user`.\n\n### Explicit Loading\n\nIn some scenarios, the config should not be a global singleton, but loaded explicitly and passed around locally.\nInstead of defining `CONFIG_SOURCES` as class variable, the sources can also be defined in the constructor directly:\n\n```python\nfrom pathlib import Path\n\nfrom confz import ConfZ, ConfZFileSource, ConfZEnvSource\n\nclass MyConfig(ConfZ):\n    number: int\n    text: str\n\nconfig1 = MyConfig(config_sources=ConfZFileSource(file=\'/path/to/config.yml\'))\nconfig2 = MyConfig(config_sources=ConfZEnvSource(prefix=\'CONF_\', allow=[\'text\']), number=1)\nconfig3 = MyConfig(number=1, text=\'hello world\')\n```\n\nAs can be seen, additional keyword-arguments can be provided as well.\n\n**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `ConfZ`\nbehaves like a regular _pydantic_ class.\n\n### Change Config Values\n\nIn some scenarios, you might want to change your config values, for example within a unit test. However, if you set the\n`CONFIG_SOURCES` class variable, this is not directly possible. To overcome this, every config class provides a context\nmanager to temporarily change your config:\n\n```python\nfrom pathlib import Path\n\nfrom confz import ConfZ, ConfZFileSource, ConfZDataSource\n\nclass MyConfig(ConfZ):\n    number: int\n    CONFIG_SOURCES = ConfZFileSource(file="/path/to/config.yml")\n\nprint(MyConfig().number)                            # will print the value from the config-file\n\nnew_source = ConfZDataSource(data={\'number\': 42})\nwith MyConfig.change_config_sources(new_source):\n    print(MyConfig().number)                        # will print \'42\'\n\nprint(MyConfig().number)                            # will print the value from the config-file again\n```\n\n### Early Validation\n\nBy default, your config gets loaded the first time you instantiate the class, e.g. with `MyConfig().attribute`. This\nprevents side effects like loading a file while you import your config classes. If the config class cannot populate all\nmandatory fields in the correct format, _pydantic_ will raise an error at this point. To make sure this does not happen\nin an inconvenient moment, you can also instruct `ConfZ` to load all configs beforehand:\n\n```python\nfrom confz import validate_all_configs\n\nif __name__ == \'__main__\':\n    validate_all_configs()\n    # your application code\n```\n\nThe function `validate_all_configs` will instantiate all config classes defined in your code at any (reachable)\nlocation that have `CONFIG_SOURCES` set.\n\n\n## :book: Documentation\n\nNow you\'ve seen the two ways how `ConfZ` can be used: With class variable config sources, unlocking a singleton with\nlazy loading, or with keyword argument config sources, allowing to directly load your config values. In both cases,\ndefining your config sources from files, command line arguments and environment variables is highly flexible\n(and also extendable, by the way), while _pydantic_ still makes sure that everything matches your expectations in the\nend. You\'ve also seen how to temporarily change your config for example in unit tests and how to validate\nyour singleton config classes early in the code already.\n\nThe full documentation of `ConfZ`\'s features can be found at [readthedocs](https://confz.readthedocs.io/).\n\n\n## :information_source: About\n\n`ConfZ` was programmed and will be maintained by [Zühlke](https://www.zuehlke.com).\nThe first version was realized by [Silvan](https://github.com/silvanmelchior).\nSpecial thanks to Iwan with his [ConfMe](https://github.com/iwanbolzern/ConfMe), which inspired this project.\n\nWant to contribute to `ConfZ`? Check out the contribution [instruction & guidelines](CONTRIBUTING.md).\n',
-    'author': 'Zühlke',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Zuehlke/ConfZ',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+`ConfZ` is a configuration management library for Python based on [pydantic](https://pydantic-docs.helpmanual.io/).
+It easily allows you to
 
+* load your configuration from config files, environment variables, command line arguments and more
+* transform the loaded data into a desired format and validate it
+* access the results as Python dataclass-like objects with full IDE support
+
+It furthermore supports you in common use cases like:
+
+* Multiple environments
+* Singleton with lazy loading
+* Config changes for unit tests
+* Custom config sources
+
+
+## :package: Installation
+
+`ConfZ` is on [PyPI](https://pypi.org/project/confz/) and can be installed with pip:
+
+```shell
+pip install confz
+```
+
+
+## :rocket: Quick Start
+
+The first step of using `ConfZ` is to declare your config classes and sources, for example in `config.py`:
+
+```python
+from pathlib import Path
+
+from confz import ConfZ, ConfZFileSource
+from pydantic import SecretStr, AnyUrl
+
+class DBConfig(ConfZ):
+    user: str
+    password: SecretStr
+
+class APIConfig(ConfZ):
+    host: AnyUrl
+    port: int
+    db: DBConfig
+
+    CONFIG_SOURCES = ConfZFileSource(file='/path/to/config.yml')
+```
+
+Thanks to [pydantic](https://pydantic-docs.helpmanual.io/), you can use a wide variety of
+[field types](https://pydantic-docs.helpmanual.io/usage/types/) and
+[validators](https://pydantic-docs.helpmanual.io/usage/validators/).
+
+From now on, in any other file, you can access your config directly:
+
+```python
+from config import APIConfig
+
+print(f"Serving API at {APIConfig().host}, port {APIConfig().port}.")
+```
+
+As can be seen, the config does neither have to be loaded explicitly, nor instantiated globally. `ConfZ` automatically
+loads your config as defined in `CONFIG_SOURCES` the first time you access it. Thanks to its singleton mechanism, this
+happens the first time only, afterwards you get back a cached,
+[immutable](https://pydantic-docs.helpmanual.io/usage/models/#faux-immutability) instance, behaving like any other
+_pydantic_ instance.
+
+```python
+assert APIConfig() is APIConfig()   # true because of singleton mechanism
+APIConfig().port = 1234             # raises an error because of immutability
+APIConfig().json()                  # call pydantic's method to get a json representation
+```
+
+**Note:** While the implicit and hidden loading of your config might be surprising and feel a bit like Python magic at
+first, it allows you to reduce a lot of boilerplate. Instead of having to load your config explicitly and then passing
+it down to all code layers that need it, you can directly access it from anywhere by just importing your config class
+and accessing for example `APIConfig().db.user` directly.
+
+### More Config Sources
+
+`ConfZ` is highly flexible in defining the source of your config. Do you have multiple environments? No Problem:
+
+```python
+from pathlib import Path
+
+from confz import ConfZ, ConfZFileSource
+
+class MyConfig(ConfZ):
+    ...
+    CONFIG_SOURCES = ConfZFileSource(
+        folder='/path/to/config/folder',
+        file_from_env='ENVIRONMENT'
+    )
+```
+
+Your config file can now be defined in the environment variable `ENVIRONMENT` and is relative to `folder`.
+
+You can also provide a list as config source and read for example from environment variables including a .env file and
+from command line arguments:
+
+```python
+from pathlib import Path
+from confz import ConfZ, ConfZEnvSource, ConfZCLArgSource
+
+class MyConfig(ConfZ):
+    ...
+    CONFIG_SOURCES = [
+        ConfZEnvSource(allow_all=True, file=".env.local"),
+        ConfZCLArgSource(prefix='conf_')
+    ]
+```
+
+`ConfZ` now tries to populate your config either from environment variables having the same name as your attributes or
+by reading command line arguments that start with `conf_`. Recursive models are supported too, for example if you want
+to control the user-name in the API above, you can either set the environment variable `DB.USER` or pass the command
+line argument `--conf_db.user`.
+
+### Explicit Loading
+
+In some scenarios, the config should not be a global singleton, but loaded explicitly and passed around locally.
+Instead of defining `CONFIG_SOURCES` as class variable, the sources can also be defined in the constructor directly:
+
+```python
+from pathlib import Path
+
+from confz import ConfZ, ConfZFileSource, ConfZEnvSource
+
+class MyConfig(ConfZ):
+    number: int
+    text: str
+
+config1 = MyConfig(config_sources=ConfZFileSource(file='/path/to/config.yml'))
+config2 = MyConfig(config_sources=ConfZEnvSource(prefix='CONF_', allow=['text']), number=1)
+config3 = MyConfig(number=1, text='hello world')
+```
+
+As can be seen, additional keyword-arguments can be provided as well.
+
+**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `ConfZ`
+behaves like a regular _pydantic_ class.
+
+### Change Config Values
+
+In some scenarios, you might want to change your config values, for example within a unit test. However, if you set the
+`CONFIG_SOURCES` class variable, this is not directly possible. To overcome this, every config class provides a context
+manager to temporarily change your config:
+
+```python
+from pathlib import Path
+
+from confz import ConfZ, ConfZFileSource, ConfZDataSource
+
+class MyConfig(ConfZ):
+    number: int
+    CONFIG_SOURCES = ConfZFileSource(file="/path/to/config.yml")
+
+print(MyConfig().number)                            # will print the value from the config-file
+
+new_source = ConfZDataSource(data={'number': 42})
+with MyConfig.change_config_sources(new_source):
+    print(MyConfig().number)                        # will print '42'
+
+print(MyConfig().number)                            # will print the value from the config-file again
+```
+
+### Early Validation
+
+By default, your config gets loaded the first time you instantiate the class, e.g. with `MyConfig().attribute`. This
+prevents side effects like loading a file while you import your config classes. If the config class cannot populate all
+mandatory fields in the correct format, _pydantic_ will raise an error at this point. To make sure this does not happen
+in an inconvenient moment, you can also instruct `ConfZ` to load all configs beforehand:
+
+```python
+from confz import validate_all_configs
+
+if __name__ == '__main__':
+    validate_all_configs()
+    # your application code
+```
+
+The function `validate_all_configs` will instantiate all config classes defined in your code at any (reachable)
+location that have `CONFIG_SOURCES` set.
+
+
+## :book: Documentation
+
+Now you've seen the two ways how `ConfZ` can be used: With class variable config sources, unlocking a singleton with
+lazy loading, or with keyword argument config sources, allowing to directly load your config values. In both cases,
+defining your config sources from files, command line arguments and environment variables is highly flexible
+(and also extendable, by the way), while _pydantic_ still makes sure that everything matches your expectations in the
+end. You've also seen how to temporarily change your config for example in unit tests and how to validate
+your singleton config classes early in the code already.
+
+The full documentation of `ConfZ`'s features can be found at [readthedocs](https://confz.readthedocs.io/).
+
+
+## :information_source: About
+
+`ConfZ` was programmed and will be maintained by [Zühlke](https://www.zuehlke.com).
+The first version was realized by [Silvan](https://github.com/silvanmelchior).
+Special thanks to Iwan with his [ConfMe](https://github.com/iwanbolzern/ConfMe), which inspired this project.
+
+Want to contribute to `ConfZ`? Check out the contribution [instruction & guidelines](CONTRIBUTING.md).
 
-setup(**setup_kwargs)
```

