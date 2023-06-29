# Comparing `tmp/configzen-0.4.2.tar.gz` & `tmp/configzen-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.2.tar", max compression
+gzip compressed data, was "configzen-0.4.3.tar", max compression
```

## Comparing `configzen-0.4.2.tar` & `configzen-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.4.2/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.2/configzen/__main__.py
--rw-r--r--   0        0        0     1343 2023-06-29 07:28:28.011055 configzen-0.4.2/configzen/_isolation.py
--rw-r--r--   0        0        0    79093 2023-06-29 07:15:43.040767 configzen-0.4.2/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.2/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.2/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.2/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.2/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.2/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.2/configzen/route.py
--rw-r--r--   0        0        0     1126 2023-06-29 07:06:09.671161 configzen-0.4.2/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.2/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 07:33:51.002256 configzen-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12653 2023-06-29 05:44:52.044957 configzen-0.4.2/README.md
--rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 configzen-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.4.3/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.3/configzen/__main__.py
+-rw-r--r--   0        0        0     1436 2023-06-29 08:29:56.441906 configzen-0.4.3/configzen/_isolation.py
+-rw-r--r--   0        0        0    79326 2023-06-29 08:29:56.458905 configzen-0.4.3/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.3/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.3/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.3/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.3/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.3/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.3/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.3/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 08:08:40.120106 configzen-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    12653 2023-06-29 05:44:52.044957 configzen-0.4.3/README.md
+-rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 configzen-0.4.3/PKG-INFO
```

### Comparing `configzen-0.4.2/configzen/__init__.py` & `configzen-0.4.3/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/__main__.py` & `configzen-0.4.3/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/_isolation.py` & `configzen-0.4.3/configzen/_isolation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 import collections.abc
 import contextvars
-import functools
 from typing import Any, cast
 
-from configzen.typedefs import T
+from configzen.typedefs import T, P
 
 
 def isolate_calls(
-    func: collections.abc.Callable[..., T],
-) -> collections.abc.Callable[..., T]:
+    func: collections.abc.Callable[P, T],
+) -> collections.abc.Callable[P, T]:
     """
     Decorator to copy a function call context automatically (context isolation)
     to prevent collisions.
 
     This decorator will copy the current context and run the function
     in this new isolated context.
     """
