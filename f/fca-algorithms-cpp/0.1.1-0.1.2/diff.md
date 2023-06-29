# Comparing `tmp/fca_algorithms_cpp-0.1.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/fca_algorithms_cpp-0.1.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 78037 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   163328 b- defN 23-Jun-29 11:15 fca_algorithms_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1065 b- defN 23-Jun-29 11:15 fca_algorithms_cpp-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2323 b- defN 23-Jun-29 11:15 fca_algorithms_cpp-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-29 11:15 fca_algorithms_cpp-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-29 11:15 fca_algorithms_cpp-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      545 b- defN 23-Jun-29 11:15 fca_algorithms_cpp-0.1.1.dist-info/RECORD
-6 files, 167387 bytes uncompressed, 77043 bytes compressed:  54.0%
+Zip file size: 78083 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   163328 b- defN 23-Jun-29 13:31 fca_algorithms_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1065 b- defN 23-Jun-29 13:31 fca_algorithms_cpp-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2459 b- defN 23-Jun-29 13:31 fca_algorithms_cpp-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-29 13:31 fca_algorithms_cpp-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-29 13:31 fca_algorithms_cpp-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      545 b- defN 23-Jun-29 13:31 fca_algorithms_cpp-0.1.2.dist-info/RECORD
+6 files, 167523 bytes uncompressed, 77089 bytes compressed:  54.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: fca_algorithms_cpp.pypy39-pp73-win_amd64.pyd
 Comment: 
 
-Filename: fca_algorithms_cpp-0.1.1.dist-info/LICENSE
+Filename: fca_algorithms_cpp-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: fca_algorithms_cpp-0.1.1.dist-info/METADATA
+Filename: fca_algorithms_cpp-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: fca_algorithms_cpp-0.1.1.dist-info/WHEEL
+Filename: fca_algorithms_cpp-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: fca_algorithms_cpp-0.1.1.dist-info/top_level.txt
+Filename: fca_algorithms_cpp-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fca_algorithms_cpp-0.1.1.dist-info/RECORD
+Filename: fca_algorithms_cpp-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fca_algorithms_cpp-0.1.1.dist-info/LICENSE` & `fca_algorithms_cpp-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fca_algorithms_cpp-0.1.1.dist-info/METADATA` & `fca_algorithms_cpp-0.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: fca-algorithms-cpp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cpp implementation of the lib fca_algorithms
 Home-page: https://gitlab.com/Lwr/fca_algorithms_cpp
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: MIT
 Classifier: Programming Language :: C++
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pybind11 (>=2.10.4)
 
 # FCA algorithms C++ Implementation
 
 This projects is the version of the [fca_algorithms](https://pypi.org/project/fca-algorithms/0.2.4/) PyPi module implemented in C++.
 
 ## Purpose
 
@@ -21,17 +22,17 @@
 
 So far, the only ported algorithm is inclose.
 
 ## Performance
 
 Unsurprisingly, this implementation runs much fuster than the one done totally in python. In the following, we can see an example of the difference in runtimes using `get_concepts` method from the `Concept` class of both `fca_algorithms<=0.2.x` and `fca_algorithms_cpp`.
 
-![test1](/imgs/img_test_1.png)
+![test1](https://gitlab.com/Lwr/fca_algorithms_cpp/raw/main/imgs/img_test_1.png)
 
-![test2](/imgs/img_test_2.png)
+![test2](https://gitlab.com/Lwr/fca_algorithms_cpp/raw/main/imgs/img_test_2.png)
 
 After running these tests, I decided to use this library in the [Python one](https://pypi.org/project/fca-algorithms/) so that at least the code can take advantage of the faster implementation of `inclose`.
 
 ## Future Work
 
 As said before, the ideal would be to fully implement the CPU-intensive algorithms in C++ and maintain the Python interface. Considering this, the goal would be to eventually replace the python code with full C++ one.
```

