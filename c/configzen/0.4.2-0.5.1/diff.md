# Comparing `tmp/configzen-0.4.2.tar.gz` & `tmp/configzen-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.2.tar", max compression
+gzip compressed data, was "configzen-0.5.1.tar", max compression
```

## Comparing `configzen-0.4.2.tar` & `configzen-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
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
+-rw-r--r--   0        0        0      536 2023-06-29 17:13:35.607166 configzen-0.5.1/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.5.1/configzen/__main__.py
+-rw-r--r--   0        0        0     1437 2023-06-29 16:34:46.964275 configzen-0.5.1/configzen/_isolation.py
+-rw-r--r--   0        0        0     3394 2023-06-29 17:46:07.418020 configzen-0.5.1/configzen/_setup.py
+-rw-r--r--   0        0        0    77224 2023-06-29 17:47:37.718956 configzen-0.5.1/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.5.1/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.5.1/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.5.1/configzen/field.py
+-rw-r--r--   0        0        0     5157 2023-06-29 17:56:51.047974 configzen-0.5.1/configzen/interpolation.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.5.1/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.5.1/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.5.1/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 16:34:46.955277 configzen-0.5.1/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 18:00:11.297262 configzen-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    14350 2023-06-29 18:06:31.120725 configzen-0.5.1/README.md
+-rw-r--r--   0        0        0    14869 1970-01-01 00:00:00.000000 configzen-0.5.1/PKG-INFO
```

### Comparing `configzen-0.4.2/configzen/__main__.py` & `configzen-0.5.1/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/_isolation.py` & `configzen-0.5.1/configzen/_isolation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 import collections.abc
 import contextvars
-import functools
 from typing import Any, cast
 
