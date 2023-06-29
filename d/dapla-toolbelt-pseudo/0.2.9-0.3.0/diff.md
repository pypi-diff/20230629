# Comparing `tmp/dapla_toolbelt_pseudo-0.2.9.tar.gz` & `tmp/dapla_toolbelt_pseudo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-0.2.9.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-0.3.0.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-0.2.9.tar` & `dapla_toolbelt_pseudo-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-06-07 08:47:01.077868 dapla_toolbelt_pseudo-0.2.9/LICENSE
--rw-r--r--   0        0        0     4899 2023-06-07 08:47:01.077868 dapla_toolbelt_pseudo-0.2.9/README.md
--rw-r--r--   0        0        0     2460 2023-06-07 08:47:15.313956 dapla_toolbelt_pseudo-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1214 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      833 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      455 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0      888 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      377 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     6617 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/builder.py
--rw-r--r--   0        0        0    11256 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     5248 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/models.py
--rw-r--r--   0        0        0    12949 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/ops.py
--rw-r--r--   0        0        0      668 2023-06-07 08:47:01.081868 dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.9/setup.py
--rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-29 17:16:03.878216 dapla_toolbelt_pseudo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4899 2023-06-29 17:16:03.878216 dapla_toolbelt_pseudo-0.3.0/README.md
+-rw-r--r--   0        0        0     2460 2023-06-29 17:16:15.194205 dapla_toolbelt_pseudo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1214 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      833 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      455 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0      888 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      377 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     6631 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/builder.py
+-rw-r--r--   0        0        0    12048 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     5248 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/models.py
+-rw-r--r--   0        0        0    13585 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/ops.py
+-rw-r--r--   0        0        0      668 2023-06-29 17:16:03.882216 dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.3.0/setup.py
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-0.3.0/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/LICENSE` & `dapla_toolbelt_pseudo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/README.md` & `dapla_toolbelt_pseudo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/pyproject.toml` & `dapla_toolbelt_pseudo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "0.2.9"
+version = "0.3.0"
 description = "Pseudonymization extensions for Dapla Toolbelt"
 authors = ["Team Skyinfrastruktur <dapla@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/builder.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,10 +153,10 @@
             keysets=KeyWrapper(pseudo_func.key).keyset_list(),
         ),
         target_content_type=Mimetypes.JSON,
         target_uri=None,
         compression=None,
     )
     response: requests.Response = _client().pseudonymize(
-        pseudonymize_request, _dataframe_to_json(dataframe), stream=True
+        pseudonymize_request, _dataframe_to_json(dataframe), timeout=None, stream=True
     )
     return PseudonymizationResult(dataframe=pd.json_normalize(response.json()))
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def __auth_token(self) -> str:
         return str(AuthClient.fetch_personal_token()) if self.static_auth_token is None else str(self.static_auth_token)
 
     def pseudonymize(
         self,
         pseudonymize_request: PseudonymizeFileRequest,
         data: _BinaryFileDecl,
+        timeout: t.Optional[int],
         stream: bool = False,
         name: t.Optional[str] = None,
     ) -> requests.Response:
         """Pseudonymize data from a file-like object.
 
         Choose between streaming the result back, or storing it as a file in GCS (by providing a `targetUri`).
 
@@ -62,24 +63,27 @@
         Pseudo rules will most times refer to crypto keys. You can provide your own keys to use (via the `keysets`
         param) or use one of the predefined keys: `ssb-common-key-1` or `ssb-common-key-2`.
 
         See https://dapla-pseudo-service.staging-bip-app.ssb.no/api-docs/redoc#tag/Pseudo-operations/operation/pseudonymizeFile
 
         :param pseudonymize_request: the request to send to Dapla Pseudo Service
         :param data: file handle that should be pseudonymized
+        :param timeout: connection and read timeout, see
+            https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
         :param stream: set to true if the results should be chunked into pieces, e.g. if you operate on large files.
         :param name: optional name for logging purposes
         :return: pseudonymized data
         """
         return self._post_to_pseudo_service(
             self.PSEUDONYMIZE_FILE_ENDPOINT,
             pseudonymize_request,
             data,
             self._extract_name(data, pseudonymize_request.target_content_type, name),
             pseudonymize_request.target_content_type,
+            timeout,
             stream,
         )
 
     def _extract_name(self, data: t.BinaryIO, content_type: Mimetypes, name: t.Optional[str]) -> str:
         if name is None:
             try:
                 name = data.name
