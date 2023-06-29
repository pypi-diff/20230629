# Comparing `tmp/draccus-0.4.1.tar.gz` & `tmp/draccus-0.4.2.tar.gz`

## Comparing `draccus-0.4.1.tar` & `draccus-0.4.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.4.1/.all-contributorsrc
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.4.1/python-package.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.4.1/setup.cfg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/draccus.iml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/vcs.xml
--rw-r--r--   0        0        0    38288 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/workspace.xml
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/api.md
--rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/argparse2pyrallis.gif
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/index.md
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/step_by_step.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/argparsing.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/cfgparsing.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/choice_types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/fields.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/help_formatter.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/py.typed
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/config_parsers.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/decoding.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/encoding.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/registry_utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/__init__.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/choice_wrapper.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/dataclass_wrapper.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/docstring.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/field_metavar.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/field_wrapper.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/suppressing_argparse.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/wrapper.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.4.1/examples/choice_class_demo.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.4.1/examples/demo.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_argparse_choice_types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_argparse_choice_types_plugin.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_base.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_bools.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_choice_types.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_decoding.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_default_args.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_docstrings.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_enums.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_inheritance.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_lists.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_optional.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_optional_union.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_tuples.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_union.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/testutils.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/draccus_choice_plugins/gpt.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/draccus_choice_plugins/model_config.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.4.1/LICENSE
--rw-r--r--   0        0        0    20257 2020-02-02 00:00:00.000000 draccus-0.4.1/README.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 draccus-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 draccus-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.4.2/.all-contributorsrc
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.4.2/python-package.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.4.2/setup.cfg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/draccus.iml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    39068 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/api.md
+-rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/argparse2pyrallis.gif
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/index.md
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/step_by_step.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/__init__.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/argparsing.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/cfgparsing.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/choice_types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/fields.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/help_formatter.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/py.typed
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/config_parsers.py
+-rw-r--r--   0        0        0    12653 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/decoding.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/encoding.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/registry_utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/__init__.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/choice_wrapper.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/dataclass_wrapper.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/docstring.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/field_metavar.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/field_wrapper.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/suppressing_argparse.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/wrapper.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.4.2/examples/choice_class_demo.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.4.2/examples/demo.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_argparse_choice_types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_argparse_choice_types_plugin.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_base.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_bools.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_choice_types.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_decoding.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_default_args.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_docstrings.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_enums.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_inheritance.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_lists.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_optional.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_optional_union.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_tuples.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_union.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/testutils.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/draccus_choice_plugins/gpt.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/draccus_choice_plugins/model_config.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.4.2/LICENSE
+-rw-r--r--   0        0        0    20257 2020-02-02 00:00:00.000000 draccus-0.4.2/README.md
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 draccus-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    20931 2020-02-02 00:00:00.000000 draccus-0.4.2/PKG-INFO
```

### Comparing `draccus-0.4.1/.all-contributorsrc` & `draccus-0.4.2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/.pre-commit-config.yaml` & `draccus-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/mkdocs.yml` & `draccus-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/python-package.yml` & `draccus-0.4.2/python-package.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/.github/workflows/pytest.yml` & `draccus-0.4.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/.github/workflows/python-publish.yml` & `draccus-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/.idea/draccus.iml` & `draccus-0.4.2/.idea/draccus.iml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/.idea/workspace.xml` & `draccus-0.4.2/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `draccus-0.4.1/.idea/workspace.xml` & `draccus-0.4.2/.idea/workspace.xml`

