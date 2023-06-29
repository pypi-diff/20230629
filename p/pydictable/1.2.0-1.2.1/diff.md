# Comparing `tmp/pydictable-1.2.0.tar.gz` & `tmp/pydictable-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydictable-1.2.0.tar", last modified: Tue Jun 27 18:11:46 2023, max compression
+gzip compressed data, was "pydictable-1.2.1.tar", last modified: Thu Jun 29 07:29:08 2023, max compression
```

## Comparing `pydictable-1.2.0.tar` & `pydictable-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:11:35.000000 pydictable-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 18:11:46.135373 pydictable-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-27 18:11:35.000000 pydictable-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/pydictable/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-27 18:11:35.000000 pydictable-1.2.0/pydictable/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:11:46.135373 pydictable-1.2.0/pydictable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 18:11:46.000000 pydictable-1.2.0/pydictable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:11:46.135373 pydictable-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 18:11:35.000000 pydictable-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.670897 pydictable-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 07:28:59.000000 pydictable-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 07:29:08.670897 pydictable-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 07:28:59.000000 pydictable-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.666897 pydictable-1.2.1/pydictable/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30771 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.670897 pydictable-1.2.1/pydictable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:29:08.670897 pydictable-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:28:59.000000 pydictable-1.2.1/setup.py
```

### Comparing `pydictable-1.2.0/LICENSE` & `pydictable-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.0/README.md` & `pydictable-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.0/pydictable/core.py` & `pydictable-1.2.1/pydictable/core.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.0/pydictable/field.py` & `pydictable-1.2.1/pydictable/field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import math
+import re
 from abc import ABC
 from datetime import datetime
 from enum import EnumMeta, Enum
-from typing import Type, List, Any, Callable
+from typing import Type, List, Any
 
 from pydictable.type import Field, _BaseDictAble, DefaultFactoryType
 
 
 class DataValidationError(Exception):
     def __init__(self, path: str, err):
         super(DataValidationError, self).__init__(path, err)
@@ -80,15 +82,15 @@
         assert type(v) == int
 
     def validate(self, field_name: str, v):
         assert isinstance(v, datetime)
 
 
 class ObjectField(Field):
-    def __init__(self, obj_type: Type[_BaseDictAble], required: bool=False):
+    def __init__(self, obj_type: Type[_BaseDictAble], required: bool = False):
         super(ObjectField, self).__init__(required=required)
         self.obj_type = obj_type
 
     def from_dict(self, v):
         return self.obj_type(dict=v)
 
     def to_dict(self, v):
@@ -132,14 +134,15 @@
         return self.obj_type.spec()
 
 
 class CustomField(Field, ABC):
     """
     For advance usage
     """
+
     def __init__(self, from_json, to_json, *args, **kwargs):
         super(CustomField, self).__init__(*args, **kwargs)
         self._from_json = from_json
         self._to_json = to_json
 
     def from_dict(self, v):
         return self._from_json(v)
@@ -193,14 +196,15 @@
         return [e.name if self.is_name else e.value for e in self.enum]
 
 
 class DictValueField(Field):
     """
     Deprecated function. Use DictField instead
     """
+
     def __init__(self, value_type: Type[_BaseDictAble], required: bool = False, key: str = None):
         self.value_type = value_type
         super(DictValueField, self).__init__(required, key)
 
     def from_dict(self, v):
         return {key: self.value_type(dict=val) for key, val in v.items()}
 
@@ -328,13 +332,80 @@
                 raise DataValidationError(f'{k}.{e.path}', f'Invalid value, {str(e.err)}')
 
     def validate(self, field_name: str, value):
         assert type(value) is dict
         for k, v in value.items():
             self.key_type.validate(None, k)
             self.value_type.validate(None, v)
