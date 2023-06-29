# Comparing `tmp/cumulus_library-0.3.1.tar.gz` & `tmp/cumulus_library-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.3.1.tar` & `cumulus_library-0.3.2.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-lrwxr-xr-x   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      421 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/README.md
--rw-r--r--   0        0        0      866 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11070 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/cli.py
--rw-r--r--   0        0        0     5129 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      272 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5876 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2962 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2857 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3294 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4126 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      673 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1231 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2874 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1691 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     2241 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/patient_extensions.py
--rw-r--r--   0        0        0     1426 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      824 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 26867633 2023-06-21 20:33:20.963716 cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD10.bsv
--rw-r--r--   0        0        0  2988766 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD9.bsv
--rw-r--r--   0        0        0      394 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4824 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16059 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/study_parser.py
--rw-r--r--   0        0        0      577 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1800 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     6517 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2618 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/upload.py
--rw-r--r--   0        0        0     1586 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 cumulus_library-0.3.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-29 19:41:10.761678 cumulus_library-0.3.2/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      587 2023-06-29 19:41:10.761678 cumulus_library-0.3.2/README.md
+-rw-r--r--   0        0        0      963 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       45 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    11182 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5249 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5876 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2549 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2688 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/condition_codable_concept.sql
+-rw-r--r--   0        0        0     4176 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/denormalizer.py
+-rw-r--r--   0        0        0     2857 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3294 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4126 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      661 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1231 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1691 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     6521 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/patient_extensions.sql
+-rw-r--r--   0        0        0     1426 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-06-29 19:41:10.765678 cumulus_library-0.3.2/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2023-06-29 19:41:10.805678 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2023-06-29 19:41:10.905679 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      394 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4643 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16059 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0     1353 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0      577 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1798 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     7462 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2664 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1588 2023-06-29 19:41:10.913679 cumulus_library-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cumulus_library-0.3.2/PKG-INFO
```

### Comparing `cumulus_library-0.3.1/cumulus_library/.sqlfluff` & `cumulus_library-0.3.2/cumulus_library/.sqlfluff`

 * *Files 20% similar despite different names*

```diff
@@ -27,8 +27,10 @@
 view_cols = ["c","d"]
 col_type_list = ["a string","b string"]
 source_table = source_table
 source_id = source_id
 target_table = target_table
 target_col_prefix = prefix
 fhir_extension = fhir_extension
-code_systems = ["omb", "text"]
+ext_systems = ["omb", "text"]
+code_systems = ["http://snomed.info/sct", "http://hl7.org/fhir/sid/icd-10-cm"]
+cc_column = 'code'
```

### Comparing `cumulus_library-0.3.1/cumulus_library/base_runner.py` & `cumulus_library-0.3.2/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/cli.py` & `cumulus_library-0.3.2/cumulus_library/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path, PosixPath
 from typing import Dict, List, Optional
 
 import pyathena
 
 from pyathena.pandas.cursor import PandasCursor
 
+from cumulus_library import __version__
 from cumulus_library.cli_parser import get_parser
 from cumulus_library.study_parser import StudyManifestParser
 from cumulus_library.upload import upload_files
 
 
 # ** Don't delete! **
 # This class isn't used in the rest of the code,
@@ -258,16 +259,20 @@
 
         # returning the builder for ease of unit testing
         return builder
 
 
 def main(cli_args=None):
     """Reads CLI input/environment variables and invokes library calls"""
+
     parser = get_parser()
     args = vars(parser.parse_args(cli_args))
+    if args["version"]:
+        print(__version__)
+        sys.exit(0)
     if args["action"] is None:
         parser.print_usage()
         sys.exit(1)
     if args.get("target"):
         for target in args["target"]:
             if target == "all":
                 args["target"] = ["all"]
