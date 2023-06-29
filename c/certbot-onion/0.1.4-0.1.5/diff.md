# Comparing `tmp/certbot-onion-0.1.4.tar.gz` & `tmp/certbot-onion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.4.tar", last modified: Fri May 26 09:07:44 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.5.tar", last modified: Thu Jun 29 12:39:28 2023, max compression
```

## Comparing `certbot-onion-0.1.4.tar` & `certbot-onion-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/src/certbot_onion/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/src/certbot_onion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/src/certbot_onion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.588712 certbot-onion-0.1.5/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.588712 certbot-onion-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/src/certbot_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-29 12:39:18.000000 certbot-onion-0.1.5/src/certbot_onion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:28.592712 certbot-onion-0.1.5/src/certbot_onion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:39:28.000000 certbot-onion-0.1.5/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.4/LICENSE.md` & `certbot-onion-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.4/PKG-INFO` & `certbot-onion-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.4
+Version: 0.1.5
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `certbot-onion-0.1.4/README.md` & `certbot-onion-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.4/pyproject.toml` & `certbot-onion-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "certbot-onion"
-version = "0.1.4"
+version = "0.1.5"
 description = "Certbot authenticator plugin for the onion-csr-01 challenge"
 authors = [
     {name = "Q Misell", email = "q@as207960.net"}
 ]
 license = {text = "MIT"}
 dependencies = [
     "certbot>=2.6.0"
```

### Comparing `certbot-onion-0.1.4/rust/src/lib.rs` & `certbot-onion-0.1.5/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.4/src/certbot_onion/__init__.py` & `certbot-onion-0.1.5/src/certbot_onion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import typing
 import josepy
 import functools
-import base64
 import acme.challenges
 import certbot.errors
 import certbot.interfaces
 import certbot.plugins.common
 import certbot.achallenges
 import certbot_onion._rust
 from certbot.compat import os
@@ -85,19 +84,24 @@
 
     def get_chall_pref(self, domain: str) -> typing.Iterable[typing.Type[acme.challenges.Challenge]]:
         if domain.endswith(".onion"):
             return [OnionCSR01]
         else:
             return []
 
+    @staticmethod
+    def __match_hs(hs_domain: str, chall_domain: str) -> bool:
+        match_domain = ".".join(chall_domain.rsplit(".", 2)[-2:])
+        return hs_domain == match_domain
+
     def perform(self, achalls: typing.List[certbot.achallenges.AnnotatedChallenge]) -> \
             typing.List[OnionCSR01Response]:
         out = []
         for achall in achalls:
-            hs = next(filter(lambda x: x.domain == achall.domain, self.hs), None)
+            hs = next(filter(lambda x: self.__match_hs(x.domain, achall.domain), self.hs), None)
             if not hs:
                 raise certbot.errors.PluginError(f"Unable to find hidden service key for domain {achall.domain}")
 
             csr = certbot_onion._rust.make_csr(hs.private_key, achall.nonce)
             out.append(OnionCSR01Response(csr=bytes(csr)))
 
         return out
```

### Comparing `certbot-onion-0.1.4/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.5/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.4
+Version: 0.1.5
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

