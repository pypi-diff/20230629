# Comparing `tmp/configzen-0.4.8.tar.gz` & `tmp/configzen-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.8.tar", max compression
+gzip compressed data, was "configzen-0.5.tar", max compression
```

## Comparing `configzen-0.4.8.tar` & `configzen-0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.8/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.8/configzen/__main__.py
--rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.8/configzen/_isolation.py
--rw-r--r--   0        0        0     2925 2023-06-29 09:31:01.297959 configzen-0.4.8/configzen/_setup.py
--rw-r--r--   0        0        0    74707 2023-06-29 09:35:47.594054 configzen-0.4.8/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.8/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.8/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.8/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.8/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.8/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.8/configzen/route.py
--rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.8/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.8/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 09:37:18.882463 configzen-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.8/README.md
--rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5/configzen/__main__.py
+-rw-r--r--   0        0        0     1437 2023-06-29 16:34:46.964275 configzen-0.5/configzen/_isolation.py
+-rw-r--r--   0        0        0     3394 2023-06-29 17:46:07.418020 configzen-0.5/configzen/_setup.py
+-rw-r--r--   0        0        0    77224 2023-06-29 17:47:37.718956 configzen-0.5/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.5/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.5/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.5/configzen/field.py
+-rw-r--r--   0        0        0     5157 2023-06-29 17:56:51.047974 configzen-0.5/configzen/interpolation.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.5/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.5/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 16:34:46.955277 configzen-0.5/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5/LICENSE
+-rw-r--r--   0        0        0     1471 2023-06-29 17:58:47.956651 configzen-0.5/pyproject.toml
+-rw-r--r--   0        0        0    14113 2023-06-29 17:37:24.088159 configzen-0.5/README.md
+-rw-r--r--   0        0        0    14636 1970-01-01 00:00:00.000000 configzen-0.5/PKG-INFO
```

### Comparing `configzen-0.4.8/configzen/__init__.py` & `configzen-0.5/configzen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # flake8: noqa
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 from pydantic import validator as field_validator
 
-from . import config, decorators, field, processor, route
+from . import config, decorators, field, interpolation, processor, route
 from .config import *
 from .decorators import *
 from .field import *
+from .interpolation import *
 from .processor import *
 from .route import *
 
 __all__ = (
     *config.__all__,
     *field.__all__,
+    *interpolation.__all__,
     *processor.__all__,
     *decorators.__all__,
     *route.__all__,
     "field_validator",
 )
 
-del annotations, TYPE_CHECKING
+del annotations
```

### Comparing `configzen-0.4.8/configzen/__main__.py` & `configzen-0.5/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/_isolation.py` & `configzen-0.5/configzen/_isolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import collections.abc
 import contextvars
 from typing import Any, cast
 
-from configzen.typedefs import T, P
+from configzen.typedefs import P, T
 
 
 def isolate_calls(
     func: collections.abc.Callable[P, T],
 ) -> collections.abc.Callable[P, T]:
     """
     Decorator to copy a function call context automatically (context isolation)
```

### Comparing `configzen-0.4.8/configzen/_setup.py` & `configzen-0.5/configzen/_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 by setting the environment variable ``CONFIGZEN_SETUP`` to ``0``.
 """
 
 from __future__ import annotations
 
 import ast
 import collections.abc
+import ipaddress
 import pathlib
 from typing import TYPE_CHECKING, Any
 
 from pydantic.json import ENCODERS_BY_TYPE
 
-from configzen.config import export_hook, field_hook, ConfigModel
+from configzen.config import ConfigModel, export_hook, field_hook
 
 if TYPE_CHECKING:
     from configzen.typedefs import ConfigModelT
 
 for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
     export_hook.register(obj_type, obj_encoder)
 
@@ -77,14 +78,26 @@
             # There might be some following validator, let it be like that
             return value
         else:
             return cls(data)
     return value
 
 
