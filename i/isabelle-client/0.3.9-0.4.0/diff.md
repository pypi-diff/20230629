# Comparing `tmp/isabelle-client-0.3.9.tar.gz` & `tmp/isabelle_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isabelle-client-0.3.9.tar", max compression
+gzip compressed data, was "isabelle_client-0.4.0.tar", max compression
```

## Comparing `isabelle-client-0.3.9.tar` & `isabelle_client-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle-client-0.3.9/LICENSE
--rw-r--r--   0        0        0     4148 2022-09-29 10:12:35.509720 isabelle-client-0.3.9/README.rst
--rw-r--r--   0        0        0      897 2022-09-29 10:12:35.601741 isabelle-client-0.3.9/isabelle_client/__init__.py
--rw-r--r--   0        0        0     3351 2022-08-24 07:23:02.446777 isabelle-client-0.3.9/isabelle_client/conftest.py
--rw-r--r--   0        0        0    11617 2022-08-24 07:23:02.450778 isabelle-client-0.3.9/isabelle_client/isabelle__client.py
--rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle-client-0.3.9/isabelle_client/py.typed
--rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle-client-0.3.9/isabelle_client/resources/Cygwin-Isabelle.bat
--rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle-client-0.3.9/isabelle_client/resources/example.txt
--rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle-client-0.3.9/isabelle_client/resources/isabelle
--rw-r--r--   0        0        0     5186 2022-08-24 07:23:02.462778 isabelle-client-0.3.9/isabelle_client/socket_communication.py
--rw-r--r--   0        0        0     4339 2022-09-13 13:31:05.953877 isabelle-client-0.3.9/isabelle_client/utils.py
--rw-r--r--   0        0        0     3441 2022-09-29 10:12:35.613743 isabelle-client-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     5004 2022-09-29 10:19:02.882473 isabelle-client-0.3.9/setup.py
--rw-r--r--   0        0        0     5211 2022-09-29 10:19:02.883760 isabelle-client-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4774 2023-05-29 14:48:08.562757 isabelle_client-0.4.0/README.rst
+-rw-r--r--   0        0        0      897 2023-06-29 08:41:16.138251 isabelle_client-0.4.0/isabelle_client/__init__.py
+-rw-r--r--   0        0        0     1862 2023-03-29 15:20:44.432379 isabelle_client-0.4.0/isabelle_client/conftest.py
+-rw-r--r--   0        0        0    11629 2023-06-29 08:41:16.138251 isabelle_client-0.4.0/isabelle_client/isabelle__client.py
+-rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle_client-0.4.0/isabelle_client/py.typed
+-rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle_client-0.4.0/isabelle_client/resources/Cygwin-Isabelle.bat
+-rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle_client-0.4.0/isabelle_client/resources/example.txt
+-rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle_client-0.4.0/isabelle_client/resources/isabelle
+-rw-r--r--   0        0        0     5283 2023-06-29 08:41:16.142251 isabelle_client-0.4.0/isabelle_client/socket_communication.py
+-rw-r--r--   0        0        0     6766 2023-04-29 10:14:23.981789 isabelle_client-0.4.0/isabelle_client/utils.py
+-rw-r--r--   0        0        0     3354 2023-06-29 08:41:16.142251 isabelle_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5840 1970-01-01 00:00:00.000000 isabelle_client-0.4.0/PKG-INFO
```

### Comparing `isabelle-client-0.3.9/LICENSE` & `isabelle_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.9/README.rst` & `isabelle_client-0.4.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|Binder|\ |PyPI version|\ |Anaconda version|\ |CircleCI|\ |Documentation Status|\ |codecov|
+|Binder|\ |PyPI version|\ |Anaconda version|\ |CircleCI|\ |Documentation Status|\ |codecov|\ |DOI|
 
 Python client for Isabelle server
 =================================
 
 ``isabelle-client`` is a TCP client for
 `Isabelle <https://isabelle.in.tum.de>`__ server. For more information
 about the server see part 4 of `the Isabelle system
@@ -31,78 +31,88 @@
 
    docker build -t isabelle-client https://github.com/inpefess/isabelle-client.git
    docker run -it --rm -p 8888:8888 isabelle-client jupyter-lab --ip=0.0.0.0 --port=8888
 
 How to use
 ==========
 
-Follow the `usage
+.. code:: python
+
+   from isabelle_client import get_isabelle_client, start_isabelle_server
+   
+   # start Isabelle server
+   server_info, _ = start_isabelle_server()
+   # create a client object
+   isabelle = get_isabelle_client(server_info)
+   # send a theory file from the current directory to the server
+   response = isabelle.use_theories(
+       theories=["Example"], master_dir=".", watchdog_timeout=0
+   )
+   # shut the server down
+   isabelle.shutdown()
+
+
+For more details, follow the `usage
 example <https://isabelle-client.readthedocs.io/en/latest/usage-example.html#usage-example>`__
 from documentation, run the
 `script <https://github.com/inpefess/isabelle-client/blob/master/examples/example.py>`__,
 or use ``isabelle-client`` from a
 `notebook <https://github.com/inpefess/isabelle-client/blob/master/examples/example.ipynb>`__,
 e.g. with
 `Binder <https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb>`__ (Binder might fail with 'Failed to create temporary user for ...' error which is `well known <https://mybinder-sre.readthedocs.io/en/latest/incident-reports/2018-02-20-jupyterlab-announcement.html>`__ and related neither to ``isabelle-client`` nor to the provided ``Dockerfile``. If that happens, try to run Docker as described in the section above).
 
