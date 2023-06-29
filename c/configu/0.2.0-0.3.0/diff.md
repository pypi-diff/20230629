# Comparing `tmp/configu-0.2.0.tar.gz` & `tmp/configu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configu-0.2.0.tar", max compression
+gzip compressed data, was "configu-0.3.0.tar", max compression
```

## Comparing `configu-0.2.0.tar` & `configu-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1753 2023-06-22 12:18:20.254169 configu-0.2.0/README.md
--rw-r--r--   0        0        0      644 2023-06-22 12:18:20.254169 configu-0.2.0/configu/__init__.py
--rw-r--r--   0        0        0      182 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/__init__.py
--rw-r--r--   0        0        0    11244 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/eval_command.py
--rw-r--r--   0        0        0     1033 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/export_command.py
--rw-r--r--   0        0        0     2496 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/upsert_command.py
--rw-r--r--   0        0        0      423 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/__init__.py
--rw-r--r--   0        0        0      354 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/command.py
--rw-r--r--   0        0        0     6446 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_schema.py
--rw-r--r--   0        0        0     1383 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_set.py
--rw-r--r--   0        0        0      457 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_store.py
--rw-r--r--   0        0        0    11311 2023-06-22 12:18:54.814052 configu-0.2.0/configu/core/generated.py
--rw-r--r--   0        0        0      223 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/__init__.py
--rw-r--r--   0        0        0     2481 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/configu_store.py
--rw-r--r--   0        0        0     1326 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/in_memory_store.py
--rw-r--r--   0        0        0     2488 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/json_file_store.py
--rw-r--r--   0        0        0     1239 2023-06-22 12:18:20.254169 configu-0.2.0/configu/utils.py
--rw-r--r--   0        0        0     1815 2023-06-22 12:19:33.917935 configu-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 configu-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1753 2023-06-29 07:04:01.013370 configu-0.3.0/README.md
+-rw-r--r--   0        0        0      714 2023-06-29 07:04:01.013370 configu-0.3.0/configu/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/__init__.py
+-rw-r--r--   0        0        0    11921 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/eval_command.py
+-rw-r--r--   0        0        0     1033 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/export_command.py
+-rw-r--r--   0        0        0     3070 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/upsert_command.py
+-rw-r--r--   0        0        0      423 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/command.py
+-rw-r--r--   0        0        0     6880 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_schema.py
+-rw-r--r--   0        0        0     1822 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_set.py
+-rw-r--r--   0        0        0      995 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_store.py
+-rw-r--r--   0        0        0    11311 2023-06-29 07:04:29.245509 configu-0.3.0/configu/core/generated.py
+-rw-r--r--   0        0        0      342 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/__init__.py
+-rw-r--r--   0        0        0      904 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/aws_secrets_manager_store.py
+-rw-r--r--   0        0        0     2495 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/configu_store.py
+-rw-r--r--   0        0        0     1373 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/in_memory_store.py
+-rw-r--r--   0        0        0     2496 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/json_file_store.py
+-rw-r--r--   0        0        0     3271 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/key_value_store.py
+-rw-r--r--   0        0        0     1239 2023-06-29 07:04:01.013370 configu-0.3.0/configu/utils.py
+-rw-r--r--   0        0        0     1904 2023-06-29 07:05:02.477689 configu-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 configu-0.3.0/PKG-INFO
```

### Comparing `configu-0.2.0/README.md` & `configu-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `configu-0.2.0/configu/commands/eval_command.py` & `configu-0.3.0/configu/commands/eval_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,19 +64,32 @@
         "previous": Optional[EvalCommandReturn],
     },
     total=False,
 )
 
 
 class EvalCommand(Command[EvalCommandReturn]):
-    """"""
+    """
+    The Eval command is used to fetch and validate `Config`s from `ConfigStore`
+    on demand.
+    """
 
     parameters: EvalCommandParameters
 
     def __init__(self, parameters: EvalCommandParameters) -> None:
+        """
+        Creates a new EvalCommand.
+        :param parameters: dict
+            The command's parameters. Includes the following:
+             - store: the `ConfigStore` from which to fetch
+             - set: the `ConfigSet` to fetch
+             - schema: `ConfigSchema` to validate the config being fetched
+             - configs (optional): a dictionary of overrides to the fetched
+                `Config`s
+        """
         super().__init__(parameters)
 
     def _eval_from_configs_override(
         self, result: EvalCommandReturn
     ) -> EvalCommandReturn:
         if not self.parameters.get("configs"):
             return {}
@@ -268,14 +281,19 @@
                 )
                 template_keys.remove(key)
                 has_rendered_at_least_once = True
             should_render_templates = has_rendered_at_least_once
         return result
 
     def run(self):
+        """
+        Runs the eval command.
+        :return EvalCommandReturn:
+        Contains the command's results and metadata
+        """
         store = self.parameters["store"]
         set_ = self.parameters["set"]
         schema = self.parameters["schema"]
         store.init()
         schema_contents = ConfigSchema.parse(schema)
         result: EvalCommandReturn = {
             key: {
```