@@ -92,15 +96,19 @@
 
         if "/" in name:
             name = name.split("/")[-1]  # Pseudo service expects a file name, not a path
 
         return name
 
     def depseudonymize_file(
-        self, depseudonymize_request: DepseudonymizeFileRequest, file_path: str, stream: bool = False
+        self,
+        depseudonymize_request: DepseudonymizeFileRequest,
+        file_path: str,
+        timeout: t.Optional[int],
+        stream: bool = False,
     ) -> requests.Response:
         """Depseudonymize a file (JSON or CSV - or a zip with potentially multiple such files) by uploading the file.
 
         Notice that only certain whitelisted users can depseudonymize data.
 
         Choose between streaming the result back, or storing it as a file in GCS (by providing a `targetUri`).
 
@@ -119,21 +127,27 @@
         Pseudo rules will most times refer to crypto keys. You can provide your own keys to use (via the `keysets`
         param) or use one of the predefined keys: `ssb-common-key-1` or `ssb-common-key-2`.
 
         See https://dapla-pseudo-service.staging-bip-app.ssb.no/api-docs/redoc#tag/Pseudo-operations/operation/depseudonymizeFile
 
         :param request_json: the request JSON to send to Dapla Pseudo Service
         :param file_path: path to a local file that should be depseudonymized
+        :param timeout: connection and read timeout, see
+            https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
         :param stream: set to true if the results should be chunked into pieces, e.g. if you operate on large files.
         :return: depseudonymized data
         """
-        return self._process_file("depseudonymize", depseudonymize_request, file_path, stream)
+        return self._process_file("depseudonymize", depseudonymize_request, file_path, timeout, stream)
 
     def repseudonymize_file(
-        self, repseudonymize_request: RepseudonymizeFileRequest, file_path: str, stream: bool = False
+        self,
+        repseudonymize_request: RepseudonymizeFileRequest,
+        file_path: str,
+        timeout: t.Optional[int],
+        stream: bool = False,
     ) -> requests.Response:
         """Repseudonymize a file (JSON or CSV - or a zip with potentially multiple such files) by uploading the file.
 
         Repseudonymization is done by first applying depseudonuymization and then pseudonymization to fields of the file.
 
         Choose between streaming the result back, or storing it as a file in GCS (by providing a `targetUri`).
 
@@ -154,30 +168,41 @@
         Pseudo rules will most times refer to crypto keys. You can provide your own keys to use (via the `keysets`
         param) or use one of the predefined keys: `ssb-common-key-1` or `ssb-common-key-2`.
 
         See https://dapla-pseudo-service.staging-bip-app.ssb.no/api-docs/redoc#tag/Pseudo-operations/operation/repseudonymizeFile
 
         :param request_json: the request JSON to send to Dapla Pseudo Service
         :param file_path: path to a local file that should be depseudonymized
+        :param timeout: connection and read timeout, see
+            https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
         :param stream: set to true if the results should be chunked into pieces, e.g. if you operate on large files.
         :return: repseudonymized data
         """
-        return self._process_file("repseudonymize", repseudonymize_request, file_path, stream)
+        return self._process_file("repseudonymize", repseudonymize_request, file_path, timeout, stream)
 
     def _process_file(
-        self, operation: str, request: APIModel, file_path: str, stream: bool = False
+        self, operation: str, request: APIModel, file_path: str, timeout: t.Optional[int], stream: bool = False
     ) -> requests.Response:
         file_name = os.path.basename(file_path).split("/")[-1]
         content_type = Mimetypes(mimetypes.MimeTypes().guess_type(file_path)[0])
 
         with open(file_path, "rb") as f:
-            return self._post_to_pseudo_service(f"{operation}/file", request, f, file_name, content_type, stream)
+            return self._post_to_pseudo_service(
+                f"{operation}/file", request, f, file_name, content_type, timeout, stream
+            )
 
     def _post_to_pseudo_service(
-        self, path: str, request: APIModel, data: t.BinaryIO, name: str, content_type: Mimetypes, stream: bool = False
+        self,
+        path: str,
+        request: APIModel,
+        data: t.BinaryIO,
+        name: str,
+        content_type: Mimetypes,
+        timeout: t.Optional[int],
+        stream: bool = False,
     ) -> requests.Response:
         auth_token = self.__auth_token()
         data_spec: _FileSpecDecl = (name, data, content_type)
         request_spec: _FileSpecDecl = (None, request.to_json(), str(Mimetypes.JSON))
         response = requests.post(
             url=f"{self.pseudo_service_url}/{path}",
             headers={
@@ -185,15 +210,15 @@
                 "Accept-Encoding": "gzip",
             },
             files={
                 "data": data_spec,
                 "request": request_spec,
             },
             stream=stream,
-            timeout=30,  # seconds
+            timeout=timeout,
         )
         response.raise_for_status()
         return response
 
     def export_dataset(self, request_json: str) -> requests.Response:
         """Export a dataset in GCS to CSV or JSON, and optionally depseudonymize the data.
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/models.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/ops.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 
 def pseudonymize(
     dataset: _DatasetDecl,
     fields: t.Optional[t.List[_FieldDecl]] = None,
     sid_fields: t.Optional[t.List[str]] = None,
     key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
+    timeout: t.Optional[int] = None,
     stream: bool = True,
 ) -> requests.Response:
     """Pseudonymize specified fields of a dataset.
 
     The dataset may be supplied as:
         - A local file on disk (string or Path)
         - A file handle (io.BufferedReader)
