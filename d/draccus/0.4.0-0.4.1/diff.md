# Comparing `tmp/draccus-0.4.0.tar.gz` & `tmp/draccus-0.4.1.tar.gz`

## Comparing `draccus-0.4.0.tar` & `draccus-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.4.0/.all-contributorsrc
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.4.0/python-package.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.4.0/setup.cfg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.4.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.4.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/draccus.iml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0    36841 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/workspace.xml
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.4.0/docs/api.md
--rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.4.0/docs/argparse2pyrallis.gif
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.4.0/docs/index.md
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.4.0/docs/step_by_step.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/argparsing.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/cfgparsing.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/choice_types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/fields.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/help_formatter.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/py.typed
--rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/parsers/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/parsers/config_parsers.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/parsers/decoding.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/parsers/encoding.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/parsers/registry_utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/__init__.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/choice_wrapper.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/dataclass_wrapper.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/docstring.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/field_metavar.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/field_wrapper.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/suppressing_argparse.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.4.0/draccus/wrappers/wrapper.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.4.0/examples/choice_class_demo.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.4.0/examples/demo.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_argparse_choice_types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_argparse_choice_types_plugin.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_base.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_bools.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_choice_types.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_decoding.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_default_args.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_docstrings.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_enums.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_inheritance.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_lists.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_optional.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_optional_union.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_tuples.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_union.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/testutils.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/draccus_choice_plugins/gpt.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.4.0/tests/draccus_choice_plugins/model_config.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.4.0/LICENSE
--rw-r--r--   0        0        0    20231 2020-02-02 00:00:00.000000 draccus-0.4.0/README.md
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 draccus-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    20873 2020-02-02 00:00:00.000000 draccus-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.4.1/.all-contributorsrc
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.4.1/python-package.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.4.1/setup.cfg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/draccus.iml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    38288 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/api.md
+-rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/argparse2pyrallis.gif
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/index.md
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.4.1/docs/step_by_step.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/argparsing.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/cfgparsing.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/choice_types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/fields.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/help_formatter.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/py.typed
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/config_parsers.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/decoding.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/encoding.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/parsers/registry_utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/__init__.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/choice_wrapper.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/dataclass_wrapper.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/docstring.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/field_metavar.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/field_wrapper.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/suppressing_argparse.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.4.1/draccus/wrappers/wrapper.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.4.1/examples/choice_class_demo.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.4.1/examples/demo.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_argparse_choice_types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_argparse_choice_types_plugin.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_base.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_bools.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_choice_types.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_decoding.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_default_args.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_docstrings.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_enums.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_inheritance.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_lists.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_optional.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_optional_union.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_tuples.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_union.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/testutils.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/draccus_choice_plugins/gpt.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.4.1/tests/draccus_choice_plugins/model_config.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.4.1/LICENSE
+-rw-r--r--   0        0        0    20257 2020-02-02 00:00:00.000000 draccus-0.4.1/README.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 draccus-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 draccus-0.4.1/PKG-INFO
```

### Comparing `draccus-0.4.0/.all-contributorsrc` & `draccus-0.4.1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.pre-commit-config.yaml` & `draccus-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/mkdocs.yml` & `draccus-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/python-package.yml` & `draccus-0.4.1/python-package.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.github/workflows/pytest.yml` & `draccus-0.4.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.github/workflows/python-publish.yml` & `draccus-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.idea/draccus.iml` & `draccus-0.4.1/.idea/draccus.iml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.idea/workspace.xml` & `draccus-0.4.1/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `draccus-0.4.0/.idea/workspace.xml` & `draccus-0.4.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="sigh">
+    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="add preliminary support for dataclass lists">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/draccus/utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/draccus/utils.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/draccus/wrappers/dataclass_wrapper.py" beforeDir="false" afterPath="$PROJECT_DIR$/draccus/wrappers/dataclass_wrapper.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_lists.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_lists.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -60,15 +64,15 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "TODO_SCOPE": "All Places",
     "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "plugin__registry",
+    "git-widget-placeholder": "main",
     "last.edited.regexp": "usage: draccus [-h] [--config_path str] [--person.type {adult,child}]\n               [--person.age int] [--person.name str]\n               [--person.favorite_toy str]\n\noptions:\n  -h, --help            show this help message and exit\n  --config_path str     Path for a config file to parse with draccus (default:\n                        None)\n\nSomething:\n\nPerson ['person']:\n\n  --person.type {adult,child}\n                        Which type of Person ['person'] to use (default: None)\n\nAdult ['person']:\n\n  --person.name str     Person's name (default: None)\n  --person.age int\n\nChild ['person']:\n\n  --person.name str     Person's name (default: None)\n  --person.favorite_toy str\n                        Child's favorite toy (default: None)",
     "last_opened_file_path": "/Users/dlwh/src/draccus/tests",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
@@ -77,80 +81,80 @@
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/examples"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.pytest in test_argparse_choice_types_plugin.py">
-    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+  <component name="RunManager" selected="Python tests.pytest for test_optional.test_optional_parameter_group">
+    <configuration name="pytest for test_optional.test_optional_parameter_group" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help&quot;"/>
+      <option name="_new_target" value="&quot;test_optional.test_optional_parameter_group&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
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
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_argparse_choice_types.test_choice_registry_argparse" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
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
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types.test_choice_registry_argparse&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_argparse_choice_types.test_choice_registry_examine_help" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
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
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types.test_choice_registry_examine_help&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_list_of_dataclasses&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="pytest in test_argparse_choice_types_plugin.py" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -165,46 +169,32 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_argparse_choice_types_plugin.py&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.pytest in test_argparse_choice_types_plugin.py"/>
-        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse"/>
+        <item itemvalue="Python tests.pytest for test_optional.test_optional_parameter_group"/>
+        <item itemvalue="Python tests.pytest for tests.test_lists.test_list_of_dataclasses"/>
         <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help"/>
-        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types.test_choice_registry_examine_help"/>
-        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types.test_choice_registry_argparse"/>
+        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse"/>
+        <item itemvalue="Python tests.pytest in test_argparse_choice_types_plugin.py"/>
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
-      <workItem from="1687548821702" duration="20819000"/>
-    </task>
-    <task id="LOCAL-00006" summary="fix test for 3.8">
-      <created>1687461033647</created>
-      <option name="number" value="00006"/>
-      <option name="presentableId" value="LOCAL-00006"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687461033647</updated>
-    </task>
-    <task id="LOCAL-00007" summary="sigh">
-      <created>1687462383416</created>
-      <option name="number" value="00007"/>
-      <option name="presentableId" value="LOCAL-00007"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687462383416</updated>
+      <workItem from="1687548821702" duration="26979000"/>
     </task>
     <task id="LOCAL-00008" summary="build docs">
       <created>1687462423085</created>
       <option name="number" value="00008"/>
       <option name="presentableId" value="LOCAL-00008"/>
       <option name="project" value="LOCAL"/>
       <updated>1687462423085</updated>
@@ -527,15 +517,29 @@
     <task id="LOCAL-00054" summary="sigh">
       <created>1687672466700</created>
       <option name="number" value="00054"/>
       <option name="presentableId" value="LOCAL-00054"/>
       <option name="project" value="LOCAL"/>
       <updated>1687672466700</updated>
     </task>
-    <option name="localTasksCounter" value="55"/>
+    <task id="LOCAL-00055" summary="add project urls for draccus">
+      <created>1687758989161</created>
+      <option name="number" value="00055"/>
+      <option name="presentableId" value="LOCAL-00055"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1687758989161</updated>
+    </task>
+    <task id="LOCAL-00056" summary="ultimately unnecessary, but it works">
+      <created>1687759609235</created>
+      <option name="number" value="00056"/>
+      <option name="presentableId" value="LOCAL-00056"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1687759609235</updated>
+    </task>
+    <option name="localTasksCounter" value="57"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -545,17 +549,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="add type method"/>
-    <MESSAGE value="why was prefix here?"/>
-    <MESSAGE value="cleanup"/>
     <MESSAGE value="update docs"/>
     <MESSAGE value="comment"/>
     <MESSAGE value="strawman choice type"/>
     <MESSAGE value="add decorator"/>
     <MESSAGE value="encode/decode choice types, add tests"/>
     <MESSAGE value="add docs, expose __init__"/>
     <MESSAGE value="rename, add demo"/>
@@ -570,15 +571,18 @@
     <MESSAGE value="i hate python"/>
     <MESSAGE value="plugin registries basically work"/>
     <MESSAGE value="update docs a bit"/>
     <MESSAGE value="update version"/>
     <MESSAGE value="update mypy version"/>
     <MESSAGE value="make pytest ignore the test plugins dir to not confuse the registration"/>
     <MESSAGE value="sigh"/>
-    <option name="LAST_COMMIT_MESSAGE" value="sigh"/>
+    <MESSAGE value="add project urls for draccus"/>
+    <MESSAGE value="ultimately unnecessary, but it works"/>
+    <MESSAGE value="add preliminary support for dataclass lists"/>
+    <option name="LAST_COMMIT_MESSAGE" value="add preliminary support for dataclass lists"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/draccus/parsers/decoding.py</url>
           <line>101</line>
@@ -601,19 +605,21 @@
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_base_test_basic_required_argument.coverage" NAME="pytest for tests.test_base.test_basic_required_argument Coverage Results" MODIFIED="1687463263242" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry.coverage" NAME="pytest for test_choice_types.test_class_registry Coverage Results" MODIFIED="1687504378733" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_doesnt_parse_non_bools.coverage" NAME="pytest for tests.test_bools.test_bool_doesnt_parse_non_bools Coverage Results" MODIFIED="1687457197879" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_tuples_test_each_type_is_used_correctly.coverage" NAME="pytest for tests.test_tuples.test_each_type_is_used_correctly Coverage Results" MODIFIED="1687460314264" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry_decode.coverage" NAME="pytest for test_choice_types.test_class_registry_decode Coverage Results" MODIFIED="1687504658088" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_inheritance_test_subclasses_with_same_base_class_with_args.coverage" NAME="pytest for tests.test_inheritance.test_subclasses_with_same_base_class_with_args Coverage Results" MODIFIED="1687554125735" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_argparse Coverage Results" MODIFIED="1687566492053" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_plugin_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse Coverage Results" MODIFIED="1687670249590" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_plugin_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse Coverage Results" MODIFIED="1687760916671" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_test_passing_enum_to_choice.coverage" NAME="pytest for tests.test_enums.test_passing_enum_to_choice Coverage Results" MODIFIED="1687554307878" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_one_element.coverage" NAME="pytest for tests.test_lists.test_list_one_element Coverage Results" MODIFIED="1687554263882" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help Coverage Results" MODIFIED="1687596218199" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help Coverage Results" MODIFIED="1687760920532" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$choice_class_demo.coverage" NAME="choice_class_demo Coverage Results" MODIFIED="1687505257500" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/examples"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_parameter_group.coverage" NAME="pytest for test_optional.test_optional_parameter_group Coverage Results" MODIFIED="1688020223360" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_of_dataclasses.coverage" NAME="pytest for tests.test_lists.test_list_of_dataclasses Coverage Results" MODIFIED="1688019897140" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_examine_help Coverage Results" MODIFIED="1687594973111" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_seed.coverage" NAME="pytest for test_optional.test_optional_seed Coverage Results" MODIFIED="1687463071605" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_attributes_work.coverage" NAME="pytest for tests.test_bools.test_bool_attributes_work Coverage Results" MODIFIED="1687457200730" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_in_test_argparse_choice_types_plugin_py.coverage" NAME="pytest in test_argparse_choice_types_plugin.py Coverage Results" MODIFIED="1687670438197" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_choice_registry_encode.coverage" NAME="pytest for test_choice_types.test_choice_registry_encode Coverage Results" MODIFIED="1687504823786" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `draccus-0.4.0/.idea/inspectionProfiles/Project_Default.xml` & `draccus-0.4.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/docs/api.md` & `draccus-0.4.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/docs/argparse2pyrallis.gif` & `draccus-0.4.1/docs/argparse2pyrallis.gif`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/docs/index.md` & `draccus-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/docs/step_by_step.md` & `draccus-0.4.1/docs/step_by_step.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/argparsing.py` & `draccus-0.4.1/draccus/argparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/cfgparsing.py` & `draccus-0.4.1/draccus/cfgparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/choice_types.py` & `draccus-0.4.1/draccus/choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/fields.py` & `draccus-0.4.1/draccus/fields.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/help_formatter.py` & `draccus-0.4.1/draccus/help_formatter.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/options.py` & `draccus-0.4.1/draccus/options.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/utils.py` & `draccus-0.4.1/draccus/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,14 +202,23 @@
         return next(
             filter(None, (get_dataclass_type_arg(arg) for arg in get_type_arguments(t))),
             None,
         )
     return None
 
 
+def is_optional_or_union_with_dataclass_type_arg(t: Type) -> bool:
+    if is_union(t) or is_optional(t):
+        return any(
+            is_dataclass_type(arg) or is_optional_or_union_with_dataclass_type_arg(arg)
+            for arg in get_type_arguments(t)
+        )
+    return False
+
+
 def get_type_arguments(container_type: Type) -> Tuple[Type, ...]:
     # return getattr(container_type, "__args__", ())
     return get_args(container_type)
 
 
 def get_type_name(some_type: Type):
     result = getattr(some_type, "__name__", str(some_type))
```

