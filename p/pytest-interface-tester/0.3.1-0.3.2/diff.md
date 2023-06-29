# Comparing `tmp/pytest-interface-tester-0.3.1.tar.gz` & `tmp/pytest-interface-tester-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-interface-tester-0.3.1.tar", last modified: Tue May  9 14:13:33 2023, max compression
+gzip compressed data, was "pytest-interface-tester-0.3.2.tar", last modified: Thu Jun 29 07:52:02 2023, max compression
```

## Comparing `pytest-interface-tester-0.3.1.tar` & `pytest-interface-tester-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.778787 pytest-interface-tester-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/interface_tester/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/interface_tester/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/cli/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/interface_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/interface_tester/schema_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 14:13:33.000000 pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:13:33.782787 pytest-interface-tester-0.3.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/tests/unit/test_collect_interface_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/tests/unit/test_collect_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-09 14:13:18.000000 pytest-interface-tester-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.276118 pytest-interface-tester-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/interface_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/interface_tester/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/cli/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/interface_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/interface_tester/schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 07:52:02.000000 pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.276118 pytest-interface-tester-0.3.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:52:02.280119 pytest-interface-tester-0.3.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/tests/unit/test_collect_interface_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/tests/unit/test_collect_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-29 07:51:49.000000 pytest-interface-tester-0.3.2/tox.ini
```

### Comparing `pytest-interface-tester-0.3.1/.github/workflows/build_wheels.yaml` & `pytest-interface-tester-0.3.2/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/.github/workflows/quality_checks.yaml` & `pytest-interface-tester-0.3.2/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/PKG-INFO` & `pytest-interface-tester-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/pytest-interface-tester
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

### Comparing `pytest-interface-tester-0.3.1/README.md` & `pytest-interface-tester-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/interface_tester/cli/discover.py` & `pytest-interface-tester-0.3.2/interface_tester/cli/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ):
     """Pretty-print a listing of the interface tests specified in charm-relation-interfaces."""
     return _pprint_tests(path, include)
 
 
 def _pprint_tests(path: Path = Path(), include="*"):
     """Pretty-print a listing of the interface tests specified in this repository."""
-    print(f"collecting tests from root = {path.absolute()}...")
+    print(f"collecting tests for {include} from root = {path.absolute()}")
     tests = collect_tests(path=path, include=include)
     print("Discovered:")
 
     def pprint_case(case: "_InterfaceTestCase"):
         state = "yes" if case.input_state else "no"
         schema_config = case.schema if isinstance(case.schema, SchemaConfig) else "custom"
         print(f"      - {case.name}:: {case.event} (state={state}, schema={schema_config})")
```

### Comparing `pytest-interface-tester-0.3.1/interface_tester/collector.py` & `pytest-interface-tester-0.3.2/interface_tester/collector.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/interface_tester/errors.py` & `pytest-interface-tester-0.3.2/interface_tester/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/interface_tester/interface_test.py` & `pytest-interface-tester-0.3.2/interface_tester/interface_test.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/interface_tester/plugin.py` & `pytest-interface-tester-0.3.2/interface_tester/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/interface_tester/runner.py` & `pytest-interface-tester-0.3.2/interface_tester/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import typing
 from typing import Dict, List, Optional, Type
 
 from ops.charm import CharmBase
-from scenario import Event, Relation, State, trigger
+from scenario import Event, Relation, State, Context
 
 from .errors import InvalidTestCaseError
 from .interface_test import SchemaConfig, logger
 from .schema_base import DataBagSchema
 
 if typing.TYPE_CHECKING:
     from .interface_test import _InterfaceTestCase
 
 
 def _assert_case_plays(
-    event: Event, state: State, charm_type: Type["CharmBase"], meta, actions, config
+        event: Event, state: State, charm_type: Type["CharmBase"], meta, actions, config
 ) -> State:
     try:
