# Comparing `tmp/troubadix-23.6.2.tar.gz` & `tmp/troubadix-23.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.6.2.tar", max compression
+gzip compressed data, was "troubadix-23.6.3.tar", max compression
```

## Comparing `troubadix-23.6.2.tar` & `troubadix-23.6.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    35149 2023-06-20 14:44:19.581933 troubadix-23.6.2/LICENSE
--rw-r--r--   0        0        0     2730 2023-06-20 14:44:19.581933 troubadix-23.6.2/README.md
--rw-r--r--   0        0        0     2516 2023-06-20 14:44:19.585933 troubadix-23.6.2/pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2450 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     6010 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   124978 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8566 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4043 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2172 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9557 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/troubadix.py
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-29 07:15:50.444448 troubadix-23.6.3/LICENSE
+-rw-r--r--   0        0        0     2730 2023-06-29 07:15:50.444448 troubadix-23.6.3/README.md
+-rw-r--r--   0        0        0     2516 2023-06-29 07:15:50.448448 troubadix-23.6.3/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2450 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-06-29 07:15:50.448448 troubadix-23.6.3/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-06-29 07:15:50.452448 troubadix-23.6.3/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   125168 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4507 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8566 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-06-29 07:15:50.452448 troubadix-23.6.3/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3790 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4043 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9557 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-06-29 07:15:50.456448 troubadix-23.6.3/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.3/PKG-INFO
```

### Comparing `troubadix-23.6.2/LICENSE` & `troubadix-23.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/README.md` & `troubadix-23.6.3/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/pyproject.toml` & `troubadix-23.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.6.2"
+version = "23.6.3"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.6.2/tests/__init__.py` & `troubadix-23.6.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/helper/__init__.py` & `troubadix-23.6.3/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.6.3/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/helper/test_patterns.py` & `troubadix-23.6.3/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/__init__.py` & `troubadix-23.6.3/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/fail.nasl` & `troubadix-23.6.3/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/fail2.nasl` & `troubadix-23.6.3/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test.nasl` & `troubadix-23.6.3/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_badwords.py` & `troubadix-23.6.3/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_copyright_text.py` & `troubadix-23.6.3/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_copyright_year.py` & `troubadix-23.6.3/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_creation_date.py` & `troubadix-23.6.3/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_cve_format.py` & `troubadix-23.6.3/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_cvss_format.py` & `troubadix-23.6.3/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_dependencies.py` & `troubadix-23.6.3/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_dependency_category_order.py` & `troubadix-23.6.3/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.6.3/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_deprecated_functions.py` & `troubadix-23.6.3/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_double_end_points.py` & `troubadix-23.6.3/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_duplicate_oid.py` & `troubadix-23.6.3/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.6.3/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_encoding.py` & `troubadix-23.6.3/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.6.3/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.3/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.6.3/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.6.3/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.6.3/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.6.3/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.6.3/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.6.3/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.6.3/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_grammar.py` & `troubadix-23.6.3/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.6.3/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_illegal_characters.py` & `troubadix-23.6.3/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_log_messages.py` & `troubadix-23.6.3/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.6.3/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.6.3/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.6.3/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.6.3/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_newlines.py` & `troubadix-23.6.3/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.6.3/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.3/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_qod.py` & `troubadix-23.6.3/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_reporting_consistency.py` & `troubadix-23.6.3/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.6.3/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.6.3/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.6.3/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_category.py` & `troubadix-23.6.3/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_copyright.py` & `troubadix-23.6.3/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_family.py` & `troubadix-23.6.3/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_tag_form.py` & `troubadix-23.6.3/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.6.3/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.6.3/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.6.3/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_xref_form.py` & `troubadix-23.6.3/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_script_xref_url.py` & `troubadix-23.6.3/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_security_messages.py` & `troubadix-23.6.3/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.6.3/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_solution_text.py` & `troubadix-23.6.3/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_solution_type.py` & `troubadix-23.6.3/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_spelling.py` & `troubadix-23.6.3/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_tabs.py` & `troubadix-23.6.3/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_todo_tbd.py` & `troubadix-23.6.3/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.6.3/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_using_display.py` & `troubadix-23.6.3/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_valid_oid.py` & `troubadix-23.6.3/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.6.3/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.6.3/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/plugins/test_vt_placement.py` & `troubadix-23.6.3/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/__init__.py` & `troubadix-23.6.3/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.6.3/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.6.3/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.6.3/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.6.3/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.6.3/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.6.3/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_argparser.py` & `troubadix-23.6.3/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_helper.py` & `troubadix-23.6.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_naslinter.py` & `troubadix-23.6.3/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_reporter.py` & `troubadix-23.6.3/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_results.py` & `troubadix-23.6.3/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/tests/test_runner.py` & `troubadix-23.6.3/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/__init__.py` & `troubadix-23.6.3/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/argparser.py` & `troubadix-23.6.3/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/codespell/codespell.exclude` & `troubadix-23.6.3/troubadix/codespell/codespell.exclude`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # 0x00:  01 67 65 74 6E 61 6D 65 69 6E 66 6F 3A 20 54 65    .getnameinfo: Te
 # 0x0010:  73 65 72 20 20 20 20 20 20 48 6F 73 74 28 73 29    ser      Host(s)
 # 0x0020:  0D 0A 46 72 6F 6D 3A 20 3C 73 69 70 3A 6D 69 73    ..From: <sip:mis
 # 0x00E0:  74 65 20 69 6E 64 65 78 20 69 68 61 76 65 20 64    te index ihave d
 # 0x00F0:  75 70 6C 69 63 61 74 65 20 6D 69 6D 65 20 66 6F    uplicate mime fo
 # 0x01D0:  45 20 63 6F 6D 6D 61 6E 64 20 72 65 63 65 69 76    E command receiv
                    0x02,			# ByteOrder (little endian)
+# 0x06B0:  0B A5 3D 1F FF AC 6A C7 1E 4A 4A 84 6E 44 FF 6A    ..=...j..JJ.nD.j
 # 0x10:  70 65 63 69 66 69 65 64 20 75 73 65 72 2E 0D 0A    pecified user...
 # 0x20:  64 79 0D 0A 45 52 52 4F 52 20 43 6F 6D 6D 61 6E    dy..ERROR Comman
 # 0x20:  6D 65 73 73 61 67 65 2E 48 61 6E 64 73 68 61 6B    message.Handshak
 # 0x50:  72 6F 2E 70 72 6F 64 75 63 74 2E 64 65 76 69 63    ro.product.devic
 # 0x50:  A1 37 43 6F 6E 6E 65 63 74 69 6F 6E 20 66 72 6F    .7Connection fro
 #0x60:  AC 13 28 D3 B3 A5 BA F0 FD D6 FA 22 BF 4D F2 4D    ..(........".M.M
   10001 from WAN (if port-forwarding is enabled to allow remote configuration, then it is a good
@@ -164,15 +165,14 @@
 cgi[29] = "fom.cgi";         cve[29] = "CVE-2002-0230";
 "cgi-bin/fom",
 cgis[i++] = "/aktivate/cgi-bin/catgy.cgi";
 cgis[i++] = "/cgi-bin/fom.cgi";
 cgis[i++] = "/cgi-bin/fom/fom.cgi";
  - chage gives correct information (#216635)
 "chage --inactive <DAYS> <USER> for existing users.';
-# Charles Thier <cthier@thethiers.net>
         check_matches = re.finditer('[^\r\n]*[#]+[ ]*([Tt]hunderbird|[Ss]ea[Mm]onkey|[Hh]ot[Ff]ix|[Ff]irefox|[Pp]ower[Pp]oint( Viewer)?)[ ]*[Cc]heck[^\r\n]*\n', text)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt (server auth)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt server auth
 Christian Loos discovered an information disclosure flaw which may reveal RSS feeds URLs, and thus ticket data.
 Christian Loos discovered a remote denial of service vulnerability, exploitable via the email gateway and affecting any installation which accepts mail from untrusted sources. Depending on RT's logging configuration, a remote attacker can take advantage of this flaw to cause CPU and excessive disk usage.
 chunks in CAF audio files. If a user or automated system were tricked into
   Cisco ACI Multi-Site Orchestrator (MSO) to send a specific API request to a managed Cisco APIC or
@@ -193,16 +193,14 @@
   common_files_dir_id = 'oval:org.mitre.oval:obj:281';
 # Comparison Engine Power 'product.comparision.php' SQL Injection Vulnerability
 complete_xml = string (complete_xml, '<oval_system_characteristics xmlns="http://oval.mitre.org/XMLSchema/oval-system-characteristics-5" xmlns:ind-sc="http://oval.mitre.org/XMLSchema/oval-system-characteristics-5#independent" xmlns:oval="http://oval.mitre.org/XMLSchema/oval-common-5" xmlns:oval-sc="http://oval.mitre.org/XMLSchema/oval-system-characteristics-5" xmlns:win-sc="http://oval.mitre.org/XMLSchema/oval-system-characteristics-5#windows" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://oval.mitre.org/XMLSchema/oval-system-characteristics-5 oval-system-characteristics-schema.xsd http://oval.mitre.org/XMLSchema/oval-common-5 oval-common-schema.xsd http://oval.mitre.org/XMLSchema/oval-system-characteristics-5#windows windows-system-characteristics-schema.xsd http://oval.mitre.org/XMLSchema/oval-system-characteristics-5#independent independent-system-characteristics-schema.xsd">');
 "config.sys", "io.sys", "msdos.sys", "pagefile.sys",
   "Connection: TE, close\r\n",
                   "Connection: TE,,Keep-Alive\r\n\r\n" );
   control of Cisco Nexus 9000 Series Fabric Switches in Application Centric Infrastructure (ACI)
-# Copyright (C) 2005 Charles Thier
-# Copyright (C) 2005 Holm Diening / SLITE IT-Security (holm.diening@slite.de)
 # Copyright (c) 2008 Tim Brown
 # Copyright (C) 2008 Tim Brown
 # Copyright (c) 2008 Tim Brown and Portcullis Computer Security Ltd
 # Copyright (c) 2009 Tim Brown
 # Copyright (C) 2009 Tim Brown
 # Copyright (c) 2009 Tim Brown and Portcullis Computer Security Ltd
 Corrected a badly constracted file which could have allowed treating of
@@ -400,15 +398,14 @@
     guess += '\n- Huawei TE Device';
 "hanlder\n",
  have resul... [Please see the references for more information on the vulnerabilities]");
  * Heap-based buffer overflow when scanning crypted PE files
 Helin, Andre Bargull, Massimiliano Tomassoli, laf.intel, Massimiliano
   hello_data += clen + _ciphers;
 "H", "HSI",
-# Holm Diening / SLITE IT-Security (holm.diening@slite.de)
   - HP Helion Eucalyptus does not correctly check IAM user's permissions for accessing versioned objects and ACLs.
     hp_printer['login_success'] = '<?hp te.includeSubPage';
 # <HTML>Acess not granted.</HTML>
 # <HTML>Acess to resource EDITION not granted.</HTML>
 # http://nto.github.io/AirPlay.html#video-httprequests
         - https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-
 # Huawei TE Device Detection
@@ -763,14 +760,15 @@
   script_add_preference(name:"Install hash test Programm on the Target", type:"checkbox", value:"no", id:2);
   script_add_preference(name:"Mark unrechable Hosts as dead (not scanning)", type:"checkbox", value:"yes", id:5); # nb: Don't change this name and id, these are hardcoded / used in GVMd
   script_add_preference(name:"Network type", type:"radio", value:"Mixed (use RFC 1918);Private LAN;Public WAN (Internet);Public LAN", id:8);
   script_add_preference(name:"No ARP or ND Ping", type:"checkbox", value:"no", id:25);
   script_add_preference(name:"Report about unrechable Hosts", type:"checkbox", value:"no", id:6);
   script_add_preference(name:"Value", type:"entry", value:"O:BAG:BAD:(A;;RC;;;BA)", id:1);
   script_copyright("Copyright (C) 2005 Charles Thier");
+  script_copyright("Copyright (C) 2005 Holm Diening / SLITE IT-Security");
   script_copyright("Copyright (C) 2008 E-Soft Inc. http://www.securityspace.com & Tim Brown");
   script_copyright("Copyright (C) 2008 Tim Brown and Vlatko Kosturjak");
   script_copyright("Copyright (C) 2009 Tim Brown");
   script_copyright("(c) Tim Brown and Portcullis Computer Security Ltd, 2008");
   script_mandatory_keys("AAS/banner");
   script_mandatory_keys("aas/detected");
   script_mandatory_keys("Jasig CAS server/Installed");
@@ -810,14 +808,15 @@
   script_name("Kaseya VAS ConntectWise ManagedITSync RCE Vulnerability");
   script_name("Kaseya VAS PowerShell Execution Vulnerability");
   script_name("Kubernetes Dashboard Public WAN (Internet) / Public LAN Accessible");
   script_name("Mesosphere Marathon Web UI Public WAN (Internet) / Public LAN Accessible");
   script_name("Nidesoft MP3 Converter SEH Local Buffer Overflow Vulnerability - Windows");
   script_name("Palo Alto PAN-OS SD WAN Vulnerability (CVE-2020-2009)");
   script_name("Petite Annonce <= 1.0 'categoriemoteur' XSS Vulnerability");
+  script_name("Schneider Electric PowerLogic ION7400 / PM8000 / ION9000 Unsecure Protocol Vulnerability (SEVD-2023-129-03, OT:ICEFALL)");
   script_name("Siemens SICWEB Auto-Logon on Public WAN (Internet) / Public LAN (HTTP)");
   script_name("Sphinx Search Server Public WAN (Internet) / Public LAN Accessible");
   script_name("Swarmpit Web UI Public WAN (Internet) / Public LAN Accessible");
   script_name("WAN Emulator Remote Command Execution Vulnerabilities");
   script_name("Wiesemann & Theis GmbH W&T OPC Server Version Detection (Windows)");
   script_name("Wireshark Steam IHS Discovery/CoAP Dissector DoS Vulnerabilities (Mac OS X)");
   script_name("Wireshark Steam IHS Discovery/CoAP Dissector DoS Vulnerabilities (Windows)");
@@ -1062,14 +1061,16 @@
 solution = "Ensure the SSLCipherSuite includes all of the following:!NULL:!SSLv2:!RC4:!aNULL:!3DES:!IDEA values.
 solution = "Ensure the SSLCipherSuite includes all of the following:!NULL:!SSLv2:!RC4:!aNULL values.
 solution = "mount -o remount,ro PARTITION";
  * some OSCP improvments
 Soyeon Park and Wen Xu discovered a type error in the v8 javascript
 Soyeon Park and Wen Xu discovered memory corruption issues that
 Soyeon Park and Wen Xu discovered the use of a wrong type in the v8
+# SPDX-FileCopyrightText: 2005 Charles Thier
+# SPDX-FileCopyrightText: 2005 Holm Diening / SLITE IT-Security
 specially crafted IPv6 Neighbor Discovery (ND) packet destined to an EX Series Ethernet Switches to cause a slow
  Specially crafted MIME headers could cause openssl's ans1 parser to dereference a NULL pointer leading to a Denial of Service (CVE-2006-7250) or fail verfication
  * Specially crafted MIME headers could cause OpenSSL's ans1 parser to dereference a NULL pointer leading to a Denial of Service (CVE-2006-7250) or fail verfication
  spurrious errors due to Go returning -EINTR from I/O syscalls much more
 SSLCipherSuite ALL:!EXP:!NULL:!LOW:!SSLv2:!RC4:!aNULL";
 SSLCipherSuite ALL:!EXP:!NULL:!LOW:!SSLv2:!RC4:!aNULL:!3DES:!IDEA";
  stack oveflow allowing local root escalation (bsc#1130116).");
```

