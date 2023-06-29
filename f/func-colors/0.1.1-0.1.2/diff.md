# Comparing `tmp/func_colors-0.1.1.tar.gz` & `tmp/func_colors-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_colors-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "func_colors-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `func_colors-0.1.1.tar` & `func_colors-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-05-29 01:13:16.866088 func_colors-0.1.1/LICENSE
--rw-r--r--   0        0        0      179 2023-05-29 01:57:08.076941 func_colors-0.1.1/func_colors/__init__.py
--rw-r--r--   0        0        0     2297 2023-05-29 01:55:07.549703 func_colors-0.1.1/func_colors/colors.py
--rw-r--r--   0        0        0      323 2023-05-29 01:23:04.065695 func_colors-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 func_colors-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-06-29 14:09:50.762378 func_colors-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0      179 2023-06-29 14:16:38.042670 func_colors-0.1.2/func_colors/__init__.py
+-rwxr-xr-x   0        0        0     2431 2023-06-29 14:18:09.200541 func_colors-0.1.2/func_colors/colors.py
+-rwxr-xr-x   0        0        0      323 2023-06-29 14:20:39.709461 func_colors-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 func_colors-0.1.2/PKG-INFO
```

### Comparing `func_colors-0.1.1/LICENSE` & `func_colors-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `func_colors-0.1.1/func_colors/colors.py` & `func_colors-0.1.2/func_colors/colors.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 
 
 class Code(Enum):
     def __init__(self, code, kind):
         self.code = code
         self.kind = kind
 
-    red = '\033[1;31m', Kind.COLOR
-    green = '\033[1;32m', Kind.COLOR
-    yellow = '\033[1;33m', Kind.COLOR
-    blue = '\033[1;34m', Kind.COLOR
-    magenta = '\033[1;35m', Kind.COLOR
-    cyan = '\033[1;36m', Kind.COLOR
-    reset = '\033[0m', Kind.RESET
+    red = "\033[1;31m", Kind.COLOR
+    green = "\033[1;32m", Kind.COLOR
+    yellow = "\033[1;33m", Kind.COLOR
+    blue = "\033[1;34m", Kind.COLOR
+    magenta = "\033[1;35m", Kind.COLOR
+    cyan = "\033[1;36m", Kind.COLOR
+    reset = "\033[0m", Kind.RESET
 
 
 class ColoredString:
     def __init__(self, color):
         self.color = color
         self.values = []
 
     def __str__(self, depth=0):
         self_code = Code[self.color].code
         result = self_code
         total_values = len(self.values)
 
         for i in range(total_values):
             value = self.values[i]
-            next_value = self.values[i+1] if i+1 < total_values else None
+            next_value = self.values[i + 1] if i + 1 < total_values else None
             value_is_colored_string = isinstance(value, ColoredString)
 
             if value_is_colored_string:
-                result += value.__str__(depth=depth+1)
+                result += value.__str__(depth=depth + 1)
             else:
                 result += str(value)
 
-            if (
-                next_value
-                and value_is_colored_string
-                and isinstance(next_value, str)
-            ):
+            if next_value and value_is_colored_string and isinstance(next_value, str):
                 result += self_code
 
         if depth == 0:
             result += Code.reset.code
 
         return result
 
@@ -80,13 +76,17 @@
             self.context.colored_string.values.append(value)
 
         return self.context.colored_string
 
 
 class ColorContext:
     def __init__(self):
-        self._define_color_methods()
+        self.__define_default_color_methods()
         self.colored_string = None
 
-    def _define_color_methods(self):
+    def __define_default_color_methods(self):
         for code in filter(lambda c: c.kind == Kind.COLOR, Code):
             self.__setattr__(code.name, ColorMethod(self, code.name))
+
+    def define_color_methods(self, methods):
+        for method_name, method_code in methods:
+            self.__setattr__(method_name, ColorMethod(self, method_code.name))
```