```

### Comparing `cumulus_library-0.3.1/cumulus_library/cli_parser.py` & `cumulus_library-0.3.2/cumulus_library/cli_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,18 @@
 following order of preference is used to select credentials:
   - explicit command line arguments
   - cumulus environment variables (see docs for more info)
   - Normal boto profile order (AWS env vars, ~/.aws/credentials, ~/.aws/config)""",
         epilog="See 'cumulus-library -h [action]' for usage of a specific action",
     )
 
+    parser.add_argument(
+        "--version", action="store_true", help="Display cumulus-library version number"
+    )
+
     actions = parser.add_subparsers(
         title="actions",
         help="Available library actions",
         dest="action",
     )
 
     create = actions.add_parser(
```

### Comparing `cumulus_library-0.3.1/cumulus_library/helper.py` & `cumulus_library-0.3.2/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-0.3.2/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/schema/columns.py` & `cumulus_library-0.3.2/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/schema/counts.py` & `cumulus_library-0.3.2/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/schema/typesystem.py` & `cumulus_library-0.3.2/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/schema/valueset.py` & `cumulus_library-0.3.2/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/condition.sql`

 * *Files 8% similar despite different names*

```diff
@@ -43,43 +43,31 @@
     date_trunc('year', date(tc.recordeddate)) AS recorded_year
 FROM temp_condition AS tc,
     unnest(category) AS t_category (category_coding), --noqa
     unnest(category_coding.coding) AS t_category_coding (category_row), --noqa
     unnest(code.coding) AS t_coding (code_row) --noqa
 WHERE tc.recordeddate BETWEEN date('2016-01-01') AND current_date;
 
-CREATE TABLE core__join_condition_icd AS
-SELECT
-    cc.subject_ref,
-    cc.encounter_ref,
-    cc.recorded_month AS cond_month,
-    ce.enc_class.code AS enc_class_code,
-    vil.code AS cond_code,
-    vil.code_display AS cond_code_display
-FROM core__condition AS cc, core__encounter AS ce, vocab__icd_legend AS vil
-WHERE
-    cc.encounter_ref = ce.encounter_ref
-    AND cc.cond_code.coding[1].code = vil.code; --noqa
-
-CREATE TABLE core__count_condition_icd10_month AS
+CREATE TABLE core__count_condition_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT cc.subject_ref) AS cnt_subject,
         count(DISTINCT cc.encounter_ref) AS cnt_encounter,
-        vil.code_display,
+        cccc.display AS display,
         cc.recorded_month,
         ce.enc_class
-    FROM core__condition AS cc, core__encounter AS ce, vocab__icd_legend AS vil
-    WHERE
-        cc.encounter_ref = ce.encounter_ref
-        AND cc.cond_code.coding[1].code = vil.code --noqa
-    GROUP BY cube(vil.code_display, cc.recorded_month, ce.enc_class)
+    FROM core__condition AS cc
+    INNER JOIN core__encounter AS ce
+        ON cc.encounter_ref = ce.encounter_ref
+    LEFT JOIN core__condition_codable_concepts AS cccc
+        ON cc.condition_id = cccc.id
+    GROUP BY cube(display, cc.recorded_month, ce.enc_class)
 )
 
 SELECT
     powerset.cnt_subject AS cnt,
     powerset.recorded_month AS cond_month,
-    powerset.code_display AS cond_code_display,
+    powerset.display AS cond_code_display,
     enc_class.code AS enc_class_code
 FROM powerset
 WHERE powerset.cnt_subject >= 10
 ORDER BY powerset.cnt_subject DESC, powerset.cnt_encounter DESC;
```

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.3.2/cumulus_library/studies/core/manifest.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 study_prefix = "core"
 
 [python_config]
 file_names = [
-    "patient_extensions.py",
+    "denormalizer.py",
 ]
 
 [sql_config]
 file_names = [
     "setup.sql",
     "fhir_define.sql",
     "patient.sql",
@@ -22,11 +22,11 @@
 
 [export_config]
 export_list = [
     "core__count_patient",
     "core__count_encounter_month",
     "core__count_documentreference_month",
     "core__count_observation_lab_month",
-    "core__count_condition_icd10_month",
+    "core__count_condition_month",
     "core__count_medicationrequest_month",
     "core__meta_date",
 ]
```

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/observation.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/patient.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.3.2/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.3.2/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.3.2/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.3.2/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.3.2/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.3.2/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,37 +13,32 @@
 
 class VocabIcdRunner(BaseRunner):
     def run_executor(self, cursor: object, schema: str, verbose: bool):
         self.create_icd_legend(self, cursor, schema, verbose)
 
     @staticmethod
     def clean_row(row, filename):
-        """Removes non-SQL safe charatcers from the input row.
-
-        WARNING: This function, for the intended datasource specifically, drops the last
-        column since it is a known duplicate. This should be re-examined for other
-        datasources
-        """
-        for i in range(len(row) - 1):
+        """Removes non-SQL safe charatcers from the input row."""
+        for i in range(len(row)):
             cell = str(row[i]).replace("'", "").replace(";", ",")
             row[i] = cell
-        return row[:-1]
+        return row
 
     def create_icd_legend(
-        self, cursor: object, schema: str, verbose: bool, partition_size: int = 2000
+        self, cursor: object, schema: str, verbose: bool, partition_size: int = 1200
     ):
         """input point from make.execute_sql_template.
 
         :param cursor: A database cursor object
         :param schema: the schema/db name, matching the cursor
         :param verbose: if true, outputs raw query, else displays progress bar
         :partition_size: number of lines to read. Athena queries have a char limit.
         """
         table_name = "vocab__icd"
-        icd_files = ["ICD10", "ICD9"]
+        icd_files = ["ICD10CM_2023AA", "ICD10PCS_2023AA", "ICD9CM_2023AA"]
         path = Path(__file__).parent
         query_count = 1  # accounts for static CTAS query
         for filename in icd_files:
             query_count += (
                 sum(1 for i in open(f"{path}/{filename}.bsv", "rb")) / partition_size
             )
 
@@ -76,15 +71,15 @@
         table_name,
         path,
         icd_files,
         progress,
         task,
     ):
         """Constructs queries and posts to athena."""
-        headers = ["CUI", "TUI", "TTY", "CODE", "SAB", "STR"]
+        headers = ["CUI", "TTY", "CODE", "SAB", "STR"]
         header_types = [f"{x} string" for x in headers]
         rows_processed = 0
         dataset = []
         created = False
         for filename in icd_files:
             with open(f"{path}/{filename}.bsv", "r") as file:
                 # For the first row in the dataset, we want to coerce types from
```

### Comparing `cumulus_library-0.3.1/cumulus_library/study_parser.py` & `cumulus_library-0.3.2/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-0.3.2/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.3.2/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.1/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.3.2/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 CREATE TABLE {{ target_table }} AS (
     WITH
-    {%- for system in code_systems %}
+    {%- for system in ext_systems %}
 
     system_{{ system }} AS (
         SELECT DISTINCT
             s.id,
             '{{ loop.index0 }}' AS priority,
             '{{ system }}' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS {{ target_col_prefix }}_code,
@@ -17,15 +17,15 @@
             ext_parent.ext.url = '{{ fhir_extension }}'
             AND ext_child.ext.url = '{{ system }}'
             AND ext_child.ext.valuecoding.display != ''
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
-        {%- for system in code_systems %}
+        {%- for system in ext_systems %}
         SELECT
             id,
             priority,
             system,
             {{ target_col_prefix }}_code,
             {{ target_col_prefix }}_display
         FROM system_{{ system }}
```

### Comparing `cumulus_library-0.3.1/cumulus_library/template_sql/templates.py` & `cumulus_library-0.3.2/cumulus_library/template_sql/templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,40 +127,64 @@
     def __init__(
         self,
         source_table: str,
         source_id: str,
         target_table: str,
         target_col_prefix: str,
         fhir_extension: str,
-        code_systems: List[str],
+        ext_systems: List[str],
     ):
         self.source_table = source_table
         self.source_id = source_id
         self.target_table = target_table
         self.target_col_prefix = target_col_prefix
         self.fhir_extension = fhir_extension
-        self.code_systems = code_systems
+        self.ext_systems = ext_systems
 
 
 def get_extension_denormalize_query(config: ExtensionConfig) -> str:
     """extracts target extension from a table into a denormalized table
 
     This function is targeted at a complex extension element that is at the root
     of a FHIR resource - as an example, see the 5 codes at the root node of
     http://hl7.org/fhir/us/core/STU6/StructureDefinition-us-core-patient.html.
     The template will create a new table with the extension data, in arrays,
