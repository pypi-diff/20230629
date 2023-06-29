# Comparing `tmp/oelint_adv-3.9.3.tar.gz` & `tmp/oelint_adv-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oelint_adv-3.9.3.tar", last modified: Wed Jan  5 12:52:09 2022, max compression
+gzip compressed data, was "oelint_adv-3.9.4.tar", last modified: Sun Jan 16 09:53:18 2022, max compression
```

## Comparing `oelint_adv-3.9.3.tar` & `oelint_adv-3.9.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-05 12:52:09.319595 oelint_adv-3.9.3/
--rw-rw-r--   0 icke      (1000) icke      (1000)     1320 2019-12-27 13:24:23.000000 oelint_adv-3.9.3/LICENSE
--rw-rw-r--   0 icke      (1000) icke      (1000)       59 2020-02-07 18:08:14.000000 oelint_adv-3.9.3/MANIFEST.in
--rw-rw-r--   0 icke      (1000) icke      (1000)    22977 2022-01-05 12:52:09.319595 oelint_adv-3.9.3/PKG-INFO
--rw-rw-r--   0 icke      (1000) icke      (1000)    17590 2021-12-14 10:52:13.000000 oelint_adv-3.9.3/README.md
-drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-05 12:52:09.303595 oelint_adv-3.9.3/oelint_adv/
--rw-rw-r--   0 icke      (1000) icke      (1000)       23 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/__init__.py
--rw-rw-r--   0 icke      (1000) icke      (1000)    12847 2021-12-02 18:46:49.000000 oelint_adv-3.9.3/oelint_adv/__main__.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     8748 2021-11-08 14:28:13.000000 oelint_adv-3.9.3/oelint_adv/cls_rule.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      675 2021-11-04 08:48:45.000000 oelint_adv-3.9.3/oelint_adv/color.py
-drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-05 12:52:09.319595 oelint_adv-3.9.3/oelint_adv/rule_base/
--rw-rw-r--   0 icke      (1000) icke      (1000)        0 2020-02-07 18:08:00.000000 oelint_adv-3.9.3/oelint_adv/rule_base/__init__.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1021 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_append_protvars.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      968 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_include.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      710 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_includevsrequire.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      571 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_nospaces.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1936 2021-12-14 10:50:45.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2443 2021-11-14 09:32:33.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1501 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_signedoff.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2637 2021-12-14 10:45:38.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      966 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_require.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1650 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_underscores.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2147 2021-11-04 12:30:24.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_func_spec.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1360 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_newline_consecutive.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1088 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_newline_end.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1120 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_begin.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1099 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_cont.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      951 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_empty.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1121 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_end.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1049 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_notabs.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1670 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_addnotaskbody.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      687 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_anon_python.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2888 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_customorder.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1225 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_doc_strings.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      870 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_heredocs.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      789 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_multiappends.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      924 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_no_cp.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      668 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_no_mkdir.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      739 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_nopython_prefix.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1538 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_order.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1010 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_python_prefix.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1891 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_appendop.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      731 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_autorev.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      908 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_bbvars.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      932 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_bugtracker_url.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1160 2021-12-08 09:16:33.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_depends_append.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2321 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_depends_ordered.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      963 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_descriptionsame.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      982 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_descriptiontooshort.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      628 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_doublemodify.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2124 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_duplicates.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      833 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesextrapaths.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      792 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesextrapathsop.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      744 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesoverride.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      770 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_homepage.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1495 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_homepageping.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1355 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_inconsspaces.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      689 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_insaneskip.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1172 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_license_remote.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1012 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_licfileprefix.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2127 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_misspell.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1552 2021-10-31 08:45:48.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_multilineindent.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1168 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_notneededspace.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      973 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_p_usage.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1611 2021-10-31 08:45:48.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pkgspecific.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      862 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pn_usage.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      802 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      848 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_quoted.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      840 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_rootfscmd.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1183 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_section_lowercase.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      721 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_spaces_assignment.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2424 2021-11-04 12:30:24.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_spec.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     4970 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1092 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_append.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1153 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_domains.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1445 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_file.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1255 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_gittag.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1741 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1082 2021-11-08 13:53:06.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_wildcard.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      723 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_summary_80chars.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      701 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_summary_linebreaks.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      957 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_trailslash.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1083 2022-01-05 11:24:39.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_bbclassextends.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1431 2021-11-06 12:04:51.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_downloadfilename.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     3019 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_filessetting.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      994 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_improperinherit.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1321 2021-11-14 09:32:33.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_listappend.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1487 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_mandatory_exists.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      869 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_multiinclude.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      916 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_multiinherit.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      774 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_native_filename.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      792 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_nativesdk_filename.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1687 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_order.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     2665 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_pathhardcode.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1265 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_suggested.py
--rw-rw-r--   0 icke      (1000) icke      (1000)     1601 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_variable_override.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      891 2021-11-08 14:30:50.000000 oelint_adv-3.9.3/oelint_adv/rule_file.py
-drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-05 12:52:09.319595 oelint_adv-3.9.3/oelint_adv/rule_jetm/
--rw-rw-r--   0 icke      (1000) icke      (1000)        0 2020-02-07 18:08:00.000000 oelint_adv-3.9.3/oelint_adv/rule_jetm/__init__.py
--rw-rw-r--   0 icke      (1000) icke      (1000)      898 2021-10-27 16:53:15.000000 oelint_adv-3.9.3/oelint_adv/rule_jetm/rule_var_depends_singleline.py
-drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-05 12:52:09.303595 oelint_adv-3.9.3/oelint_adv.egg-info/
--rw-rw-r--   0 icke      (1000) icke      (1000)    22977 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/PKG-INFO
--rw-rw-r--   0 icke      (1000) icke      (1000)     4434 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/SOURCES.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)        1 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/dependency_links.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)       57 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/entry_points.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)       96 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/requires.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)       11 2022-01-05 12:52:09.000000 oelint_adv-3.9.3/oelint_adv.egg-info/top_level.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)       99 2021-11-04 12:30:06.000000 oelint_adv-3.9.3/requirements.txt
--rw-rw-r--   0 icke      (1000) icke      (1000)     1014 2022-01-05 12:52:09.323595 oelint_adv-3.9.3/setup.cfg
--rw-rw-r--   0 icke      (1000) icke      (1000)     1786 2022-01-05 12:31:26.000000 oelint_adv-3.9.3/setup.py
+drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-16 09:53:18.384067 oelint_adv-3.9.4/
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1320 2019-12-27 13:24:23.000000 oelint_adv-3.9.4/LICENSE
+-rw-rw-r--   0 icke      (1000) icke      (1000)       59 2020-02-07 18:08:14.000000 oelint_adv-3.9.4/MANIFEST.in
+-rw-rw-r--   0 icke      (1000) icke      (1000)    22977 2022-01-16 09:53:18.384067 oelint_adv-3.9.4/PKG-INFO
+-rw-rw-r--   0 icke      (1000) icke      (1000)    17590 2021-12-14 10:52:13.000000 oelint_adv-3.9.4/README.md
+drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-16 09:53:18.356068 oelint_adv-3.9.4/oelint_adv/
+-rw-rw-r--   0 icke      (1000) icke      (1000)       23 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/__init__.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)    12847 2021-12-02 18:46:49.000000 oelint_adv-3.9.4/oelint_adv/__main__.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     8748 2021-11-08 14:28:13.000000 oelint_adv-3.9.4/oelint_adv/cls_rule.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      675 2021-11-04 08:48:45.000000 oelint_adv-3.9.4/oelint_adv/color.py
+drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-16 09:53:18.384067 oelint_adv-3.9.4/oelint_adv/rule_base/
+-rw-rw-r--   0 icke      (1000) icke      (1000)        0 2020-02-07 18:08:00.000000 oelint_adv-3.9.4/oelint_adv/rule_base/__init__.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1021 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_append_protvars.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      968 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_include.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      710 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_includevsrequire.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      571 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_nospaces.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1936 2021-12-14 10:50:45.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2443 2021-11-14 09:32:33.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1501 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_signedoff.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2637 2021-12-14 10:45:38.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      966 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_require.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1650 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_underscores.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2147 2021-11-04 12:30:24.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_func_spec.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1360 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_newline_consecutive.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1088 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_newline_end.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1120 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_begin.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1099 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_cont.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      951 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_empty.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1121 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_end.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1049 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_notabs.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1670 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_addnotaskbody.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      687 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_anon_python.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2888 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_customorder.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1225 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_doc_strings.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      870 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_heredocs.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      789 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_multiappends.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      924 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_no_cp.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      668 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_no_mkdir.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      739 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_nopython_prefix.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1538 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_order.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1010 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_python_prefix.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1891 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_appendop.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      731 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_autorev.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      908 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_bbvars.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      932 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_bugtracker_url.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1160 2021-12-08 09:16:33.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_depends_append.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2321 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_depends_ordered.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      963 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_descriptionsame.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      982 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_descriptiontooshort.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      628 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_doublemodify.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2124 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_duplicates.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      833 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesextrapaths.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      792 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesextrapathsop.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      744 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesoverride.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      770 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_homepage.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1495 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_homepageping.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1355 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_inconsspaces.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      689 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_insaneskip.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1172 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_license_remote.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1012 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_licfileprefix.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2127 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_misspell.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1552 2021-10-31 08:45:48.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_multilineindent.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1168 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_notneededspace.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      973 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_p_usage.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1611 2021-10-31 08:45:48.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pkgspecific.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      862 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pn_usage.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      802 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      942 2022-01-16 09:53:05.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_quoted.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      840 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_rootfscmd.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1183 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_section_lowercase.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      721 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_spaces_assignment.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2424 2021-11-04 12:30:24.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_spec.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     4970 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1092 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_append.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1153 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_domains.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1445 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_file.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1255 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_gittag.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1741 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1082 2021-11-08 13:53:06.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_wildcard.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      723 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_summary_80chars.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      701 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_summary_linebreaks.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      957 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_trailslash.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1083 2022-01-05 11:24:39.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_bbclassextends.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1431 2021-11-06 12:04:51.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_downloadfilename.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     3019 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_filessetting.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      994 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_improperinherit.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1321 2021-11-14 09:32:33.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_listappend.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1487 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_mandatory_exists.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      869 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_multiinclude.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      916 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_multiinherit.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      774 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_native_filename.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      792 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_nativesdk_filename.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1687 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_order.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     2665 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_pathhardcode.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1265 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_suggested.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1601 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_variable_override.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      891 2021-11-08 14:30:50.000000 oelint_adv-3.9.4/oelint_adv/rule_file.py
+drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-16 09:53:18.384067 oelint_adv-3.9.4/oelint_adv/rule_jetm/
+-rw-rw-r--   0 icke      (1000) icke      (1000)        0 2020-02-07 18:08:00.000000 oelint_adv-3.9.4/oelint_adv/rule_jetm/__init__.py
+-rw-rw-r--   0 icke      (1000) icke      (1000)      898 2021-10-27 16:53:15.000000 oelint_adv-3.9.4/oelint_adv/rule_jetm/rule_var_depends_singleline.py
+drwxrwxr-x   0 icke      (1000) icke      (1000)        0 2022-01-16 09:53:18.356068 oelint_adv-3.9.4/oelint_adv.egg-info/
+-rw-rw-r--   0 icke      (1000) icke      (1000)    22977 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/PKG-INFO
+-rw-rw-r--   0 icke      (1000) icke      (1000)     4434 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/SOURCES.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)        1 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/dependency_links.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)       57 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/entry_points.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)       96 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/requires.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)       11 2022-01-16 09:53:18.000000 oelint_adv-3.9.4/oelint_adv.egg-info/top_level.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)       99 2021-11-04 12:30:06.000000 oelint_adv-3.9.4/requirements.txt
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1014 2022-01-16 09:53:18.384067 oelint_adv-3.9.4/setup.cfg
+-rw-rw-r--   0 icke      (1000) icke      (1000)     1786 2022-01-16 09:53:13.000000 oelint_adv-3.9.4/setup.py
```

### Comparing `oelint_adv-3.9.3/LICENSE` & `oelint_adv-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/PKG-INFO` & `oelint_adv-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint_adv
-Version: 3.9.3
+Version: 3.9.4
 Summary: Advanced bitbake-recipe linter
 Home-page: https://github.com/priv-kweihmann/oelint-adv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Description: oelint-adv
         ==========