### Comparing `configu-0.2.0/configu/commands/export_command.py` & `configu-0.3.0/configu/commands/export_command.py`

 * *Files identical despite different names*

### Comparing `configu-0.2.0/configu/commands/upsert_command.py` & `configu-0.3.0/configu/commands/upsert_command.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,22 +18,37 @@
         "schema": ConfigSchema,
         "configs": Dict[str, str],
     },
 )
 
 
 class UpsertCommand(Command):
-    """"""
+    """
+    The Upsert command is used to create, update or delete Configs from a
+    ConfigStore
+    """
 
     parameters: UpsertCommandParameters
 
     def __init__(self, parameters: UpsertCommandParameters) -> None:
+        """
+        Creates a new UpsertCommand.
+        :param parameters: dict
+            The command's parameters. Includes the following:
+            - store: the `ConfigStore` to which the command will write
+            - set: the `ConfigSet` to which the command will write
+            - schema: `ConfigSchema` to validate config being written
+            - configs: a dictionary of `Config`s to upsert
+        """
         super().__init__(parameters)
 
     def run(self):
+        """
+        Runs the upsert command.
+        """
         scope_location = ["UpsertCommand", "run"]
         store = self.parameters["store"]
         set_ = self.parameters["set"]
         schema = self.parameters["schema"]
         configs = self.parameters["configs"]
         store.init()
         schema_content = ConfigSchema.parse(schema)
```

### Comparing `configu-0.2.0/configu/core/config_schema.py` & `configu-0.3.0/configu/core/config_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,49 +57,63 @@
         ),
         "Currency": pyvalidator.is_currency,
     }
     PROPS = list(Cfgu.__annotations__.keys())
 
 
 class ConfigSchema(IConfigSchema):
-    """"""
+    """
+    A Python representation of the schema stored in a .cfgu.json file.
+    """
 
     CFGU = ConfigSchemaDefinition
 
     TYPES = {
         f".{schema_type.value}": schema_type
         for schema_type in ConfigSchemaType
     }
     EXT = " | ".join(
         ["".join(ext) for ext in zip(cycle(CFGU.EXT), TYPES.keys())]
     )
 
     def __init__(self, path: str) -> None:
+        """
+        Creates a new ConfigSchema
+        :param path: path the the config file
+        """
         error_location = [self.__class__.__name__, self.__init__.__name__]
         if re.match(rf".*({ConfigSchema.EXT})", path) is None:
             raise ValueError(
                 error_message(
                     f"invalid path {path}",
                     error_location,
                     f"file extension must be {ConfigSchema.EXT}",
                 )
             )
         super().__init__(path=path, type=ConfigSchema.TYPES[Path(path).suffix])
 
     def read(self) -> str:
+        """
+        Reads the config schema file
+        :return: contents of the config schema
+        """
         try:
             with open(self.path, mode="r", encoding="utf-8") as schema_file:
                 file_content = schema_file.read()
             return file_content
         except (OSError, Exception):
             return ""
 
     @classmethod
     def parse(cls, scheme: "ConfigSchema") -> Dict[str, Cfgu]:
-        """"""
+        """
+        Parses the given ConfigSchema
+        :param scheme: The ConfigSchema to parse
+        :return: A dictionary of configurations.
+        """
         error_location = [cls.__name__, "parse"]
         schema_content = scheme.read()
         if scheme.type == ConfigSchemaType.JSON:
             try:
                 schema_content = json.loads(schema_content)
                 schema_content = config_schema_contents_from_dict(
                     schema_content
```

### Comparing `configu-0.2.0/configu/core/generated.py` & `configu-0.3.0/configu/core/generated.py`

 * *Files identical despite different names*

### Comparing `configu-0.2.0/configu/stores/configu_store.py` & `configu-0.3.0/configu/stores/configu_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     def __call__(self, r):
         r.headers["token"] = self.token
         return r
 
 
 class ConfiguConfigStore(ConfigStore):
+    """A `ConfigStore` persisted by Configu (https://app.configu.com)"""
+
     _headers: Dict
     _auth: AuthBase
     _url: str
 
     def __init__(
         self, store_config: Union[ConfiguStoreConfiguration, dict]
     ) -> None:
@@ -65,15 +67,14 @@
         response = requests.post(
             url=self._url,
             headers=self._headers,
             auth=self._auth,
             json=queries_json,
         )
         response.raise_for_status()
-        print([Config(**args) for args in response.json()])
         return [Config(**args) for args in response.json()]
 
     def set(self, configs: List[Union[Config, dict]]) -> None:
         configs = [
             Config(**config) if isinstance(config, dict) else config
             for config in configs
         ]
```

### Comparing `configu-0.2.0/configu/stores/in_memory_store.py` & `configu-0.3.0/configu/stores/in_memory_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Union
 
 from ..core import Config, ConfigStoreQuery, ConfigStore
 from ..core.generated import config_store_query_from_dict, config_from_dict
 
 
 class InMemoryConfigStore(ConfigStore):
+    """A `ConfigStore` persisted in-memory"""
+
     _data: List[Config]
 
     def __init__(self) -> None:
         super().__init__(type="in-memory")
         self._data = []
 
     def get(self, queries: List[ConfigStoreQuery]) -> List[Config]:
```

### Comparing `configu-0.2.0/configu/stores/json_file_store.py` & `configu-0.3.0/configu/stores/json_file_store.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,26 +8,37 @@
     config_store_contents_to_dict,
     ConfigStoreContentsElement,
     config_store_contents_element_from_dict,
 )
 
 
 class JsonFileConfigStore(ConfigStore):
