# Comparing `tmp/databricks_session-0.2.1.tar.gz` & `tmp/databricks_session-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_session-0.2.1.tar", max compression
+gzip compressed data, was "databricks_session-0.2.2.tar", max compression
```

## Comparing `databricks_session-0.2.1.tar` & `databricks_session-0.2.2.tar`

### file list

```diff
@@ -1,82 +1,7 @@
--rw-r--r--   0        0        0      134 2023-06-27 20:27:02.007908 databricks_session-0.2.1/.git/FETCH_HEAD
--rw-r--r--   0        0        0       21 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/HEAD
--rw-r--r--   0        0        0      423 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/config
--rwxr-xr-x   0        0        0       73 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/description
--rwxr-xr-x   0        0        0      478 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     2308 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0        0        0     3650 2023-06-27 20:27:01.431903 databricks_session-0.2.1/.git/hooks/update.sample
--rw-r--r--   0        0        0     2156 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/index
--rwxr-xr-x   0        0        0      240 2023-06-27 20:27:01.427903 databricks_session-0.2.1/.git/info/exclude
--rw-r--r--   0        0        0      217 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/logs/HEAD
--rw-r--r--   0        0        0      226 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      336 2023-06-27 20:27:02.007908 databricks_session-0.2.1/.git/logs/refs/remotes/origin/main
--rw-r--r--   0        0        0      322 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/03/4e848032092eaf8ef96eac731b6ed5961987f3
--rw-r--r--   0        0        0       83 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/0c/8c3816362e4f4b5cbb587dbb20ba7e0f2bdc47
--rw-r--r--   0        0        0       82 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/24/eab5e15c1b0ca711315422777797afa4386411
--rw-r--r--   0        0        0    57327 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/2f/70bb779cf5d44a19ccb07a3b1e3593a7a87e3a
--rw-r--r--   0        0        0      672 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/33/0835805685f967c0d7ff4a40fc73a8962827e2
--rw-r--r--   0        0        0       38 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/3c/ed3581bb601ae91b1e1da4b8f4f520855a065e
--rw-r--r--   0        0        0     1593 2023-06-27 20:27:01.967908 databricks_session-0.2.1/.git/objects/4d/d50be6579f9d92bfc833753ebea2be0f55a318
--rw-r--r--   0        0        0       51 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/4e/61089cbf580ed30b0586c7e622b08a5ac753d3
--rw-r--r--   0        0        0      122 2023-06-27 20:27:01.967908 databricks_session-0.2.1/.git/objects/55/cdf5b85f28092a298195817ef00a782066f584
--rw-r--r--   0        0        0     3943 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/59/65e4e4ee69db5fb6c656fe852e6b2782b67390
--rw-r--r--   0        0        0      439 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/71/6ce33c6ad0f16ee739bf9061118917ddf80438
--rw-r--r--   0        0        0       41 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/71/7ab457193f390f8fe9648f29ede3e4d3cc42d9
--rw-r--r--   0        0        0     2152 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/75/938926bb080e7cf3a98bc77e593682d095d79f
--rw-r--r--   0        0        0      266 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/81/5d493fcb83a95d2b71f156112efd48767fa1d8
--rw-r--r--   0        0        0      133 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/89/248219c5d8ad04193730b7ce08ac83c2ee4063
--rw-r--r--   0        0        0     1395 2023-06-27 20:27:01.967908 databricks_session-0.2.1/.git/objects/8f/6ade8a7241926217bc3e7b226fb9bff6ad7366
--rw-r--r--   0        0        0      665 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/94/eacce9677d11bbd9dfba2f044adb38bb447845
--rw-r--r--   0        0        0       26 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/bb/87656e2e4cb6e1c10750b8bc02aef5600bf899
--rw-r--r--   0        0        0     1298 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/d1/8fc82f1e383ba7d1f9b2a32a438c52c0cdccee
--rw-r--r--   0        0        0     1572 2023-06-27 20:27:01.967908 databricks_session-0.2.1/.git/objects/d1/9e2c2c707e5abd11a270fa04a60c14414750d7
--rw-r--r--   0        0        0      238 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/d7/c817f211ea631a218910207a18eae497944cc6
--rw-r--r--   0        0        0       57 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/da/a158c7122740757e5df842c5d7e962101c51ab
--rw-r--r--   0        0        0     1300 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/df/a3773293275701141674b565033e920e2c27f5
--rw-r--r--   0        0        0      559 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/e5/970a9a8c97310240e7ceb0ad12de128ffb3eb7
--rw-r--r--   0        0        0       15 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0      824 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/ec/3df8fa8a0cb0012ea41ad9e7ccc40a3caa5195
--rw-r--r--   0        0        0      106 2023-06-27 20:27:01.975908 databricks_session-0.2.1/.git/objects/ee/2b78177e5cba9615784b822f28263481866add
--rw-r--r--   0        0        0      869 2023-06-27 20:27:01.967908 databricks_session-0.2.1/.git/objects/f3/b6cff04f053b938b2380803d8e81744fb01f8d
--rw-r--r--   0        0        0      115 2023-06-27 20:27:02.003908 databricks_session-0.2.1/.git/objects/f4/b85638b562e49c8b27afb38259afba5b5a6691
--rw-r--r--   0        0        0       56 2023-06-27 20:27:01.963908 databricks_session-0.2.1/.git/objects/fc/e262124261545357747b4e5682f26a123a81bb
--rw-r--r--   0        0        0       41 2023-06-27 20:27:02.023909 databricks_session-0.2.1/.git/refs/heads/main
--rw-r--r--   0        0        0       41 2023-06-27 20:27:02.007908 databricks_session-0.2.1/.git/refs/remotes/origin/main
--rw-r--r--   0        0        0       41 2023-06-27 20:27:01.947908 databricks_session-0.2.1/.git/shallow
--rw-r--r--   0        0        0       44 2023-06-27 20:27:02.019909 databricks_session-0.2.1/.gitcommit
--rw-r--r--   0        0        0     1665 2023-06-27 20:27:02.019909 databricks_session-0.2.1/.github/workflows/python-cd.yml
--rw-r--r--   0        0        0     3284 2023-06-27 20:27:02.019909 databricks_session-0.2.1/.github/workflows/python-ci.yml
--rw-r--r--   0        0        0     3127 2023-06-27 20:27:02.019909 databricks_session-0.2.1/.gitignore
--rw-r--r--   0        0        0      181 2023-06-27 20:27:02.019909 databricks_session-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0     5336 2023-06-27 20:27:02.019909 databricks_session-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     4406 2023-06-27 20:27:02.019909 databricks_session-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     9085 2023-06-27 20:27:02.019909 databricks_session-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1083 2023-06-27 20:27:02.019909 databricks_session-0.2.1/LICENSE
--rw-r--r--   0        0        0       10 2023-06-27 20:27:02.019909 databricks_session-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0      510 2023-06-27 20:27:02.019909 databricks_session-0.2.1/Makefile
--rw-r--r--   0        0        0     1186 2023-06-27 20:27:02.019909 databricks_session-0.2.1/README.md
--rw-r--r--   0        0        0      619 2023-06-27 20:27:02.019909 databricks_session-0.2.1/SECURITY.md
--rw-r--r--   0        0        0     3798 2023-06-27 20:27:02.019909 databricks_session-0.2.1/databricks_session.py
--rw-r--r--   0        0        0      203 2023-06-27 20:27:02.019909 databricks_session-0.2.1/environment.yml
--rw-r--r--   0        0        0      551 2023-06-27 20:27:02.019909 databricks_session-0.2.1/it.py
--rw-r--r--   0        0        0      105 2023-06-27 20:27:02.019909 databricks_session-0.2.1/main.py
--rw-r--r--   0        0        0       25 2023-06-27 20:27:02.019909 databricks_session-0.2.1/package.json
--rw-r--r--   0        0        0        0 2023-06-27 20:27:02.019909 databricks_session-0.2.1/pip.conf
--rw-r--r--   0        0        0   167449 2023-06-27 20:27:02.023909 databricks_session-0.2.1/poetry.lock
--rw-r--r--   0        0        0      716 2023-06-27 20:27:02.023909 databricks_session-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      120 2023-06-27 20:27:02.023909 databricks_session-0.2.1/requirements.txt
--rw-r--r--   0        0        0       66 2023-06-27 20:27:02.023909 databricks_session-0.2.1/setup.cfg
--rw-r--r--   0        0        0     3145 2023-06-27 20:27:02.023909 databricks_session-0.2.1/setup.py
--rw-r--r--   0        0        0       22 2023-06-27 20:27:02.023909 databricks_session-0.2.1/version.py
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 databricks_session-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 06:37:45.542819 databricks_session-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1186 2023-06-29 06:37:45.542819 databricks_session-0.2.2/README.md
+-rw-r--r--   0        0        0       87 2023-06-29 06:37:45.666819 databricks_session-0.2.2/main.py
+-rw-r--r--   0        0        0      719 2023-06-29 06:37:45.666819 databricks_session-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3145 2023-06-29 06:37:45.666819 databricks_session-0.2.2/setup.py
+-rw-r--r--   0        0        0       22 2023-06-29 06:37:45.666819 databricks_session-0.2.2/version.py
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 databricks_session-0.2.2/PKG-INFO
```

### Comparing `databricks_session-0.2.1/LICENSE` & `databricks_session-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_session-0.2.1/README.md` & `databricks_session-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_session-0.2.1/pyproject.toml` & `databricks_session-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "databricks-session"
-version = "0.2.1"
+version = "0.2.2"
 description = "A simple util to get a spark and mlflow session objects from an .env file"
 authors = ["Carlos Escobar <carlosdavidescobar@gmai.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "*"}]
+packages = [{include = "*.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mlflow = "^2.4.1"
 databricks-connect = "^13.1.0"
 pydantic = "^1.10.9"
 python-dotenv = "^1.0.0"
```

### Comparing `databricks_session-0.2.1/setup.py` & `databricks_session-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `databricks_session-0.2.1/PKG-INFO` & `databricks_session-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-session
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple util to get a spark and mlflow session objects from an .env file
 License: MIT
 Author: Carlos Escobar
 Author-email: carlosdavidescobar@gmai.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