```diff
@@ -1,19 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="add preliminary support for dataclass lists">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/draccus/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/draccus/utils.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/draccus/wrappers/dataclass_wrapper.py" beforeDir="false" afterPath="$PROJECT_DIR$/draccus/wrappers/dataclass_wrapper.py" afterDir="false"/>
+    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="improve exceptions when something goes wrong">
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test_lists.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_lists.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -81,15 +77,15 @@
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/examples"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.pytest for test_optional.test_optional_parameter_group">
+  <component name="RunManager" selected="Python tests.pytest for tests.test_lists.test_list_of_dataclasses">
     <configuration name="pytest for test_optional.test_optional_parameter_group" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
@@ -116,106 +112,85 @@
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_collection_no_type (1)" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
-      <option name="_new_parameters" value="&quot;&quot;"/>
+      <option name="_new_parameters" value="&quot;dict-Dict-value4-{1: 2}&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_collection_no_type&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_lists.test_list_of_dataclasses" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_collection_no_type" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_lists.test_list_of_dataclasses&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_collection_no_type&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest in test_argparse_choice_types_plugin.py" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_list_of_dataclasses" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_argparse_choice_types_plugin.py&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_list_of_dataclasses&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.pytest for test_optional.test_optional_parameter_group"/>
         <item itemvalue="Python tests.pytest for tests.test_lists.test_list_of_dataclasses"/>
+        <item itemvalue="Python tests.pytest for tests.test_lists.test_collection_no_type (1)"/>
+        <item itemvalue="Python tests.pytest for tests.test_lists.test_collection_no_type"/>
+        <item itemvalue="Python tests.pytest for test_optional.test_optional_parameter_group"/>
         <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help"/>
-        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse"/>
-        <item itemvalue="Python tests.pytest in test_argparse_choice_types_plugin.py"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment=""/>
       <created>1687456901125</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1687456901125</updated>
       <workItem from="1687456902334" duration="32485000"/>
-      <workItem from="1687548821702" duration="26979000"/>
-    </task>
-    <task id="LOCAL-00008" summary="build docs">
-      <created>1687462423085</created>
-      <option name="number" value="00008"/>
-      <option name="presentableId" value="LOCAL-00008"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687462423085</updated>
-    </task>
-    <task id="LOCAL-00009" summary="test?">
-      <created>1687463332472</created>
-      <option name="number" value="00009"/>
-      <option name="presentableId" value="LOCAL-00009"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687463332472</updated>
-    </task>
-    <task id="LOCAL-00010" summary="test?">
-      <created>1687463414691</created>
-      <option name="number" value="00010"/>
-      <option name="presentableId" value="LOCAL-00010"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687463414691</updated>
+      <workItem from="1687548821702" duration="33145000"/>
     </task>
     <task id="LOCAL-00011" summary="wtf">
       <created>1687463618770</created>
       <option name="number" value="00011"/>
       <option name="presentableId" value="LOCAL-00011"/>
       <option name="project" value="LOCAL"/>
       <updated>1687463618770</updated>
@@ -531,15 +506,36 @@
     <task id="LOCAL-00056" summary="ultimately unnecessary, but it works">
       <created>1687759609235</created>
       <option name="number" value="00056"/>
       <option name="presentableId" value="LOCAL-00056"/>
       <option name="project" value="LOCAL"/>
       <updated>1687759609235</updated>
     </task>
-    <option name="localTasksCounter" value="57"/>
+    <task id="LOCAL-00057" summary="add preliminary support for dataclass lists">
+      <created>1688020376283</created>
+      <option name="number" value="00057"/>
+      <option name="presentableId" value="LOCAL-00057"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688020376283</updated>
+    </task>
+    <task id="LOCAL-00058" summary="fix merging of int keys">
+      <created>1688062131122</created>
+      <option name="number" value="00058"/>
+      <option name="presentableId" value="LOCAL-00058"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688062131122</updated>
+    </task>
+    <task id="LOCAL-00059" summary="improve exceptions when something goes wrong">
+      <created>1688064033785</created>
+      <option name="number" value="00059"/>
+      <option name="presentableId" value="LOCAL-00059"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688064033785</updated>
+    </task>
+    <option name="localTasksCounter" value="60"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -549,16 +545,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="update docs"/>
-    <MESSAGE value="comment"/>
     <MESSAGE value="strawman choice type"/>
     <MESSAGE value="add decorator"/>
     <MESSAGE value="encode/decode choice types, add tests"/>
     <MESSAGE value="add docs, expose __init__"/>
     <MESSAGE value="rename, add demo"/>
     <MESSAGE value="stupid"/>
     <MESSAGE value="wip choice wrappers"/>
@@ -574,52 +568,66 @@
     <MESSAGE value="update version"/>
     <MESSAGE value="update mypy version"/>
     <MESSAGE value="make pytest ignore the test plugins dir to not confuse the registration"/>
     <MESSAGE value="sigh"/>
     <MESSAGE value="add project urls for draccus"/>
     <MESSAGE value="ultimately unnecessary, but it works"/>
     <MESSAGE value="add preliminary support for dataclass lists"/>
-    <option name="LAST_COMMIT_MESSAGE" value="add preliminary support for dataclass lists"/>
+    <MESSAGE value="fix merging of int keys"/>
+    <MESSAGE value="improve exceptions when something goes wrong"/>
+    <option name="LAST_COMMIT_MESSAGE" value="improve exceptions when something goes wrong"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/draccus/parsers/decoding.py</url>
           <line>101</line>
           <option name="timeStamp" value="5"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/testutils.py</url>
-          <line>117</line>
+          <line>121</line>
           <option name="timeStamp" value="27"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/draccus/choice_types.py</url>
           <line>104</line>
           <option name="timeStamp" value="29"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/draccus/parsers/config_parsers.py</url>
+          <line>33</line>
+          <option name="timeStamp" value="31"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_lists.py</url>
+          <line>103</line>
+          <option name="timeStamp" value="32"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_base_test_basic_required_argument.coverage" NAME="pytest for tests.test_base.test_basic_required_argument Coverage Results" MODIFIED="1687463263242" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry.coverage" NAME="pytest for test_choice_types.test_class_registry Coverage Results" MODIFIED="1687504378733" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_collection_no_type.coverage" NAME="pytest for tests.test_lists.test_collection_no_type Coverage Results" MODIFIED="1688060693847" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_doesnt_parse_non_bools.coverage" NAME="pytest for tests.test_bools.test_bool_doesnt_parse_non_bools Coverage Results" MODIFIED="1687457197879" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_tuples_test_each_type_is_used_correctly.coverage" NAME="pytest for tests.test_tuples.test_each_type_is_used_correctly Coverage Results" MODIFIED="1687460314264" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry_decode.coverage" NAME="pytest for test_choice_types.test_class_registry_decode Coverage Results" MODIFIED="1687504658088" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_inheritance_test_subclasses_with_same_base_class_with_args.coverage" NAME="pytest for tests.test_inheritance.test_subclasses_with_same_base_class_with_args Coverage Results" MODIFIED="1687554125735" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_argparse Coverage Results" MODIFIED="1687566492053" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_plugin_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse Coverage Results" MODIFIED="1687760916671" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_test_passing_enum_to_choice.coverage" NAME="pytest for tests.test_enums.test_passing_enum_to_choice Coverage Results" MODIFIED="1687554307878" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_one_element.coverage" NAME="pytest for tests.test_lists.test_list_one_element Coverage Results" MODIFIED="1687554263882" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help Coverage Results" MODIFIED="1687760920532" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$choice_class_demo.coverage" NAME="choice_class_demo Coverage Results" MODIFIED="1687505257500" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/examples"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_parameter_group.coverage" NAME="pytest for test_optional.test_optional_parameter_group Coverage Results" MODIFIED="1688020223360" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
-    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_of_dataclasses.coverage" NAME="pytest for tests.test_lists.test_list_of_dataclasses Coverage Results" MODIFIED="1688019897140" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_collection_no_type__1_.coverage" NAME="pytest for tests.test_lists.test_collection_no_type (1) Coverage Results" MODIFIED="1688062023358" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_of_dataclasses.coverage" NAME="pytest for tests.test_lists.test_list_of_dataclasses Coverage Results" MODIFIED="1688063356342" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_examine_help Coverage Results" MODIFIED="1687594973111" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_seed.coverage" NAME="pytest for test_optional.test_optional_seed Coverage Results" MODIFIED="1687463071605" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_attributes_work.coverage" NAME="pytest for tests.test_bools.test_bool_attributes_work Coverage Results" MODIFIED="1687457200730" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_in_test_argparse_choice_types_plugin_py.coverage" NAME="pytest in test_argparse_choice_types_plugin.py Coverage Results" MODIFIED="1687670438197" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_choice_registry_encode.coverage" NAME="pytest for test_choice_types.test_choice_registry_encode Coverage Results" MODIFIED="1687504823786" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `draccus-0.4.1/.idea/inspectionProfiles/Project_Default.xml` & `draccus-0.4.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/docs/api.md` & `draccus-0.4.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/docs/argparse2pyrallis.gif` & `draccus-0.4.2/docs/argparse2pyrallis.gif`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/docs/index.md` & `draccus-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/docs/step_by_step.md` & `draccus-0.4.2/docs/step_by_step.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/argparsing.py` & `draccus-0.4.2/draccus/argparsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from collections import defaultdict
 from functools import wraps
 from gettext import gettext
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, Generic, Optional, Sequence, Text, Type, TypeVar, Union
 
+import mergedeep
+
 from draccus import cfgparsing, utils
 from draccus.help_formatter import SimpleHelpFormatter
 from draccus.parsers import decoding
 from draccus.utils import Dataclass, PyrallisException
 from draccus.wrappers import DataclassWrapper
 from draccus.wrappers.suppressing_argparse import SuppressingArgumentParser
 
@@ -135,19 +137,19 @@
             if config_path is not None:
                 warnings.warn(UserWarning(f"Overriding default {config_path} with {new_config_path}"))
             config_path = new_config_path
             del parsed_arg_values[utils.CONFIG_ARG]
 
         if config_path is not None:
             file_args = cfgparsing.load_config(open(config_path, "r"))
-            file_args = utils.flatten(file_args, sep=".")
-            file_args.update(parsed_arg_values)
-            parsed_arg_values = file_args
+        else:
+            file_args = {}
 
         deflat_d = utils.deflatten(parsed_arg_values, sep=".")
+        deflat_d = mergedeep.merge(file_args, deflat_d)
         cfg = decoding.decode(self.config_class, deflat_d)
 
         return cfg
 
 
 def parse(
     config_class: Type[T],
```