### Comparing `troubadix-23.6.2/troubadix/codespell/codespell.ignore` & `troubadix-23.6.3/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/helper/__init__.py` & `troubadix-23.6.3/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/helper/helper.py` & `troubadix-23.6.3/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.6.3/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/helper/patterns.py` & `troubadix-23.6.3/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugin.py` & `troubadix-23.6.3/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/__init__.py` & `troubadix-23.6.3/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/badwords.py` & `troubadix-23.6.3/troubadix/plugins/badwords.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,20 +27,17 @@
 # hexstr(openvas) = '6f70656e766173'
 DEFAULT_BADWORDS = [
     "cracker",
     "openvas",
     "OpenVAS",
     "4f70656e564153",
     "6f70656e766173",
-    # nb:
-    # - VT should be used instead
-    # - using a space before/after to make the check a little bit more strict
-    # - this could be made less strict later once the whole feed is "clean"
-    "NVT ",
-    " NVT",
+    # nb: VT/vt should be used instead
+    "NVT",
+    "nvt",
 ]
 
 _IGNORE_FILES = [
     "gb_openvas",
     "gb_gsa_",
     "http_func.inc",
     "misc_func.inc",
@@ -82,25 +79,38 @@
     "openvas_1808149858",
     "evil.zip -> openvas.jsp",
     'url = "/openvas.jsp";',
     'if( "OpenVAS RCE Test" >< buf )',
     'the file "/openvas.jsp" was created',
     "/var/lib/openvas/plugins/",
     "INVT ",  # INVT Electric VT Designer
+    "invt_",  # cpe:/a:invt_electric
     "HostDetails/NVT",  # Can't be changed right now...
+    "# LSS-NVT-",  # Identifier from a third-party which shouldn't be changed
+    ", nvt:",  # Can't be changed right now...
+    "Hu1nvt5qm",  # Part of a bigger blob
+    "gz3nvtPjk",  # Same as above
+    "0EAnvtBAK",  # Same as above
 ]
 
 STARTS_WITH_EXCEPTIONS = [
     "# OpenVAS Vulnerability Test",
     "# OpenVAS Include File",
     "  script_",
     "# $Id: ",
 ]
 