+@field_hook.register(ipaddress.IPv4Address)
+@field_hook.register(ipaddress.IPv6Address)
+def _eval_ipaddress(
+    cls: type[ipaddress.IPv4Address | ipaddress.IPv6Address], value: Any
+) -> ipaddress.IPv4Address | ipaddress.IPv6Address | Any:
+    if isinstance(value, str) and value.casefold() == "localhost":
+        if issubclass(cls, ipaddress.IPv6Address):
+            return cls("::1")
+        return cls("127.0.0.1")
+    return value
+
+
 @field_hook.register(ConfigModel)
 def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
     """
     Load a model using dict literal evaluation.
     Solves nested dictionaries problem in INI files.
 
     Parameters
```

### Comparing `configzen-0.4.8/configzen/config.py` & `configzen-0.5/configzen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,14 @@
 import copy
 import dataclasses
 import functools
 import importlib
 import io
 import os
 import pathlib
-import re
-import string
 import urllib.parse
 import urllib.request
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
@@ -96,24 +94,30 @@
 from configzen._isolation import isolate, isolate_async, isolate_calls
 from configzen.errors import (
     ConfigAccessError,
     ResourceLookupError,
     UnavailableParserError,
     UnspecifiedParserError,
 )
+from configzen.interpolation import (
+    INTERPOLATION_NAMESPACE_TOKEN,
+    include_const,
+    interpolate,
+    include,
+)
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.route import ConfigRoute
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
+    ConfigRouteLike,
     IncludeExcludeT,
     NormalizedResourceT,
     RawResourceT,
-    ConfigRouteLike,
     T,
 )
 
 try:
     import aiofiles
 
     AIOFILES_AVAILABLE = True
@@ -127,21 +131,24 @@
     "ConfigMeta",
     "export_hook",
     "field_hook",
     "export_model",
     "export_model_async",
 )
 
-_URL_SCHEMES: set[str] = set(
+ALL_URL_SCHEMES: set[str] = set(
     urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
 ) - {""}
+
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
+
 INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
+INTERPOLATION_INCLUSIONS: str = "__interpolation_inclusions__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
 ] = contextvars.ContextVar("current_context", default=None)
 
 current_interpolation_tracker: contextvars.ContextVar[
     dict[str, Any] | None
@@ -480,15 +487,15 @@
             processor_class = Processor[ConfigModelT]
 
         self.processor_class = processor_class
         self.parser_name = parser_name
 
         if isinstance(resource, (str, os.PathLike)) and not (
             isinstance(resource, str)
-            and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
+            and urllib.parse.urlparse(str(resource)).scheme in ALL_URL_SCHEMES
         ):
             raw_path = os.fspath(resource)
             resource = pathlib.Path(raw_path)
             if (
                 raw_path.startswith(".")
                 and resource.parts
                 and not resource.parts[0].startswith(".")
@@ -1423,14 +1430,15 @@
     ----------
     initial_state
         The initial configuration state.
 
     """
 
     initial_state: dict[str, Any]
+    interpolation_namespace: dict[str, Any]
 
     @abc.abstractmethod
     def trace_route(self) -> collections.abc.Iterator[str]:
         """Trace the route to where the configuration subcontext points to."""
 
     @property
     def route(self) -> ConfigRoute:
@@ -1458,23 +1466,28 @@
 
         Returns
         -------
         The new subcontext.
         """
         if part is None:
             return self
-        return Subcontext(self, part)
+        return Subcontext(self, part, self.interpolation_namespace.setdefault(part, {}))
 
     @property
     @abc.abstractmethod
     def agent(self) -> ConfigAgent[ConfigModelT]:
         """The configuration agent responsible for loading and saving."""
 
     @property
     @abc.abstractmethod
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        """Top-level interpolation namespace."""
+
+    @property
+    @abc.abstractmethod
     def owner(self) -> ConfigModelT | None:
         """
         The top-level configuration model instance,
         holding all adjacent contexts.
         """
 
     @property
@@ -1502,28 +1515,32 @@
     _initial_state: dict[str, Any]
 
     def __init__(
         self,
         agent: ConfigAgent[ConfigModelT],
         owner: ConfigModelT | None = None,
     ) -> None:
-        self._agent = agent
-        self._owner = None
         self._initial_state = {}
-
+        self._owner = None
+        self._agent = agent
+        self.interpolation_namespace = {}
         self.owner = owner
 
     def trace_route(self) -> collections.abc.Iterator[str]:
         yield from ()
 
     @property
     def agent(self) -> ConfigAgent[ConfigModelT]:
         return self._agent
 
     @property
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        return self.interpolation_namespace
+
+    @property
     def at(self) -> ConfigModelT | None:
         return self.owner
 
     @property
     def owner(self) -> ConfigModelT | None:
         return self._owner
 
@@ -1558,22 +1575,34 @@
     ----------
     parent
         The parent context.
     part
         The name of the item nested in the item the parent context points to.
     """
 
-    def __init__(self, parent: BaseContext[ConfigModelT], part: str) -> None:
+    __slots__ = ("_parent", "_part", "_interpolation_namespace")
+
+    def __init__(
+        self,
+        parent: BaseContext[ConfigModelT],
+        part: str,
+        interpolation_namespace: dict[str, Any],
+    ) -> None:
         self._parent = parent
         self._part = part
