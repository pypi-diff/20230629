# Comparing `tmp/github_fine_grained_token_client-1.0.2.tar.gz` & `tmp/github_fine_grained_token_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_fine_grained_token_client-1.0.2.tar", max compression
+gzip compressed data, was "github_fine_grained_token_client-1.0.3.tar", max compression
```

## Comparing `github_fine_grained_token_client-1.0.2.tar` & `github_fine_grained_token_client-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-04-03 21:57:00.219366 github_fine_grained_token_client-1.0.2/LICENSE
--rw-r--r--   0        0        0     2920 2023-04-03 21:57:00.219366 github_fine_grained_token_client-1.0.2/README.md
--rw-r--r--   0        0        0     2256 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/__init__.py
--rw-r--r--   0        0        0      529 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/abstract_http_session.py
--rw-r--r--   0        0        0    10737 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/app.py
--rw-r--r--   0        0        0    37322 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/asynchronous_client.py
--rw-r--r--   0        0        0     9393 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/cli.py
--rw-r--r--   0        0        0     2492 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/common.py
--rw-r--r--   0        0        0     2146 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/credentials.py
--rw-r--r--   0        0        0      441 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/dev.py
--rw-r--r--   0        0        0     7054 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/permissions.py
--rw-r--r--   0        0        0     3927 2023-04-03 21:57:00.220366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/persisting_http_session.py
--rw-r--r--   0        0        0     2817 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/two_factor_authentication.py
--rw-r--r--   0        0        0        0 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/__init__.py
--rw-r--r--   0        0        0      458 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/asyncio.py
--rw-r--r--   0        0        0      677 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/bs4.py
--rw-r--r--   0        0        0      568 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/sequences.py
--rw-r--r--   0        0        0     1564 2023-04-03 21:57:00.221366 github_fine_grained_token_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 github_fine_grained_token_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 19:03:44.061691 github_fine_grained_token_client-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2920 2023-06-29 19:03:44.061691 github_fine_grained_token_client-1.0.3/README.md
+-rw-r--r--   0        0        0     2256 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/abstract_http_session.py
+-rw-r--r--   0        0        0    10737 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/app.py
+-rw-r--r--   0        0        0    36910 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/asynchronous_client.py
+-rw-r--r--   0        0        0     9393 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/cli.py
+-rw-r--r--   0        0        0     2492 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/common.py
+-rw-r--r--   0        0        0     2146 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/credentials.py
+-rw-r--r--   0        0        0      441 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/dev.py
+-rw-r--r--   0        0        0     7054 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/permissions.py
+-rw-r--r--   0        0        0     3927 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/persisting_http_session.py
+-rw-r--r--   0        0        0     2817 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/two_factor_authentication.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:03:44.085691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/asyncio.py
+-rw-r--r--   0        0        0      677 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/bs4.py
+-rw-r--r--   0        0        0      568 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/sequences.py
+-rw-r--r--   0        0        0     1564 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 github_fine_grained_token_client-1.0.3/PKG-INFO
```

### Comparing `github_fine_grained_token_client-1.0.2/LICENSE` & `github_fine_grained_token_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/README.md` & `github_fine_grained_token_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/__init__.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/__init__.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/abstract_http_session.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/abstract_http_session.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/app.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/app.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/asynchronous_client.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/asynchronous_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,16 +462,16 @@
         Create a new fine-grained token on GitHub.
 
         Args:
             name: Name of the token to create.
             expires: Expiration date of the token to create. GitHub currently
                 only allows expiration dates up to 1 year in the future.
             description: Description of the token to create.
-            resource_owner: Owner of the token to create. Defaults to whatever
-                GitHub selects by default (always logged-in user I guess).
+            resource_owner: Owner of the token to create. Defaults to username
+                used to log in.
             scope: The token's desired scope.
             permissions: Permissions the token should have, as a mapping from
                 permissions to the desired value (read or write = read+write).
 
         Returns:
             The created token.
         """
@@ -479,22 +479,16 @@
         expires_date = (
             date.today() + expires
             if isinstance(expires, timedelta)
             else expires
         )
         if permissions is None:
             permissions = {}
-        if (
-            isinstance(scope, SelectRepositories)
-            and resource_owner != self.credentials.username
-        ):
-            raise ValueError(
-                "select repositories can only be specified for user-owned "
-                "tokens"
-            )
+        if resource_owner is None:
+            resource_owner = self.credentials.username
         # /normalize and validate args
         async with self._auth_handling_get(
             "/settings/personal-access-tokens/new"
         ) as response:
             html = await self._get_parsed_response_html(response)
         # get dynamic form data
         authenticity_token = self._get_authenticity_token(
@@ -508,35 +502,30 @@
         elif isinstance(scope, AllRepositories):
             install_target = "all"
             repository_ids = []
         elif isinstance(scope, SelectRepositories):
             install_target = "selected"
             # fetch repo IDs given names
             repository_ids = [
-                await self._get_repository_id(
-                    self.credentials.username,  # TODO configurable
-                    repository_name,
-                )
+                await self._get_repository_id(resource_owner, repository_name)
                 for repository_name in scope.names
             ]
         else:
             raise ValueError(f"invalid scope {scope}")
         async with self._auth_handling_post(
             "/settings/personal-access-tokens",
             data={
                 "authenticity_token": authenticity_token,
                 "user_programmatic_access[name]": name,
                 "user_programmatic_access[default_expires_at]": "custom",
                 "user_programmatic_access[custom_expires_at]": (
                     expires_date.strftime("%Y-%m-%d")
                 ),
                 "user_programmatic_access[description]": description,
-                "target_name": self.credentials.username
-                if resource_owner is None
-                else resource_owner,
+                "target_name": resource_owner,
                 "install_target": install_target,
                 "repository_ids[]": repository_ids,
                 **{
                     "integration[default_permissions]"
                     f"[{permission_key.value}]": (
                         permissions.get(
                             permission_key, PermissionValue.NONE
```

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/cli.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/cli.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/common.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/common.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/credentials.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/credentials.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/permissions.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/permissions.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/persisting_http_session.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/persisting_http_session.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/two_factor_authentication.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/two_factor_authentication.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/bs4.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/bs4.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/github_fine_grained_token_client/utils/sequences.py` & `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/sequences.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.2/pyproject.toml` & `github_fine_grained_token_client-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "github-fine-grained-token-client"
-version = "1.0.2"
+version = "1.0.3"
 description = "Library and CLI tool for creating fine-grained GitHub tokens"
 authors = ["smheidrich <smheidrich@weltenfunktion.de>"]
 readme = "README.md"
 homepage = "https://smheidrich.gitlab.io/github-fine-grained-token-client/"
 repository = "https://gitlab.com/smheidrich/github-fine-grained-token-client"
 documentation = "https://smheidrich.gitlab.io/github-fine-grained-token-client/"
```

### Comparing `github_fine_grained_token_client-1.0.2/PKG-INFO` & `github_fine_grained_token_client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-fine-grained-token-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library and CLI tool for creating fine-grained GitHub tokens
 Home-page: https://smheidrich.gitlab.io/github-fine-grained-token-client/
 Author: smheidrich
 Author-email: smheidrich@weltenfunktion.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

