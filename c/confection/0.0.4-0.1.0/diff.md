# Comparing `tmp/confection-0.0.4.tar.gz` & `tmp/confection-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confection-0.0.4.tar", last modified: Tue Jan 10 10:42:37 2023, max compression
+gzip compressed data, was "confection-0.1.0.tar", last modified: Thu Jun 29 08:12:12 2023, max compression
```

## Comparing `confection-0.0.4.tar` & `confection-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:37.537575 confection-0.0.4/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-01-10 10:42:18.000000 confection-0.0.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-01-10 10:42:18.000000 confection-0.0.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    18875 2023-01-10 10:42:37.537575 confection-0.0.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    17792 2023-01-10 10:42:18.000000 confection-0.0.4/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:37.533575 confection-0.0.4/confection/
--rw-r--r--   0 vsts      (1001) docker     (122)    46251 2023-01-10 10:42:18.000000 confection-0.0.4/confection/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:18.000000 confection-0.0.4/confection/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:37.537575 confection-0.0.4/confection/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:18.000000 confection-0.0.4/confection/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      488 2023-01-10 10:42:18.000000 confection-0.0.4/confection/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)    52446 2023-01-10 10:42:18.000000 confection-0.0.4/confection/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3627 2023-01-10 10:42:18.000000 confection-0.0.4/confection/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1485 2023-01-10 10:42:18.000000 confection-0.0.4/confection/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 10:42:37.533575 confection-0.0.4/confection.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    18875 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 10:42:37.000000 confection-0.0.4/confection.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       86 2023-01-10 10:42:18.000000 confection-0.0.4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1374 2023-01-10 10:42:37.537575 confection-0.0.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-10 10:42:18.000000 confection-0.0.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-06-29 08:12:00.000000 confection-0.1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-06-29 08:12:00.000000 confection-0.1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    18832 2023-06-29 08:12:12.103952 confection-0.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    17749 2023-06-29 08:12:00.000000 confection-0.1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection/
+-rw-r--r--   0 vsts      (1001) docker     (122)    46489 2023-06-29 08:12:00.000000 confection-0.1.0/confection/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:00.000000 confection-0.1.0/confection/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      488 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53132 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/test_frozen_structures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3627 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4074 2023-06-29 08:12:00.000000 confection-0.1.0/confection/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18832 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      481 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-29 08:12:11.000000 confection-0.1.0/confection.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       86 2023-06-29 08:12:00.000000 confection-0.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1374 2023-06-29 08:12:12.103952 confection-0.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-06-29 08:12:00.000000 confection-0.1.0/setup.py
```

### Comparing `confection-0.0.4/LICENSE` & `confection-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `confection-0.0.4/PKG-INFO` & `confection-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.0.4
+Version: 0.1.0
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,32 +26,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Confection: The sweetest config system for Python
 
-`confection` :candy: is a lightweight library that offers a **configuration system** letting you conveniently describe arbitrary 
-trees of objects.
+`confection` :candy: is a lightweight library that offers a **configuration
+system** letting you conveniently describe arbitrary trees of objects.
 
-Configuration is a huge challenge for machine-learning code because you may want to expose almost any
-detail of any function as a hyperparameter. The setting you want to expose might be arbitrarily far
-down in your call stack, so it might need to pass all the way through the CLI or REST API,
-through any number of intermediate functions, affecting the interface of everything along the way.
-And then once those settings are added, they become hard to remove later. Default values also
-become hard to change without breaking backwards compatibility.
-
-To solve this problem, `confection` offers a config system that lets you easily describe arbitrary trees of objects.
-The objects can be created via function calls you register using a simple decorator syntax. You can even version the
-functions you create, allowing you to make improvements without breaking backwards compatibility. The most similar
-config system we’re aware of is [Gin](https://github.com/google/gin-config), which uses a similar syntax, and also 
-allows you to link the configuration system to functions in your code using a decorator. `confection`'s config system is 
-simpler and emphasizes a different workflow via a subset of Gin’s functionality.
+Configuration is a huge challenge for machine-learning code because you may want
+to expose almost any detail of any function as a hyperparameter. The setting you
+want to expose might be arbitrarily far down in your call stack, so it might
+need to pass all the way through the CLI or REST API, through any number of
+intermediate functions, affecting the interface of everything along the way. And
+then once those settings are added, they become hard to remove later. Default
+values also become hard to change without breaking backwards compatibility.
+
+To solve this problem, `confection` offers a config system that lets you easily
+describe arbitrary trees of objects. The objects can be created via function
+calls you register using a simple decorator syntax. You can even version the
+functions you create, allowing you to make improvements without breaking
+backwards compatibility. The most similar config system we’re aware of is
+[Gin](https://github.com/google/gin-config), which uses a similar syntax, and
+also allows you to link the configuration system to functions in your code using
+a decorator. `confection`'s config system is simpler and emphasizes a different
+workflow via a subset of Gin’s functionality.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/14/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=28)
+[![tests](https://github.com/explosion/confection/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/confection/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/confection.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/confection/releases)
 [![pypi Version](https://img.shields.io/pypi/v/confection.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/confection/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/confection.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/confection)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## ⏳ Installation
 
@@ -97,37 +101,45 @@
   "nlp": {
     "use_vectors": false,
     "lang": "en"
   }
 }
 ```
 