### Comparing `draccus-0.4.0/draccus/parsers/config_parsers.py` & `draccus-0.4.1/draccus/parsers/config_parsers.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/parsers/decoding.py` & `draccus-0.4.1/draccus/parsers/decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/parsers/encoding.py` & `draccus-0.4.1/draccus/parsers/encoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/parsers/registry_utils.py` & `draccus-0.4.1/draccus/parsers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/choice_wrapper.py` & `draccus-0.4.1/draccus/wrappers/choice_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/dataclass_wrapper.py` & `draccus-0.4.1/draccus/wrappers/dataclass_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,26 +156,29 @@
     #     field_wrapper = field_wrapper_class(field, parent=self, prefix=self.prefix)
     #     logger.debug(f"wrapped field at {field_wrapper.dest} has a default value of {field_wrapper.default}")
     #     return field_wrapper
     elif utils.is_choice_type(field.type):
         return ChoiceWrapper(cast(Type[ChoiceType], field.type), field.name, parent=parent, _field=field)
 
     elif utils.is_tuple_or_list_of_dataclasses(field.type):
-        raise NotImplementedError(
-            f"Field {field.name} is of type {field.type}, which isn't supported yet. (container of a dataclass type)"
-        )
+        logger.debug(f"wrapped field at {field.name} is a list of dataclasses, treating a ordinary field for argparse")
+        field_wrapper = FieldWrapper(field, parent=parent)
+        return field_wrapper
+        # raise NotImplementedError(
+        #     f"Field {field.name} is of type {field.type}, which isn't supported yet. (container of a dataclass type)"
+        # )
 
     elif dataclasses.is_dataclass(field.type):
         # handle a nested dataclass attribute
         dataclass, name = (cast(DataclassType, field.type)), field.name
         child_wrapper = DataclassWrapper(dataclass, name, parent=parent, _field=field)
         return child_wrapper
 