+        self.interpolation_namespace = interpolation_namespace
 
     @property
     def agent(self) -> ConfigAgent[ConfigModelT]:
         return self._parent.agent
 
+    @property
+    def toplevel_interpolation_namespace(self) -> dict[str, Any]:
+        return self._parent.toplevel_interpolation_namespace
+
     def trace_route(self) -> collections.abc.Iterator[str]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
     def at(self) -> ConfigAt[ConfigModelT]:
         if self.owner is None:
@@ -1667,16 +1696,17 @@
     if not isinstance(disallow_interpolation, bool):
         disallowed_interpolation_fields = set(disallow_interpolation)
     if (
         field.field_info.extra.get("interpolate", True)
         and field.alias not in disallowed_interpolation_fields
     ):
         old_value = post_hook_value
-        new_value = interpolate(
-            post_hook_value, cls.get_interpolation_context() | values
+        new_value = field_hook(
+            field.outer_type_,
+            interpolate(post_hook_value, cls, values.copy())
         )
         if old_value != new_value:
             interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
         post_hook_value = new_value
     return post_hook_value
 
 
@@ -1696,16 +1726,18 @@
         name: str,
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **kwargs: Any,
     ) -> type:
         namespace |= dict.fromkeys(
             (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
-        )
-        namespace[INTERPOLATION_TRACKER] = pydantic.PrivateAttr(default_factory=dict)
+        ) | {INTERPOLATION_TRACKER: pydantic.PrivateAttr(default_factory=dict)}
+
+        if namespace.get(INTERPOLATION_INCLUSIONS) is None:
+            namespace[INTERPOLATION_INCLUSIONS] = {}
 
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
 
         model = super().__new__(cls, name, bases, namespace, **kwargs)
         for field in model.__fields__.values():
             if field.pre_validators is None:
@@ -1721,33 +1753,14 @@
                     *field.pre_validators,
                 ]
         model_encoder = model.__json_encoder__
         model.__json_encoder__ = functools.partial(_json_encoder, model_encoder)
         return cast(type, model)
 
 
-class ConfigInterpolationTemplate(string.Template):
-    idpattern = r"(?a:[_a-z][\\\.\[\]_a-z0-9]*)"
-    flags = re.IGNORECASE | re.UNICODE
-
-
-@functools.singledispatch
-def interpolate(value: Any, _ctx: dict[str, Any]) -> Any:
-    return value
-
-
-@interpolate.register(str)
-def _interpolate_str(value: str, ctx: dict[str, Any]) -> str:
-    template = ConfigInterpolationTemplate(value)
-    return template.safe_substitute(ctx)
-
-
-# todo(bswck): Interpolation for compound types. Quite non-trivial.
-
-
 class ConfigMeta(pydantic.BaseSettings.Config):
     """
     Meta-configuration for configuration models.
 
     See https://docs.pydantic.dev/latest/usage/model_config/ for more information
     on model configurations.
 
@@ -1819,14 +1832,17 @@
 
     def _init_private_attributes(self) -> None:
         super()._init_private_attributes()
         local = contextvars.copy_context()
         object.__setattr__(self, LOCAL, local)
         tok = getattr(self, TOKEN, None)
         if tok:
+            context = current_context.get()
+            if context is not None:
+                context.interpolation_namespace |= self.dict()
             current_context.reset(tok)
 
     def export(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
@@ -2321,21 +2337,64 @@
         """
         context = get_context(self)
         if context.agent.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         return await context.agent.write_async(blob, **kwargs)
 
-    @staticmethod
-    def get_interpolation_context() -> dict[str, Any]:
+    @classmethod
+    def _evaluate_interpolation_namespaces(cls) -> dict[str | None, dict[str, Any]]:
+        inclusions = getattr(cls, INTERPOLATION_INCLUSIONS)
+        return {
+            namespace_id: evaluate_namespace()
+            for namespace_id, evaluate_namespace in inclusions.items()
+        }
+
+    @classmethod
+    def get_interpolation_namespace(
+        cls,
+        identifiers: set[str],
+        closest_namespace: dict[str, Any],
+    ) -> tuple[Any, dict[str, Any]]:
         """
         Get the interpolation context of this configuration model.
-        This must be either static or class method.
         """