-
+            
     def of(self):
         return {
             'key': self.key_type.spec(),
             'value': self.value_type.spec()
-        }
+        }   
+         
+
+class RegexField(Field):
+    def __init__(self, regex_string: str, *args, **kwargs):
+        super(RegexField, self).__init__(*args, **kwargs)
+        self.regex_string = regex_string
+
+    def from_dict(self, v):
+        return v
+
+    def to_dict(self, v):
+        return v
+
+    def validate_dict(self, field_name: str, v):
+        assert re.match(self.regex_string, v), f"{v} for {field_name} should be in proper format"
+
+    def validate(self, field_name: str, v):
+        assert isinstance(v, str)
+
+    def of(self):
+        return {'regex': self.regex_string}
+
+
+class RangeIntField(Field):
+    def __init__(self, min_val: int = 0, max_val: int = math.inf, *args, **kwargs):
+        super(RangeIntField, self).__init__(*args, **kwargs)
+        self.min_val = min_val
+        self.max_val = max_val
+
+    def from_dict(self, v):
+        return v
+
+    def to_dict(self, v):
+        return v
+
+    def validate_dict(self, field_name: str, v):
+        assert self.min_val <= v <= self.max_val, \
+            f"{v} for {field_name} should be in range {self.min_val} to {self.max_val}"
+
+    def validate(self, field_name: str, v):
+        assert isinstance(v, int)
+
+    def of(self):
+        return {'min': self.min_val, 'max': self.max_val}
+
+
+class RangeFloatField(Field):
+    def __init__(self, min_val: float = 0.0, max_val: float = math.inf, *args, **kwargs):
+        super(RangeFloatField, self).__init__(*args, **kwargs)
+        self.min_val = min_val
+        self.max_val = max_val
+
+    def from_dict(self, v):
+        return v
+
+    def to_dict(self, v):
+        return v
+
+    def validate_dict(self, field_name: str, v):
+        assert self.min_val <= v <= self.max_val, \
+            f"{v} for {field_name} should be in range {self.min_val} to {self.max_val}"
+
+    def validate(self, field_name: str, v):
+        assert isinstance(v, float)
+
+    def of(self):
+        return {'min': self.min_val, 'max': self.max_val}
```

### Comparing `pydictable-1.2.0/pydictable/test_core.py` & `pydictable-1.2.1/pydictable/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
+import math
 from datetime import datetime
 from enum import Enum
 from time import sleep
-from typing import List, Dict, Optional, Tuple, Union, Any
+from typing import List, Dict, Optional, Union, Any
 from unittest import TestCase
 
 from pydictable.core import DictAble
 from pydictable.field import IntField, StrField, ListField, ObjectField, DatetimeField, CustomField, MultiTypeField, \
-    EnumField, DictField, DictValueField, UnionField, DataValidationError
+    EnumField, DictField, DictValueField, UnionField, DataValidationError, RegexField, RangeIntField, RangeFloatField
 
 
 class TestCore(TestCase):
     def __assert_json_equal(self, json_1, json_2):
         self.assertEqual(json.dumps(json_1), json.dumps(json_2))
 
     def test_basic(self):
@@ -351,16 +352,16 @@
 
         User()
         User(dict={})
 
         class User(DictAble):
             pins: Dict[str, Address] = DictValueField(Address)
 
-        u = User(pins={'a': Address(pin='333')})
-        u = User(dict={'pins': {'a': {'pin': '333'}}})
+        User(pins={'a': Address(pin='333')})
+        User(dict={'pins': {'a': {'pin': '333'}}})
 
     def test_union_field(self):
         class User(DictAble):
             roll_no = UnionField([IntField(), StrField()])
 
         self.assertEqual(User(roll_no="1").roll_no, "1")
         self.assertEqual(User(roll_no=1).roll_no, 1)
@@ -772,15 +773,15 @@
         _now = datetime(2023, 5, 19)
         self.assertEqual(DOB(date=_now).date, _now)
 
         self.assertEqual(DOB(dict={}).date, now)
         self.assertEqual(DOB(dict={'date': None}).date, now)
 
         millis = 1684462306000
