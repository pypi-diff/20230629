# Comparing `tmp/fw_utils-4.2.9-py3-none-any.whl.zip` & `tmp/fw_utils-4.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22033 bytes, number of entries: 14
+Zip file size: 22153 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1747 b- defN 80-Jan-01 00:00 fw_utils/__init__.py
 -rw-r--r--  2.0 unx     2914 b- defN 80-Jan-01 00:00 fw_utils/datetime.py
 -rw-r--r--  2.0 unx     3095 b- defN 80-Jan-01 00:00 fw_utils/dicts.py
 -rw-r--r--  2.0 unx     5436 b- defN 80-Jan-01 00:00 fw_utils/files.py
--rw-r--r--  2.0 unx     8838 b- defN 80-Jan-01 00:00 fw_utils/filters.py
--rw-r--r--  2.0 unx    10485 b- defN 80-Jan-01 00:00 fw_utils/formatters.py
+-rw-r--r--  2.0 unx     9250 b- defN 80-Jan-01 00:00 fw_utils/filters.py
+-rw-r--r--  2.0 unx    10502 b- defN 80-Jan-01 00:00 fw_utils/formatters.py
 -rw-r--r--  2.0 unx    15077 b- defN 80-Jan-01 00:00 fw_utils/parsers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_utils/py.typed
 -rw-r--r--  2.0 unx     4382 b- defN 80-Jan-01 00:00 fw_utils/state.py
 -rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 fw_utils/testing.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.2.9.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.2.9.dist-info/RECORD
-14 files, 59179 bytes uncompressed, 20321 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.3.0.dist-info/RECORD
+14 files, 59608 bytes uncompressed, 20441 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: fw_utils/state.py
 Comment: 
 
 Filename: fw_utils/testing.py
 Comment: 
 
-Filename: fw_utils-4.2.9.dist-info/LICENSE
+Filename: fw_utils-4.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_utils-4.2.9.dist-info/METADATA
+Filename: fw_utils-4.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_utils-4.2.9.dist-info/WHEEL
+Filename: fw_utils-4.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_utils-4.2.9.dist-info/RECORD
+Filename: fw_utils-4.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_utils/filters.py

```diff
@@ -149,26 +149,34 @@
             return False
         return OPERATORS[self.op](value, self.num)
 
 
 class SetFilter(ExpressionFilter):
     """Set filter."""
 
-    operators = ["=", "!="]  # ie. in / not in
+    operators = ["=", "!=", "=~", "!~"]  # ie. in / not in
+    pattern: t.Optional[t.Pattern]
 
     def __init__(self, field: str, op: str, value: str) -> None:
         """Initialize set filter from str value."""
         super().__init__(field, op, value.lower())
+        try:
+            self.pattern = re.compile(value) if "~" in op else None
+        except re.error as exc:
+            raise ValueError(f"Invalid pattern: {value} - {exc}") from exc
 
     def match(self, value: t.Union[list, set, t.Any]) -> bool:
         """Return that the given item is in the given list/set."""
         values = value if isinstance(value, (list, set)) else self.getval(value)
         if not values:
             return False
-        return OPERATORS[self.op](self.value in [v.lower() for v in values], True)
+        for value in values:
+            if OPERATORS[self.op](value, self.pattern or self.value):
+                return True
+        return False
 
 
 class StringFilter(ExpressionFilter):
     """String filter."""
 
     operators = STRING_OPS
     string: t.Union[str, t.Pattern]
@@ -246,17 +254,18 @@
 
 def parse_filter_expression(
     expression: str,
     factory: t.Dict[str, t.Type[ExpressionFilter]],
     validate: t.Callable[[str], str] = None,
 ) -> ExpressionFilter:
     """Parse and return filter from expression string (factory)."""
-    expr_split = re.split(rf"({'|'.join(OPERATORS)})", expression, maxsplit=1)
+    expr_split = re.split(rf"(?<=\w)({'|'.join(OPERATORS)})", expression, maxsplit=1)
     if len(expr_split) != 3:
         raise ValueError(f"invalid filter expression: {expression}")
     field, op, value = expr_split
+    # TODO consider to enable shorthands based on factories if no validator passed
     field = validate(field) if validate else field
-    filter_cls: t.Type[ExpressionFilter] = StringFilter
+    filter_cls: t.Optional[t.Type[ExpressionFilter]] = None
     for k, filter_cls in factory.items():
         if field == k or k.endswith("*") and field.startswith(k[:-1]):
             break
-    return filter_cls(field, op, value)
+    return (filter_cls or StringFilter)(field, op, value)
```