```

### Comparing `oelint_adv-3.9.3/README.md` & `oelint_adv-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/__main__.py` & `oelint_adv-3.9.4/oelint_adv/__main__.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/cls_rule.py` & `oelint_adv-3.9.4/oelint_adv/cls_rule.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/color.py` & `oelint_adv-3.9.4/oelint_adv/color.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_append_protvars.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_append_protvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_include.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_include.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_includevsrequire.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_includevsrequire.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_nospaces.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_nospaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_signedoff.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_signedoff.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_require.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_require.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_file_underscores.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_file_underscores.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_func_spec.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_func_spec.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_newline_consecutive.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_newline_consecutive.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_newline_end.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_newline_end.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_begin.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_begin.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_cont.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_cont.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_empty.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_empty.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_nospace_line_end.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_nospace_line_end.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_notabs.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_notabs.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_addnotaskbody.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_addnotaskbody.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_anon_python.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_anon_python.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_customorder.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_customorder.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_doc_strings.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_doc_strings.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_heredocs.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_heredocs.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_multiappends.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_multiappends.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_no_cp.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_no_cp.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_no_mkdir.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_no_mkdir.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_nopython_prefix.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_nopython_prefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_order.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_order.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_tasks_python_prefix.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_tasks_python_prefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_appendop.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_appendop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_autorev.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_autorev.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_bbvars.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_bbvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_bugtracker_url.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_bugtracker_url.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_depends_append.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_depends_append.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_depends_ordered.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_depends_ordered.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_descriptionsame.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_descriptionsame.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_descriptiontooshort.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_descriptiontooshort.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_doublemodify.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_doublemodify.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_duplicates.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_duplicates.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesextrapaths.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesextrapaths.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesextrapathsop.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesextrapathsop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_filesoverride.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_filesoverride.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_homepage.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_homepage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_homepageping.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_homepageping.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_inconsspaces.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_inconsspaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_insaneskip.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_insaneskip.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_license_remote.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_license_remote.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_licfileprefix.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_licfileprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_misspell.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_misspell.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_multilineindent.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_multilineindent.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_notneededspace.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_notneededspace.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_p_usage.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_p_usage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pkgspecific.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pkgspecific.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pn_usage.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pn_usage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_quoted.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_quoted.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,10 +14,11 @@
             filename=_file, classifier=Variable.CLASSIFIER)
         for i in items:
             if i.VarName == 'inherit':
                 continue
             # Don't use VarValueStripped here as we explicitly want the quotes
             # at the beginning and the end of the value
             val = i.VarValue.strip()
