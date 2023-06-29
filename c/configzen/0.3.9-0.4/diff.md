# Comparing `tmp/configzen-0.3.9.tar.gz` & `tmp/configzen-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.9.tar", max compression
+gzip compressed data, was "configzen-0.4.tar", max compression
```

## Comparing `configzen-0.3.9.tar` & `configzen-0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.9/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.9/configzen/__main__.py
--rw-r--r--   0        0        0    69581 2023-06-21 19:46:41.922698 configzen-0.3.9/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.9/configzen/decorators.py
--rw-r--r--   0        0        0     3635 2023-06-21 19:36:00.617371 configzen-0.3.9/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.9/configzen/field.py
--rw-r--r--   0        0        0    26257 2023-06-21 19:40:28.209184 configzen-0.3.9/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.9/configzen/py.typed
--rw-r--r--   0        0        0     4686 2023-06-21 19:36:00.610371 configzen-0.3.9/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-21 19:40:00.222571 configzen-0.3.9/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.9/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-21 19:46:55.134889 configzen-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.9/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.4/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4/configzen/__main__.py
+-rw-r--r--   0        0        0     1286 2023-06-29 07:05:41.644836 configzen-0.4/configzen/_isolation.py
+-rw-r--r--   0        0        0    79152 2023-06-29 07:05:45.058201 configzen-0.4/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4/configzen/route.py
+-rw-r--r--   0        0        0     1126 2023-06-29 07:06:09.671161 configzen-0.4/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4/LICENSE
+-rw-r--r--   0        0        0     1471 2023-06-29 07:10:09.485977 configzen-0.4/pyproject.toml
+-rw-r--r--   0        0        0    12653 2023-06-29 05:44:52.044957 configzen-0.4/README.md
+-rw-r--r--   0        0        0    13242 1970-01-01 00:00:00.000000 configzen-0.4/PKG-INFO
```

### Comparing `configzen-0.3.9/configzen/__init__.py` & `configzen-0.4/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.9/configzen/__main__.py` & `configzen-0.4/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.9/configzen/config.py` & `configzen-0.4/configzen/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,48 +54,51 @@
     # otherhost  # <- not anotherhost, because we reloaded only port
     # 5432
 """
 
 from __future__ import annotations
 
 import abc
+import ast
 import asyncio
 import collections.abc
 import contextvars
 import copy
 import dataclasses
 import functools
 import io
 import os
 import pathlib
+import re
+import string
 import urllib.parse
 import urllib.request
 from typing import (
+    TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
     Literal,
     Optional,
     cast,
+    get_origin,
     no_type_check,
     overload,
 )
 
 import anyconfig
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
-from pydantic.fields import (  # type: ignore[attr-defined]
-    ModelField,
-    make_generic_validator,
-    Undefined
-)
+from pydantic.fields import make_generic_validator  # type: ignore[attr-defined]
+from pydantic.fields import ModelField, Undefined
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
+from configzen._isolation import isolate, isolate_async, isolate_calls
 from configzen.errors import (
     ConfigAccessError,
     ResourceLookupError,
     UnavailableParserError,
     UnspecifiedParserError,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
@@ -103,15 +106,16 @@
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
     IncludeExcludeT,
     NormalizedResourceT,
     RawResourceT,
-    SupportsRoute,
+    ConfigRouteLike,
+    T,
 )
 
 try:
     import aiofiles
 
     AIOFILES_AVAILABLE = True
 except ImportError:
@@ -122,30 +126,35 @@
     "ConfigAgent",
     "ConfigModel",
     "ConfigMeta",
     "save",
     "save_async",
     "reload",
     "reload_async",
-    "pre_serialize",
-    "post_deserialize",
-    "export",
-    "export_async",
+    "export_hook",
+    "field_hook",
+    "export_model",
+    "export_model_async",
 )
 
 _URL_SCHEMES: set[str] = set(
     urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
 ) - {""}
 CONTEXT: str = "__context__"
 TOKEN: str = "__context_token__"
 LOCAL: str = "__local__"
+INTERPOLATION_TRACKER: str = "__interpolation_tracker__"
 
 current_context: contextvars.ContextVar[
     BaseContext[Any] | None
-    ] = contextvars.ContextVar("current_context", default=None)
+] = contextvars.ContextVar("current_context", default=None)
+
+current_interpolation_tracker: contextvars.ContextVar[
+    dict[str, Any] | None
+] = contextvars.ContextVar("current_interpolation_tracker", default=None)
 
 _exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
     "_exporting", default=False
 )
 
 
 def _get_defaults_from_model_class(
@@ -157,15 +166,15 @@
         if not field.field_info.exclude and not field.required:
             if isinstance(default, pydantic.BaseModel):
                 default = default.dict()
             defaults[field.alias] = default
     return defaults
 
 
-def _get_object_dict(obj: Any) -> dict[str, Any]:
+def _get_object_state(obj: Any) -> dict[str, Any]:
     obj_dict = obj
     if not isinstance(obj, dict):
         obj_dict = obj.__dict__
     return cast(dict[str, Any], obj_dict)
 
 
 def _is_namedtuple(
@@ -173,15 +182,15 @@
 ) -> bool:
     return (
         isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
     )
 
 
 @functools.singledispatch
-def pre_serialize(obj: Any) -> Any:
+def export_hook(obj: Any) -> Any:
     """
     Convert a value to a format that can be safely serialized.
 
     This function is used to convert values that are not supported by
     `anyconfig` to a format that can be safely serialized. It is used
     internally by `ConfigModel` and `AsyncConfigModel` to convert
     values before saving them to a file.
@@ -192,52 +201,90 @@
         The value to convert.
 
     Returns
     -------
     Any
     """
     if dataclasses.is_dataclass(obj):
-        return pre_serialize(dataclasses.asdict(obj))
+        return export_hook(dataclasses.asdict(obj))
     if _is_namedtuple(obj):
-        return _ps_namedtuple(obj)
+        return _export_namedtuple(obj)
     return obj
 
 
 for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
-    pre_serialize.register(obj_type, obj_encoder)
+    export_hook.register(obj_type, obj_encoder)
 
+field_hook_registrars: Any = functools.singledispatch(lambda _cls, value: value)
 
-@functools.singledispatch
-def post_deserialize(cls: Any, value: Any) -> Any:
-    """
-    Load a value into a type after deserialization.
+if TYPE_CHECKING:
 
-    This function is used to load values that are not supported by
-    `anyconfig` to a format that can be used at runtime. It is used
-    by pydantic while performing validation.
+    class _FieldHookType:
+        def __call__(self, cls: type[T], value: Any) -> Any:
+            ...
 
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
+        def register(
+            self,
+            cls: type[T],
+            func: collections.abc.Callable[[type[T], Any], Any] | None = None,
+        ) -> collections.abc.Callable[
+            [collections.abc.Callable[[type[T], Any], Any]],
+            collections.abc.Callable[[type[T] | Any, Any], Any],
+        ]:
+            ...
 
-    value
-        The value to load.
+        def dispatch(
+            self, cls: type[T]
+        ) -> collections.abc.Callable[[type[T] | Any, Any], Any]:
+            ...
 