-How to Contribute
-=================
-
-`Pull requests <https://github.com/inpefess/isabelle-client/pulls>`__
-are welcome. To start:
-
-.. code:: sh
-
-   git clone https://github.com/inpefess/isabelle-client
-   cd isabelle-client
-   # activate python virtual environment with Python 3.7+
-   pip install -U pip
-   pip install -U setuptools wheel poetry
-   poetry install
-   # recommended but not necessary
-   pre-commit install
-
-To check the code quality before creating a pull request, one might run
-the script
-`local-build.sh <https://github.com/inpefess/isabelle-client/blob/master/local-build.sh>`__.
-It locally does nearly the same as the CI pipeline after the PR is
-created.
-
-Reporting issues or problems with the software
-==============================================
-
-Questions and bug reports are welcome on `the
-tracker <https://github.com/inpefess/isabelle-client/issues>`__.
-
 More documentation
 ==================
 
 More documentation can be found
 `here <https://isabelle-client.readthedocs.io/en/latest>`__.
 
-Video example
-=============
+Similar Software
+================
+
+There are Python clients to other interactive theorem provers, for
+example:
+
+* `for Lean
+  <https://github.com/leanprover-community/lean-client-python>`__
+* `for Coq <https://github.com/IBM/pycoq>`__
+* `another one for Coq <https://github.com/ejgallego/pycoq>`__
+
+Modules helping to inetract with Isabelle server from Python are
+parts of the `Proving for Fun
+<https://github.com/maxhaslbeck/proving-contest-backends>`__ project.
+
+There are also clients to Isabelle server in other programming
+languages, e.g. `this one in Rust
+<https://lib.rs/crates/isabelle-client>`__.
 
-.. image:: https://isabelle-client.readthedocs.io/en/latest/_images/tty.gif
-	   
 How to cite
 ===========
 
-If you’re writing a research paper, you can cite Isabelle client
+If you’re writing a research paper, you can cite the Isabelle client
 using the `following DOI
 <https://doi.org/10.1007/978-3-031-16681-5_24>`__. You can also cite
-Isabelle 2021 (and the earlier version of the client) with `this
-DOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.
+Isabelle 2021 (and the earlier version of the client) with `this DOI
+<https://doi.org/10.1007/978-3-030-81097-9_20>`__. There also is a
+somewhat more complete (but unpublished) `pre-print
+<https://arxiv.org/abs/2212.11173>`__.
+
+How to Contribute
+=================
+
+Please follow `the contribution guide <https://isabelle-client.readthedocs.io/en/latest/contributing.html>`__ while adhering to `the code of conduct <https://isabelle-client.readthedocs.io/en/latest/code-of-conduct.html>`__.
+
 
 .. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg
    :target: https://badge.fury.io/py/isabelle-client
 .. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg
    :target: https://anaconda.org/conda-forge/isabelle-client
 .. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg
    :target: https://circleci.com/gh/inpefess/isabelle-client
 .. |Documentation Status| image:: https://readthedocs.org/projects/isabelle-client/badge/?version=latest
    :target: https://isabelle-client.readthedocs.io/en/latest/?badge=latest
 .. |codecov| image:: https://codecov.io/gh/inpefess/isabelle-client/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/inpefess/isabelle-client
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb
-
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.1007%2F978--3--031--16681--5__24-blue
+   :target: https://doi.org/10.1007/978-3-031-16681-5_24
```

### Comparing `isabelle-client-0.3.9/isabelle_client/__init__.py` & `isabelle_client-0.4.0/isabelle_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 Boris Shminke
+# Copyright 2021-2023 Boris Shminke
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,8 +13,8 @@
 # limitations under the License.
 # noqa: D205
 """A Python client to `Isabelle <https://isabelle.in.tum.de>`__ server."""
 from isabelle_client.isabelle__client import IsabelleClient
 from isabelle_client.socket_communication import IsabelleResponse
 from isabelle_client.utils import get_isabelle_client, start_isabelle_server
 