-        return {}
+        context = current_context.get()
+        interpolation_context = {}
+
+        namespaces = cls._evaluate_interpolation_namespaces()
+        if context is not None:
+            namespaces.setdefault(None, {}).update(
+                context.toplevel_interpolation_namespace
+            )
+        for identifier in identifiers:
+            (
+                namespace_identifier,
+                specifies_namespace,
+                raw_identifier,
+            ) = identifier.rpartition(INTERPOLATION_NAMESPACE_TOKEN)
+            namespace = namespaces.get(None, {})
+            if specifies_namespace:
+                namespace |= namespaces[namespace_identifier]
+            else:
+                namespace |= closest_namespace
+
+            try:
+                value = at(namespace, raw_identifier)
+            except ResourceLookupError:
+                if not specifies_namespace:
+                    raise
+                value = at(closest_namespace, raw_identifier)
+            interpolation_context[identifier] = value
+            if raw_identifier not in closest_namespace:
+                interpolation_context[raw_identifier] = value
+
+        if len(identifiers) == 1:
+            return interpolation_context[identifiers.pop()], interpolation_context
+        return None, interpolation_context
 
     @classmethod
     def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
         """
         Called when this configuration model is being initialized as a field
         of some other configuration model.
         """
@@ -2356,9 +2415,12 @@
         reload_async = isolate_calls(reload_async)
         save = isolate_calls(save)
         save_async = isolate_calls(save_async)
         export = isolate_calls(export)
         export_async = isolate_calls(export_async)
 
 
+setattr(ConfigModel, INTERPOLATION_INCLUSIONS, None)
+include.register(ConfigModel, include_const)
+
 if os.getenv("CONFIGZEN_SETUP") != "0":
     importlib.import_module("._setup", package=__package__)
```

### Comparing `configzen-0.4.8/configzen/decorators.py` & `configzen-0.5/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/errors.py` & `configzen-0.5/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/field.py` & `configzen-0.5/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/processor.py` & `configzen-0.5/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/route.py` & `configzen-0.5/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/configzen/typedefs.py` & `configzen-0.5/configzen/typedefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import contextlib
 import os
 import pathlib
 import sys
 from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
 
 if sys.version_info >= (3, 10):
-    from typing import TypeAlias, ParamSpec
+    from typing import ParamSpec, TypeAlias
 else:
-    from typing_extensions import TypeAlias, ParamSpec
+    from typing_extensions import ParamSpec, TypeAlias
 
 if TYPE_CHECKING:
     from aiofiles.base import AiofilesContextManager
     from aiofiles.threadpool.text import AsyncTextIOWrapper
 
     from configzen.config import ConfigModel
     from configzen.route import ConfigRoute
```

### Comparing `configzen-0.4.8/LICENSE` & `configzen-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.8/pyproject.toml` & `configzen-0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.8"
+version = "0.5"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.8/README.md` & `configzen-0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 ### Preprocessing
 
 _configzen_ provides built-in preprocessing directives to your configuration files,
 offering features such as extending configuration files directly from other configuration files (without writing any
 code).
 You might think of it as something that is analogous
 to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats))
-and with some extra features planned.
+broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats)).
 The directive `^copy` may also be handy in quick conversions between the mentioned formats.
 See [Preprocessing directives](#preprocessing-directives) for more information.
 
 ## Supported file formats
 
 _configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
 As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
@@ -156,15 +155,15 @@
 or save the whole configuration:
 
 ```python
 >>> db_config.save()
 39
 ```
 
-### Preprocessing directives
+### Preprocessing
 
 To see supported preprocessing directives,
 see [Supported preprocessing directives](#supported-preprocessing-directives).
 
 #### Basic usage
 
 Having a base configuration file like this (`base.json`):
@@ -225,14 +224,81 @@
 
 | Directive  | Is the referenced file preprocessed? | Is the directive preserved on export? |
 |------------|--------------------------------------|---------------------------------------|
 | `^extend`  | Yes                                  | Yes                                   |
 | `^include` | Yes                                  | No                                    |
 | `^copy`    | No                                   | No                                    |
 
+
+### Interpolation
+
+#### Basic interpolation
+
+You can use interpolation in your configuration files:
+
+```yaml
+cpu:
+  cores: 4
+num_workers: ${cpu.cores}
+```
+
+```python
+>>> from configzen import ConfigModel
+...
+>>> class CPUConfig(ConfigModel):
+...     cores: int
+...
+>>> class AppConfig(ConfigModel):
+...     cpu: CPUConfig
+...     num_workers: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(num_workers=4, num_jobs=4)
+```
+
+
+#### Synchronizing interpolated configuration (inclusion)
+
+You can share independent configuration models as namespaces through inclusion:
+
+```yaml
+# database.yml
+host: ${app_config::db_host}
+port: ${app_config::expose}
+```
+
+```yaml
+# app.yml
+db_host: localhost
+expose: 8000
+```
+
+```python
+>>> from configzen import ConfigModel, include
+>>>
+>>> @include("app_config")
+... class DatabaseConfig(ConfigModel):
+...     host: IPv4Address
+...     port: int
+...
+>>> class AppConfig(ConfigModel):
+...     db_host: str
+...     expose: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(db_host='localhost', expose=8000)
+>>> db_config = DatabaseConfig.load("database.yml")
+DatabaseConfig(host=IPv4Address('localhost'), port=8000)
+```
+
+You do not have to pass a variable name to `@include`, though. `@include` lets you overwrite the main interpolation namespace
+or one with a separate name (here: `app_config`) with configuration models, dictionaries and their factories.
+
 ## Setup
 
 In order to use _configzen_ in your project, install it with your package manager, for example `pip`:
 
 ```bash
 pip install configzen
 ```
```

### Comparing `configzen-0.4.8/PKG-INFO` & `configzen-0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.8
+Version: 0.5
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -34,16 +34,15 @@
 ### Preprocessing
 
 _configzen_ provides built-in preprocessing directives to your configuration files,
 offering features such as extending configuration files directly from other configuration files (without writing any
 code).
 You might think of it as something that is analogous
 to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats))