@@ -78,14 +79,16 @@
             with open("./data/personer.json", 'wb') as f:
                 shutil.copyfileobj(res.raw, f)
 
     :param data: path to file, file handle or dataframe
     :param fields: list of fields that should be pseudonymized
     :param sid_fields: list of fields that should be mapped to stabil ID and pseudonymized
     :param key: either named reference to a "global" key or a keyset json
+    :param timeout: connection and read timeout, see
+        https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
     :param stream: true if the results should be chunked into pieces (use for large data)
     :return: pseudonymized data
     """
     if not fields and not sid_fields:
         raise ValueError("At least one of fields and sid_fields must be specified.")
 
     # Avoid later type errors by making sure we have lists
@@ -124,23 +127,26 @@
         pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()),
         target_content_type=content_type,
         target_uri=None,
         compression=None,
     )
 
     if file_handle is not None:
-        return _client().pseudonymize(pseudonymize_request, file_handle, stream=stream, name=name)
+        return _client().pseudonymize(pseudonymize_request, file_handle, stream=stream, name=name, timeout=timeout)
     else:
-        return _client()._process_file("pseudonymize", pseudonymize_request, str(dataset), stream=stream)
+        return _client()._process_file(
+            "pseudonymize", pseudonymize_request, str(dataset), stream=stream, timeout=timeout
+        )
 
 
 def depseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
     key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
+    timeout: t.Optional[int] = None,
     stream: bool = True,
 ) -> requests.Response:
     """Depseudonymize specified fields of a local file.
 
     This is the inverse operation of "pseudonymize". Special privileges will be required (e.g. only whitelisted users)
     will be allowed to depseudonymize data.
 
@@ -165,35 +171,38 @@
         with depseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:
             with open("./data/personer_deid.json", 'wb') as f:
                 shutil.copyfileobj(res.raw, f)
 
     :param file_path: path to a local file, e.g. ./path/to/data-deid.json. Supported file formats: csv, json
     :param fields: list of fields that should be depseudonymized
     :param key: either named reference to a "global" key or a keyset json
+    :param timeout: connection and read timeout, see
+        https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
     :param stream: true if the results should be chunked into pieces (use for large data)
     :return: depseudonymized data
     """
     content_type = mimetypes.MimeTypes().guess_type(file_path)[0]
     k = KeyWrapper(key)
     rules = _rules_of(fields=fields, sid_fields=[], key=k.key_id)
     req = DepseudonymizeFileRequest(
         pseudo_config=PseudoConfig(rules=rules, keysets=k.keyset_list()),
         target_content_type=content_type,
         target_uri=None,
         compression=None,
     )
 
-    return _client().depseudonymize_file(req, file_path, stream=stream)
+    return _client().depseudonymize_file(req, file_path, stream=stream, timeout=timeout)
 
 
 def repseudonymize(
     file_path: str,
     fields: t.List[_FieldDecl],
     source_key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
     target_key: t.Union[str, PseudoKeyset] = PredefinedKeys.SSB_COMMON_KEY_1,
+    timeout: t.Optional[int] = None,
     stream: bool = True,
 ) -> requests.Response:
     """Repseudonymize specified fields of a local, previously pseudonymized file.
 
     You will need to provide a crypto key for both the source data and a key that should be used for
     re-pseudonymization.
 
@@ -219,14 +228,16 @@
             with open("./data/personer.json", 'wb') as f:
                 shutil.copyfileobj(res.raw, f)
 
     :param file_path: path to a local file, e.g. ./path/to/data.json. Supported file formats: csv, json
     :param fields: list of fields that should be pseudonymized
     :param source_key: either named reference to a "global" key or a keyset json - used for depseudonymization
     :param target_key: either named reference to a "global" key or a keyset json - used for pseudonymization