### Comparing `draccus-0.4.1/draccus/cfgparsing.py` & `draccus-0.4.2/draccus/cfgparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/choice_types.py` & `draccus-0.4.2/draccus/choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/fields.py` & `draccus-0.4.2/draccus/fields.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/help_formatter.py` & `draccus-0.4.2/draccus/help_formatter.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/options.py` & `draccus-0.4.2/draccus/options.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/utils.py` & `draccus-0.4.2/draccus/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             removed[key] = d.pop(key)
     return d, removed
 
 
 def flatten(d, parent_key=None, sep="."):
     items = []
     for k, v in d.items():
-        new_key = parent_key + sep + k if parent_key else k
+        new_key = f"{parent_key}{sep}{k}" if parent_key else k
         if isinstance(v, c_abc.MutableMapping):
             items.extend(flatten(v, parent_key=new_key, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
```

### Comparing `draccus-0.4.1/draccus/parsers/config_parsers.py` & `draccus-0.4.2/draccus/parsers/config_parsers.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/parsers/decoding.py` & `draccus-0.4.2/draccus/parsers/decoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,23 +243,27 @@
         return val if val is None else decode(val)
 
     return _decode_optional
 
 
 def try_functions(*funcs: Callable[[Any], T]) -> Callable[[Any], Union[T, Any]]:
     """Tries to use the functions in succession, else returns the same value unchanged."""
+    if len(funcs) == 0:
+        raise ValueError("Must provide at least one function to try")
+    elif len(funcs) == 1:
+        return funcs[0]
 
     def _try_functions(val: Any) -> Union[T, Any]:
+        exceptions = []
         for func in funcs:
             try:
                 return func(val)
-            except Exception:
-                continue
-        # If no function worked, raise an exception
-        raise TypeError(f"No valid parsing for value {val}")
+            except Exception as e:
+                exceptions.append(e)
+        raise TypeError(f"No valid parsing for value {val}: {exceptions}") from exceptions[0]
 
     return _try_functions
 
 
 @typing.no_type_check
 def decode_union(*types: Type[T]) -> Callable[[Any], Union[T, Any]]:
     types = list(types)
```

### Comparing `draccus-0.4.1/draccus/parsers/encoding.py` & `draccus-0.4.2/draccus/parsers/encoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/parsers/registry_utils.py` & `draccus-0.4.2/draccus/parsers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/choice_wrapper.py` & `draccus-0.4.2/draccus/wrappers/choice_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/dataclass_wrapper.py` & `draccus-0.4.2/draccus/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/docstring.py` & `draccus-0.4.2/draccus/wrappers/docstring.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/field_metavar.py` & `draccus-0.4.2/draccus/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/field_wrapper.py` & `draccus-0.4.2/draccus/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/suppressing_argparse.py` & `draccus-0.4.2/draccus/wrappers/suppressing_argparse.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/draccus/wrappers/wrapper.py` & `draccus-0.4.2/draccus/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/examples/choice_class_demo.py` & `draccus-0.4.2/examples/choice_class_demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/examples/demo.py` & `draccus-0.4.2/examples/demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/conftest.py` & `draccus-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_argparse_choice_types.py` & `draccus-0.4.2/tests/test_argparse_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_argparse_choice_types_plugin.py` & `draccus-0.4.2/tests/test_argparse_choice_types_plugin.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_base.py` & `draccus-0.4.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_bools.py` & `draccus-0.4.2/tests/test_bools.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_choice_types.py` & `draccus-0.4.2/tests/test_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_decoding.py` & `draccus-0.4.2/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_default_args.py` & `draccus-0.4.2/tests/test_default_args.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_docstrings.py` & `draccus-0.4.2/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_enums.py` & `draccus-0.4.2/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_inheritance.py` & `draccus-0.4.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_lists.py` & `draccus-0.4.2/tests/test_lists.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Set, Tuple, Type
+from typing import Any, Dict, List, Optional, Set, Tuple, Type
 
 import pytest
 
 from .testutils import ParsingError, TestSetup, format_list_using_brackets, parametrize, raises
 
 
 def test_list_one_element(simple_attribute):
@@ -82,39 +82,63 @@
         assert result == SomeClass(a=value)
 
 
 @parametrize(
     "item_type, type_hint, value, arg",
     [
         (list, List, [1, 2, 3], "[1, 2, 3]"),
+        (Optional[list], Optional[List], [1, 2, 3], "[1, 2, 3]"),
         (set, Set, {1, 2, 3}, "[1, 2, 3]"),
         (tuple, Tuple, (1, 2, 3), "[1, 2, 3]"),
         (dict, Dict, {1: 2}, "{1: 2}"),
     ],
 )
 def test_collection_no_type(item_type, type_hint, value, arg):
     @dataclass
     class ContainerHint(TestSetup):
         a: type_hint
 
     c = ContainerHint.setup(f"--a '{arg}'")
     assert c.a == value
 
+    c = ContainerHint.setup(config=f"""a: {arg}""")
+    assert c.a == value
+
     @dataclass
     class ContainerType(TestSetup):
         a: item_type
 
     c = ContainerType.setup(f"--a '{arg}'")
     assert c.a == value
 
+    c = ContainerType.setup(config=f"""a: {arg}""")
+    assert c.a == value
+
 
 def test_list_of_dataclasses():
     @dataclass
     class Inner(TestSetup):
-        a: int
+        a: float
 
     @dataclass
     class Outer(TestSetup):
-        a: List[Inner]
+        a: Optional[List[Inner]]
 
     c = Outer.setup("""--a '[{"a": 1}, {"a": 2}]'""")
     assert c.a == [Inner(a=1), Inner(a=2)]
+
+    @dataclass
+    class OptionalOuter(TestSetup):
+        b: Optional[Outer] = None
+
+    c = OptionalOuter.setup("""--b.a '[{"a": 1}, {"a": 2}]'""")
+    assert c.b == Outer(a=[Inner(a=1), Inner(a=2)])
+
+    yaml = """
+b:
+    a:
+        - a: 1
+        - a: 2
+    """
+    c = OptionalOuter.setup(config=yaml)
+
+    assert c.b == Outer(a=[Inner(a=1), Inner(a=2)])
```

### Comparing `draccus-0.4.1/tests/test_optional.py` & `draccus-0.4.2/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_tuples.py` & `draccus-0.4.2/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/test_utils.py` & `draccus-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/tests/testutils.py` & `draccus-0.4.2/tests/testutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import shlex
 import string
 import sys
+import tempfile
 from contextlib import contextmanager, redirect_stderr, suppress
 from io import StringIO
 from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar, cast
 
 import pytest
 
 import draccus
@@ -74,30 +75,33 @@
 
 
 T = TypeVar("T")
 
 
 class TestSetup:
     @classmethod
-    def setup(
-        cls: Type[Dataclass],
-        arguments: Optional[str] = "",
-    ) -> Dataclass:
+    def setup(cls: Type[Dataclass], arguments: Optional[str] = "", config: Optional[str] = None) -> Dataclass:
         """Basic setup for a tests.
 
         Keyword Arguments:
             arguments {Optional[str]} -- The arguments to pass to the parser (default: {""})
             dest {Optional[str]} -- the attribute where the argument should be stored. (default: {None})
 
         Returns:
             {cls}} -- the class's type.
         """
         if arguments is not None:
             arguments = shlex.split(arguments)  # type: ignore
-        cfg = draccus.parse(config_class=cls, args=arguments, prog="draccus")
+        if config is not None:
+            f = tempfile.NamedTemporaryFile(suffix=".yaml")
+            with open(f.name, "w") as fd:
+                fd.write(config)
+            cfg = draccus.parse(config_class=cls, args=arguments, prog="draccus", config_path=f.name)
+        else:
+            cfg = draccus.parse(config_class=cls, args=arguments, prog="draccus")
         return cfg
 
     @classmethod
     def get_help_text(
         cls,
     ) -> str:
         import contextlib
```

### Comparing `draccus-0.4.1/.gitignore` & `draccus-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/LICENSE` & `draccus-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/README.md` & `draccus-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.1/pyproject.toml` & `draccus-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "draccus"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="David Hall", email="dlwh@cs.stanford.edu" },
     { name="Sidd Karamcheti"},
 ]
 description = "A framework for simple dataclass-based configurations."
 readme = "README.md"
 requires-python = ">=3.6"
@@ -18,14 +18,15 @@
 "License :: OSI Approved :: MIT License",
 "Operating System :: OS Independent",
 ]
 dependencies = [
   "typing-inspect>=0.9.0",
   "dataclasses; python_version < '3.7'",
   "pyyaml",
+  "mergedeep"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dlwh/draccus"
 "Bug Tracker" = "https://github.com/dlwh/draccus/issues"
 
 [tool.hatch.extras]
```

### Comparing `draccus-0.4.1/PKG-INFO` & `draccus-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.4.1
+Version: 0.4.2
 Summary: A framework for simple dataclass-based configurations.
 Project-URL: Homepage, https://github.com/dlwh/draccus
 Project-URL: Bug Tracker, https://github.com/dlwh/draccus/issues
 Author: Sidd Karamcheti
 Author-email: David Hall <dlwh@cs.stanford.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: dataclasses; python_version < '3.7'
+Requires-Dist: mergedeep
 Requires-Dist: pyyaml
 Requires-Dist: typing-inspect>=0.9.0
 Description-Content-Type: text/markdown
 
 <!--
 <p align="center"><img src="https://raw.githubusercontent.com/eladrich/pyrallis/master/docs/pyrallis_logo.png" alt="logo" width="70%" /></p>
```