-    Returns
-    -------
-    The loaded value.
-    """
-    if isinstance(value, cls):
-        return value
-    return cls(value)
+    field_hook: _FieldHookType = _FieldHookType()
+
+else:
+
+    def field_hook(cls: type[Any], value: Any) -> Any:
+        """
+        Automatically registered pre-validator for values in fields
+        where the outer type is `cls`.
+
+        This function is used to load values that are not supported by
+        `anyconfig` to a format that can be used at runtime. It is used
+        by pydantic while performing validation.
+
+        Parameters
+        ----------
+        cls
+            The type to load the value into.
+
+        value
+            The value to load.
+
+        Returns
+        -------
+        The loaded value.
+        """
+        origin = get_origin(cls)
+        try:
+            if isinstance(value, origin or cls):
+                return value
+        except TypeError:
+            return value
+        if origin:
+            cls = origin
+        try:
+            cast_func = field_hook_registrars.dispatch(cls)
+        except KeyError:
+            return value
+        return cast_func(cls, value)
+
+    field_hook.register = field_hook_registrars.register
 
 
 @functools.singledispatch
-def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
+def export_model(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
@@ -245,80 +292,129 @@
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return obj.export(**kwargs)
     return cast(dict[str, Any], obj.dict(**kwargs))
 
 
 @functools.singledispatch
-async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
+async def export_model_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return await obj.export_async(**kwargs)
     return cast(dict[str, Any], await obj.dict_async(**kwargs))
 
 
-@pre_serialize.register(list)
-def _ps_list(obj: list[Any]) -> list[Any]:
+@export_hook.register(pathlib.PureWindowsPath)
+def _export_windows_path(obj: pathlib.PureWindowsPath) -> str:
+    """
+    Convert a Windows path to a string.
+
+    Parameters
+    ----------
+    obj
+        The path to convert.
+
+    Returns
+    -------
+    The converted path.
+    """
+    return obj.as_posix()
+
+
+@export_hook.register(list)
+def _export_list(obj: list[Any]) -> list[Any]:
     """
     Convert a list to safely-serializable form.
 
     Parameters
     ----------
     obj
         The list to convert.
 
     Returns
     -------
     The converted list.
     """
-    return [pre_serialize(item) for item in obj]
+    return [export_hook(item) for item in obj]
 
 
-@pre_serialize.register(collections.abc.Mapping)
-def _ps_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
+@export_hook.register(collections.abc.Mapping)
+def _export_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
     """
     Convert a mapping to safely-serializable form.
 
     Parameters
     ----------
     obj
         The mapping to convert.
 
     Returns
     -------
     The converted mapping.
     """
-    return {k: pre_serialize(v) for k, v in obj.items()}
+    return {k: export_hook(v) for k, v in obj.items()}
 
 
 @functools.singledispatch
-def _ps_namedtuple(obj: tuple[Any, ...]) -> Any:
+def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
     """
     Convert a namedtuple to safely-serializable form.
 
     Parameters
     ----------
     obj
         The namedtuple to convert.
 
     Returns
     -------
     The converted namedtuple (likely a list).
     """
-    # Initially I wanted it to be pre_serialize(obj._asdict()), but
+    # Initially I wanted it to be export(obj._asdict()), but
     # pydantic doesn't seem to be friends with custom NamedTuple-s.
-    return pre_serialize(list(obj))
+    return export_hook(list(obj))
+
+
+@field_hook.register(dict)
+@field_hook.register(list)
+def _eval_literals(cls: type[Any], value: Any) -> Any:
+    """
+    Load a dict/list using literal evaluation.
+    Solves nested dictionaries problem in INI files.
+
+    Parameters
+    ----------
+    cls
+        The type to load the value into.
+
+    value
+        The value to load.
+
+    Returns
+    -------
+    The loaded value.
+    """
+    if isinstance(value, cls):
+        return value
+    if isinstance(value, str):
+        try:
+            data = ast.literal_eval(value)
+        except (SyntaxError, ValueError):
+            # There might be some following validator, let it be like that
+            return value
+        else:
+            return cls(data)
+    return cls(value)
 
 
 def _delegate_ac_options(
     load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
 ) -> None:
     for key, value in options.items():
         if key.startswith("dump_"):
@@ -384,15 +480,15 @@
     ------
     ValueError
     """
 
     _resource: NormalizedResourceT
     processor_class: type[Processor[ConfigModelT]]
     create_if_missing: bool
-    relative: bool = False
+    is_relative: bool = False
     allowed_url_schemes: set[str]
     use_pydantic_json: bool = True
     default_load_options: dict[str, Any] = {}
     default_dump_options: dict[str, Any] = {
         # These are usually desirable for configuration files.
         # If you want to change them, you can do so by monkey-patching
         # these variables. You can also change `load_options` and
@@ -435,19 +531,31 @@
         "by_alias",
         "include",
         "exclude",
         "exclude_unset",
         "exclude_defaults",
         "exclude_none",
     }
