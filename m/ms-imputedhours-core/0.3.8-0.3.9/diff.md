# Comparing `tmp/ms_imputedhours_core-0.3.8.tar.gz` & `tmp/ms_imputedhours_core-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.8.tar", max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.9.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.8.tar` & `ms_imputedhours_core-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    35149 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/LICENSE
--rw-r--r--   0        0        0     2401 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/README.md
--rw-r--r--   0        0        0       22 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/__init__.py
--rw-r--r--   0        0        0     3238 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/__init__.py
--rw-r--r--   0        0        0     3228 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/test_agreements.py
--rw-r--r--   0        0        0     2472 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/__init__.py
--rw-r--r--   0        0        0     9750 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/test_employee.py
--rw-r--r--   0        0        0     7158 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/__init__.py
--rw-r--r--   0        0        0     6373 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_capacity.py
--rw-r--r--   0        0        0     9019 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0        0        0    10493 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0        0        0      171 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/constants.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
--rw-r--r--   0        0        0     4491 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0        0        0     6206 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0        0        0      776 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0        0        0      654 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0        0        0     3599 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0        0        0      423 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/dates.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/__init__.py
--rw-r--r--   0        0        0     3828 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/hours.py
--rw-r--r--   0        0        0      203 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/__init__.py
--rw-r--r--   0        0        0      678 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/test_office.py
--rw-r--r--   0        0        0      950 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2401 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     2472 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     9750 2023-05-30 08:20:11.552553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     7158 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     6373 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__tests__/test_capacity.py
+-rw-r--r--   0        0        0     8995 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10582 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      654 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-05-30 08:20:11.556553 ms_imputedhours_core-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.9/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.8/LICENSE` & `ms_imputedhours_core-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/README.md` & `ms_imputedhours_core-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_capacity.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__tests__/test_capacity.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,29 +173,29 @@
         office_name = 'Madrid - ing'
         expected_result = {
             'employee1@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee1 Doe',
+                'name': 'Employee1',
             },
             'employee2@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 0.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee20@makingscience.com',
-                'name': 'Employee2 Doe',
+                'name': 'Employee2',
             },
             'employee4@makingscience.com': {
                 'real_capacity': 0.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 100,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee4 Doe',
+                'name': 'Employee4',
             },
         }
         result = get_all_employee_data_by_range(
             from_date,
             to_date,
             office_name,
         )
@@ -231,29 +231,29 @@
         office_name = 'Madrid - ing'
         expected_result = {
             'employee1@makingscience.com': {
                 'real_capacity': 59.0,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 27.12,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee1 Doe',
+                'name': 'Employee1',
             },
             'employee2@makingscience.com': {
                 'real_capacity': 59.0,
                 'current_capacity': 0.0,
                 'current_percentage_hours_imputed': 0.0,
                 'supervisor': 'employee20@makingscience.com',
-                'name': 'Employee2 Doe',
+                'name': 'Employee2',
             },
             'employee4@makingscience.com': {
                 'real_capacity': 29.5,
                 'current_capacity': 16.0,
                 'current_percentage_hours_imputed': 54.24,
                 'supervisor': 'employee2@makingscience.com',
-                'name': 'Employee4 Doe',
+                'name': 'Employee4',
             },
         }
         result = get_all_employee_data_by_range(
             from_date,
             to_date,
             office_name,
         )
```

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,30 +360,31 @@
             return 'null'
 
     totalTimeSpent = data['data']['totalTimeSpent'] * 1000
     successfactor_data = data.pop('successfactor_data')
     enddate = _get_date_value(successfactor_data.get('enddate'))
     startdate = _get_date_value(successfactor_data.get("hiring_date"))
 
-    return "('{email}','{yearSelected}','{monthSelected}',{totalTimeSpent},{fte},'{office}',{capacity},{realcapacity},{startdate},{enddate})".format(  # noqa: E501
+    return "('{email}','{yearSelected}','{monthSelected}',{totalTimeSpent},{fte},'{office}',{capacity},{realcapacity},{startdate},{enddate}, '{department}')".format(  # noqa: E501
         email=email,
         yearSelected=data["yearSelected"],
         monthSelected=data["monthSelected"],
         totalTimeSpent=totalTimeSpent,
         fte=successfactor_data["FTE"],
         office=successfactor_data["office_name"],
         capacity=data["agreementHours"]["totalHours"] * MS_FOR_HOUR,
         realcapacity=data["agreementHours"]["realcapacity"] * MS_FOR_HOUR,
         startdate=startdate,
         enddate=enddate,
+        department=successfactor_data.get('department', ''),
     )
 
 
 def insert_batch_capacities(capacities):
-    query = f"INSERT INTO `{BIGQUERY_EMPLOYEE_CAPACITY}` (email, year, month, jira, fte, office, capacity, realcapacity, startdate, enddate) VALUES "  # noqa: E501
+    query = f"INSERT INTO `{BIGQUERY_EMPLOYEE_CAPACITY}` (email, year, month, jira, fte, office, capacity, realcapacity, startdate, enddate, department) VALUES "  # noqa: E501
     values = ",".join(capacities)
 
     return execute_query(query + values)
 
 
 def remove_data(year, month, office):
     query = f"DELETE FROM `{BIGQUERY_EMPLOYEE_CAPACITY}` WHERE year='{year}' AND month='{month}' AND office='{office}'"  # noqa: E501
```

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,19 @@
 
         if email not in data_json.keys():
             data_json[email] = {}
 
         fte = data.get('fte', EMPTY_FTE) or EMPTY_FTE  # For null values
         data_json[email]['supervisor'] = data.get('supervisor', '')
         data_json[email]['office_name'] = data.get('office', '')
+        data_json[email]['department'] = data.get('department', '')
         data_json[email]['FTE'] = float(fte.replace(',', '.'))
         data_json[email]['hiring_date'] = hiringdate
         data_json[email]['enddate'] = enddate
-        data_json[email]['name'] = "{} {}".format(
-            data.get('name', ''), data.get('lastname', '')
-        )
+        data_json[email]['name'] = data.get('name', '')
 
     return data_json
 
 
 def transform_all_capacities(capacities):
     data_json = {}
```

### Comparing `ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.9/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.8/pyproject.toml` & `ms_imputedhours_core-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-imputedhours-core"
-version = "0.3.8"
+version = "0.3.9"
 description = "Python library to collect data about jira imputed hours and employee agreements"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_imputedhours_core"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_imputedhours_core-0.3.8/PKG-INFO` & `ms_imputedhours_core-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python library to collect data about jira imputed hours and employee agreements
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