-and with some extra features planned.
+broadened to any from the supported configuration file formats (see [Supported file formats](#supported-file-formats)).
 The directive `^copy` may also be handy in quick conversions between the mentioned formats.
 See [Preprocessing directives](#preprocessing-directives) for more information.
 
 ## Supported file formats
 
 _configzen_ uses [anyconfig](https://pypi.org/project/anyconfig/) to serialize and deserialize data and does not operate on any protocol-specific entities.
 As an example result, comments in your configuration files are lost on save[^1], but you can exchange file formats without any hassle.
@@ -178,15 +177,15 @@
 or save the whole configuration:
 
 ```python
 >>> db_config.save()
 39
 ```
 
-### Preprocessing directives
+### Preprocessing
 
 To see supported preprocessing directives,
 see [Supported preprocessing directives](#supported-preprocessing-directives).
 
 #### Basic usage
 
 Having a base configuration file like this (`base.json`):
@@ -247,14 +246,81 @@
 
 | Directive  | Is the referenced file preprocessed? | Is the directive preserved on export? |
 |------------|--------------------------------------|---------------------------------------|
 | `^extend`  | Yes                                  | Yes                                   |
 | `^include` | Yes                                  | No                                    |
 | `^copy`    | No                                   | No                                    |
 
+
+### Interpolation
+
+#### Basic interpolation
+
+You can use interpolation in your configuration files:
+
+```yaml
+cpu:
+  cores: 4
+num_workers: ${cpu.cores}
+```
+
+```python
+>>> from configzen import ConfigModel
+...
+>>> class CPUConfig(ConfigModel):
+...     cores: int
+...
+>>> class AppConfig(ConfigModel):
+...     cpu: CPUConfig
+...     num_workers: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(num_workers=4, num_jobs=4)
+```
+
+
+#### Synchronizing interpolated configuration (inclusion)
+
+You can share independent configuration models as namespaces through inclusion:
+
+```yaml
+# database.yml
+host: ${app_config::db_host}
+port: ${app_config::expose}
+```
+
+```yaml
+# app.yml
+db_host: localhost
+expose: 8000
+```
+
+```python
+>>> from configzen import ConfigModel, include
+>>>
+>>> @include("app_config")
+... class DatabaseConfig(ConfigModel):
+...     host: IPv4Address
+...     port: int
+...
+>>> class AppConfig(ConfigModel):
+...     db_host: str
+...     expose: int
+...
+>>> app_config = AppConfig.load("app.yml")
+>>> app_config
+AppConfig(db_host='localhost', expose=8000)
+>>> db_config = DatabaseConfig.load("database.yml")
+DatabaseConfig(host=IPv4Address('localhost'), port=8000)
+```
+
+You do not have to pass a variable name to `@include`, though. `@include` lets you overwrite the main interpolation namespace
+or one with a separate name (here: `app_config`) with configuration models, dictionaries and their factories.
+
 ## Setup
 
 In order to use _configzen_ in your project, install it with your package manager, for example `pip`:
 
 ```bash
 pip install configzen
 ```
```