-The config is divided into sections, with the section name in square brackets – for
-example, `[training]`. Within the sections, config values can be assigned to keys using `=`. Values can also be referenced
-from other sections using the dot notation and placeholders indicated by the dollar sign and curly braces. For example,
-`${training.use_vectors}` will receive the value of use_vectors in the training block. This is useful for settings that
-are shared across components.
-
-The config format has three main differences from Python’s built-in `configparser`:
-
-1. JSON-formatted values. `confection` passes all values through `json.loads` to interpret them. You can use atomic
-   values like strings, floats, integers or booleans, or you can use complex objects such as lists or maps.
-2. Structured sections. `confection` uses a dot notation to build nested sections. If you have a section named
-   `[section.subsection]`, `confection` will parse that into a nested structure, placing subsection within section.
-3. References to registry functions. If a key starts with `@`, `confection` will interpret its value as the name of a
-   function registry, load the function registered for that name and pass in the rest of the block as arguments. If type
-   hints are available on the function, the argument values (and return value of the function) will be validated against
-   them. This lets you express complex configurations, like a training pipeline where `batch_size` is populated by a
-   function that yields floats.
-
-There’s no pre-defined scheme you have to follow; how you set up the top-level sections is up to you. At the end of
-it, you’ll receive a dictionary with the values that you can use in your script – whether it’s complete initialized
+The config is divided into sections, with the section name in square brackets –
+for example, `[training]`. Within the sections, config values can be assigned to
+keys using `=`. Values can also be referenced from other sections using the dot
+notation and placeholders indicated by the dollar sign and curly braces. For
+example, `${training.use_vectors}` will receive the value of use_vectors in the
+training block. This is useful for settings that are shared across components.
+
+The config format has three main differences from Python’s built-in
+`configparser`:
+
+1. JSON-formatted values. `confection` passes all values through `json.loads` to
+   interpret them. You can use atomic values like strings, floats, integers or
+   booleans, or you can use complex objects such as lists or maps.
+2. Structured sections. `confection` uses a dot notation to build nested
+   sections. If you have a section named `[section.subsection]`, `confection`
+   will parse that into a nested structure, placing subsection within section.
+3. References to registry functions. If a key starts with `@`, `confection` will
+   interpret its value as the name of a function registry, load the function
+   registered for that name and pass in the rest of the block as arguments. If
+   type hints are available on the function, the argument values (and return
+   value of the function) will be validated against them. This lets you express
+   complex configurations, like a training pipeline where `batch_size` is
+   populated by a function that yields floats.
+
+There’s no pre-defined scheme you have to follow; how you set up the top-level
+sections is up to you. At the end of it, you’ll receive a dictionary with the
+values that you can use in your script – whether it’s complete initialized
 functions, or just basic settings.
 
-For instance, let’s say you want to define a new optimizer. You'd define its arguments in `config.cfg` like so:
+For instance, let’s say you want to define a new optimizer. You'd define its
+arguments in `config.cfg` like so:
 
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
@@ -158,18 +170,19 @@
 
 # Load the config file from disk, resolve it and fetch the instantiated optimizer object.
 config = Config().from_disk("./config.cfg")
 resolved = registry.resolve(config)
 optimizer = resolved["optimizer"]  # MyCoolOptimizer(learn_rate=0.001, gamma=1e-08)
 ```
 
-Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function in the "optimizers" registry and then
-call it with the arguments `learn_rate` and `gamma`. If the function has type annotations, it will also validate the
-input. For instance, if `learn_rate` is annotated as a float and the config defines a string, `confection` will raise an
-error.
+Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function
+in the "optimizers" registry and then call it with the arguments `learn_rate`
+and `gamma`. If the function has type annotations, it will also validate the
+input. For instance, if `learn_rate` is annotated as a float and the config
+defines a string, `confection` will raise an error.
 
 The Thinc documentation offers further information on the configuration system:
 
 - [recursive blocks](https://thinc.ai/docs/usage-config#registry-recursive)
 - [defining variable positional arguments](https://thinc.ai/docs/usage-config#registries-args)
 - [using interpolation](https://thinc.ai/docs/usage-config#config-interpolation)
 - [using custom registries](https://thinc.ai/docs/usage-config#registries-custom)
@@ -177,17 +190,18 @@
 - [using base schemas](https://thinc.ai/docs/usage-config#advanced-types-base-schema)
 - [filling a configuration with defaults](https://thinc.ai/docs/usage-config#advanced-types-fill-defaults)
 
 ## 🎛 API
 
 ### <kbd>class</kbd> `Config`
 
-This class holds the model and training [configuration](https://thinc.ai/docs/usage-config) and can load and save the
-INI-style configuration format from/to a string, file or bytes. The `Config` class is a subclass of `dict` and uses
-Python’s `ConfigParser` under the hood.
+This class holds the model and training
+[configuration](https://thinc.ai/docs/usage-config) and can load and save the
+INI-style configuration format from/to a string, file or bytes. The `Config`
+class is a subclass of `dict` and uses Python’s `ConfigParser` under the hood.
 
 #### <sup><kbd>method</kbd> `Config.__init__`</sup>
 
 Initialize a new `Config` object with optional data.
 
 ```python
 from confection import Config
