# Comparing `tmp/exasol-script-languages-container-ci-setup-1.0.0.tar.gz` & `tmp/exasol_script_languages_container_ci_setup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol-script-languages-container-ci-setup-1.0.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci_setup-1.1.0.tar", max compression
```

## Comparing `exasol-script-languages-container-ci-setup-1.0.0.tar` & `exasol_script_languages_container_ci_setup-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,59 @@
--rw-r--r--   0        0        0     1063 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/LICENSE
--rw-r--r--   0        0        0      376 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/__init__.py
--rw-r--r--   0        0        0     1260 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py
--rw-r--r--   0        0        0     1257 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py
--rw-r--r--   0        0        0     1480 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py
--rw-r--r--   0        0        0     1508 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py
--rw-r--r--   0        0        0     1542 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py
--rw-r--r--   0        0        0     1205 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/health.py
--rw-r--r--   0        0        0     1287 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py
--rw-r--r--   0        0        0     1549 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py
--rw-r--r--   0        0        0     1986 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py
--rw-r--r--   0        0        0     1140 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py
--rw-r--r--   0        0        0     1124 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py
--rw-r--r--   0        0        0     1467 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py
--rw-r--r--   0        0        0      173 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/common.py
--rw-r--r--   0        0        0        0 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/options/__init__.py
--rw-r--r--   0        0        0      148 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/options/aws_options.py
--rw-r--r--   0        0        0      727 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/options/logging.py
--rw-r--r--   0        0        0     3173 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/health_check.py
--rw-r--r--   0        0        0        0 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/__init__.py
--rw-r--r--   0        0        0     7546 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/aws_access.py
--rw-r--r--   0        0        0     1964 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/ci_build.py
--rw-r--r--   0        0        0     8752 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/deployer.py
--rw-r--r--   0        0        0     3112 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py
--rw-r--r--   0        0        0      716 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py
--rw-r--r--   0        0        0     1707 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/release_build.py
--rw-r--r--   0        0        0      327 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/render_template.py
--rw-r--r--   0        0        0      950 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py
--rw-r--r--   0        0        0      971 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py
--rw-r--r--   0        0        0     5897 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py
--rw-r--r--   0        0        0     1580 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py
--rwxr-xr-x   0        0        0      131 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/main.py
--rw-r--r--   0        0        0     2265 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml
--rw-r--r--   0        0        0      237 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/buildspec_batch_entry.yaml
--rw-r--r--   0        0        0      222 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/buildspec_hull.yaml
--rw-r--r--   0        0        0      390 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/config_schema.json
--rw-r--r--   0        0        0     1354 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml
--rw-r--r--   0        0        0     4094 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml
--rw-r--r--   0        0        0     3926 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml
--rw-r--r--   0        0        0      359 2023-03-28 14:33:01.386923 exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/slc_source_credential.yaml
--rw-r--r--   0        0        0      748 2023-03-28 14:33:01.390923 exasol-script-languages-container-ci-setup-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 exasol-script-languages-container-ci-setup-1.0.0/setup.py
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 exasol-script-languages-container-ci-setup-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/LICENSE
+-rw-r--r--   0        0        0      376 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1264 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py
+-rw-r--r--   0        0        0     1261 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py
+-rw-r--r--   0        0        0     1484 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py
+-rw-r--r--   0        0        0     1508 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py
+-rw-r--r--   0        0        0     1542 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py
+-rw-r--r--   0        0        0     1205 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/health.py
+-rw-r--r--   0        0        0     1590 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py
+-rw-r--r--   0        0        0     2225 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py
+-rw-r--r--   0        0        0     2554 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py
+-rw-r--r--   0        0        0     1108 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py
+-rw-r--r--   0        0        0     1128 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py
+-rw-r--r--   0        0        0     1471 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py
+-rw-r--r--   0        0        0      173 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/common.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/options/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-29 11:41:12.300487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/options/aws_options.py
+-rw-r--r--   0        0        0      727 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/options/logging.py
+-rw-r--r--   0        0        0     3173 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/health_check.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/__init__.py
+-rw-r--r--   0        0        0     8175 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py
+-rw-r--r--   0        0        0     8752 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/deployer.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/aws_client.py
+-rw-r--r--   0        0        0     1958 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/cloudformation_service.py
+-rw-r--r--   0        0        0     1750 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/codebuild_service.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/__init__.py
+-rw-r--r--   0        0        0     2973 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/cloudformation.py
+-rw-r--r--   0        0        0     1881 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/codebuild.py
+-rw-r--r--   0        0        0      683 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/common.py
+-rw-r--r--   0        0        0      509 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/secretsmanager.py
+-rw-r--r--   0        0        0      882 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/secretsmanager_service.py
+-rw-r--r--   0        0        0     1968 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/ci_build.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/config/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/config/config_data_model.py
+-rw-r--r--   0        0        0     2159 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/config/data_model_generator.py
+-rw-r--r--   0        0        0     2863 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py
+-rw-r--r--   0        0        0      716 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py
+-rw-r--r--   0        0        0     1711 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/release_build.py
+-rw-r--r--   0        0        0      327 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/render_template.py
+-rw-r--r--   0        0        0      950 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py
+-rw-r--r--   0        0        0      971 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py
+-rw-r--r--   0        0        0     7645 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py
+-rw-r--r--   0        0        0     1584 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py
+-rwxr-xr-x   0        0        0      131 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/main.py
+-rw-r--r--   0        0        0     2265 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml
+-rw-r--r--   0        0        0      237 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/buildspec_batch_entry.yaml
+-rw-r--r--   0        0        0      222 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/buildspec_hull.yaml
+-rw-r--r--   0        0        0      950 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/config_schema.json
+-rw-r--r--   0        0        0     1354 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml
+-rw-r--r--   0        0        0     4094 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml
+-rw-r--r--   0        0        0     3926 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml
+-rw-r--r--   0        0        0      359 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/slc_source_credential.yaml
+-rw-r--r--   0        0        0      808 2023-06-29 11:41:12.304487 exasol_script_languages_container_ci_setup-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci_setup-1.1.0/PKG-INFO
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/LICENSE` & `exasol_script_languages_container_ci_setup-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.ci_build import run_deploy_ci_build
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
 from exasol_script_languages_container_ci_setup.lib.release_build import run_deploy_release_build
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.source_credentials import run_deploy_source_credentials
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/health.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/health.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-import os
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.ci_build import run_validate_ci_build
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
-from exasol_script_languages_container_ci_setup.lib.run_start_build import run_start_ci_build
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
 @click.option('--project', type=str, required=True,
-              help="""The project name. Must be same name as used for the AWS CodeBuild release stack creation.""")
-@click.option('--branch', type=str, required=True,
-              help="""The branch of the repository which will be used(e.g. refs/heads/master).""")
-def start_ci_build(
+              help="""The project for which the stack will be created.""")
+@click.option('--project-url', type=str, required=True,
+              help="""The URL of the project on Github.""")
+def validate_ci_build(
         aws_profile: Optional[str],
         log_level: str,
         project: str,
-        branch: str):
-    """
-    This command can be used to trigger the AWS CI CodeBuild locally (not by Github Webhook).
-    """
+        project_url: str):
     set_log_level(log_level)