-__version__ = "0.3.9"
+__version__ = "0.4.0"
```

### Comparing `isabelle-client-0.3.9/isabelle_client/isabelle__client.py` & `isabelle_client-0.4.0/isabelle_client/isabelle__client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 Boris Shminke
+# Copyright 2021-2023 Boris Shminke
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -72,16 +72,16 @@
         FINISHED
         >>> print(test_response[-1].response_body)
         {"session_id": "test_session_id"}
         >>> print(test_response[-1].response_length)
         43
         >>> print(logger.info.mock_calls)
         [call('test_password\ntest_command\n'),
-        call('OK "connection OK"'),
-        call('43\nFINISHED {"session_id": "test_session_id"}')]
+         call('OK "connection OK"'),
+         call('43\nFINISHED {"session_id": "test_session_id"}')]
 
         :param command: a full text of a command to Isabelle
         :param asynchronous: if ``False``, waits for ``OK``; else waits for
             ``FINISHED``
         :returns: a list of Isabelle server responses
         """
         final_message = (
@@ -97,15 +97,15 @@
             self.logger.info(command)
         response = await get_final_message(reader, final_message, self.logger)
         return response
 
     def session_build(
         self,
         session: str,
-        dirs: List[str] = None,
+        dirs: Optional[List[str]] = None,
         verbose: bool = False,
         **kwargs,
     ) -> List[IsabelleResponse]:
         """
         Build a session from ROOT file.
 
         >>> isabelle_client = IsabelleClient(
```

### Comparing `isabelle-client-0.3.9/isabelle_client/resources/example.txt` & `isabelle_client-0.4.0/isabelle_client/resources/example.txt`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.9/isabelle_client/socket_communication.py` & `isabelle_client-0.4.0/isabelle_client/socket_communication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 Boris Shminke
+# Copyright 2021-2023 Boris Shminke
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,16 +35,20 @@
     :param response_length: a length of JSON response
     """
 
     response_type: str
     response_body: str
     response_length: Optional[int] = None
 
-    def __str__(self):
-        """Pretty print Isabelle server response."""
+    def __str__(self) -> str:
+        """
+        Pretty print Isabelle server response.
+
+        :returns: a string representation of Isabelle server response
+        """
         return (
             (
                 f"{self.response_length}\n"
                 if self.response_length is not None
                 else ""
             )
             + self.response_type
@@ -126,15 +130,15 @@
     >>> for response in asyncio.run(awaiter()):
     ...     print(response)
     OK "connection OK"
     43
     FINISHED {"session_id": "test_session_id"}
     >>> print(test_logger.info.mock_calls)
     [call('OK "connection OK"'),
-    call('43\nFINISHED {"session_id": "test_session_id"}')]
+     call('43\nFINISHED {"session_id": "test_session_id"}')]
 
     :param reader: a ``StreamReader`` connected to Isabelle server
     :param final_message: a set of possible final message types
     :param logger: a logger where to send all server replies
     :returns: the final response from Isabelle server
     """
     response_list = []
```

### Comparing `isabelle-client-0.3.9/pyproject.toml` & `isabelle_client-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 [tool.poetry]
 name = "isabelle-client"
-version = "0.3.9"
+version = "0.4.0"
 description = "A client to Isabelle proof assistant server"
 authors = ["Boris Shminke <boris@shminke.ml>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/isabelle-client"
 readme = "README.rst"
 classifiers=[
+	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.7",	
 	"License :: OSI Approved :: Apache Software License",
 	"Operating System :: OS Independent",
 	"Intended Audience :: Science/Research",
 	"Development Status :: 4 - Beta",
 	"Environment :: Console",
 	"Natural Language :: English",
 	"Topic :: Scientific/Engineering :: Artificial Intelligence",
 	"Typing :: Typed"
 ]
 include = ["isabelle_client/py.typed"]
 
 [tool.poetry.dependencies]
-python = ">= 3.7.1, < 4.0"
+python = ">= 3.8.1, < 3.12"
 importlib-resources = {version = "*", markers = "python_version < \"3.9\""}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pylint = "*"
 mypy = "*"
 pytest-cov = "*"
 pre-commit = "*"
 black = "*"
 flake8 = "*"
-sphinx-rtd-theme = "*"
 sphinx-autodoc-typehints = "*"
 types-dataclasses = "*"
-jupyterlab = "*"
 pydocstyle = "*"
 tox = "*"
 pyenchant = "*"
 tbump = "*"
-nbconvert = {version = "*", extras = ["webpdf"]}
+toml = "*"
+furo = "*"
+jedi = "*"
 
 [tool.black]
 line-length=79
 
 [tool.isort]
 profile = "black"
 src_paths = ["isabelle_client"]
@@ -56,15 +56,14 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = """--doctest-modules --cov isabelle_client --cov-report xml
     --cov-report term-missing --cov-fail-under=100
     --junit-xml test-results/isabelle-client.xml"""
 testpaths = ["isabelle_client"]
-doctest_optionflags = "NORMALIZE_WHITESPACE"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "from importlib.resources import files"
 ]
 
@@ -75,45 +74,45 @@
     "pylint.extensions.mccabe",
     "pylint.extensions.set_membership",
 ]
 
 [tool.pylint.parameter_documentation]
 accept-no-param-doc = false
 accept-no-raise-doc = false