-    FILEEXT_PARSER_ALIASES: ClassVar[dict[str, str]] = {
+    ALIAS_FILE_EXTENSIONS: ClassVar[dict[str, str]] = {
         "yml": "yaml",
-        "toml": "toml",
         "conf": "ini",
         "cfg": "ini",
+        # Note: CBOR (RFC 7049) is deprecated, use CBOR (RFC 8949) instead.
+        "cbor": "cbor2",
+        # https://github.com/msgpack/msgpack/issues/291#issuecomment-1370526984
+        "mpk": "msgpack",
+        "pkl": "pickle",
+    }
+    BINARY_AC_PARSERS: ClassVar[set[str]] = {
+        "ion",
+        "bson",
+        "cbor",
+        "cbor2",
+        "msgpack",
+        "pickle",
     }
 
     def __init__(
         self,
         resource: RawResourceT,
         ac_parser: str | None = None,
         processor_class: type[Processor[ConfigModelT]] | None = None,
@@ -465,19 +573,23 @@
         create_if_missing
             Whether to automatically create missing keys when loading the configuration.
         default_kwargs
             Default keyword arguments to pass while opening the resource.
         use_pydantic_json
             Whether to use Pydantic's JSON encoder/decoder instead of the default
             anyconfig one.
+        uses_binary_data
+            Whether to treat the data as binary. Defaults to True for BSON,
+            CBOR, MessagePack and Pickle formats.
         **kwargs
             Additional keyword arguments to pass to
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
         self._ac_parser = None
+        self._uses_binary_data = kwargs.get("uses_binary_data", False)
 
         if processor_class is None:
             processor_class = Processor[ConfigModelT]
 
         self.processor_class = processor_class
         self.ac_parser = ac_parser
 
@@ -488,15 +600,15 @@
             raw_path = os.fspath(resource)
             resource = pathlib.Path(raw_path)
             if (
                 raw_path.startswith(".")
                 and resource.parts
                 and not resource.parts[0].startswith(".")
             ):
-                self.relative = True
+                self.is_relative = True
 
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
         self.default_kwargs = kwargs.pop(
             "default_kwargs", self.predefined_default_kwargs.copy()
         )
@@ -551,28 +663,40 @@
             value = value.casefold()
         self._ac_parser = value
 
     def _guess_ac_parser(self) -> str | None:
         ac_parser = None
         if isinstance(self.resource, pathlib.Path):
             suffix = self.resource.suffix[1:].casefold()
+            supported_parsers = anyconfig.list_types()
             if not suffix:
+                recognized_file_extensions = supported_parsers + [
+                    alias + "(-> " + actual_parser + ")"
+                    for alias, actual_parser in self.ALIAS_FILE_EXTENSIONS.items()
+                    if actual_parser in supported_parsers
+                ]
                 msg = (
                     "Could not guess the anyconfig parser to use for "
                     f"{self.resource!r}.\n"
-                    f"Available parsers: {', '.join(anyconfig.list_types())}"
+                    f"Recognized file extensions: {recognized_file_extensions}"
                 )
                 raise UnspecifiedParserError(msg)
-            ac_parser = self.FILEEXT_PARSER_ALIASES.get(suffix, suffix)
+            ac_parser = self.ALIAS_FILE_EXTENSIONS.get(suffix, suffix)
+            if (
+                ac_parser == "cbor2"
+                and "cbor2" not in supported_parsers
+                and "cbor" in supported_parsers
+            ):
+                ac_parser = "cbor"
         return ac_parser
 
     def load_into(
         self,
         config_class: type[ConfigModelT],
-        blob: str,
+        blob: str | bytes,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration into a `ConfigModel` subclass.
 
         Parameters
@@ -594,15 +718,15 @@
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     async def async_load_into(
         self,
         config_class: type[ConfigModelT],
-        blob: str,
+        blob: str | bytes,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration into a `ConfigModel` subclass asynchronously.
 
         Parameters
@@ -623,15 +747,15 @@
         dict_config = await self.load_dict_async(blob, ac_parser=ac_parser, **kwargs)
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     def _load_dict_impl(
         self,
-        blob: str,
+        blob: str | bytes,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
         ac_parser = ac_parser or self.ac_parser or self._guess_ac_parser()
         if ac_parser is None:
             msg = "Cannot read configuration because `ac_parser` was not specified"
             raise UnspecifiedParserError(msg)
@@ -648,15 +772,15 @@
                 f"got {type(loaded).__name__}."
             )
             raise TypeError(msg)
         return dict(loaded)
 
     def load_dict(
         self,
-        blob: str,
+        blob: str | bytes,
         ac_parser: str | None = None,
         *,
         preprocess: bool = True,
         **kwargs: Any,
     ) -> dict[str, Any]:
         """
         Load the configuration into a dictionary. The dictionary is
@@ -680,15 +804,15 @@
         loaded = self._load_dict_impl(blob, ac_parser=ac_parser, **kwargs)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
         return loaded
 
     async def load_dict_async(
         self,
-        blob: str,
+        blob: str | bytes,
         ac_parser: str | None = None,
         *,
         preprocess: bool = True,
         **kwargs: Any,
     ) -> dict[str, Any]:
         """
         Load the configuration into a dictionary asynchronously.
@@ -737,19 +861,17 @@
         if ac_parser is None:
             ac_parser = self.ac_parser
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
-            tok = _exporting.set(True)  # noqa: FBT003
-            ctx = contextvars.copy_context()
-            _exporting.reset(tok)
-            return ctx.run(config.json, **export_kwargs)
-        data = export(config, **export_kwargs)
+            _exporting.set(True)  # noqa: FBT003
+            return isolate(config.json, **export_kwargs)
+        data = export_model(config, **export_kwargs)
         return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     async def dump_config_async(
         self,
         config: ConfigModelT,
         ac_parser: str | None = None,
         **kwargs: Any,
@@ -773,19 +895,17 @@
         if ac_parser is None:
             ac_parser = self.ac_parser
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
-            tok = _exporting.set(True)  # noqa: FBT003
-            task = asyncio.create_task(config.json_async(**export_kwargs))
-            _exporting.reset(tok)
-            return await task
-        data = await export_async(config, **export_kwargs)
+            _exporting.set(True)  # noqa: FBT003
+            return await isolate_async(config.json_async, **export_kwargs)
+        data = await export_model_async(config, **export_kwargs)
         return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
         **kwargs: Any,
@@ -811,21 +931,33 @@
         if ac_parser is None:
             msg = (
                 "Cannot write configuration because `ac_parser` was not specified"
                 f"for agent {self}"
             )
             raise UnspecifiedParserError(msg)
         kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(pre_serialize(data), ac_parser=ac_parser, **kwargs)
+        return anyconfig.dumps(export_hook(data), ac_parser=ac_parser, **kwargs)
 
     @property
     def is_url(self) -> bool:
-        """Whether the resource is a URL."""
+        """
+        Whether the resource is a URL.
+
+        This simply checks if the resource object is a string, since local paths
+        are converted into `pathlib.Path` objects.
+        """
         return isinstance(self.resource, str)
 
+    @property
+    def uses_binary_data(self) -> bool:
+        """
+        Whether the resource uses bytes for storing data, not str.
+        """
+        return self._uses_binary_data or self.ac_parser in self.BINARY_AC_PARSERS
+
     def open_resource(self, **kwds: Any) -> ConfigIO:
         """
         Open the configuration file.
 
         Parameters
         ----------
         **kwds
@@ -834,14 +966,16 @@
             For local files, these are passed to ``builtins.open()``.
 
         Returns
         -------
         The opened resource.
         """
         if self.resource is None:
+            if self.uses_binary_data:
+                return io.BytesIO()
             return io.StringIO()
         if self.is_url:
             url = urllib.parse.urlparse(cast(str, self.resource))
             if url.scheme not in self.allowed_url_schemes:
                 msg = (
                     f"URL scheme {url.scheme!r} is not allowed, "
                     f"must be one of {self.allowed_url_schemes!r}"
@@ -935,20 +1069,22 @@
         kwargs: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         if not kwargs:
             kwargs = self.default_kwargs
         new_kwargs = cast(dict[str, Any], kwargs).copy()
         if not self.is_url:
             if method == "read":
-                new_kwargs.setdefault("mode", "r")
+                new_kwargs.setdefault("mode", "rb" if self.uses_binary_data else "r")
             elif method == "write":
-                new_kwargs.setdefault("mode", "w")
+                new_kwargs.setdefault("mode", "wb" if self.uses_binary_data else "w")
             else:
                 msg = f"Invalid resource access method: {method!r}"
                 raise ValueError(msg)
+        if self.uses_binary_data:
+            new_kwargs.pop("encoding", None)
         return new_kwargs
 
     def read(
         self,
         *,
         config_class: type[ConfigModelT],
         create_kwargs: dict[str, Any] | None = None,
@@ -980,15 +1116,15 @@
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 self.write(blob, **(create_kwargs or {}))
             else:
                 raise
         return self.load_into(config_class, blob, **self.load_options)
 
-    def write(self, blob: str, **kwargs: Any) -> int:
+    def write(self, blob: str | bytes, **kwargs: Any) -> int:
         """
         Write the configuration file.
 
         Parameters
         ----------
         blob
             The string/bytes to write into the resource.
@@ -997,15 +1133,15 @@
 
         Returns
         -------
         The number of bytes written.
         """
         kwargs = self._get_default_kwargs("write", kwargs=kwargs)
         with self.open_resource(**kwargs) as fp:
-            return fp.write(blob)
+            return fp.write(cast(str, blob))
 
     async def read_async(
         self,
         *,
         config_class: type[ConfigModelT],
         create_kwargs: dict[str, Any] | None = None,
         **kwargs: Any,
@@ -1036,15 +1172,15 @@
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 await self.write_async(blob, **(create_kwargs or {}))
         return await self.async_load_into(config_class, blob, **self.load_options)
 
     async def write_async(
         self,
-        blob: str,
+        blob: str | bytes,
         **kwargs: Any,
     ) -> int:
         """
         Write the configuration file asynchronously.
 
         Parameters
         ----------
@@ -1055,24 +1191,26 @@
 
         Returns
         -------
         The number of bytes written.
         """
         kwargs = self._get_default_kwargs("write", kwargs=kwargs)
         async with self.open_resource_async(**kwargs) as fp:
-            return await fp.write(blob)
+            # Technically those might be also bytes,
+            # todo(bswck): type it properly
+            return await fp.write(cast(str, blob))
 
     @classmethod
     def from_directive_context(
         cls,
         ctx: DirectiveContext,
         /,
         route_separator: str = ":",
         route_class: type[ConfigRoute] | None = None,
-    ) -> tuple[ConfigAgent[ConfigModelT], SupportsRoute | None]:
+    ) -> tuple[ConfigAgent[ConfigModelT], ConfigRouteLike | None]:
         """
         Create a configuration agent from a preprocessor directive context.
         Return an optional scope that the context points to.
 
         Parameters
         ----------
         route_class
@@ -1081,15 +1219,15 @@
 
         Returns
         -------
         The configuration agent.
         """
         if route_class is None:
             route_class = ConfigRoute
-        route: SupportsRoute | None = None
+        route: ConfigRouteLike | None = None
         args: list[Any] = []
         kwargs: dict[str, Any] = {}
         if isinstance(ctx.snippet, str):
             path, _, route = ctx.snippet.partition(route_separator)
             route = ConfigRoute(
                 route.strip().replace(route_separator, route_class.TOK_DOT)
             )
@@ -1103,23 +1241,43 @@
         else:
             msg = (
                 f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
             )
             raise ValueError(msg)
         return cls(*args, **kwargs), str(route)
 
+    @classmethod
+    def register_file_extension(
+        cls,
+        file_extension: str,
+        *,
+        ac_parser: str,
+    ) -> None:
+        """
+        Register a file extension with the proper anyconfig parser to use.
+
+        Parameters
+        ----------
+        file_extension
+        ac_parser
+
+        Returns
+        -------
+        """
+        cls.ALIAS_FILE_EXTENSIONS[file_extension] = ac_parser
+
     def __repr__(self) -> str:
         resource = self.resource
         return f"{type(self).__name__}({resource=!r})"
 
 
 def at(
     mapping: Any,
-    route: SupportsRoute,
-    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _get_object_dict,
+    route: ConfigRouteLike,
+    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _get_object_state,
     agent: ConfigAgent[ConfigModelT] | None = None,
 ) -> Any:
     """
     Get an item at a route.
 
     Parameters
     ----------
@@ -1132,15 +1290,15 @@
 
     Returns
     -------
     The item at the route.
     """
     route = ConfigRoute(route)
     route_here = []
-    scope = _get_object_dict(mapping)
+    scope = _get_object_state(mapping)
     try:
         for part in route:
             route_here.append(part)
             scope = converter_func(scope)[part]
     except KeyError:
         raise ResourceLookupError(agent, route_here) from None
     return scope
@@ -1159,17 +1317,19 @@
         The mapping to use.
     route
         The route to the item.
     """
 
     owner: ConfigModelT
     mapping: dict[str, Any] | None
-    route: SupportsRoute
+    route: ConfigRouteLike
 
-    def get(self, route: SupportsRoute | None = None, default: Any = Undefined) -> Any:
+    def get(
+        self, route: ConfigRouteLike | None = None, default: Any = Undefined
+    ) -> Any:
         """
         Get the value of the item.
 
         Parameters
         ----------
         route
             The route to the item. If not given, the sole route of this item is used.
@@ -1207,20 +1367,20 @@
         Returns
         -------
         The updated mapping.
         """
         route = list(ConfigRoute(self.route))
         mapping = self.mapping or self.owner
         key = route.pop()
-        scope = _get_object_dict(mapping)
+        scope = _get_object_state(mapping)
         route_here = []
         try:
             for part in route:
                 route_here.append(part)
-                scope = _get_object_dict(scope[part])
+                scope = _get_object_state(scope[part])
             scope[key] = value
         except KeyError:
             raise ConfigAccessError(self.owner, route_here) from None
         return mapping
 
     async def save_async(self, **kwargs: Any) -> int:
         """
@@ -1625,15 +1785,18 @@
 
     Returns
     -------
     The context of the configuration model.
     """
     context = get_context_or_none(config)
     if context is None:
-        raise RuntimeError("Cannot get context of unbound configuration model")
+        raise RuntimeError(
+            "This model is either inside a list "
+            "or was not loaded by a configuration agent."
+        )
     return context
 
 
 def get_context_or_none(config: ConfigModelT) -> BaseContext[ConfigModelT] | None:
     """
     Get the context of the configuration model safely.
 
@@ -1647,19 +1810,54 @@
     The context of the configuration model.
     """
     return cast(
         Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
     )
 
 
+# noinspection PyUnusedLocal
+@make_generic_validator
+def _common_field_validator(
+    cls: type[ConfigModelT],
+    v: Any,
+    values: dict[str, Any],
+    field: pydantic.fields.ModelField,
+    config: pydantic.BaseConfig,
+) -> Any:
+    post_hook_value = field_hook(field.outer_type_, v)
+    disallow_interpolation = getattr(config, "disallow_interpolation", False)
+    disallowed_interpolation_fields = set()
+
+    interpolation_tracker = current_interpolation_tracker.get()
+
+    if interpolation_tracker is None:
+        interpolation_tracker = {}
+        current_interpolation_tracker.set(interpolation_tracker)
+
+    if not isinstance(disallow_interpolation, bool):
+        disallowed_interpolation_fields = set(disallow_interpolation)
+    if (
+        field.field_info.extra.get("interpolate", True)
+        and field.alias not in disallowed_interpolation_fields
+    ):
+        old_value = post_hook_value
+        new_value = interpolate(
+            post_hook_value, cls.get_interpolation_context() | values
+        )
+        if old_value != new_value:
+            interpolation_tracker[field.alias] = (old_value, copy.copy(new_value))
+        post_hook_value = new_value
+    return post_hook_value
+
+
 def _json_encoder(
     model_encoder: collections.abc.Callable[..., Any], value: Any, **kwargs: Any
 ) -> Any:
     initial_state_type = type(value)
-    converted_value = pre_serialize(value)
+    converted_value = export_hook(value)
     if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
 class ConfigModelMetaclass(ModelMetaclass):
     def __new__(
@@ -1668,85 +1866,174 @@
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **kwargs: Any,
     ) -> type:
         namespace |= dict.fromkeys(
             (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
         )
+        namespace[INTERPOLATION_TRACKER] = pydantic.PrivateAttr(default_factory=dict)
 
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
 
-        new_class = super().__new__(cls, name, bases, namespace, **kwargs)
-        for field in new_class.__fields__.values():
+        model = super().__new__(cls, name, bases, namespace, **kwargs)
+        for field in model.__fields__.values():
+            if field.pre_validators is None:
+                field.pre_validators = []
+            field.pre_validators[:] = [_common_field_validator, *field.pre_validators]
             if type(field.outer_type_) is ConfigModelMetaclass:
-                if field.pre_validators is None:
-                    field.pre_validators = []
                 validator = make_generic_validator(
                     field.outer_type_.__field_setup__  # type: ignore[attr-defined]
                 )
-                field.pre_validators.insert(0, validator)
-        new_class.__json_encoder__ = functools.partial(
-            _json_encoder,
-            new_class.__json_encoder__,
-        )
-        return cast(type, new_class)
+                field.pre_validators[:] = [
+                    _common_field_validator,
+                    validator,
+                    *field.pre_validators,
+                ]
+        model_encoder = model.__json_encoder__
+        model.__json_encoder__ = functools.partial(_json_encoder, model_encoder)
+        return cast(type, model)
+
+
+class ConfigInterpolationTemplate(string.Template):
+    idpattern = r"(?a:[_a-z][\\\.\[\]_a-z0-9]*)"
+    flags = re.IGNORECASE | re.UNICODE
+
+
+@functools.singledispatch
+def interpolate(value: Any, _ctx: dict[str, Any]) -> Any:
+    return value
+
+
+@interpolate.register(str)
+def _interpolate_str(value: str, ctx: dict[str, Any]) -> str:
+    template = ConfigInterpolationTemplate(value)
+    return template.safe_substitute(ctx)
+
+
+# Interpolation for mutable types is a non-trivial task.
+
+# @interpolate.register(dict)
+# def _interpolate_dict(value: dict[Any, Any], ctx: dict[str, Any]) -> dict[Any, Any]:
+#     return {
+#         interpolate(k, ctx): interpolate(v, ctx) for k, v in value.items()
+#     }
+#
+#
+# @interpolate.register(list)
+# def _interpolate_lst(value: list, ctx: dict[str, Any]) -> list[Any]:
+#     return {
+#         interpolate(k, ctx): interpolate(v, ctx) for k, v in value.items()
+#     }
+
+
+class ConfigMeta(pydantic.BaseSettings.Config):
+    """
+    Meta-configuration for configuration models.
+
+    See https://docs.pydantic.dev/latest/usage/model_config/ for more information
+    on model configurations.
+
+    Attributes
+    ----------
+    resource
+        The configuration resource to read from/write to.
+
+        If a string, it will be interpreted as a path to a file.
+
+    ac_parser
+        The anyconfig parser to use.
+
+    autoupdate_forward_refs
+        Whether to automatically update forward references
+        when `ConfigModel.load()` or `ConfigModel.load_async()`
+        methods are called. For convenience, defaults to `True`.
+
+    And all other attributes from `pydantic.BaseSettings.Config`.
+    """
+
+    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
+    ac_parser: str | None = None
+    validate_assignment: bool = True
+    autoupdate_forward_refs: bool = True
+
+    Extra = pydantic.Extra
 
 
 class ConfigModel(
     pydantic.BaseSettings,
     metaclass=ConfigModelMetaclass,
     root=True,
 ):
     """The base class for configuration models."""
 
+    __config__ = ConfigMeta
+
     def __init__(self, **kwargs: Any) -> None:
         # Set private attributes via the constructor
         # to allow preprocessor-related instances to exist.
         for private_attr in self.__private_attributes__:
             value = kwargs.pop(private_attr, Undefined)
             if value is not Undefined:
-                setattr(self, private_attr, value)
                 if private_attr == CONTEXT:
+                    context = current_context.get()
+                    if context:
+                        value = context
                     current_context.set(value)
+                object.__setattr__(self, private_attr, value)
         super().__init__(**kwargs)
 
+    def __deepcopy__(
+        self: ConfigModelT, memodict: dict[Any, Any] | None = None
+    ) -> ConfigModelT:
+        state = dict(self._iter(to_dict=False))
+        state.pop(LOCAL, None)
+        state.pop(TOKEN, None)
+        clone = copy.deepcopy(state)
+        return type(self).parse_obj(
+            {
+                field.alias: clone[field_name]
+                for field_name, field in self.__fields__.items()
+            }
+        )
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        getattr(self, LOCAL).run(super().__setattr__, key, value)
+
     def _init_private_attributes(self) -> None:
         super()._init_private_attributes()
         local = contextvars.copy_context()
-        setattr(self, LOCAL, local)
+        object.__setattr__(self, LOCAL, local)
         tok = getattr(self, TOKEN, None)
         if tok:
             current_context.reset(tok)
 
+    @isolate_calls
     def export(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
-        tok = _exporting.set(True)  # noqa: FBT003
-        ctx = contextvars.copy_context()
-        _exporting.reset(tok)
-        return ctx.run(self.dict, **kwargs)
+        _exporting.set(True)  # noqa: FBT003
+        return isolate(self.dict, **kwargs)
 
+    @isolate_calls
     async def export_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
-        tok = _exporting.set(True)  # noqa: FBT003
-        task = asyncio.create_task(self.dict_async(**kwargs))
-        _exporting.reset(tok)
-        return await task
+        _exporting.set(True)  # noqa: FBT003
+        return await isolate_async(self.dict_async, **kwargs)
 
     async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Get the dictionary representation of the configuration model.
 
         Returns
         -------
@@ -1785,54 +2072,70 @@
             data = data[ROOT_KEY]
         return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
 
     def _iter(  # type: ignore[override]
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
-            state = {}
+            state: dict[str, Any] = {}
             for key, value in super()._iter(**kwargs):
-                field = self.__fields__.get(key)
-                actual_key = field.alias if field else key
-                state[actual_key] = value
+                state |= [self._iter_hook(key, value)]
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 context.agent.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     async def _iter_async(
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
-            state = {}
+            state: dict[str, Any] = {}
             for key, value in super()._iter(**kwargs):
-                field = self.__fields__.get(key)
-                actual_key = field.alias if field else key
-                state[actual_key] = value
+                state |= [self._iter_hook(key, value)]
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 await context.agent.processor_class.export_async(
                     state, metadata=metadata
                 )
             return ((key, value) for key, value in state.items())
         return super()._iter(**kwargs)
 
+    def _iter_hook(
+        self,
+        key: str,
+        value: Any,
+    ) -> tuple[str, Any]:
+        interpolation_tracker = getattr(self, LOCAL).get(current_interpolation_tracker)
+        field = self.__fields__.get(key)
+        actual_key = field.alias if field else key
+        interpolation_track = interpolation_tracker.get(actual_key)
+        if interpolation_track:
+            old_value, new_value = interpolation_track
+            # if value != new_value:
+            #     raise InterpolationError(
+            #         f"Cannot restore the value of {actual_key!r} "
+            #         "before interpolation."
+            #     )
+            value = old_value
+        return actual_key, value
+
     @classmethod
     @no_type_check
     def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
         if _exporting.get():
-            exporter = export.dispatch(type(value))
+            exporter = export_model.dispatch(type(value))
             if (
-                isinstance(value, BaseModel) or exporter != export.dispatch(object)
+                isinstance(value, BaseModel)
+                or exporter != export_model.dispatch(object)
             ) and to_dict:
-                value_dict = export(value, **kwds)
+                value_dict = export_model(value, **kwds)
                 if ROOT_KEY in value_dict:
                     return value_dict[ROOT_KEY]
                 return value_dict
         return super()._get_value(value, to_dict=to_dict, **kwds)
 
     @classmethod
     def _resolve_agent(
@@ -1870,15 +2173,15 @@
         It is a copy of the configuration state
         at the last time of loading, reloading or saving.
         """
         return get_context(self).initial_state
 
     def at(
         self: ConfigModelT,
-        route: SupportsRoute | None = None,
+        route: ConfigRouteLike | None = None,
     ) -> ConfigModelT | ConfigAt[ConfigModelT]:
         """
         Lazily point to a specific item in the configuration.
 
         Parameters
         ----------
         route
@@ -1896,33 +2199,25 @@
                 self_at = context.at
             if self_at is not None:
                 return self_at
             return self
         return ConfigAt(self, None, route)
 
     @overload
-    def get(
-        self: ConfigModelT,
-        route: None = None,
-        default: Any = ...
-    ) -> ConfigModelT:
+    def get(self: ConfigModelT, route: None = None, default: Any = ...) -> ConfigModelT:
         ...
 
     @overload
     def get(
-        self: ConfigModelT,
-        route: SupportsRoute = ...,
-        default: Any = ...
+        self: ConfigModelT, route: ConfigRouteLike = ..., default: Any = ...
     ) -> Any:
         ...
 
     def get(
-        self,
-        route: SupportsRoute | None = None,
-        default: Any = Undefined
+        self, route: ConfigRouteLike | None = None, default: Any = Undefined
     ) -> Any:
         """
         Get a value from the configuration.
 
         Parameters
         ----------
         route
@@ -1959,29 +2254,16 @@
         Returns
         -------
         None
         """
         context = get_context(self)
         self.__dict__.update(context.initial_state)
 
-    def __deepcopy__(
-        self: ConfigModelT, memodict: dict[Any, Any] | None = None
-    ) -> ConfigModelT:
-        state = dict(self._iter(to_dict=False))
-        state.pop(LOCAL, None)
-        state.pop(TOKEN, None)
-        clone = copy.deepcopy(state)
-        return type(self).parse_obj(
-            {
-                field.alias: clone[field_name]
-                for field_name, field in self.__fields__.items()
-            }
-        )
-
     @classmethod
+    @isolate_calls
     def load(
         cls: type[ConfigModelT],
         resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
         ac_parser: str | None = None,
         **kwargs: Any,
@@ -2006,54 +2288,55 @@
         self
         """
         agent = cls._resolve_agent(
             resource,
             ac_parser=ac_parser,
             create_if_missing=create_if_missing,
         )
-        context = Context(agent)  # type: Context[ConfigModelT]
-        current_context.set(context)
+        current_context.set(Context(agent))
         local = contextvars.copy_context()
         if getattr(
             cls.__config__,
             "autoupdate_forward_refs",
             ConfigMeta.autoupdate_forward_refs,
         ):
             cls.update_forward_refs()
-        config = agent.read(config_class=cls, **kwargs)
-        setattr(config, LOCAL, local)
+        config = local.run(agent.read, config_class=cls, **kwargs)
+        object.__setattr__(config, LOCAL, local)
+        context = cast(Context[ConfigModelT], local.get(current_context))
         context.owner = config
         context.initial_state = config.__dict__
         return config
 
+    @isolate_calls
     def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        tok = current_context.set(get_context(context.owner))
+        current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = context.agent.read(config_class=type(self), **kwargs)
         else:
-            changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
-        current_context.reset(tok)
+            changed = reload(cast(ConfigModelT, context.at), **kwargs)
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
+    @isolate_calls
     def save(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file.
 
         Parameters
@@ -2077,15 +2360,15 @@
             return result
         return save(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
-    def write(self, blob: str, **kwargs: Any) -> int:
+    def write(self, blob: str | bytes, **kwargs: Any) -> int:
         """
         Overwrite the configuration file with the given string or bytes.
 
         Parameters
         ----------
         blob
             The blob to write to the configuration file.
@@ -2099,14 +2382,15 @@
         context = get_context(self)
         if context.agent.is_url:
             msg = "Writing to URLs is not yet supported"
             raise NotImplementedError(msg)
         return context.agent.write(blob, **kwargs)
 
     @classmethod
+    @isolate_calls
     async def load_async(
         cls: type[ConfigModelT],
         resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         ac_parser: str | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
@@ -2129,55 +2413,59 @@
         Returns
         -------
         self
         """
         agent = cls._resolve_agent(
             resource, create_if_missing=create_if_missing, ac_parser=ac_parser
         )
-        context = Context(agent)  # type: Context[ConfigModelT]
-        current_context.set(context)
+        current_context.set(Context(agent))
         local = contextvars.copy_context()
         if getattr(
             cls.__config__,
             "autoupdate_forward_refs",
             ConfigMeta.autoupdate_forward_refs,
         ):
             cls.update_forward_refs()
-        config = await agent.read_async(config_class=cls, **kwargs)
-        setattr(config, LOCAL, local)
+        task = local.run(
+            asyncio.create_task, agent.read_async(config_class=cls, **kwargs)
+        )
+        config = await task
+        object.__setattr__(config, LOCAL, local)
+        context = cast(Context[ConfigModelT], local.get(current_context))
         context.owner = config
         return config
 
+    @isolate_calls
     async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        tok = current_context.set(get_context(context.owner))
+        current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = await context.agent.read_async(config_class=type(self), **kwargs)
         else:
             changed = await reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
-        current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
         self.update(state)
         return self
 
+    @isolate_calls
     async def save_async(
         self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
     ) -> int:
         """
         Save the configuration to the configuration file asynchronously.
 
         Parameters
@@ -2191,28 +2479,26 @@
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
-            tok = _exporting.set(True)  # noqa: FBT003
-            task = asyncio.create_task(context.agent.dump_config_async(self, **kwargs))
-            _exporting.reset(tok)
-            blob = await task
+            _exporting.set(True)  # noqa: FBT003
+            blob = await context.agent.dump_config_async(self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
-    async def write_async(self, blob: str, **kwargs: Any) -> int:
+    async def write_async(self, blob: str | bytes, **kwargs: Any) -> int:
         """
         Overwrite the configuration file asynchronously with the given string or bytes.
 
         Parameters
         ----------
         blob
             The blob to write to the configuration file.
@@ -2225,51 +2511,62 @@
         """
         context = get_context(self)
         if context.agent.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         return await context.agent.write_async(blob, **kwargs)
 
+    @staticmethod
+    def get_interpolation_context() -> dict[str, Any]:
+        """
+        Get the interpolation context of this configuration model.
+        This must be either static or class method.
+        """
+        return {}
+
     @classmethod
-    def __field_setup__(cls, value: Any, field: ModelField) -> Any:
+    def __field_setup__(cls, value: dict[str, Any], field: ModelField) -> Any:
         """
         Called when this configuration model is being initialized as a field
         of some other configuration model.
         """
         context = current_context.get()
         if context is not None:
             subcontext = context.enter(field.name)
             tok = current_context.set(subcontext)
-            state = _get_object_dict(value)
-            state[TOKEN] = tok
-            state[LOCAL] = contextvars.copy_context()
+            return _get_object_state(value) | {
+                TOKEN: tok,
+                LOCAL: contextvars.copy_context(),
+            }
         return value
 
 
-class ConfigMeta(pydantic.BaseSettings.Config):
+@field_hook.register(ConfigModel)
+def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
     """
-    Meta-configuration for the `ConfigModel` class.
+    Load a model using dict literal evaluation.
+    Solves nested dictionaries problem in INI files.
 
-    Attributes
+    Parameters
     ----------
-    resource
-        The configuration resource to read from/write to.
-
-        If a string, it will be interpreted as a path to a file.
-
-    ac_parser
-        The anyconfig parser to use.
+    cls
+        The type to load the value into.
 
-    autoupdate_forward_refs
-        Whether to automatically update forward references
-        when `ConfigModel.load()` or `ConfigModel.load_async()`
-        methods are called. For convenience, defaults to `True`.
+    value
+        The value to load.
 
-    And all other attributes from `pydantic.BaseSettings.Config`.
+    Returns
+    -------
+    The loaded value.
     """
-
-    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
-    ac_parser: str | None = None
-    validate_assignment: bool = True
-    autoupdate_forward_refs: bool = True
-
-    Extra = pydantic.Extra
+    data = value
+    if isinstance(value, str):
+        try:
+            data = ast.literal_eval(value)
+        except (SyntaxError, ValueError):
+            # Note: Strings resembling models is probably not intended
+            # to be used with automatic pickle/JSON parsing.
+            # return cls.parse_raw(value)
+            return data
+        else:
+            return cls.parse_obj(data)
+    return data
```

### Comparing `configzen-0.3.9/configzen/decorators.py` & `configzen-0.4/configzen/decorators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 import collections.abc
+import contextlib
 import functools
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, cast
 
-from configzen.config import export, export_async, post_deserialize, pre_serialize
+from configzen.config import export_hook, export_model, export_model_async, field_hook
 
 if TYPE_CHECKING:
     from configzen.typedefs import ConfigModelT, T
 
 __all__ = (
     "with_exporter",
     "with_async_exporter",
-    "with_post_deserialize",
-    "with_pre_serialize",
+    "with_field_hook",
+    "with_export_hook",
 )
 
 
-def with_pre_serialize(
+def with_export_hook(
     func: collections.abc.Callable[[T], Any], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
     Register a pre-serialization converter function for a type.
 
     Parameters
     ----------
@@ -36,102 +37,145 @@
     -------
     The conversion result class.
 
     Usage
     -----
     .. code-block:: python
 
-        @with_pre_serialize(converter_func)
+        @with_export_hook(converter_func)
         class MyClass:
             ...
 
     """
     if cls is None:
-        return functools.partial(with_pre_serialize, func)
+        return functools.partial(with_export_hook, func)
 
-    pre_serialize.register(cls, func)
+    export_hook.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
         def validator_gen() -> (
             collections.abc.Iterator[collections.abc.Callable[[Any], Any]]
         ):
-            yield lambda value: post_deserialize.dispatch(cls)(cls, value)
+            hook_func = field_hook.dispatch(cls)  # type: ignore[arg-type]
+            yield lambda value: hook_func(cls, value)
 
-        cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
+        with contextlib.suppress(TypeError):
+            cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
 
-def with_post_deserialize(
-    func: collections.abc.Callable[[Any], T], cls: type[T] | None = None
+def with_field_hook(
+    func: collections.abc.Callable[[type[T], Any], T], cls: type[T] | None = None
 ) -> type[T] | Any:
     """
-    Register a loader function for a type.
+    Register a field hook for a type.
 
     Parameters
     ----------
     func
         The loader function.
     cls
         The type to register the loader for.
 
     Returns
     -------
     The loading result class.
     """
 
     if cls is None:
-        return functools.partial(with_post_deserialize, func)
+        return functools.partial(with_field_hook, func)
 
-    post_deserialize.register(cls, func)
+    field_hook.register(cls, func)
     return cls
 
 
 def with_exporter(
-    func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
+    func: collections.abc.Callable[[ConfigModelT], dict[str, Any]] | None = None,
     cls: type[ConfigModelT] | None = None,
+    **predefined_kwargs: Any,
 ) -> type[ConfigModelT] | Any:
     """
-    Register a custom exporter for a type.
+    Register a custom exporter for a configuration model class.
 
     Parameters
     ----------
     func
         The exporter function.
     cls
         The type to register the exporter for.
     """
     if cls is None:
         return functools.partial(with_exporter, func)
 
-    export.register(cls, func)
-    if export_async.dispatch(cls) is export_async:
+    if func and predefined_kwargs:
+        raise NotImplementedError(
+            "specifying both a function and predefined kwargs is not supported"
+        )
 
-        async def default_async_func(obj: Any) -> Any:
-            return func(obj)
+    if func is None:
 
-        export_async.register(cls, default_async_func)
+        def func(obj: Any, **kwargs: Any) -> Any:
+            kwargs |= predefined_kwargs
+            return obj.export(**kwargs)
+
+        export_model.register(cls, func)
+
+        if export_model_async.dispatch(cls) is export_model_async:
+
+            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+                kwargs |= predefined_kwargs
+                return await obj.export_async(**kwargs)
+
+            export_model_async.register(cls, default_async_func)
+    else:
+        export_model.register(cls, func)
+        if export_model_async.dispatch(cls) is export_model_async:
+
+            async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+                nonlocal func
+                if TYPE_CHECKING:
+                    func = cast(collections.abc.Callable[..., dict[str, Any]], func)
+
+                return func(obj, **kwargs)
+
+            export_model_async.register(cls, default_async_func)
     return cls
 
 
 def with_async_exporter(
     func: collections.abc.Callable[
         [ConfigModelT], collections.abc.Coroutine[Any, Any, dict[str, Any]]
-    ],
+    ]
+    | None = None,
     cls: type[ConfigModelT] | None = None,
+    **predefined_kwargs: Any,
 ) -> type[ConfigModelT] | Any:
     """
-    Register a custom exporter for a type.
+    Register a custom exporter for a configuration model class.
 
     Parameters
     ----------
     func
         The exporter function.
     cls
         The type to register the exporter for.
     """
     if cls is None:
         return functools.partial(with_exporter, func)
 
-    export_async.register(cls, func)
+    if func and predefined_kwargs:
+        raise NotImplementedError(
+            "specifying both a function and default kwargs is not supported"
+        )
+
+    if func is None:
+
+        async def default_async_func(obj: Any, **kwargs: Any) -> Any:
+            kwargs |= predefined_kwargs
+            return await obj.export_async(**kwargs)
+
+        export_model_async.register(cls, default_async_func)
+    else:
+        export_model_async.register(cls, func)
     return cls
```

### Comparing `configzen-0.3.9/configzen/errors.py` & `configzen-0.4/configzen/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     from configzen.typedefs import ConfigModelT
 
 
 class ConfigError(Exception):
     """An error occurred while loading a configuration."""
 
 
+class InterpolationError(ConfigError):
+    """An error occurred with regard to interpolating a configuration."""
+
+
 class IncorrectConfigError(ConfigError):
     """An error occurred while loading a configuration."""
 
 
 class InternalSyntaxError(ConfigError):
     """Error in route syntax."""
 
@@ -62,21 +66,21 @@
 class UnavailableParserError(ConfigError):
     MISSING_DEPENDENCIES: dict[str, str] = {
         "yaml": "pyyaml (or ruamel.yaml)",
         "toml": "toml",
         "ion": "anyconfig-ion-backend",
         "bson": "anyconfig-bson-backend",
         "msgpack": "anyconfig-msgpack-backend",
-        "cbor": "anyconfig-cbor-backend (or anyconfig-cbor2-backend)",
+        "cbor": "anyconfig-cbor2-backend (or anyconfig-cbor-backend)",
         "configobj": "anyconfig-configobj-backend",
     }
 
     def __init__(self, parser_name: str, agent: ConfigAgent[ConfigModelT]) -> None:
         missing_dependency: str = self.MISSING_DEPENDENCIES.get(
-            parser_name, f"<the proper anyconfig backend for {parser_name} files>"
+            parser_name, f"<the proper anyconfig backend for {parser_name!r} files>"
         )
         super().__init__(
             f"The {parser_name!r} parser required to load configuration "
             f"for agent {agent} is not available.\n"
             f"Install it with `pip install {missing_dependency}`."
         )
```

### Comparing `configzen-0.3.9/configzen/field.py` & `configzen-0.4/configzen/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 from pydantic.fields import Field, FieldInfo, Undefined
 
 __all__ = ("ConfigField",)
 
 
 # noinspection PyPep8Naming
-def ConfigField(  # noqa: N802
-    default: Any = Undefined,
-    **kwargs: Any
-) -> FieldInfo:
+def ConfigField(default: Any = Undefined, **kwargs: Any) -> FieldInfo:  # noqa: N802
     # Since configzen involves BaseSettings implicitly,
     # this would be very convenient to have.
     alias = kwargs.get("alias")
     env = kwargs.get("env")
     if alias is not None and env is None:
         kwargs["env"] = alias
     return cast(FieldInfo, Field(default, **kwargs))
```

### Comparing `configzen-0.3.9/configzen/processor.py` & `configzen-0.4/configzen/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import asyncio
 import copy
 import dataclasses
 import enum
 import pathlib
 from collections.abc import Callable
-from pydantic.fields import Undefined
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
+from pydantic.fields import Undefined
 
 from configzen.errors import ConfigPreprocessingError
-from configzen.typedefs import ConfigModelT, SupportsRoute
+from configzen.typedefs import ConfigModelT, ConfigRouteLike
 
 if TYPE_CHECKING:
     from configzen.config import BaseContext, ConfigAgent
 
 __all__ = (
     "DirectiveContext",
     "directive",
@@ -93,15 +93,15 @@
 
 
 def parse_directive_call(
     prefix: str,
     directive_name: str,
 ) -> str:
     if directive_name.startswith(prefix):
-        directive_name = directive_name[len(prefix):].casefold()
+        directive_name = directive_name[len(prefix) :].casefold()
 
         if not directive_name.isidentifier():
             msg = f"Invalid directive name: {directive_name}"
             raise ConfigPreprocessingError(msg)
 
     return directive_name
 
@@ -550,15 +550,15 @@
         For more information see `copy`.
         """
         await self._substitute_async(ctx, preprocess=False, preserve=False)
 
     def _get_substitution_means(
         self, ctx: DirectiveContext  # , *, preserve: bool
     ) -> tuple[
-        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], SupportsRoute | None
+        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], ConfigRouteLike | None
     ]:
         agent_class = type(self.agent)
 
         # todo(bswck): raise on include and extend combined
         # if preserve and ???:
         #     msg = (
         #         "Using more than one ??? directive "
@@ -572,15 +572,15 @@
 
         if agent.resource == self.agent.resource:
             raise ConfigPreprocessingError(
                 f"{agent.resource} tried to {ctx.directive!r} on itself"
             )
 
         actual_agent = agent
-        if agent.relative:
+        if agent.is_relative:
             parent = cast(pathlib.Path, self.agent.resource).parent
             child = cast(pathlib.Path, agent.resource)
 
             actual_agent = copy.copy(agent)
             actual_agent.resource = parent / child
 
         return actual_agent, agent, route
@@ -618,15 +618,15 @@
             preprocess=preprocess,
             preserve=preserve,
         )
 
     @staticmethod
     def _substitute_impl(  # noqa: PLR0913
         ctx: DirectiveContext,
-        route: SupportsRoute | None,
+        route: ConfigRouteLike | None,
         *,
         source: dict[str, Any],
         agent: ConfigAgent[ConfigModelT],
         preprocess: bool,
         preserve: bool,
     ) -> None:
         from configzen.config import CONTEXT, Context, at
@@ -663,15 +663,15 @@
         Exports model state preserving substition directive calls in the model state.
 
         Parameters
         ----------
         metadata
         state
         """
-        from configzen.config import CONTEXT, at, pre_serialize
+        from configzen.config import CONTEXT, at, export_hook
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         key_order = metadata["key_order"]
         agent = context.agent
@@ -685,26 +685,26 @@
 
         substituted_values = loaded.copy()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, Undefined)
             if counterpart_value is Undefined:
                 continue
-            counterpart_value = pre_serialize(counterpart_value)
+            counterpart_value = export_hook(counterpart_value)
 
             if is_dict_like(value):
                 if EXPORT in value:
                     value.pop(CONTEXT, None)
                     cls.export(value, metadata=value.pop(EXPORT))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
-                        (orig := value.get(sub_key, Undefined))
-                        is Undefined or orig != comp
+                        (orig := value.get(sub_key, Undefined)) is Undefined
+                        or orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
@@ -738,15 +738,15 @@
         Exports model state preserving substition directive calls in the model state.
 
         Parameters
         ----------
         metadata
         state
         """
-        from configzen.config import CONTEXT, at, pre_serialize
+        from configzen.config import CONTEXT, at, export_hook
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         key_order = metadata["key_order"]
         agent = context.agent
@@ -760,26 +760,26 @@
 
         substituted_values = loaded.copy()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, Undefined)
             if counterpart_value is Undefined:
                 continue
-            counterpart_value = pre_serialize(counterpart_value)
+            counterpart_value = export_hook(counterpart_value)
 
             if is_dict_like(value):
                 if EXPORT in value:
                     value.pop(CONTEXT, None)
                     await cls.export_async(value, metadata=value.pop(EXPORT))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
-                        (orig := value.get(sub_key, Undefined))
-                        is Undefined or orig != comp
+                        (orig := value.get(sub_key, Undefined)) is Undefined
+                        or orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
@@ -810,24 +810,24 @@
         *,
         state: dict[str, Any],
         overrides: dict[str, Any],
         values: dict[str, Any],
         route: str | None,
         key_order: list[str],
     ) -> None:
-        # TODO: Optimize. We iterate over the same way too many times.
+        from configzen.config import export_hook
 
         state |= overrides
         extras: dict[str, Any] = {
             key: state.pop(key) for key in set(state) if key not in key_order
         }
 
         if values:
             substitution_directive = cls.directive(Directives.EXTEND)
-            resource = str(context.agent.resource)
+            resource = str(export_hook(context.agent.resource))
             if route:
                 resource = cls.route_separator.join((resource, route))
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
             }
```

### Comparing `configzen-0.3.9/configzen/route.py` & `configzen-0.4/configzen/route.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
 import collections.abc
 import functools
-from typing import Any, ClassVar, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from configzen.errors import InternalSyntaxError, formatted_syntax_error
 
 if TYPE_CHECKING:
-    from configzen.typedefs import SupportsRoute
+    from configzen.typedefs import ConfigRouteLike
 
 __all__ = ("ConfigRoute",)
 
 
 class ConfigRoute:
     TOK_DOT: ClassVar[str] = "."
     TOK_ESCAPE: ClassVar[str] = "\\"
     TOK_DOTLISTESC_ENTER: ClassVar[str] = "["
     TOK_DOTLISTESC_EXIT: ClassVar[str] = "]"
 
-    def __init__(self, route: SupportsRoute, *, allow_empty: bool = False) -> None:
+    def __init__(self, route: ConfigRouteLike, *, allow_empty: bool = False) -> None:
         items = self.parse(route)
         if not (allow_empty or items):
             raise ValueError("Empty configuration route")
         self.items = items
 
     @classmethod
-    def parse(cls, route: SupportsRoute) -> list[str]:
+    def parse(cls, route: ConfigRouteLike) -> list[str]:
         if isinstance(route, ConfigRoute):
             return route.items
         if isinstance(route, list):
             return route
         if isinstance(route, str):
             with formatted_syntax_error(route):
                 return cls._decompose(route)
@@ -110,15 +110,15 @@
                 self.TOK_DOTLISTESC_EXIT + self.TOK_ESCAPE + self.TOK_DOT,
             )
             if self.TOK_DOT in fragment
             else fragment.join(raw)
             for fragment in self.items
         )
 
-    def enter(self, subroute: SupportsRoute) -> ConfigRoute:
+    def enter(self, subroute: ConfigRouteLike) -> ConfigRoute:
         return type(self)(self.items + self.parse(subroute))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, ConfigRoute):
             return self.items == other.items
         if isinstance(other, str):
             return self.items == self.decompose(other)
```

### Comparing `configzen-0.3.9/configzen/typedefs.py` & `configzen-0.4/configzen/typedefs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     from configzen.config import ConfigModel
     from configzen.route import ConfigRoute
 
 T = TypeVar("T")
 
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
-SupportsRoute: TypeAlias = Union[str, list[str], "ConfigRoute"]
+ConfigRouteLike: TypeAlias = Union[str, list[str], "ConfigRoute"]
 
 ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
 AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
 RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
 NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
 IncludeExcludeT: TypeAlias = Optional[
     Union[
```

### Comparing `configzen-0.3.9/LICENSE` & `configzen-0.4/LICENSE`

 * *Files identical despite different names*