-    run_start_ci_build(AwsAccess(aws_profile), project, branch)
+    run_validate_ci_build(AwsAccess(aws_profile), project, project_url)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-import os
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.source_credentials import run_validate_source_credentials
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
-from exasol_script_languages_container_ci_setup.lib.run_start_build import run_start_release_build
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
-@click.option('--project', type=str, required=True,
-              help="""The project name. Must be same name as used for the AWS CodeBuild release stack creation.""")
-@click.option('--upload-url', type=str, required=False,
-              help="""The URL of the Github release where artifacts will be stored.""")
-@click.option('--branch', type=str, required=True,
-              help="""The branch of the repository which will be used.""")
-def start_release_build(
+@click.option('--secret-name', required=True, type=str,
+              help="Secret name for the Github user credentials stored in AWS Secret Manager.")
+@click.option('--secret-user-key', required=True, type=str,
+              help="Github user key stored as secret in AWS Secret Manager under the respective secret name.")
+@click.option('--secret-token-key', required=True, type=str,
+              help="Github user token key stored as secret in AWS Secret Manager under the respective secret name.")
+def validate_source_credentials(
         aws_profile: Optional[str],
         log_level: str,
-        project: str,
-        upload_url: str,
-        branch: str):
-    """
-    This command  triggers the AWS release Codebuild to upload the
-    release artifacts onto the given Github release, indicated by parameter 'upload_url'.
-    """
+        secret_name: str,
+        secret_user_key: str,
+        secret_token_key: str):
     set_log_level(log_level)
