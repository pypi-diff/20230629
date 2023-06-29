# Comparing `tmp/sob-1.8.0.tar.gz` & `tmp/sob-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sob-1.8.0.tar", last modified: Thu Apr  1 23:06:25 2021, max compression
+gzip compressed data, was "sob-1.9.0.tar", last modified: Fri Apr  2 05:54:16 2021, max compression
```

## Comparing `sob-1.8.0.tar` & `sob-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 23:06:25.408782 sob-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-01 23:06:25.408782 sob-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-04-01 23:06:05.000000 sob-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-04-01 23:06:05.000000 sob-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 23:06:25.408782 sob-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-04-01 23:06:05.000000 sob-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 23:06:25.408782 sob-1.8.0/sob/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-04-01 23:06:05.000000 sob-1.8.0/sob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27142 2021-04-01 23:06:05.000000 sob-1.8.0/sob/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8294 2021-04-01 23:06:05.000000 sob-1.8.0/sob/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    11920 2021-04-01 23:06:05.000000 sob-1.8.0/sob/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    34500 2021-04-01 23:06:05.000000 sob-1.8.0/sob/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)   101187 2021-04-01 23:06:05.000000 sob-1.8.0/sob/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    19688 2021-04-01 23:06:05.000000 sob-1.8.0/sob/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    14447 2021-04-01 23:06:05.000000 sob-1.8.0/sob/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    10102 2021-04-01 23:06:05.000000 sob-1.8.0/sob/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    38455 2021-04-01 23:06:05.000000 sob-1.8.0/sob/thesaurus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2021-04-01 23:06:05.000000 sob-1.8.0/sob/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 23:06:25.408782 sob-1.8.0/sob/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)    10642 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/inspect.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    14459 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/string.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-04-01 23:06:05.000000 sob-1.8.0/sob/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-04-01 23:06:05.000000 sob-1.8.0/sob/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 23:06:25.408782 sob-1.8.0/sob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-01 23:06:25.000000 sob-1.8.0/sob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-04-01 23:06:25.000000 sob-1.8.0/sob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 23:06:25.000000 sob-1.8.0/sob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 23:06:22.000000 sob-1.8.0/sob.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-04-01 23:06:25.000000 sob-1.8.0/sob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-01 23:06:25.000000 sob-1.8.0/sob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-02 05:54:16.556712 sob-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-02 05:54:16.556712 sob-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-04-02 05:53:49.000000 sob-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-04-02 05:53:49.000000 sob-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-02 05:54:16.560712 sob-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2863 2021-04-02 05:53:49.000000 sob-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-02 05:54:16.556712 sob-1.9.0/sob/
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-04-02 05:53:49.000000 sob-1.9.0/sob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27216 2021-04-02 05:53:49.000000 sob-1.9.0/sob/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8366 2021-04-02 05:53:49.000000 sob-1.9.0/sob/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11936 2021-04-02 05:53:49.000000 sob-1.9.0/sob/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34978 2021-04-02 05:53:49.000000 sob-1.9.0/sob/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)   101712 2021-04-02 05:53:49.000000 sob-1.9.0/sob/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19824 2021-04-02 05:53:49.000000 sob-1.9.0/sob/properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14447 2021-04-02 05:53:49.000000 sob-1.9.0/sob/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10108 2021-04-02 05:53:49.000000 sob-1.9.0/sob/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38103 2021-04-02 05:53:49.000000 sob-1.9.0/sob/thesaurus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4906 2021-04-02 05:53:49.000000 sob-1.9.0/sob/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-02 05:54:16.556712 sob-1.9.0/sob/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10642 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15802 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-04-02 05:53:49.000000 sob-1.9.0/sob/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-04-02 05:53:49.000000 sob-1.9.0/sob/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-02 05:54:16.556712 sob-1.9.0/sob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-04-02 05:54:16.000000 sob-1.9.0/sob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-04-02 05:54:16.000000 sob-1.9.0/sob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-02 05:54:16.000000 sob-1.9.0/sob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-02 05:54:13.000000 sob-1.9.0/sob.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-04-02 05:54:16.000000 sob-1.9.0/sob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-04-02 05:54:16.000000 sob-1.9.0/sob.egg-info/top_level.txt
```

### Comparing `sob-1.8.0/PKG-INFO` & `sob-1.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sob
-Version: 1.8.0
+Version: 1.9.0
 Summary: A framework for serializing/deserializing JSON/YAML into python class instances and vice versa
 Home-page: https://github.com/davebelais/sob
 Author: David Belais
 Author-email: david@belais.me
 License: MIT
 Description: UNKNOWN
 Keywords: rest api serialization serialize