-            if not val.startswith('"') or not val.endswith('"'):
+            if ((not val.startswith('"') or not val.endswith('"'))
+                    and (not val.startswith('\'') or not val.endswith('\''))): # noqa: W503
                 res += self.finding(i.Origin, i.InFileLine)
         return res
```

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_rootfscmd.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_rootfscmd.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_section_lowercase.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_section_lowercase.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_spaces_assignment.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_spaces_assignment.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_spec.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_spec.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_append.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_append.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_domains.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_domains.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_file.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_file.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_gittag.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_gittag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_src_uri_wildcard.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_src_uri_wildcard.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_summary_80chars.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_summary_80chars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_summary_linebreaks.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_summary_linebreaks.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_var_trailslash.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_var_trailslash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_bbclassextends.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_bbclassextends.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_downloadfilename.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_downloadfilename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_filessetting.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_filessetting.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_improperinherit.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_improperinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_listappend.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_listappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_mandatory_exists.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_mandatory_exists.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_multiinclude.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_multiinclude.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_multiinherit.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_multiinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_native_filename.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_native_filename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_nativesdk_filename.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_nativesdk_filename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_order.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_order.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_pathhardcode.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_pathhardcode.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_suggested.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_suggested.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_base/rule_vars_variable_override.py` & `oelint_adv-3.9.4/oelint_adv/rule_base/rule_vars_variable_override.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_file.py` & `oelint_adv-3.9.4/oelint_adv/rule_file.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv/rule_jetm/rule_var_depends_singleline.py` & `oelint_adv-3.9.4/oelint_adv/rule_jetm/rule_var_depends_singleline.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/oelint_adv.egg-info/PKG-INFO` & `oelint_adv-3.9.4/oelint_adv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint-adv
-Version: 3.9.3
+Version: 3.9.4
 Summary: Advanced bitbake-recipe linter
 Home-page: https://github.com/priv-kweihmann/oelint-adv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Description: oelint-adv
         ==========
```

### Comparing `oelint_adv-3.9.3/oelint_adv.egg-info/SOURCES.txt` & `oelint_adv-3.9.4/oelint_adv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/setup.cfg` & `oelint_adv-3.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `oelint_adv-3.9.3/setup.py` & `oelint_adv-3.9.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='oelint_adv',
-    version='3.9.3',
+    version='3.9.4',
     author='Konrad Weihmann',
     author_email='kweihmann@outlook.com',
     description='Advanced bitbake-recipe linter',
     long_description=_long_description,
     long_description_content_type=_long_description_content_type,
     url='https://github.com/priv-kweihmann/oelint-adv',
     packages=setuptools.find_packages(exclude=('tests',)),
```