-    run_start_release_build(AwsAccess(aws_profile), project, upload_url, branch, os.getenv("GITHUB_TOKEN"))
+    run_validate_source_credentials(AwsAccess(aws_profile), secret_name, secret_user_key, secret_token_key)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
-from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
+from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.github_draft_release_creator import GithubDraftReleaseCreator
 from exasol_script_languages_container_ci_setup.lib.run_start_build import run_start_test_release_build
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
@@ -20,22 +20,37 @@
 @click.option('--repo-name', type=str, required=True,
               help="""The repository for which the test release should be created. 
               For example 'exasol/script-languages'.""", )
 @click.option('--branch', type=str, required=True,
               help="""The branch for which the test release should be created.""")
 @click.option('--release-title', type=str, required=True,
               help="""The title of the Github draft release which will be created.""")
+@click.option('--timeout-in-seconds', type=int, required=False,
+              help="""Time to wait for the release, anymore.""")
+@click.option('--config-file', type=click.Path(file_okay=True, dir_okay=False, exists=True),
+              help="Configuration file for build (project specific).")
 def start_test_release_build(
         aws_profile: Optional[str],
         log_level: str,
         repo_name: str,
         project: str,
         branch: str,
-        release_title: str
+        release_title: str,
+        timeout_in_seconds: Optional[str],
+        config_file: Optional[str]
 ):
     """
     This command creates a release draft on Github and triggers the AWS release Codebuild to upload the
     release artifacts onto the new Github release.
     """
     set_log_level(log_level)
-    run_start_test_release_build(AwsAccess(aws_profile), GithubDraftReleaseCreator(),
-                                 repo_name, project, branch, release_title, os.getenv("GITHUB_TOKEN"))
+    run_start_test_release_build(
+        aws_access=AwsAccess(aws_profile),
+        gh_release_creator=GithubDraftReleaseCreator(),
+        repo_name=repo_name,
+        project=project,
+        branch=branch,
+        release_title=release_title,
+        gh_token=os.getenv("GITHUB_TOKEN"),
+        timeout_in_seconds=timeout_in_seconds,
+        config_file_path=config_file
+    )
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-import logging
 from typing import Optional
 
 import click
 
 from exasol_script_languages_container_ci_setup.cli.cli import cli
 from exasol_script_languages_container_ci_setup.cli.common import add_options
 from exasol_script_languages_container_ci_setup.cli.options.logging import logging_options, set_log_level
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
-from exasol_script_languages_container_ci_setup.lib.ci_build import run_deploy_ci_build, run_validate_ci_build
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.cli.options.aws_options import aws_options
+from exasol_script_languages_container_ci_setup.lib.release_build import run_validate_release_build
 
 
 @cli.command()
 @add_options(aws_options)
 @add_options(logging_options)
 @click.option('--project', type=str, required=True,
               help="""The project for which the stack will be created.""")
 @click.option('--project-url', type=str, required=True,
               help="""The URL of the project on Github.""")
