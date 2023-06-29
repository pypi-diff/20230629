# Comparing `tmp/rfernet-0.2.0.tar.gz` & `tmp/rfernet-0.3.0.tar.gz`

## Comparing `rfernet-0.2.0.tar` & `rfernet-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 rfernet-0.2.0/Cargo.toml
--rw-r--r--   0     1001      121     1070 2021-08-09 14:56:55.000000 rfernet-0.2.0/LICENSE
--rw-r--r--   0     1001      121     3090 2021-08-09 14:56:55.000000 rfernet-0.2.0/README.md
--rw-r--r--   0     1001      121      522 2021-08-09 14:56:55.000000 rfernet-0.2.0/pyproject.toml
--rw-r--r--   0     1001      121        8 2021-08-09 14:56:55.000000 rfernet-0.2.0/rust-toolchain
--rw-r--r--   0     1001      121      105 2021-08-09 14:56:55.000000 rfernet-0.2.0/src/exc.rs
--rw-r--r--   0     1001      121     2590 2021-08-09 14:56:55.000000 rfernet-0.2.0/src/lib.rs
--rw-r--r--   0        0        0     4011 1970-01-01 00:00:00.000000 rfernet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 rfernet-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     1070 2023-06-29 11:21:09.000000 rfernet-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     3090 2023-06-29 11:21:09.000000 rfernet-0.3.0/README.md
+-rw-r--r--   0     1001      123     1217 2023-06-29 11:21:09.000000 rfernet-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123        8 2023-06-29 11:21:09.000000 rfernet-0.3.0/rust-toolchain
+-rw-r--r--   0     1001      123      105 2023-06-29 11:21:09.000000 rfernet-0.3.0/src/exc.rs
+-rw-r--r--   0     1001      123     2590 2023-06-29 11:21:09.000000 rfernet-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    11138 2023-06-29 11:21:09.000000 rfernet-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     3434 1970-01-01 00:00:00.000000 rfernet-0.3.0/PKG-INFO
```

### Comparing `rfernet-0.2.0/LICENSE` & `rfernet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfernet-0.2.0/README.md` & `rfernet-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rfernet-0.2.0/src/lib.rs` & `rfernet-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rfernet-0.2.0/PKG-INFO` & `rfernet-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 Metadata-Version: 2.1
 Name: rfernet
-Version: 0.2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Rust
-Classifier: Typing :: Typed
+Version: 0.3.0
+License-File: LICENSE
 Summary: Fast Fernet bindings for Python
 Keywords: fast,fernet
 Author: Aviram Hassan <aviramyhassan@gmail.com>
 Author-email: Aviram Hassan <aviramyhassan@gmail.com>
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rfernet
 Python extension for Fernet encryption/decryption, faster than other alternatives.
 This library uses the rust library `fernet-rs` https://github.com/mozilla-services/fernet-rs.
 
 CI & Building wheels copied from `cryptography` and `orjson`
```