-accept-no-return-doc = true
+accept-no-return-doc = false
 accept-no-yields-doc = false
 default-docstring-type = "sphinx"
 
 [tool.pylint.format]
 max-line-length = 79
 
 [tool.pylint.design]
 max-statements = 10
 
 [tool.pylint.typecheck]
-generated-members = ["asyncio"]
+generated-members = ["asyncio", "os"]
 
 [tool.pylint.spelling]
 spelling-dict = "en_GB"
 spelling-private-dict-file = "spelling.dict"
 
 [tool.mypy]
 show_error_codes = true
 incremental = true
 disable_error_code = "no-redef"
 
 [[tool.mypy.overrides]]
-module = ["importlib_resources"]
+module = ["importlib_resources", "py"]
 ignore_missing_imports = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py37,py38,py39,py310
+envlist = py38,py39,py310,py311
 
 [testenv]
 deps =
     pytest-cov
     flake8
     pydocstyle
     pylint
@@ -128,15 +127,15 @@
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/isabelle-client/"
 
 [tool.tbump.version]
-current = "0.3.9"
+current = "0.4.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
@@ -148,8 +147,8 @@
 [[tool.tbump.file]]
 src = "isabelle_client/__init__.py"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 
 [[tool.tbump.file]]
-src = "doc/source/conf.py"
+src = "doc/conf.py"
```

### Comparing `isabelle-client-0.3.9/PKG-INFO` & `isabelle_client-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: isabelle-client
-Version: 0.3.9
+Version: 0.4.0
 Summary: A client to Isabelle proof assistant server
 Home-page: https://github.com/inpefess/isabelle-client
 License: Apache-2.0
 Author: Boris Shminke
 Author-email: boris@shminke.ml
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
-Requires-Dist: importlib-resources; python_version < "3.9"
+Requires-Dist: importlib-resources ; python_version < "3.9"
 Project-URL: Repository, https://github.com/inpefess/isabelle-client
 Description-Content-Type: text/x-rst
 