@@ -316,16 +330,17 @@
 
 | Argument    | Type     | Description        |
 | ----------- | -------- | ------------------ |
 | **RETURNS** | `Config` | The copied config. |
 
 #### <sup><kbd>method</kbd> `Config.interpolate`</sup>
 
-Interpolate variables like `${section.value}` or `${section.subsection}` and return a copy of the config with interpolated
-values. Can be used if a config is loaded with `interpolate=False`, e.g. via `Config.from_str`.
+Interpolate variables like `${section.value}` or `${section.subsection}` and
+return a copy of the config with interpolated values. Can be used if a config is
+loaded with `interpolate=False`, e.g. via `Config.from_str`.
 
 ```python
 from confection import Config
 
 config_str = """
 [hyper_params]
 dropout = 0.2
@@ -341,23 +356,27 @@
 
 | Argument    | Type     | Description                                    |
 | ----------- | -------- | ---------------------------------------------- |
 | **RETURNS** | `Config` | A copy of the config with interpolated values. |
 
 ##### <sup><kbd>method</kbd> `Config.merge`</sup>
 
-Deep-merge two config objects, using the current config as the default. Only merges sections and dictionaries and not
-other values like lists. Values that are provided in the updates are overwritten in the base config, and any new values
-or sections are added. If a config value is a variable like `${section.key}` (e.g. if the config was loaded with
-`interpolate=False)`, **the variable is preferred**, even if the updates provide a different value. This ensures that variable
-references aren’t destroyed by a merge.
-
-> :warning: Note that blocks that refer to registered functions using the `@` syntax are only merged if they are
-> referring to the same functions. Otherwise, merging could easily produce invalid configs, since different functions
-> can take different arguments. If a block refers to a different function, it’s overwritten.
+Deep-merge two config objects, using the current config as the default. Only
+merges sections and dictionaries and not other values like lists. Values that
+are provided in the updates are overwritten in the base config, and any new
+values or sections are added. If a config value is a variable like
+`${section.key}` (e.g. if the config was loaded with `interpolate=False)`, **the
+variable is preferred**, even if the updates provide a different value. This
+ensures that variable references aren’t destroyed by a merge.
+
+> :warning: Note that blocks that refer to registered functions using the `@`
+> syntax are only merged if they are referring to the same functions. Otherwise,
+> merging could easily produce invalid configs, since different functions can
+> take different arguments. If a block refers to a different function, it’s
+> overwritten.
 
 ```python
 from confection import Config
 
 base_config_str = """
 [training]
 patience = 10
```

### Comparing `confection-0.0.4/README.md` & `confection-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Confection: The sweetest config system for Python
 
-`confection` :candy: is a lightweight library that offers a **configuration system** letting you conveniently describe arbitrary 
-trees of objects.
+`confection` :candy: is a lightweight library that offers a **configuration
+system** letting you conveniently describe arbitrary trees of objects.
 
-Configuration is a huge challenge for machine-learning code because you may want to expose almost any
-detail of any function as a hyperparameter. The setting you want to expose might be arbitrarily far
-down in your call stack, so it might need to pass all the way through the CLI or REST API,
-through any number of intermediate functions, affecting the interface of everything along the way.
-And then once those settings are added, they become hard to remove later. Default values also
-become hard to change without breaking backwards compatibility.
-
-To solve this problem, `confection` offers a config system that lets you easily describe arbitrary trees of objects.
-The objects can be created via function calls you register using a simple decorator syntax. You can even version the
-functions you create, allowing you to make improvements without breaking backwards compatibility. The most similar
-config system we’re aware of is [Gin](https://github.com/google/gin-config), which uses a similar syntax, and also 
-allows you to link the configuration system to functions in your code using a decorator. `confection`'s config system is 
-simpler and emphasizes a different workflow via a subset of Gin’s functionality.
+Configuration is a huge challenge for machine-learning code because you may want
+to expose almost any detail of any function as a hyperparameter. The setting you
+want to expose might be arbitrarily far down in your call stack, so it might
+need to pass all the way through the CLI or REST API, through any number of
+intermediate functions, affecting the interface of everything along the way. And
+then once those settings are added, they become hard to remove later. Default
+values also become hard to change without breaking backwards compatibility.
+
+To solve this problem, `confection` offers a config system that lets you easily
+describe arbitrary trees of objects. The objects can be created via function
+calls you register using a simple decorator syntax. You can even version the
+functions you create, allowing you to make improvements without breaking
+backwards compatibility. The most similar config system we’re aware of is
+[Gin](https://github.com/google/gin-config), which uses a similar syntax, and
+also allows you to link the configuration system to functions in your code using
+a decorator. `confection`'s config system is simpler and emphasizes a different
+workflow via a subset of Gin’s functionality.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/14/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=28)
+[![tests](https://github.com/explosion/confection/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/confection/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/confection.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/confection/releases)
 [![pypi Version](https://img.shields.io/pypi/v/confection.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/confection/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/confection.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/confection)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## ⏳ Installation
 
@@ -69,37 +73,45 @@
   "nlp": {
     "use_vectors": false,
     "lang": "en"
   }
 }
 ```
 
-The config is divided into sections, with the section name in square brackets – for
-example, `[training]`. Within the sections, config values can be assigned to keys using `=`. Values can also be referenced
-from other sections using the dot notation and placeholders indicated by the dollar sign and curly braces. For example,
-`${training.use_vectors}` will receive the value of use_vectors in the training block. This is useful for settings that
-are shared across components.
-
-The config format has three main differences from Python’s built-in `configparser`:
-
-1. JSON-formatted values. `confection` passes all values through `json.loads` to interpret them. You can use atomic
-   values like strings, floats, integers or booleans, or you can use complex objects such as lists or maps.
-2. Structured sections. `confection` uses a dot notation to build nested sections. If you have a section named
-   `[section.subsection]`, `confection` will parse that into a nested structure, placing subsection within section.
-3. References to registry functions. If a key starts with `@`, `confection` will interpret its value as the name of a
-   function registry, load the function registered for that name and pass in the rest of the block as arguments. If type
-   hints are available on the function, the argument values (and return value of the function) will be validated against
-   them. This lets you express complex configurations, like a training pipeline where `batch_size` is populated by a
-   function that yields floats.
-
-There’s no pre-defined scheme you have to follow; how you set up the top-level sections is up to you. At the end of
-it, you’ll receive a dictionary with the values that you can use in your script – whether it’s complete initialized
+The config is divided into sections, with the section name in square brackets –
+for example, `[training]`. Within the sections, config values can be assigned to
+keys using `=`. Values can also be referenced from other sections using the dot
+notation and placeholders indicated by the dollar sign and curly braces. For
+example, `${training.use_vectors}` will receive the value of use_vectors in the
+training block. This is useful for settings that are shared across components.
+
+The config format has three main differences from Python’s built-in
+`configparser`:
+
+1. JSON-formatted values. `confection` passes all values through `json.loads` to
+   interpret them. You can use atomic values like strings, floats, integers or
+   booleans, or you can use complex objects such as lists or maps.
+2. Structured sections. `confection` uses a dot notation to build nested
+   sections. If you have a section named `[section.subsection]`, `confection`
+   will parse that into a nested structure, placing subsection within section.
+3. References to registry functions. If a key starts with `@`, `confection` will
+   interpret its value as the name of a function registry, load the function
+   registered for that name and pass in the rest of the block as arguments. If
+   type hints are available on the function, the argument values (and return
+   value of the function) will be validated against them. This lets you express
+   complex configurations, like a training pipeline where `batch_size` is
+   populated by a function that yields floats.
+
+There’s no pre-defined scheme you have to follow; how you set up the top-level
+sections is up to you. At the end of it, you’ll receive a dictionary with the
+values that you can use in your script – whether it’s complete initialized
 functions, or just basic settings.
 
-For instance, let’s say you want to define a new optimizer. You'd define its arguments in `config.cfg` like so:
+For instance, let’s say you want to define a new optimizer. You'd define its
+arguments in `config.cfg` like so:
 
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
@@ -130,18 +142,19 @@
 
 # Load the config file from disk, resolve it and fetch the instantiated optimizer object.
 config = Config().from_disk("./config.cfg")
 resolved = registry.resolve(config)
 optimizer = resolved["optimizer"]  # MyCoolOptimizer(learn_rate=0.001, gamma=1e-08)
 ```
 
-Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function in the "optimizers" registry and then
-call it with the arguments `learn_rate` and `gamma`. If the function has type annotations, it will also validate the
-input. For instance, if `learn_rate` is annotated as a float and the config defines a string, `confection` will raise an
-error.
+Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function
+in the "optimizers" registry and then call it with the arguments `learn_rate`
+and `gamma`. If the function has type annotations, it will also validate the
+input. For instance, if `learn_rate` is annotated as a float and the config
+defines a string, `confection` will raise an error.
 
 The Thinc documentation offers further information on the configuration system:
 
 - [recursive blocks](https://thinc.ai/docs/usage-config#registry-recursive)
 - [defining variable positional arguments](https://thinc.ai/docs/usage-config#registries-args)
 - [using interpolation](https://thinc.ai/docs/usage-config#config-interpolation)
 - [using custom registries](https://thinc.ai/docs/usage-config#registries-custom)
@@ -149,17 +162,18 @@
 - [using base schemas](https://thinc.ai/docs/usage-config#advanced-types-base-schema)
 - [filling a configuration with defaults](https://thinc.ai/docs/usage-config#advanced-types-fill-defaults)
 
 ## 🎛 API
 
 ### <kbd>class</kbd> `Config`
 
-This class holds the model and training [configuration](https://thinc.ai/docs/usage-config) and can load and save the
-INI-style configuration format from/to a string, file or bytes. The `Config` class is a subclass of `dict` and uses
-Python’s `ConfigParser` under the hood.
+This class holds the model and training
+[configuration](https://thinc.ai/docs/usage-config) and can load and save the
+INI-style configuration format from/to a string, file or bytes. The `Config`
+class is a subclass of `dict` and uses Python’s `ConfigParser` under the hood.
 
 #### <sup><kbd>method</kbd> `Config.__init__`</sup>
 
 Initialize a new `Config` object with optional data.
 
 ```python
 from confection import Config
@@ -288,16 +302,17 @@
 
 | Argument    | Type     | Description        |
 | ----------- | -------- | ------------------ |
 | **RETURNS** | `Config` | The copied config. |
 
 #### <sup><kbd>method</kbd> `Config.interpolate`</sup>
 
-Interpolate variables like `${section.value}` or `${section.subsection}` and return a copy of the config with interpolated
-values. Can be used if a config is loaded with `interpolate=False`, e.g. via `Config.from_str`.
+Interpolate variables like `${section.value}` or `${section.subsection}` and
+return a copy of the config with interpolated values. Can be used if a config is
+loaded with `interpolate=False`, e.g. via `Config.from_str`.
 
 ```python
 from confection import Config
 
 config_str = """
 [hyper_params]
 dropout = 0.2