-    elif utils.contains_dataclass_type_arg(field.type):
-        # TODO(dlwh): I don't like this
+    elif utils.is_optional_or_union_with_dataclass_type_arg(field.type):
+        # TODO(dlwh): I don't like this. Add UnionWrapper or something
         dataclass = utils.get_dataclass_type_arg(field.type)  # type: ignore
         name = field.name
         child_wrapper = DataclassWrapper(dataclass, name, default=None, parent=parent, _field=field)
         child_wrapper.required = False
         child_wrapper.optional = True
         return child_wrapper
```

### Comparing `draccus-0.4.0/draccus/wrappers/docstring.py` & `draccus-0.4.1/draccus/wrappers/docstring.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/field_metavar.py` & `draccus-0.4.1/draccus/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/field_wrapper.py` & `draccus-0.4.1/draccus/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/suppressing_argparse.py` & `draccus-0.4.1/draccus/wrappers/suppressing_argparse.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/draccus/wrappers/wrapper.py` & `draccus-0.4.1/draccus/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/examples/choice_class_demo.py` & `draccus-0.4.1/examples/choice_class_demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/examples/demo.py` & `draccus-0.4.1/examples/demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/conftest.py` & `draccus-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_argparse_choice_types.py` & `draccus-0.4.1/tests/test_argparse_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_argparse_choice_types_plugin.py` & `draccus-0.4.1/tests/test_argparse_choice_types_plugin.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_base.py` & `draccus-0.4.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_bools.py` & `draccus-0.4.1/tests/test_bools.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_choice_types.py` & `draccus-0.4.1/tests/test_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_decoding.py` & `draccus-0.4.1/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_default_args.py` & `draccus-0.4.1/tests/test_default_args.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_docstrings.py` & `draccus-0.4.1/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_enums.py` & `draccus-0.4.1/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_inheritance.py` & `draccus-0.4.1/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_lists.py` & `draccus-0.4.1/tests/test_lists.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass, field
-from typing import *
+from typing import Any, Dict, List, Set, Tuple, Type
+
 import pytest