```

### Comparing `sob-1.8.0/setup.py` & `sob-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                         kwargs["extras_require"]["all"].append(requirement)
     # Pass the modified keyword arguments to `setuptools.setup`
     setuptools.setup(**kwargs)
 
 
 setup(
     name="sob",
-    version="1.8.0",
+    version="1.9.0",
     description=(
         "A framework for serializing/deserializing JSON/YAML into python "
         "class instances and vice versa"
     ),
     url="https://github.com/davebelais/sob",
     author="David Belais",
     author_email="david@belais.me",
@@ -53,27 +53,28 @@
     install_requires=["pyyaml>=3.10", "iso8601~=0.1", "more-itertools~=8.6"],
     setup_requires=["setuptools"],
     extras_require={
         "test": [
             "mypy~=0.812",
             "tox~=3.20",
             "pytest~=5.4",
-            "flake8~=3.8",
+            "flake8~=3.9",
             "setuptools-setup-versions>=1.8.0,<2",
             "readme-md-docstrings>=0.1.0,<1",
         ],
         "dev": [
             "mypy~=0.812",
             "wheel~=0.35.1",
             "tox~=3.20",
             "pytest~=5.4",
-            "flake8~=3.8",
+            "flake8~=3.9",
             "setuptools-setup-versions>=1.8.0,<2",
             "readme-md-docstrings~=0.1.0,<2",
             "twine~=3.2",
+            "black~=20.8b1",
             "daves-dev-tools~=0.1",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `sob-1.8.0/sob/__init__.py` & `sob-1.9.0/sob/__init__.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/abc.py` & `sob-1.9.0/sob/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,17 +144,15 @@
         pass
 
     @abstractmethod
     def extend(self, values: Iterable[Union[type, "Property"]]) -> None:
         pass
 
     @abstractmethod
-    def __delitem__(  # type: ignore
-        self, index: int
-    ) -> None:
+    def __delitem__(self, index: int) -> None:  # type: ignore
         pass
 
     @abstractmethod
     def pop(self, index: int = -1) -> Union[type, "Property"]:
         pass
 
 
@@ -338,15 +336,16 @@
         ] = None,
         before_serialize: Optional[Callable[["JSONTypes"], Any]] = None,
         after_serialize: Optional[Callable[[str], str]] = None,
         before_validate: Optional[Callable[["Model"], "Model"]] = None,
         after_validate: Optional[Callable[["Model"], None]] = None,
         before_setitem: Optional[
             Callable[
-                ["Dictionary", str, "MarshallableTypes"], Tuple[str, Any],
+                ["Dictionary", str, "MarshallableTypes"],
+                Tuple[str, Any],
             ]
         ] = None,
         after_setitem: Optional[
             Callable[["Dictionary", str, "MarshallableTypes"], None]
         ] = None,
     ) -> None:
         pass
@@ -850,15 +849,19 @@
     @abstractmethod
     def __init__(
         self,
         items: Union[
             "Array", Iterable["MarshallableTypes"], str, bytes, Readable
         ] = None,
         item_types: Union[
-            Iterable[Union[type, "Property"]], type, "Property", Types, None,
+            Iterable[Union[type, "Property"]],
+            type,
+            "Property",
+            Types,
+            None,
         ] = None,
     ) -> None:
         pass
 
     @abstractmethod
     def _marshal(self) -> Sequence["JSONTypes"]:
         pass
@@ -1164,15 +1167,21 @@
     float,
     bool,
     Mapping,
     Sequence,
     NoneType,
 )
 JSONTypes = Union[
-    str, int, float, bool, Mapping[str, Any], Sequence, None,
+    str,
+    int,
+    float,
+    bool,
+    Mapping[str, Any],
+    Sequence,
+    None,
 ]
 MarshallableTypes = Union[
     bool,
     str,
     bytes,
     Model,
     Mapping[str, Any],
```

### Comparing `sob-1.8.0/sob/errors.py` & `sob-1.9.0/sob/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,27 @@
     """
 
     def __init__(
         self,
         message: Optional[str] = None,
         data: Optional[abc.MarshallableTypes] = None,
         types: Union[
-            Iterable[Union[abc.Property, type]], abc.Types, None,
+            Iterable[Union[abc.Property, type]],
+            abc.Types,
+            None,
         ] = None,
         item_types: Union[
-            Iterable[Union[abc.Property, type]], abc.Types, None,
+            Iterable[Union[abc.Property, type]],
+            abc.Types,
+            None,
         ] = None,
         value_types: Union[
-            Iterable[Union[abc.Property, type]], abc.Types, None,
+            Iterable[Union[abc.Property, type]],
+            abc.Types,
+            None,
         ] = None,
     ) -> None:
         self._message: Optional[str] = None
         self._parameter: Optional[str] = None
         self._index: Union[str, int, None] = None
         self._key: Optional[str] = None
         error_message_lines: List[str] = []
```

### Comparing `sob-1.8.0/sob/hooks.py` & `sob-1.9.0/sob/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,17 @@
 
 def type_(model: Union[type, abc.Model]) -> type:
     """
     Get the type of metadata required for an object
     """
     hooks_type: type
     assert_is_instance(
-        "model", model, (type, abc.Object, abc.Dictionary, abc.Array),
+        "model",
+        model,
+        (type, abc.Object, abc.Dictionary, abc.Array),
     )
     if isinstance(model, type):
         hooks_type = (
             Object
             if issubclass(model, abc.Object)
             else Array
             if issubclass(model, abc.Array)
```

### Comparing `sob-1.8.0/sob/meta.py` & `sob-1.9.0/sob/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -603,15 +603,18 @@
 def set_pointer(model: abc.Model, pointer_: str) -> None:
     key: str
     value: Any
     assert_is_instance("pointer_", pointer_, str)
     model._pointer = pointer_
     if isinstance(model, abc.Dictionary):
         for key, value in model.items():
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 pointer(
                     value,
                     "{}/{}".format(
                         pointer_,
                         (
                             escape_reference_token(key)
                             if isinstance(key, str)
@@ -621,15 +624,18 @@
                 )
     elif isinstance(model, abc.Object):
         property_name: str
         property_: abc.Property
         for property_name, property_ in _read_object_properties(model):
             key = property_.name or property_name
             value = getattr(model, property_name)
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 pointer(
                     value,
                     "{}/{}".format(
                         pointer_,
                         (
                             escape_reference_token(key)
                             if isinstance(key, str)
@@ -637,54 +643,72 @@
                         ),
                     ),
                 )
     elif isinstance(model, abc.Array):
         index: int
         for index in range(len(model)):
             value = model[index]
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 pointer(value, "%s/%s" % (pointer_, str(index)))
 
 
 def pointer(model: abc.Model, pointer_: Optional[str] = None) -> Optional[str]:
     """
     Get or set a model's pointer
     """
     assert_is_instance(
-        "model", model, (abc.Object, abc.Dictionary, abc.Array),
+        "model",
+        model,
+        (abc.Object, abc.Dictionary, abc.Array),
     )
     if pointer_ is not None:
         set_pointer(model, pointer_)
     return get_pointer(model)
 
 
-def _traverse_models(model_instance: abc.Model,) -> Iterable[abc.Model]:
+def _traverse_models(
+    model_instance: abc.Model,
+) -> Iterable[abc.Model]:
     """
     Iterate over all child model instances
     """
     if isinstance(model_instance, abc.Dictionary):
         for value in model_instance.values():
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 yield value
     elif isinstance(model_instance, abc.Object):
         property_name: str
         for property_name in _read_object_property_names(model_instance):
             value = getattr(model_instance, property_name)
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 yield value
     elif isinstance(model_instance, abc.Array):
         for value in model_instance:
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 yield value
 
 
 # noinspection PyShadowingNames
 def set_url(model_instance: abc.Model, source_url: Optional[str]) -> None:
     assert_is_instance(
-        "model", model_instance, (abc.Object, abc.Dictionary, abc.Array),
+        "model",
+        model_instance,
+        (abc.Object, abc.Dictionary, abc.Array),
     )
     if source_url is not None:
         assert_is_instance("url_", source_url, str)
     model_instance._url = source_url
     child_model: abc.Model
     for child_model in _traverse_models(model_instance):
         set_url(child_model, source_url)
@@ -700,30 +724,41 @@
     return get_url(model)
 
 
 def set_format(
     model: abc.Model, serialization_format: Optional[str] = None
 ) -> None:
     assert_is_instance(
-        "model", model, (abc.Object, abc.Dictionary, abc.Array),
+        "model",
+        model,
+        (abc.Object, abc.Dictionary, abc.Array),
     )
     assert_is_instance("serialization_format", serialization_format, str)
     model._format = serialization_format
     if isinstance(model, abc.Dictionary):
         for value in model.values():
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 set_format(value, serialization_format)
     elif isinstance(model, abc.Object):
         for property_name in _read_object_property_names(model):
             value = getattr(model, property_name)
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 set_format(value, serialization_format)
     elif isinstance(model, abc.Array):
         for value in model:
-            if isinstance(value, (abc.Object, abc.Dictionary, abc.Array),):
+            if isinstance(
+                value,
+                (abc.Object, abc.Dictionary, abc.Array),
+            ):
                 set_format(value, serialization_format)
 
 
 def get_format(model: abc.Model) -> Optional[str]:
     return getattr(model, "_format")
 
 
@@ -948,15 +983,18 @@
         _version_object(data, specification, version_number)
     elif isinstance(data, abc.Dictionary):
         _version_dictionary(data, specification, version_number)
     elif isinstance(data, abc.Array):
         _version_array(data, specification, version_number)
 
 
-def _copy_object_to(source: abc.Object, target: abc.Object,) -> None:
+def _copy_object_to(
+    source: abc.Object,
+    target: abc.Object,
+) -> None:
     source_meta: Optional[abc.Meta] = read(source)
     assert isinstance(source_meta, (NoneType, abc.ObjectMeta))
     if (source_meta is not None) and (source_meta.properties is not None):
         for property_name in source_meta.properties.keys():
             source_property_value = getattr(source, property_name)
             target_property_value = getattr(target, property_name)
             if target_property_value and isinstance(
```

### Comparing `sob-1.8.0/sob/model.py` & `sob-1.9.0/sob/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     represent,
 )
 from .utilities.io import read
 from .utilities.string import (
     MAX_LINE_LENGTH,
     indent as indent_,
     split_long_docstring_lines,
+    suffix_long_lines,
 )
 from .utilities.types import (
     NULL,
     NoneType,
     Null,
     UNDEFINED,
     Undefined,
@@ -152,15 +153,22 @@
                     "data_read", data_read, (Iterable, Mapping, abc.Model)
                 )
             deserialized_data = data_read
             if format_ is not None:
                 meta.set_format(self, format_)
         else:
             assert_is_instance(
-                "data", data, (Iterable, Mapping, abc.Model, NoneType,)
+                "data",
+                data,
+                (
+                    Iterable,
+                    Mapping,
+                    abc.Model,
+                    NoneType,
+                ),
             )
             deserialized_data = data
         return deserialized_data
 
     def _init_pointer(self) -> None:
         """
         This function sets the root pointer value, and recursively applies
@@ -785,21 +793,21 @@
             data
         )
         # Check to see if value types are defined in the metadata
         value_types: Optional[abc.Types] = (
             instance_meta.value_types if instance_meta else None
         )
         # Recursively convert the data to generic, serializable, data types
-        marshalled_data: abc.OrderedDict[str, abc.JSONTypes] = (
-            collections.OrderedDict(
-                [
-                    (key, marshal(value, types=value_types))
-                    for key, value in data.items()
-                ]
-            )
+        marshalled_data: abc.OrderedDict[
+            str, abc.JSONTypes
+        ] = collections.OrderedDict(
+            [
+                (key, marshal(value, types=value_types))
+                for key, value in data.items()
+            ]
         )
         # Execute after-marshal hooks, if applicable
         if (instance_hooks is not None) and (
             instance_hooks.after_marshal is not None
         ):
             after_marshal_data: abc.JSONTypes = instance_hooks.after_marshal(
                 marshalled_data
@@ -830,17 +838,15 @@
         validation_errors: List[str] = []
         hooks_: Optional[abc.DictionaryHooks] = hooks.dictionary_read(self)
         data: abc.Model = self
         if hooks_ and hooks_.before_validate:
             data = hooks_.before_validate(data)
         assert isinstance(data, (NoneType, abc.Dictionary))
         meta_: Optional[abc.DictionaryMeta] = meta.dictionary_read(data)
-        value_types: Optional[abc.Types] = (
-            meta_.value_types if meta_ else None
-        )
+        value_types: Optional[abc.Types] = meta_.value_types if meta_ else None
         if value_types is not None:
             assert isinstance(data, abc.Dictionary)
             key: str
             value: abc.MarshallableTypes
             for key, value in data.items():
                 value_validation_errors = validate(
                     value, value_types, raise_errors=False
@@ -1271,15 +1277,18 @@
         """
         return getattr(self, self._get_key_property_name(key))
 
     def __copy__(self) -> abc.Object:
         return self.__class__(self)
 
     def _deepcopy_property(
-        self, property_name_: str, other: abc.Object, memo: Optional[dict],
+        self,
+        property_name_: str,
+        other: abc.Object,
+        memo: Optional[dict],
     ) -> None:
         """
         Deep-copy a property from this object to another
         """
         try:
             value = getattr(self, property_name_)
             if isinstance(value, GeneratorType):
@@ -1309,16 +1318,16 @@
                 self._deepcopy_property(property_name_, new_instance, memo)
         return new_instance
 
     def _marshal(self) -> abc.OrderedDict[str, abc.JSONTypes]:
         object_: abc.Object = self
         instance_hooks: Optional[abc.ObjectHooks] = hooks.object_read(self)
         if instance_hooks and instance_hooks.before_marshal:
-            before_marshal_object: abc.Model = (
-                instance_hooks.before_marshal(self)
+            before_marshal_object: abc.Model = instance_hooks.before_marshal(
+                self
             )
             assert isinstance(before_marshal_object, abc.Object)
             object_ = before_marshal_object
         data: abc.OrderedDict[str, abc.JSONTypes] = collections.OrderedDict()
         instance_meta: Optional[abc.ObjectMeta] = meta.object_read(object_)
         if instance_meta and instance_meta.properties is not None:
             property_name_: str
@@ -1326,16 +1335,16 @@
             for property_name_, property_ in instance_meta.properties.items():
                 value: abc.JSONTypes = getattr(object_, property_name_)
                 if value is not None:
                     data[
                         property_.name or property_name_
                     ] = _marshal_property_value(property_, value)
         if instance_hooks and instance_hooks.after_marshal:
-            after_marshal_data: abc.JSONTypes = (
-                instance_hooks.after_marshal(data)
+            after_marshal_data: abc.JSONTypes = instance_hooks.after_marshal(
+                data
             )
             assert isinstance(after_marshal_data, collections.OrderedDict)
             data = after_marshal_data
         return data
 
     def __str__(self) -> str:
         return serialize(self)
@@ -1687,21 +1696,27 @@
                 value_types = (value_types,)
         if item_types is not None:
             if isinstance(item_types, (type, abc.Property)):
                 item_types = (item_types,)
         # Instance Attributes
         self.data: abc.MarshallableTypes = data
         self.types: Union[
-            Iterable[Union[type, abc.Property]], abc.Types, None,
+            Iterable[Union[type, abc.Property]],
+            abc.Types,
+            None,
         ] = types
         self.value_types: Union[
-            Iterable[Union[type, abc.Property]], abc.Types, None,
+            Iterable[Union[type, abc.Property]],
+            abc.Types,
+            None,
         ] = value_types
         self.item_types: Union[
-            Iterable[Union[type, abc.Property]], abc.Types, None,
+            Iterable[Union[type, abc.Property]],
+            abc.Types,
+            None,
         ] = item_types
         self.meta: Optional[abc.Meta] = None
 
     def __call__(self) -> abc.MarshallableTypes:
         """
         Return `self.data` unmarshalled
         """
@@ -1876,15 +1891,16 @@
         if "item_types" in signature(type_).parameters:
             unmarshalled_data = type_(self.data, item_types=self.item_types)
         else:
             unmarshalled_data = type_(self.data)
         return unmarshalled_data
 
     def as_type(
-        self, type_: Union[type, abc.Property],
+        self,
+        type_: Union[type, abc.Property],
     ) -> abc.MarshallableTypes:
         unmarshalled_data: abc.MarshallableTypes = None
         if isinstance(type_, abc.Property):
             unmarshalled_data = _unmarshal_property_value(type_, self.data)
         elif isinstance(type_, type):
             if isinstance(
                 self.data, (dict, collections.OrderedDict, abc.Model)
@@ -2458,15 +2474,16 @@
         if value is NULL:
             setattr(object_instance, property_name_, replacement_value)
         elif isinstance(value, abc.Model):
             replace_nulls(value, replacement_value)
 
 
 def _replace_array_nulls(
-    array_instance: abc.Array, replacement_value: abc.MarshallableTypes = None,
+    array_instance: abc.Array,
+    replacement_value: abc.MarshallableTypes = None,
 ) -> None:
     index: int
     value: abc.MarshallableTypes
     for index, value in enumerate(array_instance):
         if value is NULL:
             array_instance[index] = replacement_value
         elif isinstance(value, abc.Model):
@@ -2483,15 +2500,16 @@
         if value is NULL:
             dictionary_instance[key] = replacement_value
         elif isinstance(value, abc.Model):
             replace_nulls(value, replacement_value)
 
 
 def replace_nulls(
-    model_instance: abc.Model, replacement_value: abc.MarshallableTypes = None,
+    model_instance: abc.Model,
+    replacement_value: abc.MarshallableTypes = None,
 ) -> None:
     """
     This function replaces all instances of `sob.properties.types.NULL`.
 
     Parameters:
 
     - model_instance (sob.model.Model)
@@ -2616,28 +2634,28 @@
     if 9 + len(name) + len(qualified_superclass_name) <= MAX_LINE_LENGTH:
         class_declaration = f"class {name}({qualified_superclass_name}):"
     else:
         # If the first line is still too long for PEP8--add a comment to
         # prevent linters from getting hung up
         noqa: str = "  # noqa" if len(name) + 7 > MAX_LINE_LENGTH else ""
         class_declaration = (
-            f"class {name}({noqa}\n" f"    {qualified_superclass_name}\n" "):"
+            f"class {name}({noqa}\n    {qualified_superclass_name}\n):"
         )
     return class_declaration
 
 
 def _repr_class_docstring(docstring: str = "") -> str:
     """
     Return a representation of a docstring for use in a class constructor.
     """
     repr_docstring: str = ""
     if docstring:
-        repr_docstring = (
-            '    """\n' "%s\n" '    """'
-        ) % split_long_docstring_lines(docstring)
+        repr_docstring = '    """\n{}\n    """'.format(
+            split_long_docstring_lines(docstring)
+        )
     return repr_docstring
 
 
 def _model_class_from_meta(
     metadata: abc.Meta,
 ) -> Type[Union[Array, Dictionary, Object]]:
     return (
@@ -2651,44 +2669,52 @@
 
 _REPR_MARSHALLABLE_TYPING: str = f"{_parent_module_name}.abc.MarshallableTypes"
 
 
 def _repr_class_init_from_meta(metadata: abc.Meta, module: str) -> str:
     out: List[str] = []
     if isinstance(metadata, abc.DictionaryMeta):
-        repr_value_typing: str = indent_(
-            _type_hint_from_property_types(metadata.value_types, module), 20
+        repr_value_typing: str = _type_hint_from_property_types(
+            metadata.value_types, module
+        )
+        mapping_repr_value_typing: str = suffix_long_lines(
+            indent_(repr_value_typing, 16)
+        )
+        iterable_repr_value_typing: str = suffix_long_lines(
+            indent_(repr_value_typing, 20)
         )
         out.append(
             "\n"
             "    def __init__(\n"
             "        self,\n"
             "        items: typing.Union[\n"
             f"            {_parent_module_name}.abc.Dictionary,\n"
             "            typing.Mapping[\n"
             "                str,\n"
-            f"                {repr_value_typing}\n"
+            f"                {mapping_repr_value_typing}\n"
             "            ],\n"
             "            typing.Iterable[\n"
             "                typing.Tuple[\n"
             "                    str,\n"
-            f"                    {repr_value_typing}\n"
+            f"                    {iterable_repr_value_typing}\n"
             "                ]\n"
             "            ],\n"
             f"            {_parent_module_name}.abc.Readable,\n"
             "            str,\n"
             "            bytes,\n"
             "            None,\n"
             "        ] = None,\n"
             "    ) -> None:\n"
             "        super().__init__(items)\n\n"
         )
     elif isinstance(metadata, abc.ArrayMeta):
-        repr_item_typing: str = indent_(
-            _type_hint_from_property_types(metadata.item_types, module), 20
+        repr_item_typing: str = suffix_long_lines(
+            indent_(
+                _type_hint_from_property_types(metadata.item_types, module), 20
+            )
         )
         out.append(
             "\n"
             "    def __init__(\n"
             "        self,\n"
             "        items: typing.Union[\n"
             "            typing.Iterable[\n"
@@ -2740,28 +2766,29 @@
             property_: abc.Property
             property_name_, property_ = name_and_property
             repr_comma: str = (
                 ""
                 if (property_index + 1 == metadata_properties_items_length)
                 else ","
             )
-            repr_property_typing: str = indent_(
-                _type_hint_from_property(property_, module), 12
+            repr_property_typing: str = suffix_long_lines(
+                indent_(_type_hint_from_property(property_, module), 12)
             )
             parameter_declaration: str = (
                 f"        {property_name_}: typing.Optional[\n"
                 f"            {repr_property_typing}\n"
                 f"        ] = None{repr_comma}"
             )
             out.append(parameter_declaration)
         out.append("    ) -> None:")
         if metadata.properties is not None:
             for property_name_ in metadata.properties.keys():
-                property_assignment: str = (
-                    "        self.%s = %s" % (property_name_, property_name_)
+                property_assignment: str = "        self.%s = %s" % (
+                    property_name_,
+                    property_name_,
                 )
                 # Ensure line-length aligns with PEP-8
                 if len(property_assignment) > MAX_LINE_LENGTH:
                     property_assignment = (
                         f"        self.{property_name_} = (\n"
                         f"            {property_name_}\n"
                         f"        )"
```

### Comparing `sob-1.8.0/sob/properties.py` & `sob-1.9.0/sob/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,17 @@
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
 
 def _date2str(value: date) -> str:
     return value.isoformat()
 
 
@@ -288,15 +290,17 @@
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
         date2str: Callable[[date], str] = _date2str,
         str2date: Callable[[str], date] = parse_date,
     ) -> None:
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
         self._date2str = date2str
         self._str2date = str2date
 
     def date2str(self, value: date) -> str:
         return self._date2str(value)
 
@@ -319,30 +323,30 @@
       in the desired format. The default is `datetime.isoformat`--returning
       an iso8601 compliant date-time string.
     - str2datetime (collections.Callable): A function, taking one argument
       (a datetime string), and returning a python `datetime` json_object.
       By default, this is `iso8601.parse_date`.
     """
 
-    _types: abc.Types = Types(  # type: ignore
-        (datetime,)
-    )
+    _types: abc.Types = Types((datetime,))  # type: ignore
 
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
         datetime2str: Callable[[datetime], str] = _datetime2str,
         str2datetime: Callable[[str], datetime] = parse_date,
     ) -> None:
         self._datetime2str = datetime2str
         self._str2datetime = str2datetime
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
     def datetime2str(self, value: datetime) -> str:
         return self._datetime2str(value)
 
     def str2datetime(self, value: str) -> datetime:
         return self._str2datetime(value)
@@ -360,15 +364,17 @@
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
 
 class Enumerated(Property, abc.Enumerated):
     """
     Parameters:
 
@@ -418,17 +424,15 @@
 
 
 class Number(Property, abc.Number):
     """
     See `sob.properties.Property`
     """
 
-    _types: abc.Types = Types(  # type: ignore
-        (Decimal, float, int)
-    )
+    _types: abc.Types = Types((Decimal, float, int))  # type: ignore
 
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
@@ -445,15 +449,17 @@
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
 
 class Boolean(Property, abc.Boolean):
     """
     See `sob.properties.Property`
     """
@@ -463,15 +469,17 @@
     def __init__(
         self,
         name: Optional[str] = None,
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
 
 class Array(Property, abc.ArrayProperty):
     """
     See `sob.properties.Property`...
 
@@ -479,17 +487,15 @@
 
     - item_types (type|Property|[type|Property]): The type(s) of values/objects
       contained in the array. Similar to
       `sob.properties.Property().types`, but applied to items in the
       array, not the array itself.
     """
 
-    _types: abc.Types = Types(  # type: ignore
-        (abc.Array,)
-    )
+    _types: abc.Types = Types((abc.Array,))  # type: ignore
     _item_types: Optional[abc.Types] = None
 
     def __init__(
         self,
         item_types: Union[
             type, Sequence[Union[type, Property]], Undefined, abc.Types, None
         ] = UNDEFINED,
@@ -497,15 +503,17 @@
         required: bool = False,
         versions: Optional[Sequence[Union[str, Version]]] = None,
     ) -> None:
         self._item_types: Optional[Types] = getattr(type(self), "_item_types")
         if item_types is not UNDEFINED:
             self.item_types = item_types  # type: ignore
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
     @property  # type: ignore
     def item_types(self) -> Optional[abc.Types]:  # type: ignore
         return self._item_types
 
     @item_types.setter  # type: ignore
@@ -544,17 +552,15 @@
 
     - value_types (type|Property|[type|Property]): The type(s) of
       values/objects comprising the mapped values. Similar to
       `sob.properties.Property.types`, but applies to *values* in the
       dictionary object, not the dictionary itself.
     """
 
-    _types: abc.Types = Types(  # type: ignore
-        (abc.Dictionary,)
-    )
+    _types: abc.Types = Types((abc.Dictionary,))  # type: ignore
     _value_types: Optional[abc.Types] = None
 
     def __init__(
         self,
         value_types: Optional[
             Union[type, Sequence[Union[type, Property]], Undefined]
         ] = UNDEFINED,
@@ -564,15 +570,17 @@
     ) -> None:
         self._value_types: Optional[abc.Types] = getattr(
             type(self), "_value_types"
         )
         if value_types is not UNDEFINED:
             self.value_types = value_types  # type: ignore
         super().__init__(
-            name=name, required=required, versions=versions,
+            name=name,
+            required=required,
+            versions=versions,
         )
 
     @property  # type: ignore
     def value_types(self) -> Optional[abc.Types]:
         return self._value_types
 
     @value_types.setter
```

### Comparing `sob-1.8.0/sob/request.py` & `sob-1.9.0/sob/request.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/test.py` & `sob-1.9.0/sob/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
 
 def _get_object_discrepancies_error_message(
     object_a: abc.Object, object_b: abc.Object
 ) -> str:
     a_serialized: str = serialize(object_a)
     b_serialized: str = serialize(object_b)
-    a_representation: str = (
-        "".join(line.strip() for line in repr(object_a).split("\n"))
+    a_representation: str = "".join(
+        line.strip() for line in repr(object_a).split("\n")
     )
     b_representation = "".join(
         line.strip() for line in repr(object_b).split("\n")
     )
     class_name: str = qualified_name(type(object_a))
     message = [
         "Discrepancies were found between the instance of "
@@ -278,24 +278,26 @@
                     value,
                     format_=format_,
                     raise_validation_errors=raise_validation_errors,
                 )
 
 
 def json(
-    model_instance: abc.Model, raise_validation_errors: bool = True,
+    model_instance: abc.Model,
+    raise_validation_errors: bool = True,
 ) -> None:
     model(
         model_instance=model_instance,
         format_="json",
         raise_validation_errors=raise_validation_errors,
     )
 
 
 def yaml(
-    model_instance: abc.Model, raise_validation_errors: bool = True,
+    model_instance: abc.Model,
+    raise_validation_errors: bool = True,
 ) -> None:
     model(
         model_instance=model_instance,
         format_="yaml",
         raise_validation_errors=raise_validation_errors,
     )
```

### Comparing `sob-1.8.0/sob/thesaurus.py` & `sob-1.9.0/sob/thesaurus.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,19 @@
 from .utilities.assertion import (
     assert_is_instance,
     assert_is_subclass,
     assert_not_is_instance,
 )
 from .utilities.inspect import calling_module_name
 from .utilities.io import read
-from .utilities.string import MAX_LINE_LENGTH, class_name, property_name
+from .utilities.string import (
+    class_name,
+    suffix_long_lines,
+    property_name,
+)
 from .utilities.types import NULL, NoneType, Null, UNDEFINED, Undefined
 
 __all__: List[str] = ["Synonyms", "Thesaurus"]
 
 
 def _read(data: abc.Readable) -> str:
     string_data: str
@@ -157,15 +161,17 @@
                 MutableTypes()
                 if types_ is None
                 else types_
                 if isinstance(types_, abc.MutableTypes)
                 else MutableTypes(types_)
             )
             _update_types(
-                mutable_types, new_types, memo=memo,
+                mutable_types,
+                new_types,
+                memo=memo,
             )
             types_ = mutable_types
         metadata.properties[key].types = types_  # type: ignore
 
 
 def _update_object_class_from_meta(
     object_class: type,
@@ -798,15 +804,17 @@
     def isdisjoint(
         self, other: Iterable[Union[abc.Readable, abc.MarshallableTypes]]
     ) -> bool:
         return self._set.isdisjoint(self._get_set(other))
 
 
 def get_class_meta_attribute_assignment_source(
-    class_name_: str, attribute_name: str, metadata: abc.Meta,
+    class_name_: str,
+    attribute_name: str,
+    metadata: abc.Meta,
 ) -> str:
     """
     This function generates source code for setting a metadata attribute on
     a class.
 
     Parameters:
 
@@ -822,35 +830,23 @@
             "object"
             if isinstance(metadata, abc.ObjectMeta)
             else "array"
             if isinstance(metadata, abc.ArrayMeta)
             else "dictionary"
         ),
     )
-
-    def noqa_line_if_long(line: str) -> str:
-        # We want to add "  # noqa" at the end of any line
-        # which is within 4 spaces of the maximum line length, since
-        # reformatting with `black` will add an additional 4 spaces.
-        if len(line) > (MAX_LINE_LENGTH - 4):
-            line = f"{line}  # noqa"
-        return line
-
     # We insert "  # type: ignore" at the end of the first line where the value
     # is assigned due to mypy issues with properties having getters and setters
-    represent_metadata_attribute: str = "\n".join(
-        map(
-            noqa_line_if_long,
-            repr(getattr(metadata, attribute_name)).split("\n"),
-        )
-    )
-    return (
-        f"{writable_function_name}(  # type: ignore\n"
-        f"    {class_name_}\n"
-        f").{attribute_name} = {represent_metadata_attribute}"
+    return suffix_long_lines(
+        (
+            f"{writable_function_name}(  # type: ignore\n"
+            f"    {suffix_long_lines(class_name_, -4)}\n"
+            f").{attribute_name} = {repr(getattr(metadata, attribute_name))}"
+        ),
+        -4,
     )
 
 
 @collections.abc.MutableMapping.register
 class Thesaurus:
     """
     TODO
@@ -1098,15 +1094,17 @@
         # the calling module.
         module_name: str = calling_module_name(2)
         module: ModuleType = ModuleType(module_name)
         exec(self._get_module_source(module_name, name=name), module.__dict__)
         return module
 
     def save_module(
-        self, path: str, name: Callable[[str], str] = class_name_from_pointer,
+        self,
+        path: str,
+        name: Callable[[str], str] = class_name_from_pointer,
     ) -> None:
         """
         This method generates and saves the source code for a module
         defining data models applicable to the data contained in this
         thesaurus.
 
         Parameters:
```

### Comparing `sob-1.8.0/sob/types.py` & `sob-1.9.0/sob/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         return self._list.__len__()
 
     def _append(self, value: Union[type, abc.Property]) -> None:
         _validate_type_or_property(value)
         self._list.append(value)
 
     def _extend(
-        self, values: Union[Iterable[Union[type, abc.Property]], abc.Types],
+        self,
+        values: Union[Iterable[Union[type, abc.Property]], abc.Types],
     ) -> None:
         value: Union[type, abc.Property]
         for value in values:
             self._append(value)
 
     def __getitem__(self, index: int) -> Union[type, abc.Property]:
         return self._list.__getitem__(index)
```

### Comparing `sob-1.8.0/sob/utilities/__init__.py` & `sob-1.9.0/sob/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/utilities/assertion.py` & `sob-1.9.0/sob/utilities/assertion.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/utilities/inspect.py` & `sob-1.9.0/sob/utilities/inspect.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/utilities/io.py` & `sob-1.9.0/sob/utilities/io.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/utilities/string.py` & `sob-1.9.0/sob/utilities/string.py`

 * *Files 9% similar despite different names*

```diff
@@ -312,22 +312,25 @@
 ) -> str:
     """
     Indent text by `number_of_spaces` starting at line index `start` and
     stopping at line index `stop`.
     """
     indented_text = string
     if ("\n" in string) or start == 0:
-        lines = string.split("\n")
+        lines: List[str] = string.split("\n")
         if stop:
             if stop < 0:
                 stop = len(lines) - stop
         else:
             stop = len(lines)
-        for i in range(start, stop):
-            lines[i] = (" " * number_of_spaces) + lines[i]
+        index: int
+        for index in range(start, stop):
+            line: str = lines[index]
+            line_indent: str = " " * number_of_spaces
+            lines[index] = f"{line_indent}{line}".rstrip()
         indented_text = "\n".join(lines)
     return indented_text
 
 
 def url_directory_and_file_name(url: str) -> Tuple[str, str]:
     """
     Split a URL into a directory path and file name
@@ -391,15 +394,15 @@
                 len(wrapped_line) + len(word) + indent_length
             ) <= max_line_length:
                 wrapped_line += word
             else:
                 lines.append(indent_ + wrapped_line.rstrip())
                 wrapped_line = "" if not word.strip() else word
         if wrapped_line:
-            lines.append(indent_ + wrapped_line.rstrip())
+            lines.append(f"{indent_}{wrapped_line}".rstrip())
         wrapped_line = "\n".join(lines)
     else:
         wrapped_line = line
     return wrapped_line
 
 
 def split_long_docstring_lines(
@@ -411,27 +414,61 @@
     >>> print(split_long_docstring_lines(
     ...     '    Lorem ipsum dolor sit amet, consectetur adipiscing elit. '
     ...     'Nullam faucibu odio a urna elementum, eu tempor nisl efficitu'
     ... ))
         Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam faucibu
         odio a urna elementum, eu tempor nisl efficitu
     """
+    line: str
     indent_: str = "    "
     if "\t" in docstring:
         docstring = docstring.replace("\t", indent_)
-    lines = docstring.split("\n")
+    lines: List[str] = docstring.split("\n")
     indentation_length: int = sys.maxsize
-    for line in lines:
+    for line in filter(lambda line: line, lines):
         match = re.match(r"^[ ]+", line)
         if match:
             indentation_length = min(indentation_length, len(match.group()))
         else:
             indentation_length = 0
             break
-    wrapped_lines = []
-    for line in lines:
-        wrapped_lines.append(
-            split_long_comment_line(
-                indent_ + line[indentation_length:], max_line_length, prefix=""
+    if indentation_length < sys.maxsize:
+        wrapped_lines: List[str] = []
+        for line in lines:
+            wrapped_lines.append(
+                split_long_comment_line(
+                    indent_ + line[indentation_length:],
+                    max_line_length,
+                    prefix="",
+                )
             )
-        )
-    return "\n".join(wrapped_lines)
+        docstring = "\n".join(wrapped_lines)
+    # Strip trailing whitespace and empty lines
+    return re.sub(r"[ ]+(\n|$)", r"\1", docstring)
+
+
+def suffix_long_lines(
+    text: str, max_line_length: int = MAX_LINE_LENGTH, suffix: str = "  # noqa"
+) -> str:
+    """
+    This function adds a suffix to the end of any line of code longer than
+    `max_line_length`.
+
+    Parameters:
+
+    - text (str): Text representing python code
+    - max_line_length (int) = 79:
+      The length at which a line should have the `suffix` appended. If
+      this is a *negative* integer (or zero), the sum of this integer +
+      `MAX_LINE_LENGTH` is used
+    - suffix (str) = "  # noqa": The default suffix indicates to linters that
+      a long line should be permitted
+    """
+    if max_line_length <= 0:
+        max_line_length += MAX_LINE_LENGTH
+
+    def suffix_line_if_long(line: str) -> str:
+        if len(line) > max_line_length and not line.endswith(suffix):
+            line = f"{line}{suffix}"
+        return line
+
+    return "\n".join(map(suffix_line_if_long, text.split("\n")))
```

### Comparing `sob-1.8.0/sob/utilities/types.py` & `sob-1.9.0/sob/utilities/types.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob/version.py` & `sob-1.9.0/sob/version.py`

 * *Files identical despite different names*

### Comparing `sob-1.8.0/sob.egg-info/PKG-INFO` & `sob-1.9.0/sob.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sob
-Version: 1.8.0
+Version: 1.9.0
 Summary: A framework for serializing/deserializing JSON/YAML into python class instances and vice versa
 Home-page: https://github.com/davebelais/sob
 Author: David Belais
 Author-email: david@belais.me
 License: MIT
 Description: UNKNOWN
 Keywords: rest api serialization serialize
```

### Comparing `sob-1.8.0/sob.egg-info/requires.txt` & `sob-1.9.0/sob.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 iso8601~=0.1
 more-itertools~=8.6
 
 [all]
 mypy~=0.812
 tox~=3.20
 pytest~=5.4
-flake8~=3.8
+flake8~=3.9
 setuptools-setup-versions<2,>=1.8.0
 readme-md-docstrings<1,>=0.1.0
 wheel~=0.35.1
 readme-md-docstrings<2,~=0.1.0
 twine~=3.2
+black~=20.8b1
 daves-dev-tools~=0.1
 
 [dev]
 mypy~=0.812
 wheel~=0.35.1
 tox~=3.20
 pytest~=5.4
-flake8~=3.8
+flake8~=3.9
 setuptools-setup-versions<2,>=1.8.0
 readme-md-docstrings<2,~=0.1.0
 twine~=3.2
+black~=20.8b1
 daves-dev-tools~=0.1
 
 [test]
 mypy~=0.812
 tox~=3.20
 pytest~=5.4
-flake8~=3.8
+flake8~=3.9
 setuptools-setup-versions<2,>=1.8.0
 readme-md-docstrings<1,>=0.1.0
```