-    mapped 1-1 to the table id. You can specify multiple coding systems
+    mapped 1-1 to the table id. You can specify multiple systems
     in the ExtensionConfig passed to this function. For each patient, we'll
-    take the data from the first coding system we find for each patient.
+    take the data from the first extension coding system we find for each patient.
 
     :param config: An instance of ExtensionConfig.
     """
     path = Path(__file__).parent
     with open(f"{path}/extension_denormalize.sql.jinja") as extension_denormalize:
         return Template(extension_denormalize.read()).render(
             source_table=config.source_table,
             source_id=config.source_id,
             target_table=config.target_table,
             target_col_prefix=config.target_col_prefix,
             fhir_extension=config.fhir_extension,
-            code_systems=config.code_systems,
+            ext_systems=config.ext_systems,
+        )
+
+
+def get_codeable_concept_denormalize_query(
+    source_table: str, cc_column: str, target_table: str, code_systems: List[str]
+) -> str:
+    """extracts codeable concepts from a specified table.
+
+    See http://hl7.org/fhir/datatypes-definitions.html#CodeableConcept for more info
+
+    :param source_table: the table to extract extensions from
+    :param cc_column: the column containing the codeableConcept you want to extract
+    :param target_table: the name of the table to create
+    :param code_systems: a list of coding systems, in preference order, to use to select data
+    """
+    path = Path(__file__).parent
+    with open(
+        f"{path}/codeable_concept_denormalize.sql.jinja"
+    ) as extension_denormalize:
+        return Template(extension_denormalize.read()).render(
+            source_table=source_table,
+            cc_column=cc_column,
+            target_table=target_table,
+            code_systems=code_systems,
         )
```

### Comparing `cumulus_library-0.3.1/cumulus_library/upload.py` & `cumulus_library-0.3.2/cumulus_library/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+""" Handles pushing data to the aggregator"""
 import sys
 
 from pathlib import Path
 
 import requests
 from rich.progress import Progress, TaskID
```

### Comparing `cumulus_library-0.3.1/pyproject.toml` & `cumulus_library-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "cumulus-library"
-version = "0.3.1"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
@@ -24,14 +23,15 @@
 keywords = ["FHIR", "SQL", "Health Informatics"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+dynamic=["version"]
 [project.optional-dependencies]
 dev = [
     "black",
     "pylint",
 ]
 test = [
     "pytest",
```

### Comparing `cumulus_library-0.3.1/PKG-INFO` & `cumulus_library-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.3.1
+Version: 0.3.2
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -29,9 +29,16 @@
 Provides-Extra: dev
 Provides-Extra: test
 
 # Cumulus Library - Core
 
 A framework for designing, executing, and distributing SQL queries packaged as "studies", e.g., for quality monitoring, clinical research, or public health. Part of the [SMART on FHIR Cumulus Project](https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/)
 
+## Installing
+
+For end users, just run `pip install cumulus-library`. 
+For running from source, checkout the repo, and at the project root run `pip install -e .`.
+
+
+
 For more information, [browse the documentation](https://docs.smarthealthit.org/cumulus/library).
```