+    :param timeout: connection and read timeout, see
+        https://requests.readthedocs.io/en/latest/user/advanced/?highlight=timeout#timeouts
     :param stream: true if the results should be chunked into pieces (use for large data)
     :return: repseudonymized data
     """
     content_type = _content_type_of(file_path)
     source_key_wrapper = KeyWrapper(source_key)
     target_key_wrapper = KeyWrapper(target_key)
     source_rules = _rules_of(fields=fields, sid_fields=[], key=source_key_wrapper.key_id)
@@ -235,15 +246,15 @@
         source_pseudo_config=PseudoConfig(rules=source_rules, keysets=source_key_wrapper.keyset_list()),
         target_pseudo_config=PseudoConfig(rules=target_rules, keysets=target_key_wrapper.keyset_list()),
         target_content_type=content_type,
         target_uri=None,
         compression=None,
     )
 
-    return _client().repseudonymize_file(req, file_path, stream=stream)
+    return _client().repseudonymize_file(req, file_path, stream=stream, timeout=timeout)
 
 
 def _client() -> PseudoClient:
     return PseudoClient(
         pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
         auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
     )
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-0.3.0/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-0.2.9/setup.py` & `dapla_toolbelt_pseudo-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pyhumps>=3.8.0,<4.0.0',
  'pylibmagic>=0.2.2,<0.3.0',
  'python-magic>=0.4.27,<0.5.0',
  'types-requests>=2.28.11,<3.0.0']
 
 setup_kwargs = {
     'name': 'dapla-toolbelt-pseudo',
-    'version': '0.2.9',
+    'version': '0.3.0',
     'description': 'Pseudonymization extensions for Dapla Toolbelt',
     'long_description': '# Pseudonymization extensions for Dapla Toolbelt\n\n[![PyPI](https://img.shields.io/pypi/v/dapla-toolbelt-pseudo.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/dapla-toolbelt-pseudo.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/dapla-toolbelt-pseudo)][python version]\n[![License](https://img.shields.io/pypi/l/dapla-toolbelt-pseudo)][license]\n\n[![Tests](https://github.com/statisticsnorway/dapla-toolbelt-pseudo/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[status]: https://pypi.org/project/dapla-toolbelt-pseudo/\n[python version]: https://pypi.org/project/dapla-toolbelt-pseudo\n[tests]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/dapla-toolbelt-pseudo\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nPseudonymize, repseudonymize and depseudonymize data on Dapla.\n\n## Usage\n\nSee the [command-line reference] for details.\n\n### Pseudonymize\n\n```python\nfrom dapla_pseudo import pseudonymize\n\n# Pseudonymize fields in a local file using the default key:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"])\n\n# Pseudonymize fields in a local file, explicitly denoting the key to use:\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n\n# Pseudonymize a local file using a custom key:\nimport json\ncustom_keyset = json.dumps(    {\n    "encryptedKeyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",\n    "keysetInfo": {\n        "primaryKeyId": 1234567890,\n        "keyInfo": [\n            {\n                "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",\n                "status": "ENABLED",\n                "keyId": 1234567890,\n                "outputPrefixType": "TINK",\n            }\n        ],\n    },\n    "kekUri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1",\n})\npseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key=custom_keyset)\n\n# Operate on data in a streaming manner:\nimport shutil\nwith pseudonymize("./data/personer.json", fields=["fnr", "fornavn", "etternavn"], stream=True) as res:\n    with open("./data/personer_deid.json", \'wb\') as f:\n        res.raw.decode_content = True\n        shutil.copyfileobj(res.raw, f)\n\n# Map certain fields to stabil ID\npseudonymize(file_path="./data/personer.json", fields=["fornavn"], sid_fields=["fnr"])\n```\n\n### Repseudonymize\n\n```python\nfrom dapla_pseudo import repseudonymize\n\n# Repseudonymize fields in a local file, denoting source and target keys to use:\nrepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], source_key="ssb-common-key-1", target_key="ssb-common-key-2")\n```\n\n### Depseudonymize\n\n```python\nfrom dapla_pseudo import depseudonymize\n\n# Depseudonymize fields in a local file using the default key:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"])\n\n# Depseudonymize fields in a local file, explicitly denoting the key to use:\ndepseudonymize(file_path="./data/personer_deid.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")\n```\n\n_Note that depseudonymization requires elevated access privileges._\n\n## Requirements\n\n- [Dapla Toolbelt](https://github.com/statisticsnorway/dapla-toolbelt)\n\n## Installation\n\nYou can install _dapla-toolbelt-pseudo_ via [pip] from [PyPI]:\n\n```console\npip install dapla-toolbelt-pseudo\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Pseudonymization extensions for Dapla Toolbelt_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/LICENSE\n[contributor guide]: https://github.com/statisticsnorway/dapla-toolbelt-pseudo/blob/main/CONTRIBUTING.md\n[command-line reference]: https://statisticsnorway.github.io/dapla-toolbelt-pseudo\n',
     'author': 'Team Skyinfrastruktur',
     'author_email': 'dapla@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/dapla-toolbelt-pseudo',
```

### Comparing `dapla_toolbelt_pseudo-0.2.9/PKG-INFO` & `dapla_toolbelt_pseudo-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 0.2.9
+Version: 0.3.0
 Summary: Pseudonymization extensions for Dapla Toolbelt
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Team Skyinfrastruktur
 Author-email: dapla@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

