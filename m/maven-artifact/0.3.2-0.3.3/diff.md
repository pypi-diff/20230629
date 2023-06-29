# Comparing `tmp/maven_artifact-0.3.2.tar.gz` & `tmp/maven_artifact-0.3.3.tar.gz`

## Comparing `maven_artifact-0.3.2.tar` & `maven_artifact-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/.envrc
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/_version.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/dev-requirements.txt
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/.github/workflows/linting.yml
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/.github/workflows/pypi-build-n-publish.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/__init__.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/artifact.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/downloader.py
--rwxr-xr-x   0        0        0     4937 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/main.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/requestor.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/resolver.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/src/maven_artifact/utils.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/tests/integration/maven_artifact/test_downloader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/tests/unit/conftest.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/tests/unit/maven_artifact/test_artifact.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/.gitignore
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/README.md
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 maven_artifact-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/.envrc
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/_version.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/dev-requirements.txt
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/.github/workflows/linting.yml
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/.github/workflows/pypi-build-n-publish.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/artifact.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/downloader.py
+-rwxr-xr-x   0        0        0     4937 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/main.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/requestor.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/resolver.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/src/maven_artifact/utils.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/tests/integration/maven_artifact/test_downloader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/tests/unit/maven_artifact/test_artifact.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/.gitignore
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/README.md
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 maven_artifact-0.3.3/PKG-INFO
```

### Comparing `maven_artifact-0.3.2/.github/dependabot.yml` & `maven_artifact-0.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/.github/workflows/linting.yml` & `maven_artifact-0.3.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/.github/workflows/pypi-build-n-publish.yml` & `maven_artifact-0.3.3/.github/workflows/pypi-build-n-publish.yml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/src/maven_artifact/artifact.py` & `maven_artifact-0.3.3/src/maven_artifact/artifact.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/src/maven_artifact/downloader.py` & `maven_artifact-0.3.3/src/maven_artifact/downloader.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/src/maven_artifact/main.py` & `maven_artifact-0.3.3/src/maven_artifact/main.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/src/maven_artifact/requestor.py` & `maven_artifact-0.3.3/src/maven_artifact/requestor.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         if self.username and self.password:
             token = self.username + ":" + self.password
             headers["Authorization"] = f"Basic {base64.b64encode(token.encode()).decode()}"
         elif Utils.is_base64(self.password):
             headers["Authorization"] = f"Basic {self.password}"
         elif self.token:
-            headers["Authorization"] = f"Bearer {base64.b64encode(self.token.encode()).decode()}"
+            headers["Authorization"] = f"Bearer {self.token}"
 
         try:
             response = getattr(requests, method)(url, headers=headers, **kwargs)
             response.raise_for_status()
             if onSuccess:
                 return onSuccess(response)
             return response
```

### Comparing `maven_artifact-0.3.2/src/maven_artifact/resolver.py` & `maven_artifact-0.3.3/src/maven_artifact/resolver.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/src/maven_artifact/utils.py` & `maven_artifact-0.3.3/src/maven_artifact/utils.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/tests/unit/maven_artifact/test_artifact.py` & `maven_artifact-0.3.3/tests/unit/maven_artifact/test_artifact.py`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/README.md` & `maven_artifact-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/pyproject.toml` & `maven_artifact-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maven_artifact-0.3.2/PKG-INFO` & `maven_artifact-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maven-artifact
-Version: 0.3.2
+Version: 0.3.3
 Summary: Download and resolve maven artifacts
 Author-email: Erlend Hamnaberg <erlend@hamnaberg.net>
 License-Expression: Apache-2.0
 Keywords: artifact,download,maven,mvn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