-        self.assertEqual(DOB(dict={'date': millis}).date, datetime.fromtimestamp(millis/1000))
+        self.assertEqual(DOB(dict={'date': millis}).date, datetime.fromtimestamp(millis / 1000))
 
         class DOB(DictAble):
             date: datetime = DatetimeField(default_factory=(datetime.now, (), {}))
             date_2: datetime = DatetimeField(default=datetime.now())
 
         self.assertLessEqual((DOB().date - datetime.now()).total_seconds(), 1e2)
 
@@ -796,7 +797,67 @@
 
         class Number(DictAble):
             num: int = IntField(default_factory=(math, (8,), {'b': 5}))
 
         self.assertEqual(Number().num, 40)
         self.assertEqual(Number(dict={'num': None}).num, 40)
         self.assertEqual(Number(dict={'num': 5}).num, 5)
+
+    def test_regex(self):
+        class Profile(DictAble):
+            panNumber: str = RegexField(required=False, regex_string=r"^[A-Z]{5}[0-9]{4}[A-Z]$")
+            email: str = RegexField(regex_string=r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$")
+
+        try:
+            Profile(dict={'email': 'xyz'})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: xyz for email should be in proper format')
+
+        try:
+            Profile(dict={'email': 'abc@gmail.com', 'panNumber': '12345'})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: 12345 for panNumber should be in proper format')
+
+        profile = Profile(dict={'email': 'abc@gmail.com', 'panNumber': 'ABCDE1234H'})
+
+        self.assertEqual(
+            profile.get_input_spec(),
+            {
+                'email': {
+                    'type': 'RegexField', 'required': False,
+                    'of': {'regex': '^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$'}
+                },
+                'panNumber': {'type': 'RegexField', 'required': False, 'of': {'regex': '^[A-Z]{5}[0-9]{4}[A-Z]$'}}
+            }
+        )
+
+    def test_range(self):
+        class Profile(DictAble):
+            salary: int = RangeIntField(required=False, max_val=100000, min_val=1000)
+            expenses: float = RangeFloatField(required=False, max_val=10000.0)
+            donation: float = RangeFloatField(required=False, min_val=100.0)
+
+        try:
+            Profile(dict={'salary': 10000000})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: 10000000 for salary should be in range 1000 to 100000')
+
+        try:
+            Profile(dict={'salary': 10000, 'expenses': 100000.0})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: 100000.0 for expenses should be in range 0.0 to 10000.0')
+
+        try:
+            Profile(dict={'salary': 100000, 'expenses': 1000.0, 'donation': 10.0})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: 10.0 for donation should be in range 100.0 to inf')
+
+        profile = Profile(dict={'salary': 10000, 'expenses': 1000.0, 'donation': 1000.0})
+
+        self.assertEqual(
+            profile.get_input_spec(),
+            {
+                'donation': {'type': 'RangeFloatField', 'required': False, 'of': {'min': 100, 'max': math.inf}},
+                'expenses': {'type': 'RangeFloatField', 'required': False, 'of': {'min': 0.0, 'max': 10000}},
+                'salary': {'type': 'RangeIntField', 'required': False, 'of': {'min': 1000, 'max': 100000}}
+            }
+        )
```

### Comparing `pydictable-1.2.0/pydictable/test_field.py` & `pydictable-1.2.1/pydictable/test_field.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.0/pydictable/type.py` & `pydictable-1.2.1/pydictable/type.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.0/setup.py` & `pydictable-1.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pydictable',
-    version='1.2.0',
+    version='1.2.1',
     author='Pramod Kumar',
     author_email='pramodkumar.damam73@gmail.com',
     description='Make your classes from/to dict',
     url='https://github.com/pskd73/pydictable.git',
     packages=['pydictable'],
     include_package_data=True,
     long_description='A tool to create data modals from dict and convert it to dict. '
```

