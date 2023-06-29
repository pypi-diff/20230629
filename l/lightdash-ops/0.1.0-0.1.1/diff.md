# Comparing `tmp/lightdash_ops-0.1.0.tar.gz` & `tmp/lightdash_ops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_ops-0.1.0.tar", last modified: Thu Jun 29 02:24:42 2023, max compression
+gzip compressed data, was "lightdash_ops-0.1.1.tar", last modified: Thu Jun 29 07:49:13 2023, max compression
```

## Comparing `lightdash_ops-0.1.0.tar` & `lightdash_ops-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       76 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.env.template
--rw-r--r--   0        0        0      804 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1836 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2310 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1134 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1845 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.gitignore
--rw-r--r--   0        0        0     1383 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14060 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.pypirc
--rw-r--r--   0        0        0        8 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.python-version
--rw-r--r--   0        0        0      183 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/.yamllint
--rw-r--r--   0        0        0    11357 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/LICENSE
--rw-r--r--   0        0        0      856 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/Makefile
--rw-r--r--   0        0        0     1517 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/README.md
--rw-r--r--   0        0        0     1047 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/lint.sh
--rw-r--r--   0        0        0      994 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/publish.sh
--rwxr-xr-x   0        0        0     1396 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/setup.sh
--rwxr-xr-x   0        0        0     1170 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/test_python.sh
--rw-r--r--   0        0        0     1175 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/dev/update_resources.sh
--rw-r--r--   0        0        0     5442 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/docs/cli.md
--rw-r--r--   0        0        0      879 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/__init__.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/cli/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/cli/main.py
--rw-r--r--   0        0        0     3722 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/cli/organization_v1.py
--rw-r--r--   0        0        0     9130 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/cli/project_v1.py
--rw-r--r--   0        0        0     1165 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/cli/settings.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/client.py
--rw-r--r--   0        0        0     3328 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/organization.py
--rw-r--r--   0        0        0     3628 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/project.py
--rw-r--r--   0        0        0     5168 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/space.py
--rw-r--r--   0        0        0     5351 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/lightdash/user_group.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/__init__.py
--rw-r--r--   0        0        0     1098 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/base_user.py
--rw-r--r--   0        0        0     2528 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/organization.py
--rw-r--r--   0        0        0     2625 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/project.py
--rw-r--r--   0        0        0     2849 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/project_member.py
--rw-r--r--   0        0        0     1852 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/settings.py
--rw-r--r--   0        0        0     3312 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/space.py
--rw-r--r--   0        0        0     1856 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/models/user_group.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/operators/__init__.py
--rw-r--r--   0        0        0     4895 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/operators/organization_v1.py
--rw-r--r--   0        0        0     7739 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/operators/project_v1.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/__init__.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/__init__.py
--rw-r--r--   0        0        0     1932 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/test_organization.py
--rw-r--r--   0        0        0     1604 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/test_project.py
--rw-r--r--   0        0        0      794 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/__init__.py
--rw-r--r--   0        0        0     1385 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/test_lightdash_user.py
--rw-r--r--   0        0        0     1350 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/test_manager_settings.py
--rw-r--r--   0        0        0     1279 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/test_project_member.py
--rw-r--r--   0        0        0     1389 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/test_space.py
--rw-r--r--   0        0        0     3035 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/models/test_user_group.py
--rw-r--r--   0        0        0      219 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/resources/test-organization-config-v1.yml
--rw-r--r--   0        0        0      764 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/resources/test-project-config-v1.yml
--rw-r--r--   0        0        0      325 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/resources/test-user-group-config-v1.yml
--rw-r--r--   0        0        0     2122 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/test_utils.py
--rw-r--r--   0        0        0     1932 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/tests/utils.py
--rw-r--r--   0        0        0     3615 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/lightdash_ops/utils.py
--rw-r--r--   0        0        0     2012 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-29 02:24:42.000000 lightdash_ops-0.1.0/setup.py
--rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 lightdash_ops-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.env.template
+-rw-r--r--   0        0        0      804 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1836 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2310 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1134 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1845 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1383 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14060 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.python-version
+-rw-r--r--   0        0        0      183 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.yamllint
+-rw-r--r--   0        0        0    11357 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/LICENSE
+-rw-r--r--   0        0        0      856 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/Makefile
+-rw-r--r--   0        0        0     1517 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/README.md
+-rw-r--r--   0        0        0     1047 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/lint.sh
+-rw-r--r--   0        0        0      994 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1391 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/publish.sh
+-rwxr-xr-x   0        0        0     1396 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/setup.sh
+-rwxr-xr-x   0        0        0     1170 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/test_python.sh
+-rw-r--r--   0        0        0     1175 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/update_resources.sh
+-rw-r--r--   0        0        0     5442 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/docs/cli.md
+-rw-r--r--   0        0        0      879 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/main.py
+-rw-r--r--   0        0        0     3608 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/organization_v1.py
+-rw-r--r--   0        0        0     9130 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/project_v1.py
+-rw-r--r--   0        0        0     1165 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/settings.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/client.py
+-rw-r--r--   0        0        0     3328 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/organization.py
+-rw-r--r--   0        0        0     3628 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/project.py
+-rw-r--r--   0        0        0     5168 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/space.py
+-rw-r--r--   0        0        0     5351 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/user_group.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/__init__.py
+-rw-r--r--   0        0        0     1098 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/base_user.py
+-rw-r--r--   0        0        0     2533 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/organization.py
+-rw-r--r--   0        0        0     2625 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/project.py
+-rw-r--r--   0        0        0     2854 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/project_member.py
+-rw-r--r--   0        0        0     1852 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/settings.py
+-rw-r--r--   0        0        0     3312 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/space.py
+-rw-r--r--   0        0        0     1856 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/user_group.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/__init__.py
+-rw-r--r--   0        0        0     4895 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/organization_v1.py
+-rw-r--r--   0        0        0     7739 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/project_v1.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/__init__.py
+-rw-r--r--   0        0        0     1932 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_organization.py
+-rw-r--r--   0        0        0     1604 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_project.py
+-rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/__init__.py
+-rw-r--r--   0        0        0     1385 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_lightdash_user.py
+-rw-r--r--   0        0        0     1350 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_manager_settings.py
+-rw-r--r--   0        0        0     1279 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_project_member.py
+-rw-r--r--   0        0        0     1389 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_space.py
+-rw-r--r--   0        0        0     3035 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_user_group.py
+-rw-r--r--   0        0        0      219 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-organization-config-v1.yml
+-rw-r--r--   0        0        0      764 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-project-config-v1.yml
+-rw-r--r--   0        0        0      325 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-user-group-config-v1.yml
+-rw-r--r--   0        0        0     2122 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/test_utils.py
+-rw-r--r--   0        0        0     1932 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/utils.py
+-rw-r--r--   0        0        0     3615 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/utils.py
+-rw-r--r--   0        0        0     2012 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/setup.py
+-rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 lightdash_ops-0.1.1/PKG-INFO
```

### Comparing `lightdash_ops-0.1.0/.github/CODEOWNERS` & `lightdash_ops-0.1.1/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.github/workflows/publish.yml` & `lightdash_ops-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.github/workflows/test-publish.yml` & `lightdash_ops-0.1.1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.github/workflows/test.yml` & `lightdash_ops-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.gitignore` & `lightdash_ops-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.pre-commit-config.yaml` & `lightdash_ops-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/.pylintrc` & `lightdash_ops-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/LICENSE` & `lightdash_ops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/Makefile` & `lightdash_ops-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/README.md` & `lightdash_ops-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/lint.sh` & `lightdash_ops-0.1.1/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/lint_python.sh` & `lightdash_ops-0.1.1/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/publish.sh` & `lightdash_ops-0.1.1/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/setup.sh` & `lightdash_ops-0.1.1/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/test_python.sh` & `lightdash_ops-0.1.1/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/dev/update_resources.sh` & `lightdash_ops-0.1.1/dev/update_resources.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/docs/cli.md` & `lightdash_ops-0.1.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

