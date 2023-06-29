# Comparing `tmp/pystatic-language-1.0.3.tar.gz` & `tmp/pystatic-language-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystatic-language-1.0.3.tar", last modified: Mon May 15 13:24:56 2023, max compression
+gzip compressed data, was "pystatic-language-1.1.0.tar", last modified: Thu Jun 29 08:39:53 2023, max compression
```

## Comparing `pystatic-language-1.0.3.tar` & `pystatic-language-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.593951 pystatic-language-1.0.3/
--rw-rw-rw-   0        0        0      115 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8940 2023-05-15 13:24:56.592383 pystatic-language-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7852 2023-03-16 09:20:24.000000 pystatic-language-1.0.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.0.3/build.py
--rw-rw-rw-   0        0        0      925 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.575945 pystatic-language-1.0.3/pystatic/
--rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.0.3/pystatic/base.py
--rw-rw-rw-   0        0        0     8345 2023-05-15 12:59:03.000000 pystatic-language-1.0.3/pystatic/casting.py
--rw-rw-rw-   0        0        0     1408 2023-05-15 13:02:42.000000 pystatic-language-1.0.3/pystatic/clean.py
--rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.0.3/pystatic/document.py
--rw-rw-rw-   0        0        0     5726 2023-05-15 13:12:38.000000 pystatic-language-1.0.3/pystatic/overload.py
--rw-rw-rw-   0        0        0     5831 2023-05-15 13:16:21.000000 pystatic-language-1.0.3/pystatic/private.py
--rw-rw-rw-   0        0        0     8050 2023-05-15 13:18:50.000000 pystatic-language-1.0.3/pystatic/types.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:24:56.592383 pystatic-language-1.0.3/pystatic_language.egg-info/
--rw-rw-rw-   0        0        0     8940 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 13:24:56.000000 pystatic-language-1.0.3/pystatic_language.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.0.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 13:24:56.593951 pystatic-language-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-05-15 13:24:49.000000 pystatic-language-1.0.3/setup.py
--rw-rw-rw-   0        0        0     3093 2023-05-13 16:47:31.000000 pystatic-language-1.0.3/test.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.127553 pystatic-language-1.1.0/
+-rw-rw-rw-   0        0        0      115 2023-06-29 08:39:52.000000 pystatic-language-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4116 2023-06-29 08:39:53.126554 pystatic-language-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3028 2023-06-29 08:39:46.000000 pystatic-language-1.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.1.0/build.py
+-rw-rw-rw-   0        0        0      925 2023-06-29 08:39:52.000000 pystatic-language-1.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.112555 pystatic-language-1.1.0/pystatic/
+-rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.1.0/pystatic/base.py
+-rw-rw-rw-   0        0        0     2900 2023-06-29 08:31:21.000000 pystatic-language-1.1.0/pystatic/casting.py
+-rw-rw-rw-   0        0        0     1408 2023-06-29 08:31:59.000000 pystatic-language-1.1.0/pystatic/clean.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.1.0/pystatic/document.py
+-rw-rw-rw-   0        0        0     5536 2023-06-29 08:34:59.000000 pystatic-language-1.1.0/pystatic/overload.py
+-rw-rw-rw-   0        0        0     2879 2023-06-29 08:35:26.000000 pystatic-language-1.1.0/pystatic/private.py
+-rw-rw-rw-   0        0        0     8106 2023-06-29 07:23:27.000000 pystatic-language-1.1.0/pystatic/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.125555 pystatic-language-1.1.0/pystatic_language.egg-info/
+-rw-rw-rw-   0        0        0     4116 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:39:53.127553 pystatic-language-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-06-29 08:30:42.000000 pystatic-language-1.1.0/setup.py
+-rw-rw-rw-   0        0        0     2783 2023-06-29 08:38:30.000000 pystatic-language-1.1.0/test.py
```

### Comparing `pystatic-language-1.0.3/build.py` & `pystatic-language-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.3/pyproject.toml` & `pystatic-language-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pystatic-language'
-version = '1.0.3'
+version = '1.1.0'
 description = "This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and."
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pystatic-language-1.0.3/pystatic/base.py` & `pystatic-language-1.1.0/pystatic/base.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.0.3/pystatic/clean.py` & `pystatic-language-1.1.0/pystatic/clean.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,58 +2,58 @@
 
 from typing import Iterable, Optional
 
 __all__ = [
     "clean_module"
 ]
 
-def clean_module(name: str, properties: Optional[Iterable[str]] = None) -> None:
+def clean_module(name: str, attributes: Optional[Iterable[str]] = None) -> None:
     """
     Cleans the module properties from attributes that are not in the __all__ list.
 
-    :param properties: The properties to save.
+    :param attributes: The properties to save.
     :param name: The name of the module.
     """
 
     import sys
 
     module = sys.modules[__name__]
 