-from .testutils import *
+
+from .testutils import ParsingError, TestSetup, format_list_using_brackets, parametrize, raises
 
 
 def test_list_one_element(simple_attribute):
     some_type, passed_value, expected_value = simple_attribute
 
     @dataclass
     class Container(TestSetup):
@@ -62,16 +64,16 @@
         (int, [[1, 2], [4, 5], [7, 8]]),
         (float, [[1.1, 2.1], [4.2, 5.2], [7.2, 8.2]]),
         (str, [["a", "b"], ["c", "d"], ["e", "f"]]),
         (bool, [[True, True], [True, False], [False, True]]),
     ],
 )
 def test_parse_multiple_with_list_attributes(
-        item_type: Type,
-        passed_values: List[List[Any]],
+    item_type: Type,
+    passed_values: List[List[Any]],
 ):
     @dataclass
     class SomeClass(TestSetup):
         a: List[item_type] = field(default_factory=list)  # type: ignore
         """some docstring for attribute 'a'"""
 
     for value in passed_values:
@@ -79,18 +81,18 @@
         result = SomeClass.setup(arguments)
         assert result == SomeClass(a=value)
 
 
 @parametrize(
     "item_type, type_hint, value, arg",
     [
-        (list, List, [1, 2, 3], '[1, 2, 3]'),
-        (set, Set, {1, 2, 3}, '[1, 2, 3]'),
-        (tuple, Tuple, (1, 2, 3), '[1, 2, 3]'),
-        (dict, Dict, {1: 2}, '{1: 2}')
+        (list, List, [1, 2, 3], "[1, 2, 3]"),
+        (set, Set, {1, 2, 3}, "[1, 2, 3]"),
+        (tuple, Tuple, (1, 2, 3), "[1, 2, 3]"),
+        (dict, Dict, {1: 2}, "{1: 2}"),
     ],
 )
 def test_collection_no_type(item_type, type_hint, value, arg):
     @dataclass
     class ContainerHint(TestSetup):
         a: type_hint
 