+    if isinstance(func, (classmethod, staticmethod)):
+        return type(func)(isolate_calls(func.__func__))
+
     if asyncio.iscoroutinefunction(func):
         return cast(
-            collections.abc.Callable[..., T],
+            collections.abc.Callable[P, T],
             lambda *args, **kwargs: isolate_async(func, *args, **kwargs)
         )
     return lambda *args, **kwargs: isolate(func, *args, **kwargs)
 
 
 def isolate(
     func: collections.abc.Callable[..., T],
```

### Comparing `configzen-0.4.2/configzen/config.py` & `configzen-0.4.3/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,19 +142,19 @@
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
 INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
-] = contextvars.ContextVar("current_context", default=None)
+    ] = contextvars.ContextVar("current_context", default=None)
 
 current_interpolation_tracker: contextvars.ContextVar[
     dict[str, Any] | None
-] = contextvars.ContextVar("current_interpolation_tracker", default=None)
+    ] = contextvars.ContextVar("current_interpolation_tracker", default=None)
 
 _exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
     "_exporting", default=False
 )
 
 
 def _get_defaults_from_model_class(
@@ -233,14 +233,15 @@
             ...
 
         def dispatch(
             self, cls: type[T]
         ) -> collections.abc.Callable[[type[T] | Any, Any], Any]:
             ...
 
+
     field_hook: _FieldHookType = _FieldHookType()
 
 else:
 
     def field_hook(cls: type[Any], value: Any) -> Any:
         """
         Automatically registered pre-validator for values in fields
@@ -272,14 +273,15 @@
             cls = origin
         try:
             cast_func = field_hook_registrars.dispatch(cls)
         except KeyError:
             return value
         return cast_func(cls, value)
 
+
     field_hook.register = field_hook_registrars.register
 
 
 @functools.singledispatch
 def export_model(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
@@ -2001,27 +2003,25 @@
         super()._init_private_attributes()
         local = contextvars.copy_context()
         object.__setattr__(self, LOCAL, local)
         tok = getattr(self, TOKEN, None)
         if tok:
             current_context.reset(tok)
 
-    @isolate_calls
     def export(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
         _exporting.set(True)  # noqa: FBT003
         return isolate(self.dict, **kwargs)
 
-    @isolate_calls
     async def export_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
@@ -2253,15 +2253,14 @@
         -------
         None
         """
         context = get_context(self)
         self.__dict__.update(context.initial_state)
 
     @classmethod
-    @isolate_calls
     def load(
         cls: type[ConfigModelT],
         resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
         ac_parser: str | None = None,
         **kwargs: Any,
@@ -2301,15 +2300,14 @@
         config = local.run(agent.read, config_class=cls, **kwargs)
         object.__setattr__(config, LOCAL, local)
         context = cast(Context[ConfigModelT], local.get(current_context))
         context.owner = config
         context.initial_state = config.__dict__
         return config
 
-    @isolate_calls
     def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file.
 
         Parameters
         ----------
         **kwargs
@@ -2326,15 +2324,14 @@
         else:
             changed = reload(cast(ConfigModelT, context.at), **kwargs)
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
-    @isolate_calls
     def save(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file.
 
         Parameters
@@ -2380,15 +2377,14 @@
         context = get_context(self)
         if context.agent.is_url:
             msg = "Writing to URLs is not yet supported"
             raise NotImplementedError(msg)
         return context.agent.write(blob, **kwargs)
 
     @classmethod
-    @isolate_calls
     async def load_async(
         cls: type[ConfigModelT],
         resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         ac_parser: str | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
@@ -2428,15 +2424,14 @@
         )
         config = await task
         object.__setattr__(config, LOCAL, local)
         context = cast(Context[ConfigModelT], local.get(current_context))
         context.owner = config
         return config
 
-    @isolate_calls
     async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
@@ -2455,15 +2450,14 @@
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
-    @isolate_calls
     async def save_async(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file asynchronously.
 
         Parameters
@@ -2533,14 +2527,24 @@
             tok = current_context.set(subcontext)
             return _get_object_state(value) | {
                 TOKEN: tok,
                 LOCAL: contextvars.copy_context(),
             }
         return value
 
+    if not TYPE_CHECKING:
+        load = isolate_calls(load)
+        load_async = isolate_calls(load_async)
+        reload = isolate_calls(reload)
+        reload_async = isolate_calls(reload_async)
+        save = isolate_calls(save)
+        save_async = isolate_calls(save_async)
+        export = isolate_calls(export)
+        export_async = isolate_calls(export_async)
+
 
 @field_hook.register(ConfigModel)
 def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
     """
     Load a model using dict literal evaluation.
     Solves nested dictionaries problem in INI files.
```

### Comparing `configzen-0.4.2/configzen/decorators.py` & `configzen-0.4.3/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/errors.py` & `configzen-0.4.3/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/field.py` & `configzen-0.4.3/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/processor.py` & `configzen-0.4.3/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/route.py` & `configzen-0.4.3/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/typedefs.py` & `configzen-0.4.3/configzen/typedefs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import contextlib
 import os
 import pathlib
 import sys
 from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
 
 if sys.version_info >= (3, 10):
-    from typing import TypeAlias
+    from typing import TypeAlias, ParamSpec
 else:
-    from typing_extensions import TypeAlias
+    from typing_extensions import TypeAlias, ParamSpec
 
 if TYPE_CHECKING:
     from aiofiles.base import AiofilesContextManager
     from aiofiles.threadpool.text import AsyncTextIOWrapper
 
     from configzen.config import ConfigModel
     from configzen.route import ConfigRoute
 
 T = TypeVar("T")
+P = ParamSpec("P")
 
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
 ConfigRouteLike: TypeAlias = Union[str, list[str], "ConfigRoute"]
 
 ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
 AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
 RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
```

### Comparing `configzen-0.4.2/LICENSE` & `configzen-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/pyproject.toml` & `configzen-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.2"
+version = "0.4.3"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.2/README.md` & `configzen-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/PKG-INFO` & `configzen-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.2
+Version: 0.4.3
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