-    if properties is None:
-        properties = [
+    if attributes is None:
+        attributes = [
             key for key, value in module.__dict__.items()
             if (
                 (hasattr(value, '__module__')) and
                 (value.__module__ == name)
             )
         ]
 
-    elif not isinstance(properties, list):
-        properties = list(properties)
+    elif not isinstance(attributes, list):
+        attributes = list(attributes)
     # end if
 
-    properties.extend(
+    attributes.extend(
         [
             "__name__",
             "__doc__",
             "__package__",
             "__loader__",
             "__spec__",
             "__all__",
             "__file__",
             "__cached__",
             "__builtins__",
             "__annotations__"
         ]
     )
 
-    properties = list(set(properties))
+    attributes = list(set(attributes))
 
     for key in sys.modules[name].__dict__.copy():
         if (
-            (key not in properties) and
+            (key not in attributes) and
             (key in sys.modules[name].__dict__)
         ):
             sys.modules[name].__dict__.pop(key)
         # end if
     # end for
 # end clean_module
```

### Comparing `pystatic-language-1.0.3/pystatic/overload.py` & `pystatic-language-1.1.0/pystatic/overload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # overload.py
 
 import inspect
+import warnings
 from functools import partial
-from typing import Callable, Any, Union, Tuple, Dict, Optional
+from typing import Callable, Any, Union, Tuple, Dict, Optional, Type
 
 from pystatic.types import (
     statictypes, RuntimeTypeError, RuntimeTypeWarning
 )
 
 __all__ = [
     "Overload",
-    "OverloadProtocol",
     "overload"
 ]
 
 def overload_signature_error_message(
         c: Callable, args: Tuple, kwargs: Dict[str, Any]
 ) -> str:
     """
@@ -77,36 +77,14 @@
 
     :returns: The callable method.
     """
 
     return method if is_regular_method(method) else method.__func__
 # end get_callable_method
 
-class OverloadProtocol:
-    """A class to enable the overload inside classes."""
-
-    def __getattribute__(self, key: str) -> Any:
-        """
-        Gets the attribute value.
-
-        :param key: The name of the attribute.
-
-        :return: The attribute value.
-        """
-
-        val = super().__getattribute__(key)
-
-        if isinstance(val, Overload):
-            val.instance = self
-        # end if
-
-        return val
-    # end __getattribute__
-# end OverloadProtocol
-
 def call(
         c: Method,
         instance: Any,
         args: Tuple,
         kwargs: Dict[str, Any]
 ) -> Any:
     """
@@ -167,15 +145,29 @@
         """
 
         self.signatures[inspect.signature(get_callable_method(c))] = c
 
         return self
     # end overload
 
-    # noinspection PyUnresolvedReferences
+    def __get__(self, instance: object, owner: Type) -> Any:
+        """
+        Gets the value of the callable from the object.
+
+        :param instance: The object.
+        :param owner: The class.
+
+        :return: The overload object.
+        """
+
+        self.instance = self.instance or instance
+
+        return self
+    # end __get__
+
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """
         Calls the decorated callable with the overloading match.
 
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
```

### Comparing `pystatic-language-1.0.3/pystatic/types.py` & `pystatic-language-1.1.0/pystatic/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # types.py
 
 from abc import ABCMeta
 import inspect
 import warnings
 from typing import (
-    Any, Union, Optional, Callable, Type, Sequence
+    Any, Union, Optional, Callable, Type, Sequence, TypeVar
 )
 
 from typeguard import check_type
 
 __all__ = [
     "Config",
     "RuntimeTypeWarning",
@@ -71,20 +71,28 @@
     # end __init__
 # end RuntimeValueTypeError
 
 class RuntimeTypeWarning(Warning):
     """A class to represent a runtime type warning."""
 # end RuntimeTypeWarning
 
+_R = TypeVar("_R")
+
+ValidatedCallable = Union[
+    Callable[..., _R],
+    Callable[[Union[Type, Callable[..., _R]]], Callable[..., _R]]
+]
+
+
 def __validate(
         obj: Optional[Union[Type, Callable]] = None, *,
         excluded_names: Optional[Sequence[str]] = None,
         excluded_hints: Optional[Sequence[Any]] = None,
         crush: Optional[bool] = None
-) -> Union[Callable[..., Any], Callable[[Union[Type, Callable]], Callable[..., Any]]]:
+) -> ValidatedCallable:
     """
     Wraps a callable object with runtime type enforcement.
 
     :param obj: The callable object.
     :param excluded_names: The names to exclude from the check.
     :param excluded_hints: The hints to exclude from the check.
     ude from the check.
@@ -96,15 +104,15 @@
     if crush is None:
         crush = Config.crush
     # end if
 
     excluded_names = excluded_names or ()
     excluded_hints = excluded_hints or ()
 
-    def wrap_call(*args: Any, **kwargs: Any) -> Any:
+    def wrap_call(*args: Any, **kwargs: Any) -> _R:
         """
         Wraps a callable object with runtime type enforcement.
 
         :param args: Any positional argument.
         :param kwargs: Any keyword argument.
 
         :returns: The returned value.
@@ -179,15 +187,15 @@
         return data
     # end wrap_call
 
     if obj is not None:
         return wrap_call
     
     else:
-        def wrap_wrapper(value: Union[Type, Callable]) -> Callable:
+        def wrap_wrapper(value: Union[Type, Callable[..., _R]]) -> Callable[..., _R]:
             """
             Wraps a callable object with runtime type enforcement.
 
             :param value: The callable object.
 
             :returns: The inner wrapper function.
             """
@@ -204,15 +212,15 @@
 # end __validate
 
 def validate(
         obj: Optional[Union[Type, Callable]] = None, *,
         excluded_names: Optional[Sequence[str]] = None,
         excluded_hints: Optional[Sequence[Any]] = None,
         crush: Optional[bool] = None
-) -> Union[Callable[..., Any], Callable[[Union[Any, Type, Callable]], Callable[..., Any]]]:
+) -> Union[Type, ValidatedCallable]:
     """
     Wraps a callable object with runtime type enforcement.
 
     :param obj: The callable object.
     :param excluded_names: The names to exclude from the check.
     :param excluded_hints: The hints to exclude from the check.
     :param crush: The value to raise errors.
@@ -248,15 +256,15 @@
     # end if
 # end validate
 
 def typecheck(
         value: Any,
         hint: Any,
         name: Optional[str] = None,
-        crush: Optional[bool] = True
+        crush: Optional[bool] = None
 ) -> bool:
     """
     Checks the type of variable by its type hinting.
 
     :param value: The object to check.
     :param hint: The type hinting.
     :param name: The name of the variable.
```

### Comparing `pystatic-language-1.0.3/setup.py` & `pystatic-language-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pystatic-language',
-        version='1.0.3',
+        version='1.1.0',
         description=(
             "This package is a collection of methods and classes for "
             "making python more secure, robust, and reliable. "
             "This could be achieved through the simple usage of decorators, "
             "function calls and inheritance of base classes. "
             "Generally, this package can make python a programming language, "
             "closer to other static-typed languages, "
```

### Comparing `pystatic-language-1.0.3/test.py` & `pystatic-language-1.1.0/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,55 @@
 # test.py
 
 import time
 import warnings
 
-from pystatic.overload import OverloadProtocol, overload
+from pystatic.overload import overload
 from pystatic.types import statictypes
-from pystatic.private import private, PrivatePropertyProtocol
-from pystatic.casting import Castable, cast
+from pystatic.private import private
+from pystatic.casting import cast
 
-class Demo1(Castable):
+class Demo1:
 
     def __init__(self, a, b, c, x=None):
 
         self.a = a
         self.b = b
         self.c = c
         self.x = x
 
-class Demo2(Castable):
+class Demo2(Demo1):
 
     def __init__(self, a, b, c, x=None, y=None, z=None):
 
-        self.a = a
-        self.b = b
-        self.c = c
-        self.x = x
+        super().__init__(a, b, c, x)
+
         self.y = y
         self.z = z
 
 demo2 = Demo2(0, 1, 2, 3, 4, 5)
 demo1 = cast(Demo1, demo2)
 
-print(demo2, demo2.dict)
-print(demo1, demo1.dict)
+print(demo2, type(demo2), demo2.__dict__)
+print(demo1, type(demo1), demo1.__dict__)
 
 # noinspection PyNestedDecorators
-class Foo(OverloadProtocol, PrivatePropertyProtocol):
+class Foo:
 
     c = private()
 
     def __init__(self):
 
         print("\nclass Foo:\n\n\tdef __init__(self):\n")
 
         self.c = 1
         print("\t\t>>> self.c = 1")
         print("\t\t>>> print(self.c)")
         print(f"\t\t{self.c}\n")
 
-        self.__d = 1
-        print("\t\t>>> self.__d = 1")
-        print("\t\t>>> print(self.__d)")
-        print(f"\t\t{self.__d}\n")
-
         self.c = 0
         print("\t\t>>> self.c = 0")
         print("\t\t>>> print(self.c)")
         print(f"\t\t{self.c}\n")
 
         self.__d = 0
         print("\t\t>>> self.__d = 0")
@@ -97,21 +90,26 @@
     def b(self, x: int):
         print("\n\t@statictypes(crush=False)\n\tdef b(self, x: int):")
         print(f"\n\t\t>>> print(type(x))")
         print(f"\t\t{type(x)}\n")
 
 foo = Foo()
 
+print(">>> foo.a('')")
 foo.a('')
+print(">>> foo.a(0.0)")
 foo.a(0.0)
-
+print(">>> Foo.a(0)")
 Foo.a(0)
+print(">>> Foo.a(0.0)")
 Foo.a(0.0)
 
+print(">>> foo.b(0)")
 foo.b(0)
+print(">>> foo.b(0.0)")
 # noinspection PyTypeChecker
 foo.b(0.0)
 
 time.sleep(0.2)
 
 try:
     print("\n>>> print(Foo.c)")
@@ -127,19 +125,8 @@
     print("\n>>> print(foo.c)")
     print(foo.c)
 
 except AttributeError as e:
     warnings.warn(str(e))
 # end try
 
-time.sleep(0.2)
-
-try:
-    print("\n>>> print(foo._Foo__d)")
-    # noinspection PyProtectedMember
-    print(foo._Foo__d)
-
-except AttributeError as e:
-    warnings.warn(str(e))
-# end try
-
 time.sleep(0.2)
```