-from configzen.typedefs import T
+from configzen.typedefs import P, T
 
 
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
-            lambda *args, **kwargs: isolate_async(func, *args, **kwargs)
+            collections.abc.Callable[P, T],
+            lambda *args, **kwargs: isolate_async(func, *args, **kwargs),
         )
     return lambda *args, **kwargs: isolate(func, *args, **kwargs)
 
 
 def isolate(
     func: collections.abc.Callable[..., T],
     *args: Any,
```

### Comparing `configzen-0.4.2/configzen/config.py` & `configzen-0.5.1/configzen/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,26 +54,24 @@
     # otherhost  # <- not anotherhost, because we reloaded only port
     # 5432
 """
 
 from __future__ import annotations
 
 import abc
-import ast
 import asyncio
 import collections.abc
 import contextvars
 import copy
 import dataclasses
 import functools
+import importlib
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
@@ -86,35 +84,40 @@
 )
 
 import anyconfig
 import pydantic
 from anyconfig.utils import filter_options, is_dict_like, is_list_like
 from pydantic.fields import make_generic_validator  # type: ignore[attr-defined]
 from pydantic.fields import ModelField, Undefined
-from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
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
@@ -122,31 +125,30 @@
     aiofiles = None  # type: ignore[assignment]
     AIOFILES_AVAILABLE = False
 
 __all__ = (
     "ConfigAgent",
     "ConfigModel",
     "ConfigMeta",
-    "save",
-    "save_async",
-    "reload",
-    "reload_async",
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
@@ -167,26 +169,18 @@
             if isinstance(default, pydantic.BaseModel):
                 default = default.dict()
             defaults[field.alias] = default
     return defaults
 
 
 def _get_object_state(obj: Any) -> dict[str, Any]:
-    obj_dict = obj
+    state = obj
     if not isinstance(obj, dict):
-        obj_dict = obj.__dict__
-    return cast(dict[str, Any], obj_dict)
-
-
-def _is_namedtuple(
-    obj: Any,
-) -> bool:
-    return (
-        isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
-    )
+        state = obj.__dict__  # avoidance of vars() is intended
+    return cast(dict[str, Any], state)
 
 
 @functools.singledispatch
 def export_hook(obj: Any) -> Any:
     """
     Convert a value to a format that can be safely serialized.
 
@@ -202,21 +196,25 @@
 
     Returns
     -------
     Any
     """
     if dataclasses.is_dataclass(obj):
         return export_hook(dataclasses.asdict(obj))
-    if _is_namedtuple(obj):
+    if isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields"):
         return _export_namedtuple(obj)
     return obj
 
 
-for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
-    export_hook.register(obj_type, obj_encoder)
+@functools.singledispatch
+def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
+    # Initially I wanted it to be export_hook(obj._asdict()), but
+    # pydantic doesn't seem to be friends with custom NamedTuple-s.
+    return export_hook(list(obj))
+
 
 field_hook_registrars: Any = functools.singledispatch(lambda _cls, value: value)
 
 if TYPE_CHECKING:
 
     class _FieldHookType:
         def __call__(self, cls: type[T], value: Any) -> Any:
@@ -307,114 +305,14 @@
     obj
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return await obj.export_async(**kwargs)
     return cast(dict[str, Any], await obj.dict_async(**kwargs))
 
 
-@export_hook.register(pathlib.PureWindowsPath)
-def _export_windows_path(obj: pathlib.PureWindowsPath) -> str:
-    """
-    Convert a Windows path to a string.
-
-    Parameters
-    ----------
-    obj
-        The path to convert.
-
-    Returns
-    -------
-    The converted path.
-    """
-    return obj.as_posix()
-
-
-@export_hook.register(list)
-def _export_list(obj: list[Any]) -> list[Any]:
-    """
-    Convert a list to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The list to convert.
-
-    Returns
-    -------
-    The converted list.
-    """
-    return [export_hook(item) for item in obj]
-
-
-@export_hook.register(collections.abc.Mapping)
-def _export_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
-    """
-    Convert a mapping to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The mapping to convert.
-
-    Returns
-    -------
-    The converted mapping.
-    """
-    return {k: export_hook(v) for k, v in obj.items()}
-
-
-@functools.singledispatch
-def _export_namedtuple(obj: tuple[Any, ...]) -> Any:
-    """
-    Convert a namedtuple to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The namedtuple to convert.
-
-    Returns
-    -------
-    The converted namedtuple (likely a list).
-    """
-    # Initially I wanted it to be export(obj._asdict()), but
-    # pydantic doesn't seem to be friends with custom NamedTuple-s.
-    return export_hook(list(obj))
-
-
-@field_hook.register(dict)
-@field_hook.register(list)
-def _eval_literals(cls: type[Any], value: Any) -> Any:
-    """
-    Load a dict/list using literal evaluation.
-    Solves nested dictionaries problem in INI files.
-
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
-
-    value
-        The value to load.
-
-    Returns
-    -------
-    The loaded value.
-    """
-    if isinstance(value, str):
-        try:
-            data = ast.literal_eval(value)
-        except (SyntaxError, ValueError):
-            # There might be some following validator, let it be like that
-            return value
-        else:
-            return cls(data)
-    return value
-
-
 def _delegate_ac_options(
     load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
 ) -> None:
     for key, value in options.items():
         if key.startswith("dump_"):
             actual_key = key.removeprefix("dump_")
             targets = [dump_options]
@@ -446,15 +344,15 @@
     Parameters
     ----------
     resource
         The resource to load the configuration from.
     processor
         The resource processor to use. If not specified, the processor used will
         be :class:`DefaultProcessor`.
-    ac_parser
+    parser_name
         The name of the engines to use for loading and saving the
         configuration. If not specified, the processor will be guessed
         from the file extension.
     create_if_missing
         Whether to create the file if it doesn't exist.
     use_pydantic_json
         Whether to use pydantic's JSON serialization for saving the
@@ -463,27 +361,26 @@
     kwargs
         Additional options to pass to `anyconfig` API functions.
 
     Attributes
     ----------
     create_if_missing
         Whether to create the file if it doesn't exist.
-    ac_parser
+    parser_name
         The name of the engines to use for loading and saving the
         configuration. If not specified, the processor will be guessed
         from the file extension.
     allowed_url_schemes
         The URL schemes that are allowed to be used.
 
     Raises
     ------
     ValueError
     """
 
-    _resource: NormalizedResourceT
     processor_class: type[Processor[ConfigModelT]]
     create_if_missing: bool
     is_relative: bool = False
     allowed_url_schemes: set[str]
     use_pydantic_json: bool = True
     default_load_options: dict[str, Any] = {}
     default_dump_options: dict[str, Any] = {
@@ -491,14 +388,15 @@
         # If you want to change them, you can do so by monkey-patching
         # these variables. You can also change `load_options` and
         # `dump_options` instance attributes to make a local change.
         "allow_unicode": True,
         "ensure_ascii": False,
         "indent": 2,
     }
+    _resource: NormalizedResourceT
 
     predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
     default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
 
     OPEN_KWARGS: ClassVar[set[str]] = {
         "mode",
         "buffering",
@@ -529,75 +427,75 @@
         "by_alias",
         "include",
         "exclude",
         "exclude_unset",
         "exclude_defaults",
         "exclude_none",
     }
-    ALIAS_FILE_EXTENSIONS: ClassVar[dict[str, str]] = {
+    EXTRA_FILE_EXTENSIONS: ClassVar[dict[str, str]] = {
         "yml": "yaml",
         "conf": "ini",
         "cfg": "ini",
         # Note: CBOR (RFC 7049) is deprecated, use CBOR (RFC 8949) instead.
         "cbor": "cbor2",
         # https://github.com/msgpack/msgpack/issues/291#issuecomment-1370526984
         "mpk": "msgpack",
         "pkl": "pickle",
     }
-    BINARY_AC_PARSERS: ClassVar[set[str]] = {
+    BINARY_DATA_PARSERS: ClassVar[set[str]] = {
         "ion",
         "bson",
         "cbor",
         "cbor2",
         "msgpack",
         "pickle",
     }
 
     def __init__(
         self,
         resource: RawResourceT,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         processor_class: type[Processor[ConfigModelT]] | None = None,
         *,
         create_if_missing: bool = False,
         **kwargs: Any,
     ) -> None:
         """Parameters
         ----------
         resource
             The URL to the configuration file, or a file-like object.
-        ac_parser
-            The name of the engines to use for loading and saving the configuration.
-            Defaults to 'yaml'.
+        parser_name
+            The name of the anyconfig parser to use
+            for loading and saving the configuration.
         create_if_missing
             Whether to automatically create missing keys when loading the configuration.
         default_kwargs
             Default keyword arguments to pass while opening the resource.
         use_pydantic_json
             Whether to use Pydantic's JSON encoder/decoder instead of the default
             anyconfig one.
         uses_binary_data
-            Whether to treat the data as binary. Defaults to True for BSON,
-            CBOR, MessagePack and Pickle formats.
+            Whether to treat the data as binary.
+            Defaults to True for formats listed in `ConfigAgent.BINARY_DATA_PARSERS`.
         **kwargs
             Additional keyword arguments to pass to
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
-        self._ac_parser = None
+        self._parser_name = None
         self._uses_binary_data = kwargs.get("uses_binary_data", False)
 
         if processor_class is None:
             processor_class = Processor[ConfigModelT]
 
         self.processor_class = processor_class
-        self.ac_parser = ac_parser
+        self.parser_name = parser_name
 
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
@@ -644,300 +542,302 @@
             from the file extension.
 
         Returns
         -------
         The resource of the configuration.
         """
         self._resource = value
-        if self.ac_parser is None:
-            self.ac_parser = self._guess_ac_parser()
+        if self.parser_name is None:
+            self.parser_name = self._guess_parser_name()
 
     @property
-    def ac_parser(self) -> str | None:
-        return self._ac_parser
+    def parser_name(self) -> str | None:
+        return self._parser_name
 
-    @ac_parser.setter
-    def ac_parser(self, value: str | None) -> None:
+    @parser_name.setter
+    def parser_name(self, value: str | None) -> None:
         if value is not None:
             value = value.casefold()
-        self._ac_parser = value
+        self._parser_name = value
 
-    def _guess_ac_parser(self) -> str | None:
-        ac_parser = None
+    def _guess_parser_name(self) -> str | None:
+        parser_name = None
         if isinstance(self.resource, pathlib.Path):
             suffix = self.resource.suffix[1:].casefold()
             supported_parsers = anyconfig.list_types()
             if not suffix:
                 recognized_file_extensions = supported_parsers + [
-                    alias + "(-> " + actual_parser + ")"
-                    for alias, actual_parser in self.ALIAS_FILE_EXTENSIONS.items()
-                    if actual_parser in supported_parsers
+                    alias + "(-> " + actual_parser_name + ")"
+                    for alias, actual_parser_name in self.EXTRA_FILE_EXTENSIONS.items()
+                    if actual_parser_name in supported_parsers
                 ]
                 msg = (
                     "Could not guess the anyconfig parser to use for "
                     f"{self.resource!r}.\n"
                     f"Recognized file extensions: {recognized_file_extensions}"
                 )
                 raise UnspecifiedParserError(msg)
-            ac_parser = self.ALIAS_FILE_EXTENSIONS.get(suffix, suffix)
+            parser_name = self.EXTRA_FILE_EXTENSIONS.get(suffix, suffix)
             if (
-                ac_parser == "cbor2"
+                parser_name == "cbor2"
                 and "cbor2" not in supported_parsers
                 and "cbor" in supported_parsers
             ):
-                ac_parser = "cbor"
-        return ac_parser
+                parser_name = "cbor"
+        return parser_name
 
     def load_into(
         self,
         config_class: type[ConfigModelT],
         blob: str | bytes,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration into a `ConfigModel` subclass.
 
         Parameters
         ----------
         config_class
             The `ConfigModel` subclass to load the configuration into.
         blob
             The configuration to load.
-        ac_parser
+        parser_name
             The name of the engines to use for loading the configuration.
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration.
         """
-        dict_config = self.load_dict(blob, ac_parser=ac_parser, **kwargs)
+        dict_config = self.load_dict(blob, parser_name=parser_name, **kwargs)
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     async def async_load_into(
         self,
         config_class: type[ConfigModelT],
         blob: str | bytes,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration into a `ConfigModel` subclass asynchronously.
 
         Parameters
         ----------
         config_class
             The `ConfigModel` subclass to load the configuration into.
         blob
             The configuration to load.
-        ac_parser
+        parser_name
             The name of the engines to use for loading the configuration.
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration.
         """
-        dict_config = await self.load_dict_async(blob, ac_parser=ac_parser, **kwargs)
+        dict_config = await self.load_dict_async(
+            blob, parser_name=parser_name, **kwargs
+        )
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     def _load_dict_impl(
         self,
         blob: str | bytes,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
-        ac_parser = ac_parser or self.ac_parser or self._guess_ac_parser()
-        if ac_parser is None:
-            msg = "Cannot read configuration because `ac_parser` was not specified"
+        parser_name = parser_name or self.parser_name or self._guess_parser_name()
+        if parser_name is None:
+            msg = "Cannot read configuration because `parser_name` was not specified"
             raise UnspecifiedParserError(msg)
         kwargs = self.load_options | kwargs
         try:
             loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
-                blob, ac_parser=ac_parser, **kwargs
+                blob, ac_parser=parser_name, **kwargs
             )
         except anyconfig.UnknownParserTypeError as exc:
             raise UnavailableParserError(str(exc).split()[-1], self) from exc
         if not isinstance(loaded, collections.abc.Mapping):
             msg = (
                 f"Expected a mapping as a result of loading {self.resource}, "
                 f"got {type(loaded).__name__}."
             )
             raise TypeError(msg)
         return dict(loaded)
 
     def load_dict(
         self,
         blob: str | bytes,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         *,
         preprocess: bool = True,
         **kwargs: Any,
     ) -> dict[str, Any]:
         """
         Load the configuration into a dictionary. The dictionary is
         usually used to initialize a `ConfigModel` subclass. If the
         configuration is empty, None might be returned instead of a dictionary.
 
         Parameters
         ----------
         blob
             The configuration to load.
-        ac_parser
+        parser_name
             The name of the anyconfig parser to use for loading the configuration.
         preprocess
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        loaded = self._load_dict_impl(blob, ac_parser=ac_parser, **kwargs)
+        loaded = self._load_dict_impl(blob, parser_name=parser_name, **kwargs)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
         return loaded
 
     async def load_dict_async(
         self,
         blob: str | bytes,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         *,
         preprocess: bool = True,
         **kwargs: Any,
     ) -> dict[str, Any]:
         """
         Load the configuration into a dictionary asynchronously.
 
         Parameters
         ----------
         blob
             The configuration to load.
-        ac_parser
+        parser_name
             The name of the anyconfig parser to use for loading the configuration.
         preprocess
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        loaded = self._load_dict_impl(blob, ac_parser, **kwargs)
+        loaded = self._load_dict_impl(blob, parser_name, **kwargs)
         if preprocess:
             loaded = await self.processor_class(self, loaded).preprocess_async()
         return loaded
 
     def dump_config(
         self,
         config: ConfigModelT,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> str:
         """
         Dump the configuration to a string.
 
         Parameters
         ----------
         config
             The configuration to dump.
-        ac_parser
+        parser_name
             The name of the anyconfig parser to use for saving the configuration.
         **kwargs
             Additional keyword arguments to pass to `anyconfig.dumps()`.
 
         Returns
         -------
         The dumped configuration.
         """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
+        if parser_name is None:
+            parser_name = self.parser_name
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if ac_parser == "json" and self.use_pydantic_json:
+        if parser_name == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
             _exporting.set(True)  # noqa: FBT003
             return isolate(config.json, **export_kwargs)
         data = export_model(config, **export_kwargs)
-        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
+        return self.dump_data(data, parser_name=parser_name, **kwargs)
 
     async def dump_config_async(
         self,
         config: ConfigModelT,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> str:
         """
         Dump the configuration to a string.
 
         Parameters
         ----------
         config
             The configuration to dump.
-        ac_parser
+        parser_name
             The name of the anyconfig parser to use for saving the configuration.
         **kwargs
             Additional keyword arguments to pass to `anyconfig.dumps()`.
 
         Returns
         -------
         The dumped configuration.
         """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
+        if parser_name is None:
+            parser_name = self.parser_name
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if ac_parser == "json" and self.use_pydantic_json:
+        if parser_name == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
             )
             _exporting.set(True)  # noqa: FBT003
             return await isolate_async(config.json_async, **export_kwargs)
         data = await export_model_async(config, **export_kwargs)
-        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
+        return self.dump_data(data, parser_name=parser_name, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> str:
         """
         Dump data to a string.
 
         Parameters
         ----------
         data
             The data to dump.
-        ac_parser
+        parser_name
             The name of the anyconfig parser to use for saving the configuration.
         kwargs
             Additional keyword arguments to pass to `anyconfig.dumps()`.
 
         Returns
         -------
         The dumped configuration.
         """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
-        if ac_parser is None:
+        if parser_name is None:
+            parser_name = self.parser_name
+        if parser_name is None:
             msg = (
-                "Cannot write configuration because `ac_parser` was not specified"
+                "Cannot write configuration because `parser_name` was not specified"
                 f"for agent {self}"
             )
             raise UnspecifiedParserError(msg)
         kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(export_hook(data), ac_parser=ac_parser, **kwargs)
+        return anyconfig.dumps(export_hook(data), ac_parser=parser_name, **kwargs)
 
     @property
     def is_url(self) -> bool:
         """
         Whether the resource is a URL.
 
         This simply checks if the resource object is a string, since local paths
@@ -946,15 +846,15 @@
         return isinstance(self.resource, str)
 
     @property
     def uses_binary_data(self) -> bool:
         """
         Whether the resource uses bytes for storing data, not str.
         """
-        return self._uses_binary_data or self.ac_parser in self.BINARY_AC_PARSERS
+        return self._uses_binary_data or self.parser_name in self.BINARY_DATA_PARSERS
 
     def open_resource(self, **kwds: Any) -> ConfigIO:
         """
         Open the configuration file.
 
         Parameters
         ----------
@@ -1190,15 +1090,15 @@
         Returns
         -------
         The number of bytes written.
         """
         kwargs = self._get_default_kwargs("write", kwargs=kwargs)
         async with self.open_resource_async(**kwargs) as fp:
             # Technically those might be also bytes,
-            # todo(bswck): type it properly
+            # todo(bswck): type hint it properly...
             return await fp.write(cast(str, blob))
 
     @classmethod
     def from_directive_context(
         cls,
         ctx: DirectiveContext,
         /,
@@ -1244,28 +1144,28 @@
         return cls(*args, **kwargs), str(route)
 
     @classmethod
     def register_file_extension(
         cls,
         file_extension: str,
         *,
-        ac_parser: str,
+        parser_name: str,
     ) -> None:
         """
         Register a file extension with the proper anyconfig parser to use.
 
         Parameters
         ----------
         file_extension
-        ac_parser
+        parser_name
 
         Returns
         -------
         """
-        cls.ALIAS_FILE_EXTENSIONS[file_extension] = ac_parser
+        cls.EXTRA_FILE_EXTENSIONS[file_extension] = parser_name
 
     def __repr__(self) -> str:
         resource = self.resource
         return f"{type(self).__name__}({resource=!r})"
 
 
 def at(
@@ -1389,83 +1289,67 @@
         **kwargs
             Keyword arguments to pass to the saving function.
 
         Returns
         -------
         The number of bytes written.
         """
-        return await save_async(self, **kwargs)
+        return await _save_async(self, **kwargs)
 
     def save(self, **kwargs: Any) -> int:
         """
         Save the configuration.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the saving function.
 
         Returns
         -------
         The number of bytes written.
         """
-        return save(self, **kwargs)
+        return _save(self, **kwargs)
 
     async def reload_async(self, **kwargs: Any) -> Any:
         """
         Reload the configuration asynchronously.
 
         Parameters
         ----------
         kwargs
             Keyword arguments to pass to the reloading function.
 
         Returns
         -------
         The reloaded configuration or its belonging item.
         """
-        return await reload_async(self, **kwargs)
+        return await _reload_async(self, **kwargs)
 
     def reload(self, **kwargs: Any) -> Any:
         """
         Reload the configuration.
 
         Parameters
         ----------
         kwargs
             Keyword arguments to pass to the reloading function.
 
         Returns
         -------
         The reloaded configuration or its belonging item.
         """
-        return reload(self, **kwargs)
+        return _reload(self, **kwargs)
 
 
-def save(
+def _save(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
     **kwargs: Any,
 ) -> int:
-    """
-    Save the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return config.save(write_kwargs=write_kwargs, **kwargs)
 
     if write_kwargs is None:
         write_kwargs = {}
 
@@ -1476,35 +1360,19 @@
     context = get_context(config)
     blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = config.write(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
-async def save_async(
+async def _save_async(
     section: ConfigModelT | ConfigAt[ConfigModelT],
     write_kwargs: dict[str, Any] | None = None,
     **kwargs: Any,
 ) -> int:
-    """
-    Save the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return await config.save_async(write_kwargs=write_kwargs, **kwargs)
 
     if write_kwargs is None:
         write_kwargs = {}
 
@@ -1515,59 +1383,31 @@
     context = get_context(config)
     blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = await config.write_async(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
-def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
-    """
-    Reload the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    **kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
+def _reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
     if isinstance(section, ConfigModel):
         config = section
         return config.reload()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
     newest = context.agent.read(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     ConfigAt(config, state, section.route).update(section_data)
     return section_data
 
 
-async def reload_async(
+async def _reload_async(
     section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
 ) -> Any:
-    """
-    Reload the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
     if isinstance(section, ConfigModel):
         config = section
         return await config.reload_async()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
@@ -1590,14 +1430,15 @@
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
@@ -1625,23 +1466,28 @@
 
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
@@ -1669,28 +1515,32 @@
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
 
@@ -1725,22 +1575,34 @@
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
@@ -1834,16 +1696,17 @@
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
 
 
@@ -1863,16 +1726,18 @@
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
@@ -1888,73 +1753,41 @@
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
-# Interpolation for mutable types is a non-trivial task.
-
-# @interpolate.register(dict)
-# def _interpolate_dict(value: dict[Any, Any], ctx: dict[str, Any]) -> dict[Any, Any]:
-#     return {
-#         interpolate(k, ctx): interpolate(v, ctx) for k, v in value.items()
-#     }
-#
-#
-# @interpolate.register(list)
-# def _interpolate_lst(value: list, ctx: dict[str, Any]) -> list[Any]:
-#     return {
-#         interpolate(k, ctx): interpolate(v, ctx) for k, v in value.items()
-#     }
-
-
 class ConfigMeta(pydantic.BaseSettings.Config):
     """
     Meta-configuration for configuration models.
 
     See https://docs.pydantic.dev/latest/usage/model_config/ for more information
     on model configurations.
 
     Attributes
     ----------
     resource
         The configuration resource to read from/write to.
 
         If a string, it will be interpreted as a path to a file.
 
-    ac_parser
+    parser_name
         The anyconfig parser to use.
 
     autoupdate_forward_refs
         Whether to automatically update forward references
         when `ConfigModel.load()` or `ConfigModel.load_async()`
         methods are called. For convenience, defaults to `True`.
 
     And all other attributes from `pydantic.BaseSettings.Config`.
     """
 
     resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
-    ac_parser: str | None = None
+    parser_name: str | None = None
     validate_assignment: bool = True
     autoupdate_forward_refs: bool = True
 
     Extra = pydantic.Extra
 
 
 class ConfigModel(
@@ -1999,29 +1832,30 @@
 
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
@@ -2137,34 +1971,34 @@
 
     @classmethod
     def _resolve_agent(
         cls,
         resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
     ) -> ConfigAgent[ConfigModelT]:
         if resource is None:
             resource = getattr(cls.__config__, "resource", None)
         if resource is None:
             raise ValueError("No resource specified")
-        if ac_parser is None:
-            ac_parser = getattr(cls.__config__, "ac_parser", None)
+        if parser_name is None:
+            parser_name = getattr(cls.__config__, "parser_name", None)
         agent: ConfigAgent[ConfigModelT]
         if isinstance(resource, ConfigAgent):
             agent = resource
         else:
             agent = ConfigAgent(
                 resource,
-                ac_parser=ac_parser,
+                parser_name=parser_name,
             )
         if create_if_missing is not None:
             agent.create_if_missing = create_if_missing
-        if ac_parser is not None:
-            agent.ac_parser = cast(str, ac_parser)
+        if parser_name is not None:
+            agent.parser_name = cast(str, parser_name)
         return agent
 
     @property
     def initial_state(self) -> dict[str, Any]:
         """
         The initial configuration state.
 
@@ -2253,45 +2087,44 @@
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
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file.
         To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
         resource
             The configuration resource to read from/write to.
-        ac_parser
+        parser_name
             The anyconfig parser to use.
         create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         agent = cls._resolve_agent(
             resource,
-            ac_parser=ac_parser,
+            parser_name=parser_name,
             create_if_missing=create_if_missing,
         )
         current_context.set(Context(agent))
         local = contextvars.copy_context()
         if getattr(
             cls.__config__,
             "autoupdate_forward_refs",
@@ -2301,15 +2134,14 @@
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
@@ -2320,21 +2152,20 @@
         self
         """
         context = get_context(self)
         current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = context.agent.read(config_class=type(self), **kwargs)
         else:
-            changed = reload(cast(ConfigModelT, context.at), **kwargs)
+            changed = _reload(cast(ConfigModelT, context.at), **kwargs)
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
@@ -2352,15 +2183,15 @@
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
             blob = context.agent.dump_config(self, **kwargs)
             result = self.write(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return save(
+        return _save(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
     def write(self, blob: str | bytes, **kwargs: Any) -> int:
         """
@@ -2380,44 +2211,43 @@
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
-        ac_parser: str | None = None,
+        parser_name: str | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file asynchronously.
         To reload the configuration, use the `reload_async()` method.
 
         Parameters
         ----------
         resource
             The configuration resource.
-        ac_parser
+        parser_name
             The anyconfig parser to use.
         create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         agent = cls._resolve_agent(
-            resource, create_if_missing=create_if_missing, ac_parser=ac_parser
+            resource, create_if_missing=create_if_missing, parser_name=parser_name
         )
         current_context.set(Context(agent))
         local = contextvars.copy_context()
         if getattr(
             cls.__config__,
             "autoupdate_forward_refs",
             ConfigMeta.autoupdate_forward_refs,
@@ -2428,15 +2258,14 @@
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
@@ -2447,23 +2276,22 @@
         self
         """
         context = get_context(self)
         current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = await context.agent.read_async(config_class=type(self), **kwargs)
         else:
-            changed = await reload_async(
+            changed = await _reload_async(
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
@@ -2482,15 +2310,15 @@
             if write_kwargs is None:
                 write_kwargs = {}
             _exporting.set(True)  # noqa: FBT003
             blob = await context.agent.dump_config_async(self, **kwargs)
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
-        return await save_async(
+        return await _save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
         )
 
     async def write_async(self, blob: str | bytes, **kwargs: Any) -> int:
         """
@@ -2509,21 +2337,64 @@
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
@@ -2533,38 +2404,23 @@
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
 
-@field_hook.register(ConfigModel)
-def _eval_model(cls: type[ConfigModelT], value: Any) -> ConfigModelT | Any:
-    """
-    Load a model using dict literal evaluation.
-    Solves nested dictionaries problem in INI files.
 
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
+setattr(ConfigModel, INTERPOLATION_INCLUSIONS, None)
+include.register(ConfigModel, include_const)
 
-    value
-        The value to load.
-
-    Returns
-    -------
-    The loaded value.
-    """
-    data = value
-    if isinstance(value, str):
-        try:
-            data = ast.literal_eval(value)
-        except (SyntaxError, ValueError):
-            # Note: Strings resembling models is probably not intended
-            # to be used with automatic pickle/JSON parsing.
-            # return cls.parse_raw(value)
-            return data
-        else:
-            return cls.parse_obj(data)
-    return data
+if os.getenv("CONFIGZEN_SETUP") != "0":
+    importlib.import_module("._setup", package=__package__)
```

### Comparing `configzen-0.4.2/configzen/decorators.py` & `configzen-0.5.1/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/errors.py` & `configzen-0.5.1/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/field.py` & `configzen-0.5.1/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/processor.py` & `configzen-0.5.1/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/route.py` & `configzen-0.5.1/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/configzen/typedefs.py` & `configzen-0.5.1/configzen/typedefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import contextlib
 import os
 import pathlib
 import sys
 from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
 
 if sys.version_info >= (3, 10):
-    from typing import TypeAlias
+    from typing import ParamSpec, TypeAlias
 else:
-    from typing_extensions import TypeAlias
+    from typing_extensions import ParamSpec, TypeAlias
 
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

### Comparing `configzen-0.4.2/LICENSE` & `configzen-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.2/pyproject.toml` & `configzen-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.2"
+version = "0.5.1"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.2/README.md` & `configzen-0.5.1/README.md`

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
@@ -41,15 +40,15 @@
 | properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
 | shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
 
 [//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
 [//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
 [//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
 
-If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, ac_parser)`.
+If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
 
 If your favorite backend library is not supported, please let me know by reporting it as an issue.
 Using custom backends is to be supported in the future.
 
 [^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
 The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
 
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
@@ -225,14 +224,87 @@
 
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
+AppConfig(cpu=CPUConfig(cores=4), num_workers=4)
+```
+
+
+#### Reusable configuration with namespaces
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
+>>> from ipaddress import IPv4Address
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
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=8000)
+>>> db_config.dict()
+{'host': IPv4Address('127.0.0.1'), 'port': 8000}
+>>> db_config.export()  # used when saving
+{'host': '${app_config::db_host}', 'port': '${app_config::expose}'}
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

### Comparing `configzen-0.4.2/PKG-INFO` & `configzen-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.2
+Version: 0.5.1
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
@@ -63,15 +62,15 @@
 | properties                                                                          | -                             | `properties`                 | (native)                                                                                                |
 | shellvars                                                                           | -                             | `shellvars`                  | (native)                                                                                                |
 
 [//]: # (| [ConfigObj]&#40;https://configobj.readthedocs.io/en/latest/configobj.html#introduction&#41; | `anyconfig-configobj-backend` | `configobj`                  | [configobj]&#40;https://pypi.org/project/configobj/&#41;                                                        |)
 [//]: # (| [Amazon Ion]&#40;https://en.wikipedia.org/wiki/Ion_&#40;serialization_format&#41;&#41;              | `anyconfig-ion-backend`       | `ion`                        | [ion]&#40;https://pypi.org/project/amazon.ion/&#41;                                                             |)
 [//]: # (| [MessagePack]&#40;https://en.wikipedia.org/wiki/MessagePack&#41;                            | `anyconfig-msgpack-backend`   | `msgpack`, `mpk`             | [msgpack]&#40;https://pypi.org/project/msgpack/&#41;                                                            |)
 
-If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, ac_parser)`.
+If your file extension is not recognized, you can register your own file extension by calling `ConfigAgent.register_file_extension(file_extension, parser_name)`.
 
 If your favorite backend library is not supported, please let me know by reporting it as an issue.
 Using custom backends is to be supported in the future.
 
 [^1]: A suggested alternative for comments is to use the `description` parameter in your configuration models' fields: `ConfigField(description=...)`.
 The provided field descriptions are included in JSON schemas generated by the default implementation of the `ConfigModel.schema()` method.
 
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
@@ -247,14 +246,87 @@
 
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
+AppConfig(cpu=CPUConfig(cores=4), num_workers=4)
+```
+
+
+#### Reusable configuration with namespaces
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
+>>> from ipaddress import IPv4Address
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
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=8000)
+>>> db_config.dict()
+{'host': IPv4Address('127.0.0.1'), 'port': 8000}
+>>> db_config.export()  # used when saving
+{'host': '${app_config::db_host}', 'port': '${app_config::expose}'}
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

