# Comparing `tmp/configzen-0.4.4.tar.gz` & `tmp/configzen-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.4.tar", max compression
+gzip compressed data, was "configzen-0.4.5.tar", max compression
```

## Comparing `configzen-0.4.4.tar` & `configzen-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      979 2023-06-29 09:00:26.400544 configzen-0.4.4/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.4/configzen/__main__.py
--rw-r--r--   0        0        0     1436 2023-06-29 08:29:56.441906 configzen-0.4.4/configzen/_isolation.py
--rw-r--r--   0        0        0     2916 2023-06-29 09:09:47.165217 configzen-0.4.4/configzen/_setup.py
--rw-r--r--   0        0        0    76229 2023-06-29 09:07:48.634978 configzen-0.4.4/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.4/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.4/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.4/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.4/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.4/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.4/configzen/route.py
--rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.4/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.4/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 09:12:45.278875 configzen-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.4/README.md
--rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.5/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.5/configzen/__main__.py
+-rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.5/configzen/_isolation.py
+-rw-r--r--   0        0        0     2916 2023-06-29 09:09:47.165217 configzen-0.4.5/configzen/_setup.py
+-rw-r--r--   0        0        0    76173 2023-06-29 09:14:43.431854 configzen-0.4.5/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.5/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.5/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.5/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.5/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.5/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.5/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.5/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 09:14:10.332011 configzen-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.5/README.md
+-rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.5/PKG-INFO
```

### Comparing `configzen-0.4.4/configzen/__main__.py` & `configzen-0.4.5/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/_isolation.py` & `configzen-0.4.5/configzen/_isolation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     if isinstance(func, (classmethod, staticmethod)):
         return type(func)(isolate_calls(func.__func__))
 
     if asyncio.iscoroutinefunction(func):
         return cast(
             collections.abc.Callable[P, T],
-            lambda *args, **kwargs: isolate_async(func, *args, **kwargs)
+            lambda *args, **kwargs: isolate_async(func, *args, **kwargs),
         )
     return lambda *args, **kwargs: isolate(func, *args, **kwargs)
 
 
 def isolate(
     func: collections.abc.Callable[..., T],
     *args: Any,
```

### Comparing `configzen-0.4.4/configzen/_setup.py` & `configzen-0.4.5/configzen/_setup.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/config.py` & `configzen-0.4.5/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,19 +141,19 @@
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
 INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
-    ] = contextvars.ContextVar("current_context", default=None)
+] = contextvars.ContextVar("current_context", default=None)
 
 current_interpolation_tracker: contextvars.ContextVar[
     dict[str, Any] | None
-    ] = contextvars.ContextVar("current_interpolation_tracker", default=None)
+] = contextvars.ContextVar("current_interpolation_tracker", default=None)
 
 _exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
     "_exporting", default=False
 )
 
 
 def _get_defaults_from_model_class(
@@ -193,17 +193,15 @@
 
     Returns
     -------
     Any
     """
     if dataclasses.is_dataclass(obj):
         return export_hook(dataclasses.asdict(obj))
-    if (
-        isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
-    ):
+    if isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields"):
         return _export_namedtuple(obj)
     return obj
 
 
 @functools.singledispatch
 def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
     # Initially I wanted it to be export_hook(obj._asdict()), but
@@ -230,15 +228,14 @@
             ...
 
         def dispatch(
             self, cls: type[T]
         ) -> collections.abc.Callable[[type[T] | Any, Any], Any]:
             ...
 
-
     field_hook: _FieldHookType = _FieldHookType()
 
 else:
 
     def field_hook(cls: type[Any], value: Any) -> Any:
         """
         Automatically registered pre-validator for values in fields
@@ -270,15 +267,14 @@
             cls = origin
         try:
             cast_func = field_hook_registrars.dispatch(cls)
         except KeyError:
             return value
         return cast_func(cls, value)
 
-
     field_hook.register = field_hook_registrars.register
 
 
 @functools.singledispatch
 def export_model(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
@@ -637,16 +633,17 @@
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration.
         """
-        dict_config = await self.load_dict_async(blob, parser_name=parser_name,
-                                                 **kwargs)
+        dict_config = await self.load_dict_async(
+            blob, parser_name=parser_name, **kwargs
+        )
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     def _load_dict_impl(
         self,
         blob: str | bytes,
```

### Comparing `configzen-0.4.4/configzen/decorators.py` & `configzen-0.4.5/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/errors.py` & `configzen-0.4.5/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/field.py` & `configzen-0.4.5/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/processor.py` & `configzen-0.4.5/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/route.py` & `configzen-0.4.5/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/configzen/typedefs.py` & `configzen-0.4.5/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/LICENSE` & `configzen-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/pyproject.toml` & `configzen-0.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.4"
+version = "0.4.5"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.4/README.md` & `configzen-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.4.4/PKG-INFO` & `configzen-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.4
+Version: 0.4.5
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