+    """A `ConfigStore` persisted in a json file"""
+
     _path: str
 
     def __init__(self, path: str) -> None:
         super().__init__(type="in-memory")
         self._path = path
 
     def read(self):
+        """
+        Reads JSON file contents
+        :return: The file contents, represented as a list of key/set/value
+        dicts
+        """
         with open(self._path, mode="r", encoding="utf-8") as json_file:
             data = json.load(json_file)
         return config_store_contents_from_dict(data)
 
     def write(self, next_configs: List[ConfigStoreContentsElement]):
+        """
+        Writes to the JSON file
+        :param next_configs: a list of key/set/value dicts to write
+        """
         data = config_store_contents_to_dict(next_configs)
         with open(self._path, mode="w", encoding="utf-8") as json_file:
             json.dump(data, json_file)
 
     def get(
         self, queries: List[Union[ConfigStoreQuery, dict]]
     ) -> List[ConfigStoreContentsElement]:
@@ -35,26 +46,19 @@
         queries = [
             config_store_query_from_dict(query)
             if isinstance(query, dict)
             else query
             for query in queries
         ]
         query_ids = [f"{query.set}.{query.key}" for query in queries]
-        results = []
-        for config in stored_configs:
-            for query in queries:
-                if any(
-                    [
-                        f"{config.set}.{config.key}" in query_ids,
-                        (query.set == "*" or query.set == config.set)
-                        and (query.key == "*" or query.key == config.key),
-                    ]
-                ):
-                    results.append(config)
-        return results
+        return [
+            config
+            for config in stored_configs
+            if f"{config.set}.{config.key}" in query_ids
+        ]
 
     def set(self, configs: List[Union[Config, dict]]) -> None:
         stored_configs = self.read()
         configs = [
             config_store_contents_element_from_dict(config)
             if isinstance(config, dict)
             else config_store_contents_element_from_dict(config.to_dict())
```

### Comparing `configu-0.2.0/configu/utils.py` & `configu-0.3.0/configu/utils.py`

 * *Files identical despite different names*

### Comparing `configu-0.2.0/pyproject.toml` & `configu-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configu"
-version = "0.2.0"
+version = "0.3.0"
 description = "Configu Python SDK"
 authors = ["Configu <info@configu.com>"]
 maintainers = [
   "Ron Roditi <ron@configu.com>",
   "Or Levi <orlevi128@gmail.com>"
 ]
 license = "Apache-2.0"
@@ -30,14 +30,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.28.1"
 py-validator = "^0.17.0"
 pydantic = "^1.10.6"
 chevron = "^0.14.0"
+boto3 = "^1.26.155"
+boto3-stubs = { extras = ["secretsmanager"], version = "^1.26.155" }
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0" # configs at .flake8
 black = { extras = ["d"], version = "^23.1.0" }
 pdoc = "^13.1.0" # https://pdoc.dev/docs/pdoc.html
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `configu-0.2.0/PKG-INFO` & `configu-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configu
-Version: 0.2.0
+Version: 0.3.0
 Summary: Configu Python SDK
 Home-page: https://configu.com/
 License: Apache-2.0
 Keywords: cfgu,configu,configu-sdk,configu-python-sdk
 Author: Configu
 Author-email: info@configu.com
 Maintainer: Ron Roditi
@@ -16,14 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
+Requires-Dist: boto3 (>=1.26.155,<2.0.0)
+Requires-Dist: boto3-stubs[secretsmanager] (>=1.26.155,<2.0.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: py-validator (>=0.17.0,<0.18.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://configu.com/docs/
 Project-URL: Repository, https://github.com/configu/configu
 Description-Content-Type: text/markdown
```

