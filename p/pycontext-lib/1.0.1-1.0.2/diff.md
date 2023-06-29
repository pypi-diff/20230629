# Comparing `tmp/pycontext-lib-1.0.1.tar.gz` & `tmp/pycontext-lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycontext-lib-1.0.1.tar", last modified: Tue May 30 02:17:31 2023, max compression
+gzip compressed data, was "pycontext-lib-1.0.2.tar", last modified: Thu Jun 29 12:42:08 2023, max compression
```

## Comparing `pycontext-lib-1.0.1.tar` & `pycontext-lib-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.444363 pycontext-lib-1.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-29 17:14:53.000000 pycontext-lib-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1967 2023-05-30 02:17:31.443357 pycontext-lib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-05-29 17:18:43.000000 pycontext-lib-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.419617 pycontext-lib-1.0.1/context/
--rw-rw-rw-   0        0        0     5251 2022-11-23 02:38:19.000000 pycontext-lib-1.0.1/context/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.440218 pycontext-lib-1.0.1/pycontext_lib.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      762 2023-05-30 02:17:17.000000 pycontext-lib-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 02:17:31.445585 pycontext-lib-1.0.1/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 12:42:08.275903 pycontext-lib-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1079 2023-06-29 12:04:38.000000 pycontext-lib-1.0.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1927 2023-06-29 12:42:08.275903 pycontext-lib-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2023-06-29 12:04:38.000000 pycontext-lib-1.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 12:42:08.271903 pycontext-lib-1.0.2/context/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6593 2023-06-29 12:39:23.000000 pycontext-lib-1.0.2/context/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-29 12:42:08.271903 pycontext-lib-1.0.2/pycontext_lib.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1927 2023-06-29 12:42:08.000000 pycontext-lib-1.0.2/pycontext_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      240 2023-06-29 12:42:08.000000 pycontext-lib-1.0.2/pycontext_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-29 12:42:08.000000 pycontext-lib-1.0.2/pycontext_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       84 2023-06-29 12:42:08.000000 pycontext-lib-1.0.2/pycontext_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-06-29 12:42:08.000000 pycontext-lib-1.0.2/pycontext_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      737 2023-06-29 12:41:01.000000 pycontext-lib-1.0.2/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-29 12:42:08.275903 pycontext-lib-1.0.2/setup.cfg
```

### Comparing `pycontext-lib-1.0.1/LICENSE` & `pycontext-lib-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Carl Furtado
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023 Carl Furtado
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `pycontext-lib-1.0.1/PKG-INFO` & `pycontext-lib-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1
-Name: pycontext-lib
-Version: 1.0.1
-Summary: Lots of properties that help with program context!
-Author-email: Carl Furtado <carlzfurtado@gmail.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2023 Carl Furtado
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/User0332/pycontext
-Keywords: context,properties
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyContext
-
-Install it with `pip install pycontext-lib`. Import the `context` library and explore the many context related properties!
+Metadata-Version: 2.1
+Name: pycontext-lib
+Version: 1.0.2
+Summary: Lots of properties that help with program context!
+Author-email: Carl Furtado <carlzfurtado@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2023 Carl Furtado
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/User0332/pycontext
+Keywords: context,properties
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyContext
+
+Install it with `pip install pycontext-lib`. Import the `context` library and explore the many context related properties!
```

### Comparing `pycontext-lib-1.0.1/pycontext_lib.egg-info/PKG-INFO` & `pycontext-lib-1.0.2/pycontext_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1
-Name: pycontext-lib
-Version: 1.0.1
-Summary: Lots of properties that help with program context!
-Author-email: Carl Furtado <carlzfurtado@gmail.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2023 Carl Furtado
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/User0332/pycontext
-Keywords: context,properties
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyContext
-
-Install it with `pip install pycontext-lib`. Import the `context` library and explore the many context related properties!
+Metadata-Version: 2.1
+Name: pycontext-lib
+Version: 1.0.2
+Summary: Lots of properties that help with program context!
+Author-email: Carl Furtado <carlzfurtado@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2023 Carl Furtado
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/User0332/pycontext
+Keywords: context,properties
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyContext
+
+Install it with `pip install pycontext-lib`. Import the `context` library and explore the many context related properties!
```