-|Binder|\ |PyPI version|\ |Anaconda version|\ |CircleCI|\ |Documentation Status|\ |codecov|
+|Binder|\ |PyPI version|\ |Anaconda version|\ |CircleCI|\ |Documentation Status|\ |codecov|\ |DOI|
 
 Python client for Isabelle server
 =================================
 
 ``isabelle-client`` is a TCP client for
 `Isabelle <https://isabelle.in.tum.de>`__ server. For more information
 about the server see part 4 of `the Isabelle system
@@ -57,79 +57,89 @@
 
    docker build -t isabelle-client https://github.com/inpefess/isabelle-client.git
    docker run -it --rm -p 8888:8888 isabelle-client jupyter-lab --ip=0.0.0.0 --port=8888
 
 How to use
 ==========
 
-Follow the `usage
+.. code:: python
+
+   from isabelle_client import get_isabelle_client, start_isabelle_server
+   
+   # start Isabelle server
+   server_info, _ = start_isabelle_server()
+   # create a client object
+   isabelle = get_isabelle_client(server_info)
+   # send a theory file from the current directory to the server
+   response = isabelle.use_theories(
+       theories=["Example"], master_dir=".", watchdog_timeout=0
+   )
+   # shut the server down
+   isabelle.shutdown()
+
+
+For more details, follow the `usage
 example <https://isabelle-client.readthedocs.io/en/latest/usage-example.html#usage-example>`__
 from documentation, run the
 `script <https://github.com/inpefess/isabelle-client/blob/master/examples/example.py>`__,
 or use ``isabelle-client`` from a
 `notebook <https://github.com/inpefess/isabelle-client/blob/master/examples/example.ipynb>`__,
 e.g. with
 `Binder <https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb>`__ (Binder might fail with 'Failed to create temporary user for ...' error which is `well known <https://mybinder-sre.readthedocs.io/en/latest/incident-reports/2018-02-20-jupyterlab-announcement.html>`__ and related neither to ``isabelle-client`` nor to the provided ``Dockerfile``. If that happens, try to run Docker as described in the section above).
 
-How to Contribute
-=================
-
-`Pull requests <https://github.com/inpefess/isabelle-client/pulls>`__
-are welcome. To start:
-
-.. code:: sh
-
-   git clone https://github.com/inpefess/isabelle-client
-   cd isabelle-client
-   # activate python virtual environment with Python 3.7+
-   pip install -U pip
-   pip install -U setuptools wheel poetry
-   poetry install
-   # recommended but not necessary
-   pre-commit install
-
-To check the code quality before creating a pull request, one might run
-the script
-`local-build.sh <https://github.com/inpefess/isabelle-client/blob/master/local-build.sh>`__.
-It locally does nearly the same as the CI pipeline after the PR is
-created.
-
-Reporting issues or problems with the software
-==============================================
-
-Questions and bug reports are welcome on `the
-tracker <https://github.com/inpefess/isabelle-client/issues>`__.
-
 More documentation
 ==================
 
 More documentation can be found
 `here <https://isabelle-client.readthedocs.io/en/latest>`__.
 
-Video example
-=============
+Similar Software
+================
+
+There are Python clients to other interactive theorem provers, for
+example:
+
+* `for Lean
+  <https://github.com/leanprover-community/lean-client-python>`__
+* `for Coq <https://github.com/IBM/pycoq>`__
+* `another one for Coq <https://github.com/ejgallego/pycoq>`__
+
+Modules helping to inetract with Isabelle server from Python are
+parts of the `Proving for Fun
+<https://github.com/maxhaslbeck/proving-contest-backends>`__ project.
+
+There are also clients to Isabelle server in other programming
+languages, e.g. `this one in Rust
+<https://lib.rs/crates/isabelle-client>`__.
 
-.. image:: https://isabelle-client.readthedocs.io/en/latest/_images/tty.gif
-	   
 How to cite
 ===========
 
-If you’re writing a research paper, you can cite Isabelle client
+If you’re writing a research paper, you can cite the Isabelle client
 using the `following DOI
 <https://doi.org/10.1007/978-3-031-16681-5_24>`__. You can also cite
-Isabelle 2021 (and the earlier version of the client) with `this
-DOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.
+Isabelle 2021 (and the earlier version of the client) with `this DOI
+<https://doi.org/10.1007/978-3-030-81097-9_20>`__. There also is a
+somewhat more complete (but unpublished) `pre-print
+<https://arxiv.org/abs/2212.11173>`__.
+
+How to Contribute
+=================
+
+Please follow `the contribution guide <https://isabelle-client.readthedocs.io/en/latest/contributing.html>`__ while adhering to `the code of conduct <https://isabelle-client.readthedocs.io/en/latest/code-of-conduct.html>`__.
+
 
 .. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg
    :target: https://badge.fury.io/py/isabelle-client
 .. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg
    :target: https://anaconda.org/conda-forge/isabelle-client
 .. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg
    :target: https://circleci.com/gh/inpefess/isabelle-client
 .. |Documentation Status| image:: https://readthedocs.org/projects/isabelle-client/badge/?version=latest
    :target: https://isabelle-client.readthedocs.io/en/latest/?badge=latest
 .. |codecov| image:: https://codecov.io/gh/inpefess/isabelle-client/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/inpefess/isabelle-client
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb
-
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.1007%2F978--3--031--16681--5__24-blue
+   :target: https://doi.org/10.1007/978-3-031-16681-5_24
```