## fw_utils/formatters.py

```diff
@@ -63,15 +63,15 @@
             decimals = 0 if round(quotient) >= 10 or not round(remainder, 1) else 1
             parts.append(f"{quotient + remainder:.{decimals}f}{unit}")
         elif quotient >= 1:
             parts.append(f"{int(quotient)}{unit}")
     return " ".join(parts)
 
 
-def format_url(
+def format_url(  # noqa: PLR0913
     *,
     scheme: str = "https",
     driver: str = None,
     username: str = None,
     password: str = None,
     host: str = "",
     port: int = None,
```

## Comparing `fw_utils-4.2.9.dist-info/LICENSE` & `fw_utils-4.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_utils-4.2.9.dist-info/METADATA` & `fw_utils-4.3.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-utils
-Version: 4.2.9
+Version: 4.3.0
 Summary: Common Flywheel helper utilities.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-utils
 License: MIT
 Keywords: Flywheel,helper,utility
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_utils-4.2.9.dist-info/RECORD` & `fw_utils-4.3.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 fw_utils/__init__.py,sha256=0toIsVaBlF-X0TBUQjj9fmkIU6HDGJ_MQJzjk4D89oU,1747
 fw_utils/datetime.py,sha256=8KSueLgg0OfqVNTTtqJRZI8mFrkR8aMGUyj0bT89aEg,2914
 fw_utils/dicts.py,sha256=Xh08WlC-cyJuxLsm3mNHI0x8GUfUfMBXgA6vT3mnVKA,3095
 fw_utils/files.py,sha256=Jck1ZRDXkBxXeqMcKxeywPu-SzRnxQyw--WH8J8OEL8,5436
-fw_utils/filters.py,sha256=A96uXh0d0zvAxHhdDy5scaKFfxhiOVEMzztNy8kTDus,8838
-fw_utils/formatters.py,sha256=K4va7zrFj9KZDHEkzcbRlA28ZWDnOBCb8E4XFSXrM6Y,10485
+fw_utils/filters.py,sha256=0KfFGSmwzDxkAaJb3RossMB4O3y248D83xNnQEoxbf0,9250
+fw_utils/formatters.py,sha256=Kb4ae5XLhjX1uNZJHSCLe9KjznhuMzulZ9gkp0S_oeE,10502
 fw_utils/parsers.py,sha256=S0g7fQpudkNq8xz8BgCwgnoLnsqatFUq61PwhpSrNCA,15077
 fw_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_utils/state.py,sha256=wsa1p60kVaoy-wLxMy5XjEmZO_A2CUjRLMgkrhgdVts,4382
 fw_utils/testing.py,sha256=e3qjGfECyiEk3BspMYTW85ZqRozxoDJjZTVu2qBdq3Y,3063
-fw_utils-4.2.9.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
-fw_utils-4.2.9.dist-info/METADATA,sha256=4fj4LQlU-bnMZQRckhKUTwGD90rXFtLkEv41c6-3X38,1922
-fw_utils-4.2.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_utils-4.2.9.dist-info/RECORD,,
+fw_utils-4.3.0.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
+fw_utils-4.3.0.dist-info/METADATA,sha256=NQnMAU7DGJhTmYbt8SM3Ycl-8ENlAb8JxtoI6NCksNo,1922
+fw_utils-4.3.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_utils-4.3.0.dist-info/RECORD,,
```