@@ -313,23 +328,27 @@
 
 | Argument    | Type     | Description                                    |
 | ----------- | -------- | ---------------------------------------------- |
 | **RETURNS** | `Config` | A copy of the config with interpolated values. |
 
 ##### <sup><kbd>method</kbd> `Config.merge`</sup>
 
-Deep-merge two config objects, using the current config as the default. Only merges sections and dictionaries and not
-other values like lists. Values that are provided in the updates are overwritten in the base config, and any new values
-or sections are added. If a config value is a variable like `${section.key}` (e.g. if the config was loaded with
-`interpolate=False)`, **the variable is preferred**, even if the updates provide a different value. This ensures that variable
-references aren’t destroyed by a merge.
-
-> :warning: Note that blocks that refer to registered functions using the `@` syntax are only merged if they are
-> referring to the same functions. Otherwise, merging could easily produce invalid configs, since different functions
-> can take different arguments. If a block refers to a different function, it’s overwritten.
+Deep-merge two config objects, using the current config as the default. Only
+merges sections and dictionaries and not other values like lists. Values that
+are provided in the updates are overwritten in the base config, and any new
+values or sections are added. If a config value is a variable like
+`${section.key}` (e.g. if the config was loaded with `interpolate=False)`, **the
+variable is preferred**, even if the updates provide a different value. This
+ensures that variable references aren’t destroyed by a merge.
+
+> :warning: Note that blocks that refer to registered functions using the `@`
+> syntax are only merged if they are referring to the same functions. Otherwise,
+> merging could easily produce invalid configs, since different functions can
+> take different arguments. If a block refers to a different function, it’s
+> overwritten.
 
 ```python
 from confection import Config
 
 base_config_str = """
 [training]
 patience = 10
```

### Comparing `confection-0.0.4/confection/__init__.py` & `confection-0.1.0/confection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from pydantic.fields import ModelField
 import srsly
 import catalogue
 import inspect
 import io
 import copy
 import re
+import warnings
 
-from .util import Decorator
+from .util import Decorator, SimpleFrozenDict, SimpleFrozenList
 
 # Field used for positional arguments, e.g. [section.*.xyz]. The alias is
 # required for the schema (shouldn't clash with user-defined arg names)
 ARGS_FIELD = "*"
 ARGS_FIELD_ALIAS = "VARIABLE_POSITIONAL_ARGS"
 # Aliases for fields that would otherwise shadow pydantic attributes. Can be any
 # string, so we're using name + space so it looks the same in error messages etc.
@@ -39,14 +40,20 @@
     def before_read(self, parser, section, option, value):
         # If we're dealing with a quoted string as the interpolation value,
         # make sure we load and unquote it so we don't end up with '"value"'
         try:
             json_value = srsly.json_loads(value)
             if isinstance(json_value, str) and json_value not in JSON_EXCEPTIONS:
                 value = json_value
+        except ValueError:
+            if value and value[0] == value[-1] == "'":
+                warnings.warn(
+                    f"The value [{value}] seems to be single-quoted, but values "
+                    "use JSON formatting, which requires double quotes."
+                )
         except Exception:
             pass
         return super().before_read(parser, section, option, value)
 
     def before_get(self, parser, section, option, value, defaults):
         # Mostly copy-pasted from the built-in configparser implementation.
         L = []
@@ -262,16 +269,14 @@
         # If value is a string and it contains a variable, use original value
         # (not interpreted string, which could lead to double quotes:
         # ${x.y} -> "${x.y}" -> "'${x.y}'"). Make sure to check it's a string,
         # so we're not keeping lists as strings.
         # NOTE: This currently can't handle uninterpolated values like [${x.y}]!
         if isinstance(result, str) and VARIABLE_RE.search(value):
             result = value
-        if isinstance(result, list):
-            return [self._interpret_value(v) for v in result]
         return result
 
     def _get_section_ref(self, value: Any, *, parent: List[str] = []) -> Any:
         """Get a single section reference."""
         if isinstance(value, str) and value.startswith(f'"{SECTION_PREFIX}'):
             value = try_load_json(value)
         if isinstance(value, str) and value.startswith(SECTION_PREFIX):
@@ -343,15 +348,15 @@
         )
         return dict(sorted(data.items(), key=sort_key))
 
     def _set_overrides(self, config: "ConfigParser", overrides: Dict[str, Any]) -> None:
         """Set overrides in the ConfigParser before config is interpreted."""
         err_title = "Error parsing config overrides"
         for key, value in overrides.items():
-            err_msg = "not a section value that can be overwritten"
+            err_msg = "not a section value that can be overridden"
             err = [{"loc": key.split("."), "msg": err_msg}]
             if "." not in key:
                 raise ConfigValidationError(errors=err, title=err_title)
             section, option = key.rsplit(".", 1)
             # Check for section and accept if option not in config[section]
             if section not in config:
                 raise ConfigValidationError(errors=err, title=err_title)
```

### Comparing `confection-0.0.4/confection/tests/test_config.py` & `confection-0.1.0/confection/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1375,7 +1375,31 @@
     [vars]
     a = "world"
     """
     overrides = {"vars.a": greeting}
     assert "${vars.a}" in str_cfg
     cfg = Config().from_str(str_cfg, overrides=overrides)
     assert expected in str(cfg)
+
+
+def test_warn_single_quotes():
+    str_cfg = f"""
+    [project]
+    commands = 'do stuff'
+    """
+
+    with pytest.warns(UserWarning, match="single-quoted"):
+        cfg = Config().from_str(str_cfg)
+
+    # should not warn if single quotes are in the middle
+    str_cfg = f"""
+    [project]
+    commands = some'thing
+    """
+    cfg = Config().from_str(str_cfg)
+
+
+def test_parse_strings_interpretable_as_ints():
+    """Test whether strings interpretable as integers are parsed correctly (i. e. as strings)."""
+    cfg = Config().from_str(f"""[a]\nfoo = [${{b.bar}}, "00${{b.bar}}", "y"]\n\n[b]\nbar = 3""")
+    assert cfg["a"]["foo"] == [3, "003", "y"]
+    assert cfg["b"]["bar"] == 3
```

### Comparing `confection-0.0.4/confection/tests/util.py` & `confection-0.1.0/confection/tests/util.py`

 * *Files identical despite different names*

### Comparing `confection-0.0.4/confection.egg-info/PKG-INFO` & `confection-0.1.0/confection.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.0.4
+Version: 0.1.0
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,32 +26,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Confection: The sweetest config system for Python
 
-`confection` :candy: is a lightweight library that offers a **configuration system** letting you conveniently describe arbitrary 
-trees of objects.
+`confection` :candy: is a lightweight library that offers a **configuration
+system** letting you conveniently describe arbitrary trees of objects.
 
-Configuration is a huge challenge for machine-learning code because you may want to expose almost any
-detail of any function as a hyperparameter. The setting you want to expose might be arbitrarily far
-down in your call stack, so it might need to pass all the way through the CLI or REST API,
-through any number of intermediate functions, affecting the interface of everything along the way.
-And then once those settings are added, they become hard to remove later. Default values also
-become hard to change without breaking backwards compatibility.
-
-To solve this problem, `confection` offers a config system that lets you easily describe arbitrary trees of objects.
-The objects can be created via function calls you register using a simple decorator syntax. You can even version the
-functions you create, allowing you to make improvements without breaking backwards compatibility. The most similar
-config system we’re aware of is [Gin](https://github.com/google/gin-config), which uses a similar syntax, and also 
-allows you to link the configuration system to functions in your code using a decorator. `confection`'s config system is 
-simpler and emphasizes a different workflow via a subset of Gin’s functionality.
+Configuration is a huge challenge for machine-learning code because you may want
+to expose almost any detail of any function as a hyperparameter. The setting you
+want to expose might be arbitrarily far down in your call stack, so it might
+need to pass all the way through the CLI or REST API, through any number of
+intermediate functions, affecting the interface of everything along the way. And
+then once those settings are added, they become hard to remove later. Default
+values also become hard to change without breaking backwards compatibility.
+
+To solve this problem, `confection` offers a config system that lets you easily
+describe arbitrary trees of objects. The objects can be created via function
+calls you register using a simple decorator syntax. You can even version the
+functions you create, allowing you to make improvements without breaking
+backwards compatibility. The most similar config system we’re aware of is
+[Gin](https://github.com/google/gin-config), which uses a similar syntax, and
+also allows you to link the configuration system to functions in your code using
+a decorator. `confection`'s config system is simpler and emphasizes a different
+workflow via a subset of Gin’s functionality.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/14/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=28)
+[![tests](https://github.com/explosion/confection/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/confection/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/confection.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/confection/releases)
 [![pypi Version](https://img.shields.io/pypi/v/confection.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/confection/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/confection.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/confection)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## ⏳ Installation
 
@@ -97,37 +101,45 @@
   "nlp": {
     "use_vectors": false,
     "lang": "en"
   }
 }
 ```
 
-The config is divided into sections, with the section name in square brackets – for
-example, `[training]`. Within the sections, config values can be assigned to keys using `=`. Values can also be referenced
-from other sections using the dot notation and placeholders indicated by the dollar sign and curly braces. For example,
-`${training.use_vectors}` will receive the value of use_vectors in the training block. This is useful for settings that
-are shared across components.
-
-The config format has three main differences from Python’s built-in `configparser`:
-
-1. JSON-formatted values. `confection` passes all values through `json.loads` to interpret them. You can use atomic
-   values like strings, floats, integers or booleans, or you can use complex objects such as lists or maps.
-2. Structured sections. `confection` uses a dot notation to build nested sections. If you have a section named
-   `[section.subsection]`, `confection` will parse that into a nested structure, placing subsection within section.
-3. References to registry functions. If a key starts with `@`, `confection` will interpret its value as the name of a
-   function registry, load the function registered for that name and pass in the rest of the block as arguments. If type
-   hints are available on the function, the argument values (and return value of the function) will be validated against
-   them. This lets you express complex configurations, like a training pipeline where `batch_size` is populated by a
-   function that yields floats.
-
-There’s no pre-defined scheme you have to follow; how you set up the top-level sections is up to you. At the end of
-it, you’ll receive a dictionary with the values that you can use in your script – whether it’s complete initialized
+The config is divided into sections, with the section name in square brackets –
+for example, `[training]`. Within the sections, config values can be assigned to
+keys using `=`. Values can also be referenced from other sections using the dot
+notation and placeholders indicated by the dollar sign and curly braces. For
+example, `${training.use_vectors}` will receive the value of use_vectors in the
+training block. This is useful for settings that are shared across components.
+
+The config format has three main differences from Python’s built-in
+`configparser`:
+
+1. JSON-formatted values. `confection` passes all values through `json.loads` to
+   interpret them. You can use atomic values like strings, floats, integers or
+   booleans, or you can use complex objects such as lists or maps.
+2. Structured sections. `confection` uses a dot notation to build nested
+   sections. If you have a section named `[section.subsection]`, `confection`
+   will parse that into a nested structure, placing subsection within section.
+3. References to registry functions. If a key starts with `@`, `confection` will
+   interpret its value as the name of a function registry, load the function
+   registered for that name and pass in the rest of the block as arguments. If
+   type hints are available on the function, the argument values (and return
+   value of the function) will be validated against them. This lets you express
+   complex configurations, like a training pipeline where `batch_size` is
+   populated by a function that yields floats.
+
+There’s no pre-defined scheme you have to follow; how you set up the top-level
+sections is up to you. At the end of it, you’ll receive a dictionary with the
+values that you can use in your script – whether it’s complete initialized
 functions, or just basic settings.
 
-For instance, let’s say you want to define a new optimizer. You'd define its arguments in `config.cfg` like so:
+For instance, let’s say you want to define a new optimizer. You'd define its
+arguments in `config.cfg` like so:
 
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
@@ -158,18 +170,19 @@
 
 # Load the config file from disk, resolve it and fetch the instantiated optimizer object.
 config = Config().from_disk("./config.cfg")
 resolved = registry.resolve(config)
 optimizer = resolved["optimizer"]  # MyCoolOptimizer(learn_rate=0.001, gamma=1e-08)
 ```
 
-Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function in the "optimizers" registry and then
-call it with the arguments `learn_rate` and `gamma`. If the function has type annotations, it will also validate the
-input. For instance, if `learn_rate` is annotated as a float and the config defines a string, `confection` will raise an
-error.
+Under the hood, `confection` will look up the `"my_cool_optimizer.v1"` function
+in the "optimizers" registry and then call it with the arguments `learn_rate`
+and `gamma`. If the function has type annotations, it will also validate the
+input. For instance, if `learn_rate` is annotated as a float and the config
+defines a string, `confection` will raise an error.
 
 The Thinc documentation offers further information on the configuration system:
 
 - [recursive blocks](https://thinc.ai/docs/usage-config#registry-recursive)
 - [defining variable positional arguments](https://thinc.ai/docs/usage-config#registries-args)
 - [using interpolation](https://thinc.ai/docs/usage-config#config-interpolation)
 - [using custom registries](https://thinc.ai/docs/usage-config#registries-custom)
@@ -177,17 +190,18 @@
 - [using base schemas](https://thinc.ai/docs/usage-config#advanced-types-base-schema)
 - [filling a configuration with defaults](https://thinc.ai/docs/usage-config#advanced-types-fill-defaults)
 
 ## 🎛 API
 
 ### <kbd>class</kbd> `Config`
 
-This class holds the model and training [configuration](https://thinc.ai/docs/usage-config) and can load and save the
-INI-style configuration format from/to a string, file or bytes. The `Config` class is a subclass of `dict` and uses
-Python’s `ConfigParser` under the hood.
+This class holds the model and training
+[configuration](https://thinc.ai/docs/usage-config) and can load and save the
+INI-style configuration format from/to a string, file or bytes. The `Config`
+class is a subclass of `dict` and uses Python’s `ConfigParser` under the hood.
 
 #### <sup><kbd>method</kbd> `Config.__init__`</sup>
 
 Initialize a new `Config` object with optional data.
 
 ```python
 from confection import Config
@@ -316,16 +330,17 @@
 
 | Argument    | Type     | Description        |
 | ----------- | -------- | ------------------ |
 | **RETURNS** | `Config` | The copied config. |
 
 #### <sup><kbd>method</kbd> `Config.interpolate`</sup>
 
-Interpolate variables like `${section.value}` or `${section.subsection}` and return a copy of the config with interpolated
-values. Can be used if a config is loaded with `interpolate=False`, e.g. via `Config.from_str`.
+Interpolate variables like `${section.value}` or `${section.subsection}` and
+return a copy of the config with interpolated values. Can be used if a config is
+loaded with `interpolate=False`, e.g. via `Config.from_str`.
 
 ```python
 from confection import Config
 
 config_str = """
 [hyper_params]
 dropout = 0.2
@@ -341,23 +356,27 @@
 
 | Argument    | Type     | Description                                    |
 | ----------- | -------- | ---------------------------------------------- |
 | **RETURNS** | `Config` | A copy of the config with interpolated values. |
 
 ##### <sup><kbd>method</kbd> `Config.merge`</sup>
 
-Deep-merge two config objects, using the current config as the default. Only merges sections and dictionaries and not
-other values like lists. Values that are provided in the updates are overwritten in the base config, and any new values
-or sections are added. If a config value is a variable like `${section.key}` (e.g. if the config was loaded with
-`interpolate=False)`, **the variable is preferred**, even if the updates provide a different value. This ensures that variable
-references aren’t destroyed by a merge.
-
-> :warning: Note that blocks that refer to registered functions using the `@` syntax are only merged if they are
-> referring to the same functions. Otherwise, merging could easily produce invalid configs, since different functions
-> can take different arguments. If a block refers to a different function, it’s overwritten.
+Deep-merge two config objects, using the current config as the default. Only
+merges sections and dictionaries and not other values like lists. Values that
+are provided in the updates are overwritten in the base config, and any new
+values or sections are added. If a config value is a variable like
+`${section.key}` (e.g. if the config was loaded with `interpolate=False)`, **the
+variable is preferred**, even if the updates provide a different value. This
+ensures that variable references aren’t destroyed by a merge.
+
+> :warning: Note that blocks that refer to registered functions using the `@`
+> syntax are only merged if they are referring to the same functions. Otherwise,
+> merging could easily produce invalid configs, since different functions can
+> take different arguments. If a block refers to a different function, it’s
+> overwritten.
 
 ```python
 from confection import Config
 
 base_config_str = """
 [training]
 patience = 10
```

### Comparing `confection-0.0.4/setup.cfg` & `confection-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.4
+version = 0.1.0
 description = The sweetest config system for Python
 url = https://github.com/explosion/confection
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