-COMBINED = [("find_service3.nasl", "OpenVAS-")]
+COMBINED = [
+    ("find_service3.nasl", "OpenVAS-"),
+    # nb:
+    # - Only used as variables/function parameters and not user facing
+    # - Will be changed in one go in the future and we don't need to
+    #   report this on every plugin run
+    ("host_details.inc", "nvt"),
+]
 
 
 class CheckBadwords(LineContentPlugin):
     """This plugin checks the passed VT for the use of any of
     the defined badwords. An error will be thrown if the VT contains
     such a badword.
     """
```

### Comparing `troubadix-23.6.2/troubadix/plugins/copyright_text.py` & `troubadix-23.6.3/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/copyright_year.py` & `troubadix-23.6.3/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/creation_date.py` & `troubadix-23.6.3/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/cve_format.py` & `troubadix-23.6.3/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/cvss_format.py` & `troubadix-23.6.3/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/dependencies.py` & `troubadix-23.6.3/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/dependency_category_order.py` & `troubadix-23.6.3/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.6.3/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/deprecated_functions.py` & `troubadix-23.6.3/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/double_end_points.py` & `troubadix-23.6.3/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/duplicate_oid.py` & `troubadix-23.6.3/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.6.3/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/encoding.py` & `troubadix-23.6.3/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.6.3/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.6.3/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/grammar.py` & `troubadix-23.6.3/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.6.3/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/illegal_characters.py` & `troubadix-23.6.3/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/log_messages.py` & `troubadix-23.6.3/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.6.3/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.6.3/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.6.3/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.6.3/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/newlines.py` & `troubadix-23.6.3/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.6.3/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.3/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/qod.py` & `troubadix-23.6.3/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/reporting_consistency.py` & `troubadix-23.6.3/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.6.3/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.6.3/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.6.3/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_category.py` & `troubadix-23.6.3/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_copyright.py` & `troubadix-23.6.3/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_family.py` & `troubadix-23.6.3/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_tag_form.py` & `troubadix-23.6.3/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.6.3/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.6.3/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.6.3/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_xref_form.py` & `troubadix-23.6.3/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/script_xref_url.py` & `troubadix-23.6.3/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/security_messages.py` & `troubadix-23.6.3/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.6.3/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/solution_text.py` & `troubadix-23.6.3/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/solution_type.py` & `troubadix-23.6.3/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/spelling.py` & `troubadix-23.6.3/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/tabs.py` & `troubadix-23.6.3/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/todo_tbd.py` & `troubadix-23.6.3/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.6.3/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/using_display.py` & `troubadix-23.6.3/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/valid_oid.py` & `troubadix-23.6.3/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.6.3/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.6.3/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.6.3/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/plugins/vt_placement.py` & `troubadix-23.6.3/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/reporter.py` & `troubadix-23.6.3/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/results.py` & `troubadix-23.6.3/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/runner.py` & `troubadix-23.6.3/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-23.6.3/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.6.3/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/common.py` & `troubadix-23.6.3/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.6.3/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.6.3/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.6.3/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/troubadix/troubadix.py` & `troubadix-23.6.3/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.2/PKG-INFO` & `troubadix-23.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.6.2
+Version: 23.6.3
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