-        state_out = trigger(
-            state,
-            event,
-            charm_type=charm_type,
-            meta=meta,
-            actions=actions,
-            config=config,
-        )
+        ctx = Context(charm_type, meta=meta, actions=actions, config=config)
+        state_out = ctx.run(event, state)
     except Exception as e:
         msg = (
             f"Failed check 1: scenario errored out: ({type(e).__name__}){e}. Could not play scene."
         )
         raise RuntimeError(msg) from e
     return state_out
 
@@ -59,15 +53,15 @@
     except Exception as e:
         msg = f"Failed check 3: validating schema on scene output: {e}"
         logger.error(msg)
         raise RuntimeError(msg) from e
 
 
 def _assert_schemas_valid(
-    test: "_InterfaceTestCase", state_out: State, schema: DataBagSchema, interface_name: str
+        test: "_InterfaceTestCase", state_out: State, schema: DataBagSchema, interface_name: str
 ) -> List[str]:
     """Check that all relations using the interface comply with the provided schema."""
     test_schema = test.schema
     if test_schema is SchemaConfig.skip:
         logger.info("Schema validation skipped as per interface_test_case schema config.")
         return []
 
@@ -89,25 +83,25 @@
             _assert_schema_valid(schema=schema, relation=relation)
         except RuntimeError as e:
             errors.append(e.args[0])
     return errors
 
 
 def run_test_case(
-    test: "_InterfaceTestCase",
-    schema: Optional["DataBagSchema"],
-    event: Event,
-    state: State,
-    interface_name: str,
-    # the charm type we're testing
-    charm_type: Type["CharmBase"],
-    # charm metadata yamls
-    meta: Dict,
-    config: Dict,
-    actions: Dict,
+        test: "_InterfaceTestCase",
+        schema: Optional["DataBagSchema"],
+        event: Event,
+        state: State,
+        interface_name: str,
+        # the charm type we're testing
+        charm_type: Type["CharmBase"],
+        # charm metadata yamls
+        meta: Dict,
+        config: Dict,
+        actions: Dict,
 ) -> List[str]:
     """Run an interface test case.
 
     This will run three checks in sequence:
     - play the scenario (check that the charm runs without exceptions) and
       obtain the output state
     - validate the output state (by calling the test-case-provided validator with
```

### Comparing `pytest-interface-tester-0.3.1/interface_tester/schema_base.py` & `pytest-interface-tester-0.3.2/interface_tester/schema_base.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/pyproject.toml` & `pytest-interface-tester-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pytest-interface-tester"
 
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" },
 ]
 description = "Pytest plugin for checking charm relation interface protocol compliance."
 license.text = "Apache-2.0"
 keywords = ["juju", "relation interfaces"]
 
 dependencies = [
     "pydantic==1.10.7",
     "typer==0.7.0",
-    "ops-scenario==3.0.1",
+    "ops-scenario>=4.0",
     "pytest"
 ]
 
 readme = "README.md"
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/PKG-INFO` & `pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/pytest-interface-tester
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

### Comparing `pytest-interface-tester-0.3.1/pytest_interface_tester.egg-info/SOURCES.txt` & `pytest-interface-tester-0.3.2/pytest_interface_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/tests/unit/test_collect_interface_tests.py` & `pytest-interface-tester-0.3.2/tests/unit/test_collect_interface_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     pth.write_text(
         dedent(
             f"""
 from interface_tester.interface_test import interface_test_case, Role
 from scenario import State
 
 @interface_test_case(
-    "{role}",
+    "{role.value}",
     "{event}",
     input_state={input_state},
     name="{unique_name}",
     schema='skip'
 )
 def foo(state_out: State):
     pass
```

### Comparing `pytest-interface-tester-0.3.1/tests/unit/test_collect_schemas.py` & `pytest-interface-tester-0.3.2/tests/unit/test_collect_schemas.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.3.1/tox.ini` & `pytest-interface-tester-0.3.2/tox.ini`

 * *Files identical despite different names*