@@ -100,7 +102,19 @@
     @dataclass
     class ContainerType(TestSetup):
         a: item_type
 
     c = ContainerType.setup(f"--a '{arg}'")
     assert c.a == value
 
+
+def test_list_of_dataclasses():
+    @dataclass
+    class Inner(TestSetup):
+        a: int
+
+    @dataclass
+    class Outer(TestSetup):
+        a: List[Inner]
+
+    c = Outer.setup("""--a '[{"a": 1}, {"a": 2}]'""")
+    assert c.a == [Inner(a=1), Inner(a=2)]
```

### Comparing `draccus-0.4.0/tests/test_optional.py` & `draccus-0.4.1/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_tuples.py` & `draccus-0.4.1/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/test_utils.py` & `draccus-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/tests/testutils.py` & `draccus-0.4.1/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/.gitignore` & `draccus-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/LICENSE` & `draccus-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draccus-0.4.0/README.md` & `draccus-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 > Draccus: “a large herbivorous reptilian creature, known for their ability to breathe fire.”
 
 Draccus is a fork of the excellent [Pyrallis](https://github.com/eladrich/pyrallis) library, but with
 a few changes to make it more suitable for my use cases. The main changes are:
 
 * Support for subtyping configs (that is, choosing between different configs based on a parameter)
 * WIP: Support for including config files in config files
-* WIP: Better support for type parameters
+* Better support for containers of configs (e.g. a list of configs)
 * Couple of bug fixes
 
 I swear I didn't want to fork it, but the Pyrallis devs (understandably) didn't want to merge some of
 these.
 
 
 <p align="center"><img src="https://github.com/eladrich/pyrallis/raw/master/docs/argparse2pyrallis.gif" alt="GIF" width="100%" /></p>
```

### Comparing `draccus-0.4.0/pyproject.toml` & `draccus-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "draccus"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="David Hall", email="dlwh@cs.stanford.edu" },
     { name="Sidd Karamcheti"},
 ]
 description = "A framework for simple dataclass-based configurations."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 "Programming Language :: Python :: 3",
 "License :: OSI Approved :: MIT License",
 "Operating System :: OS Independent",
 ]
 dependencies = [
-  "typing_inspect",
+  "typing-inspect>=0.9.0",
   "dataclasses; python_version < '3.7'",
   "pyyaml",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dlwh/draccus"
 "Bug Tracker" = "https://github.com/dlwh/draccus/issues"
```

### Comparing `draccus-0.4.0/PKG-INFO` & `draccus-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.4.0
+Version: 0.4.1
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
 Requires-Dist: pyyaml
-Requires-Dist: typing-inspect
+Requires-Dist: typing-inspect>=0.9.0
 Description-Content-Type: text/markdown
 
 <!--
 <p align="center"><img src="https://raw.githubusercontent.com/eladrich/pyrallis/master/docs/pyrallis_logo.png" alt="logo" width="70%" /></p>
 
 <p align="center">
 <a href="https://badge.fury.io/py/draccus"><img src="https://badge.fury.io/py/pyrallis.svg" alt="PyPI version" height="18"></a>
@@ -34,15 +34,15 @@
 > Draccus: “a large herbivorous reptilian creature, known for their ability to breathe fire.”
 
 Draccus is a fork of the excellent [Pyrallis](https://github.com/eladrich/pyrallis) library, but with
 a few changes to make it more suitable for my use cases. The main changes are:
 
 * Support for subtyping configs (that is, choosing between different configs based on a parameter)
 * WIP: Support for including config files in config files
-* WIP: Better support for type parameters
+* Better support for containers of configs (e.g. a list of configs)
 * Couple of bug fixes
 
 I swear I didn't want to fork it, but the Pyrallis devs (understandably) didn't want to merge some of
 these.
 
 
 <p align="center"><img src="https://github.com/eladrich/pyrallis/raw/master/docs/argparse2pyrallis.gif" alt="GIF" width="100%" /></p>
```