-def validate_ci_build(
+def validate_release_build(
         aws_profile: Optional[str],
         log_level: str,
         project: str,
         project_url: str):
     set_log_level(log_level)
-    run_validate_ci_build(AwsAccess(aws_profile), project, project_url)
+    run_validate_release_build(AwsAccess(aws_profile), project, project_url)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/cli/options/logging.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/cli/options/logging.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/health_check.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/health_check.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/aws_access.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 import logging
 import time
-from typing import Optional, List, Dict, Any, Iterable
+from typing import Optional, List, Dict, Iterable, Callable
 
-import boto3
 from botocore.exceptions import ClientError
 
-from exasol_script_languages_container_ci_setup.lib.deployer import Deployer
+from exasol_script_languages_container_ci_setup.lib.aws.deployer import Deployer
+from exasol_script_languages_container_ci_setup.lib.aws.wrapper.aws_client import AwsClientFactory, AwsClient
+from exasol_script_languages_container_ci_setup.lib.aws.wrapper.datamodels.cloudformation import StackResourceSummary
+from exasol_script_languages_container_ci_setup.lib.aws.wrapper.datamodels.codebuild import BuildBatchStatus
+from exasol_script_languages_container_ci_setup.lib.aws.wrapper.datamodels.common import PhysicalResourceId
+
+BUILD_STATUS_FAILURES = [BuildBatchStatus.FAILED, BuildBatchStatus.FAULT,
+                         BuildBatchStatus.STOPPED, BuildBatchStatus.TIMED_OUT]
 
 
-class AwsAccess(object):
-    def __init__(self, aws_profile: Optional[str]):
+class AwsAccess:
+    def __init__(self, aws_profile: Optional[str],
+                 aws_client_factory: AwsClientFactory = AwsClientFactory()):
+        self._aws_client_factory = aws_client_factory
         self._aws_profile = aws_profile
 
     @property
     def aws_profile_for_logging(self) -> str:
         if self._aws_profile is not None:
             return self._aws_profile
         else:
             return "{default}"
 
     @property
     def aws_profile(self) -> Optional[str]:
         return self._aws_profile
 
+    def _get_aws_client(self) -> AwsClient:
+        return self._aws_client_factory.create(profile=self._aws_profile)
+
     def upload_cloudformation_stack(self, yml: str, stack_name: str):
         """
         Deploy the cloudformation stack.
         """
         logging.debug(f"Running upload_cloudformation_stack for aws profile {self.aws_profile_for_logging}")
-        cloud_client = self._get_aws_client("cloudformation")
+        client = self._get_aws_client().create_cloudformation_service()
         try:
-            cfn_deployer = Deployer(cloudformation_client=cloud_client)
+            cfn_deployer = Deployer(cloudformation_client=client.internal_aws_client)
             result = cfn_deployer.create_and_wait_for_changeset(stack_name=stack_name, cfn_template=yml,
                                                                 parameter_values=[],
                                                                 capabilities=("CAPABILITY_IAM",), role_arn=None,
                                                                 notification_arns=None, tags=tuple())
         except Exception as e:
             logging.error(f"Error creating changeset for cloud formation template: {e}")
             raise e
@@ -48,19 +59,19 @@
 
     def read_secret_arn(self, secret_name: str):
         """"
         Uses Boto3 to retrieve the ARN of a secret.
         """
         logging.debug(f"Reading secret for getting ARN, secret name = {secret_name}, "
                       f"for aws profile {self.aws_profile_for_logging}")
-        client = self._get_aws_client(service_name='secretsmanager')
+        client = self._get_aws_client().create_secretsmanager_service()
 
         try:
-            get_secret_value_response = client.get_secret_value(SecretId=secret_name)
-            return get_secret_value_response["ARN"]
+            secret = client.get_secret_value(secret_id=PhysicalResourceId(secret_name))
+            return secret.arn
         except ClientError as e:
             logging.error("Unable to read secret")
             raise e
 
     def read_dockerhub_secret_arn(self):
         return self.read_secret_arn("Dockerhub")
 
@@ -68,76 +79,73 @@
         """
         This function pushes the YAML to AWS Cloudformation for validation
         (see https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-validate-template.html)
         Pitfall: Boto3 expects the YAML string as parameter, whereas the AWS CLI expects the file URL as parameter.
         It requires to have the AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY env variables set correctly.
         """
         logging.debug(f"Running validate_cloudformation_template for aws profile {self.aws_profile_for_logging}")
-        cloud_client = self._get_aws_client("cloudformation")
-        cloud_client.validate_template(TemplateBody=cloudformation_yml)
-
-    def _get_aws_client(self, service_name: str) -> Any:
-        if self._aws_profile is None:
-            return boto3.client(service_name)
-        aws_session = boto3.session.Session(profile_name=self._aws_profile)
-        return aws_session.client(service_name)
+        client = self._get_aws_client().create_cloudformation_service()
+        client.validate_template(template_body=cloudformation_yml)
 
-    def get_all_stack_resources(self, stack_name: str) -> List[Dict[str, str]]:
+    def get_all_stack_resources(self, stack_name: str) -> List[StackResourceSummary]:
         """
         This functions uses Boto3 to get all AWS Cloudformation resources for a specific Cloudformation stack,
         identified by parameter `stack_name`.
         The AWS API truncates at a size of 1MB, and in order to get all chunks the method must be called
         passing the previous retrieved token until no token is returned.
         """
         logging.debug(f"Running get_all_codebuild_projects for aws profile {self.aws_profile_for_logging}")
-        cf_client = self._get_aws_client('cloudformation')
-        current_result = cf_client.list_stack_resources(StackName=stack_name)
-        result = current_result["StackResourceSummaries"]
-
-        while "nextToken" in current_result:
-            current_result = cf_client.list_projects(StackName=stack_name, nextToken=current_result["nextToken"])
-            result.extend(current_result["StackResourceSummaries"])
+        client = self._get_aws_client().create_cloudformation_service()
+        stack_name_id = PhysicalResourceId(stack_name)
+        current_result = client.list_stack_resources(stack_name=stack_name_id)
+        result = current_result.stack_resource_summaries
+
+        while current_result.next_token is not None:
+            current_result = client.list_stack_resources(stack_name=stack_name_id, next_token=current_result.next_token)
+            result.extend(current_result.stack_resource_summaries)
         return result
 
-    def start_codebuild(self, project: str, environment_variables_overrides: List[Dict[str, str]], branch: str) -> None:
+    def start_codebuild(self,
+                        project: PhysicalResourceId,
+                        environment_variables_overrides: List[Dict[str, str]],
+                        branch: str,
+                        timeout_in_seconds: int,
+                        poll_interval_seconds: int = 30,
+                        sleep_function: Callable[[float], None] = time.sleep) -> None:
         """
         This functions uses Boto3 to start a batch build.
         It forwards all variables from parameter env_variables as environment variables to the CodeBuild project.
         If a branch is given, it starts the codebuild for the given branch.
         After the build has triggered it waits until the batch build finished
         :raises
             `RuntimeError` if build fails or AWS Batch build returns unknown status
         """
-        codebuild_client = self._get_aws_client("codebuild")
+        client = self._get_aws_client().create_codebuild_service()
         logging.info(f"Trigger codebuild for project {project} with branch {branch} "
                      f"and env_variables ({environment_variables_overrides})")
-        ret_val = codebuild_client.start_build_batch(projectName=project,
-                                                     sourceVersion=branch,
-                                                     environmentVariablesOverride=list(
-                                                         environment_variables_overrides))
+        build_batch = client.start_build_batch(project_name=project,
+                                               source_version=branch,
+                                               environment_variables_override=list(
+                                                   environment_variables_overrides))
 
         def wait_for(seconds: int, interval: int) -> Iterable[int]:
             for _ in range(int(seconds / interval)):
                 yield interval
 
-        build_id = ret_val['buildBatch']['id']
+        build_id = build_batch.id
         logging.debug(f"Codebuild for project {project} with branch {branch} triggered. Id is {build_id}.")
-        interval = 30
-        timeout_time_in_seconds = 60 * 60 * 2  # We wait for maximal 2h + (something)
-        for seconds_to_wait in wait_for(seconds=timeout_time_in_seconds, interval=interval):
-            time.sleep(seconds_to_wait)
+        for seconds_to_wait in wait_for(seconds=timeout_in_seconds, interval=poll_interval_seconds):
+            sleep_function(seconds_to_wait)
             logging.debug(f"Checking status of codebuild id {build_id}.")
-            build_response = codebuild_client.batch_get_build_batches(ids=[build_id])
-            logging.debug(f"Build response of codebuild id {build_id} is {build_response}")
-            if len(build_response['buildBatches']) != 1:
-                logging.error(f"Unexpected return value from 'batch_get_build_batches': {build_response}")
-            build_status = build_response['buildBatches'][0]['buildBatchStatus']
+            build_batches = client.batch_get_build_batches(build_batch_ids=[build_id])
+            logging.debug(f"Build response of codebuild id {build_id} is {build_batches}")
+            if len(build_batches) != 1:
+                logging.error(f"Unexpected return value from 'batch_get_build_batches': {build_batches}")
+            build_status = build_batches[0].build_batch_status
             logging.info(f"Build status of codebuild id {build_id} is {build_status}")
-            if build_status == 'SUCCEEDED':
+            if build_status == BuildBatchStatus.SUCCEEDED:
                 break
-            elif build_status in ['FAILED', 'FAULT', 'STOPPED', 'TIMED_OUT']:
-                raise RuntimeError(f"Build ({build_id}) failed with status: {build_status}")
-            elif build_status != "IN_PROGRESS":
-                raise RuntimeError(f"Batch build {build_id} has unknown build status: {build_status}")
+            elif build_status in BUILD_STATUS_FAILURES:
+                raise RuntimeError(f"Build ({build_id}) failed with status: {build_status.name}")
         # if loop does not break early, build wasn't successful
         else:
             raise RuntimeError(f"Batch build {build_id} ran into timeout.")
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/ci_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/ci_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.render_template import render_template
 
 CODE_BUILD_STACK_NAME = "CIBuild"
 CI_CODE_BUILD_TEMPLATE = "slc_code_build.yaml"
 
 CI_BUILD_WEBHOOK_FILTER_PATTERN = \
     r"^refs/heads/(((main|master|develop)$)|" \
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/deployer.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/aws/deployer.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Tuple, List
 
 import jsonschema
 
+from exasol_script_languages_container_ci_setup.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci_setup.lib.render_template import render_template
 
 
 @dataclass(eq=True, frozen=True, order=True)
 class Flavor(object):
     """"
     Holds the name and the formatted name used for generating the buildspec.
@@ -21,30 +22,25 @@
         return self.flavor_original.replace(".", "").replace("-", "_")
 
 
 def validate_config_file(config_file: Optional[str]):
     """
     Validates config file, path given by parameter config_file.
     :raises:
-
-        `jsonschema.exceptions.ValidationError` if the config file has invalid JSON format.
-        `jsonschema.exceptions.SchemaError` if the config file is not in accordance with the the schema.
+        `pydantic.ValidationError` if the config file has invalid JSON format.
         `ValueError` if the ignored path given in the config file does not exist.
     """
     if config_file is None:
         return
-    with open(config_file, "r") as config_file_:
-        config = json.load(config_file_)
-        config_schema = json.loads(render_template("config_schema.json"))
-        jsonschema.validate(instance=config, schema=config_schema)
-        ignored_paths = config["build_ignore"]["ignored_paths"]
-        for ignored_path in ignored_paths:
-            folder_path = Path(ignored_path)
-            if not folder_path.exists():
-                raise ValueError(f"Ignored folder '{ignored_path}' does not exist.")
+    config = Config.parse_file(config_file)
+    ignored_paths = config.build.ignore.paths
+    for ignored_path in ignored_paths:
+        folder_path = Path(ignored_path)
+        if not folder_path.exists():
+            raise ValueError(f"Ignored folder '{ignored_path}' does not exist.")
 
 
 def get_config_file_parameter(config_file: Optional[str]):
     if config_file is None:
         return ""
     return f"--config-file {config_file}"
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/release_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/release_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.render_template import render_template
 
 CODE_BUILD_STACK_NAME = "ReleaseBuild"
 RELEASE_CODEBUILD_TEMPLATE = "slc_code_release_build.yaml"
 
 
 def release_stack_name(project: str):
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import logging
 import re
-from typing import Tuple, Dict, List
+from typing import Tuple, Dict, List, Optional
 
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.wrapper.datamodels.cloudformation import StackResourceSummary
 from exasol_script_languages_container_ci_setup.lib.ci_build import ci_stack_name
+from exasol_script_languages_container_ci_setup.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci_setup.lib.github_draft_release_creator import GithubDraftReleaseCreator
 from exasol_script_languages_container_ci_setup.lib.release_build import release_stack_name
 
+AWS_CODE_BUILD_PROJECT_RESOURCE_TYPE = "AWS::CodeBuild::Project"
+DEFAULT_TIMEOUT = 3 * 60 * 60  # 3 hours
+
 
 def get_environment_variable_override(env_variable: Tuple[str, str]) -> Dict[str, str]:
     return {"name": env_variable[0], "value": env_variable[1], "type": "PLAINTEXT"}
 
 
-def get_aws_codebuild_project(resources: List[Dict[str, str]], project: str) -> Dict[str, str]:
-    matching_project = [resource for resource in resources if resource["ResourceType"] == "AWS::CodeBuild::Project"]
+def get_aws_codebuild_project(resources: List[StackResourceSummary], project: str) -> StackResourceSummary:
+    matching_project = [resource for resource in resources
+                        if resource.resource_type == AWS_CODE_BUILD_PROJECT_RESOURCE_TYPE]
     if len(matching_project) == 0:
         raise ValueError(f"No project deployed for {project}. Found following resources: {resources}")
     if len(matching_project) > 1:
         raise RuntimeError(f"Multiple projects match {project}. Found following matches: {matching_project}")
     return matching_project[0]
 
 
@@ -29,16 +35,33 @@
     """
     res = re.search(r"^https://uploads.github.com/repos/([a-zA-Z0-9\-_/]+)/releases/([\d]+)/assets", upload_url)
     if res is None:
         raise ValueError("Parameter upload_url is in unexpected format.")
     return int(res.groups()[1])
 
 
-def _execute_release_build(aws_access: AwsAccess, project: str, branch: str,
-                           release_id: int, is_dry_run: bool, gh_token: str) -> None:
+def get_timeout_in_seconds(timeout_in_seconds: Optional[int], config_file: Optional[str]) -> int:
+    if timeout_in_seconds is not None:
+        return timeout_in_seconds
+    elif config_file is not None:
+        config = Config.parse_file(config_file)
+        return config.release.timeout_in_minutes
+    else:
+        return DEFAULT_TIMEOUT
+
+
+def _execute_release_build(
+        aws_access: AwsAccess,
+        project: str,
+        branch: str,
+        release_id: int,
+        is_dry_run: bool,
+        gh_token: str,
+        timeout_in_seconds: Optional[int],
+        config_file_path: Optional[str]) -> None:
     """
     This function:
     1. Retrieve resources for the release codebuild stack for that given project
     2. Find the resource with type CodeBuild
     3. Creates the environment variables override
     4. Start and wait for batch build
     :raises:
@@ -57,52 +80,90 @@
     if gh_token is None:
         raise RuntimeError("Parameter gh_token must not be None.")
 
     env_variables = [("RELEASE_ID", f"{release_id}"),
                      ("DRY_RUN", dry_run_value),
                      ("GITHUB_TOKEN", gh_token)]
     environment_variables_overrides = list(map(get_environment_variable_override, env_variables))
-    aws_access.start_codebuild(matching_project["PhysicalResourceId"],
+    timeout_in_seconds = get_timeout_in_seconds(
+        timeout_in_seconds=timeout_in_seconds,
+        config_file=config_file_path)
+    aws_access.start_codebuild(matching_project.physical_resource_id,
                                environment_variables_overrides=environment_variables_overrides,
-                               branch=branch)
+                               branch=branch, timeout_in_seconds=timeout_in_seconds)
 
 
-def run_start_release_build(aws_access: AwsAccess, project: str, upload_url: str, branch: str, gh_token: str) -> None:
+def run_start_release_build(
+        aws_access: AwsAccess,
+        project: str,
+        upload_url: str,
+        branch: str,
+        gh_token: str,
+        timeout_in_seconds: Optional[int],
+        config_file_path: Optional[str]) -> None:
     logging.info(f"run_start_release_build for aws profile {aws_access.aws_profile_for_logging} for project {project} "
                  f"with upload url: {upload_url}")
-    _execute_release_build(aws_access, project, branch, _parse_upload_url(upload_url=upload_url), False, gh_token)
-
-
-def run_start_test_release_build(aws_access: AwsAccess, gh_release_creator: GithubDraftReleaseCreator, repo_name: str,
-                                 project: str, branch: str, release_title: str, gh_token: str) -> None:
+    _execute_release_build(
+        aws_access=aws_access,
+        project=project,
+        branch=branch,
+        release_id=_parse_upload_url(upload_url=upload_url),
+        is_dry_run=False,
+        gh_token=gh_token,
+        timeout_in_seconds=timeout_in_seconds,
+        config_file_path=config_file_path
+    )
+
+
+def run_start_test_release_build(
+        aws_access: AwsAccess,
+        gh_release_creator: GithubDraftReleaseCreator, repo_name: str,
+        project: str,
+        branch: str,
+        release_title: str,
+        gh_token: str,
+        timeout_in_seconds: Optional[int],
+        config_file_path: Optional[str]
+) -> None:
     logging.info(f"run_start_test_release_build for aws profile {aws_access.aws_profile_for_logging} "
                  f"for project {project} for branch: {branch} with title: {release_title}")
     release_id = gh_release_creator.create_release(repo_name, branch, release_title, gh_token)
-    _execute_release_build(aws_access, project, branch, release_id, True, gh_token)
+    _execute_release_build(
+        aws_access=aws_access,
+        project=project,
+        branch=branch,
+        release_id=release_id,
+        is_dry_run=True,
+        gh_token=gh_token,
+        timeout_in_seconds=timeout_in_seconds,
+        config_file_path=config_file_path
+    )
 
 
-def run_start_ci_build(aws_access: AwsAccess, project: str, branch: str) -> None:
+def run_start_ci_build(aws_access: AwsAccess, project: str, branch: str, timeout_in_seconds: int) -> None:
     logging.info(f"run_start_ci_build for aws profile {aws_access.aws_profile_for_logging} for project {project} "
                  f"on branch {branch}")
     """
     This function:
     1. Retrieve resources for the release codebuild stack for that given project
     2. Find the resource with type CodeBuild
     3. Creates the environment variables override
     4. Start and wait for batch build
     :raises:
         `RuntimeError` if build goes wrong or if anything on AWS CodeBuild is not as expected
         `ValueError` if project is not found on AWS CodeBuild or if the upload is not in expected format.
     The upload url is only be used to get the release id.
     """
-    resources = aws_access.get_all_stack_resources(ci_stack_name(project))
+    stack_name = ci_stack_name(project)
+    resources = aws_access.get_all_stack_resources(stack_name)
     matching_project = get_aws_codebuild_project(resources, project)
 
     # AwsAccess.start_codebuild() already indicates the branch (parameter `sourceVersion`)
     # However, additionally we need to override env variable CUSTOM_BRANCH which will
     # be used in the build_buildspec.yaml to forward the branch name to exasol_script_languages_container_ci.run_ci()
     # (which itself uses the parameter to evaluate build strategies)
     env_variables = [("CUSTOM_BRANCH", branch)]
     environment_variables_overrides = list(map(get_environment_variable_override, env_variables))
-    aws_access.start_codebuild(matching_project["PhysicalResourceId"],
+    aws_access.start_codebuild(matching_project.physical_resource_id,
                                environment_variables_overrides=environment_variables_overrides,
-                               branch=branch)
+                               branch=branch,
+                               timeout_in_seconds=timeout_in_seconds)
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from exasol_script_languages_container_ci_setup.lib.aws_access import AwsAccess
+from exasol_script_languages_container_ci_setup.lib.aws.aws_access import AwsAccess
 from exasol_script_languages_container_ci_setup.lib.render_template import render_template
 
 SOURCE_CREDENTIALS_STACK_NAME = "SLCSourceCredentials"
 
 
 def run_deploy_source_credentials(
         aws_access: AwsAccess,
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml` & `exasol_script_languages_container_ci_setup-1.1.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/pyproject.toml` & `exasol_script_languages_container_ci_setup-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci-setup"
-version = "1.0.0"
+version = "1.1.0"
 description = "Manages AWS cloud CI build infrastructure."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 click = "^8.1.3"
 jinja2 = ">=3.1.0"
 exasol_error_reporting_python = "^0.3.0"
-exasol-script-languages-container-ci = "^1.0.0"
-boto3 = "^1.22.0"
+exasol-script-languages-container-ci = "^1.2.0"
+boto3 = "1.26.163"
+botocore = "1.29.163"
 jsonschema = "^4.17.3"
 PyGithub = "^1.55.0"
+datamodel-code-generator = "^0.20.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `exasol-script-languages-container-ci-setup-1.0.0/PKG-INFO` & `exasol_script_languages_container_ci_setup-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-ci-setup
-Version: 1.0.0
+Version: 1.1.0
 Summary: Manages AWS cloud CI build infrastructure.
 License: MIT
 Author: Thomas Uebensee
 Author-email: ext.thomas.uebensee@exasol.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (>=1.55.0,<2.0.0)
-Requires-Dist: boto3 (>=1.22.0,<2.0.0)
+Requires-Dist: boto3 (==1.26.163)
+Requires-Dist: botocore (==1.29.163)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: exasol-script-languages-container-ci (>=1.0.0,<2.0.0)
+Requires-Dist: datamodel-code-generator (>=0.20.0,<0.21.0)
+Requires-Dist: exasol-script-languages-container-ci (>=1.2.0,<2.0.0)
 Requires-Dist: exasol_error_reporting_python (>=0.3.0,<0.4.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
```