### Comparing `lightdash_ops-0.1.0/lightdash_ops/cli/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/cli/main.py` & `lightdash_ops-0.1.1/lightdash_ops/cli/main.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/cli/organization_v1.py` & `lightdash_ops-0.1.1/lightdash_ops/cli/organization_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,22 +60,15 @@
     # Create the operator
     operator = OrganizationOperatorV1(client=client)
     # Get all members in the organization
     members = operator.get_organization_members()
     if role is not None:
         members = [member for member in members if member.role == role]
     # Format output
-    formatted_members = [
-        {
-            'member_uuid': x.uuid,
-            'email': x.email,
-            'role': x.role.value,
-        }
-        for x in members
-    ]
+    formatted_members = [member.dict() for member in members]
     print(json.dumps(formatted_members, indent=2))
 
 
 @organization_v1_app.command('grant-role')
 def grant_member_role(
         api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         email: Annotated[str, typer.Option(help='member email')],
```

### Comparing `lightdash_ops-0.1.0/lightdash_ops/cli/project_v1.py` & `lightdash_ops-0.1.1/lightdash_ops/cli/project_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/cli/settings.py` & `lightdash_ops-0.1.1/lightdash_ops/cli/settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/client.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/organization.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/project.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/space.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/lightdash/user_group.py` & `lightdash_ops-0.1.1/lightdash_ops/lightdash/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/base_user.py` & `lightdash_ops-0.1.1/lightdash_ops/models/base_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/organization.py` & `lightdash_ops-0.1.1/lightdash_ops/models/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import enum
 from typing import List
 
 from lightdash_client.models import OrganizationMemberRole
 from pydantic import BaseModel, EmailStr, Field, ValidationError, validator
 
 
-class OrganizationRole(enum.Enum):
+class OrganizationRole(str, enum.Enum):
     """Organization role"""
     ADMIN = 'admin'
     DEVELOPER = 'developer'
     EDITOR = 'editor'
     INTERACTIVE_VIEWER = 'interactive_viewer'
     MEMBER = 'member'
     VIEWER = 'viewer'
```

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/project.py` & `lightdash_ops-0.1.1/lightdash_ops/models/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/project_member.py` & `lightdash_ops-0.1.1/lightdash_ops/models/project_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pydantic import Field, FutureDate, ValidationError, validator
 
 from lightdash_ops.models.base_user import LightdashUser
 from lightdash_ops.models.settings import get_settings
 from lightdash_ops.utils import is_future_date
 
 
-class ProjectRole(enum.Enum):
+class ProjectRole(str, enum.Enum):
     """Project roles"""
     ADMIN = 'admin'
     DEVELOPER = 'developer'
     EDITOR = 'editor'
     INTERACTIVE_VIEWER = 'interactive_viewer'
     VIEWER = 'viewer'
     MEMBER = 'member'
```

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/settings.py` & `lightdash_ops-0.1.1/lightdash_ops/models/settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/space.py` & `lightdash_ops-0.1.1/lightdash_ops/models/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/models/user_group.py` & `lightdash_ops-0.1.1/lightdash_ops/models/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/operators/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/operators/organization_v1.py` & `lightdash_ops-0.1.1/lightdash_ops/operators/organization_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/operators/project_v1.py` & `lightdash_ops-0.1.1/lightdash_ops/operators/project_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/test_organization.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/lightdash/test_project.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/__init__.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/test_lightdash_user.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_lightdash_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/test_manager_settings.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_manager_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/test_project_member.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/test_space.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/models/test_user_group.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/resources/test-project-config-v1.yml` & `lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-project-config-v1.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/test_utils.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/tests/utils.py` & `lightdash_ops-0.1.1/lightdash_ops/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/lightdash_ops/utils.py` & `lightdash_ops-0.1.1/lightdash_ops/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/pyproject.toml` & `lightdash_ops-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/setup.py` & `lightdash_ops-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.0/PKG-INFO` & `lightdash_ops-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-ops
-Version: 0.1.0
+Version: 0.1.1
 Summary: The CLI enables us to operate resources on Lightdash.
 Author: yu-iskw
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

