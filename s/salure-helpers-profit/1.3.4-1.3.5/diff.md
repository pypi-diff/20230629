# Comparing `tmp/salure_helpers_profit-1.3.4.tar.gz` & `tmp/salure_helpers_profit-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.3.4.tar", last modified: Fri Jun 23 07:55:10 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-1.3.5.tar", last modified: Thu Jun 29 12:21:53 2023, max compression
```

## Comparing `salure_helpers_profit-1.3.4.tar` & `salure_helpers_profit-1.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   133896 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:55:10.000000 salure_helpers_profit-1.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-23 07:54:55.000000 salure_helpers_profit-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   138891 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/setup.py
```

### Comparing `salure_helpers_profit-1.3.4/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.4/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.4/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.4/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
         :param method: request type
         :return: status code for request and optional error message
         """
         allowed_fields = ['employee_id', 'mail_work', 'mail_private', 'mobile_work', 'mobile_private', 'nickname', 'first_name', 'initials', 'prefix', 'last_name', 'prefix_birth_name',
                           'birth_name', 'gender', 'nationality', 'birth_date', 'country_of_birth', 'ssn', 'marital_status', 'date_of_marriage', 'date_of_divorce', 'phone_work', 'phone_private', 'city_of_birth',
-                          'birth_name_separate', 'name_use', 'match_person_on']
+                          'birth_name_separate', 'name_use', 'match_person_on', 'birthname_partner', 'prefix_birthname_partner']
         required_fields = ['employee_id', 'person_id']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/KnPerson')
 
         base_body = {
@@ -84,14 +84,16 @@
         fields_to_update.update({"DaMa": data['date_of_marriage']}) if 'date_of_marriage' in data else fields_to_update
         fields_to_update.update({"DaMa": data['date_of_divorce']}) if 'date_of_divorce' in data else fields_to_update
         fields_to_update.update({"TeNr": data['phone_work']}) if 'phone_work' in data else fields_to_update
         fields_to_update.update({"TeN2": data['phone_private']}) if 'phone_private' in data else fields_to_update
         fields_to_update.update({"RsBi": data['city_of_birth']}) if 'city_of_birth' in data else fields_to_update
         fields_to_update.update({"SpNm": data['birth_name_separate']}) if 'birth_name_separate' in data else fields_to_update
         fields_to_update.update({"ViUs": data['name_use']}) if 'name_use' in data else fields_to_update
+        fields_to_update.update({"NmPa": data['birthname_partner']}) if 'birthname_partner' in data else fields_to_update
+        fields_to_update.update({"IsPa": data['prefix_birthname_partner']}) if 'prefix_birthname_partner' in data else fields_to_update
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['KnPerson']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
@@ -293,15 +295,15 @@
         # Update the request body with update fields
         base_body['KnSalesRelationPer']['Element']['Objects']['KnPerson']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
 
         return update
 
-    def update_creditor(self,method: str, data: dict, overload_fields: dict = None) -> requests.Response:
+    def update_creditor(self, method: str, data: dict, overload_fields: dict = None) -> requests.Response:
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
         :param method: request type
         :return: status code for request and optional error message
         """
         allowed_fields = ['person_id', 'internal_id', 'match_person_on', 'log_birthname_seperately', 'collective_account', 'preferred_delivery_method', 'automatic_payment', 'compact', 'payment_specification', 'remark']
@@ -487,23 +489,33 @@
         :param data: Dictionary of fields that you want to update in AFAS. Only fields listed in allowed arrays are accepted. Fields listed in required fields array, are mandatory
         :param overload_fields: Dictionary of dictionaries. Specify sub dictionaries for each section you want to update.
         Specify as key which element you want to update, available options are: schedule, salary, contract, function.
         Example: overload_fields = {"employee": {"field": value}}
         :param method: request type
         :return: status code for request and optional error message
         """
-        allowed_fields_contract = ['employee_id', 'type_of_employment', 'enddate_contract', 'termination_reason', 'termination_initiative', 'probation_period',
-                                   'probation_enddate', 'cao', 'terms_of_employment', 'type_of_contract', 'employer_number', 'type_of_employee', 'employment']
+
+        # Contract fields
         required_fields_contract = ['employee_id', 'startdate_contract']
-        allowed_fields_function = ['costcarrier_id']
+        allowed_fields_contract = ['employee_id', 'type_of_employment', 'enddate_contract', 'termination_reason', 'termination_initiative', 'probation_period',
+                                   'probation_enddate', 'cao', 'terms_of_employment', 'type_of_contract', 'employer_number', 'type_of_employee', 'employment',
+                                   'seniority_date', 'contract_chain_code', 'start_date_contract_chain', 'date_in_service_original']
+
+        # Function fields
         required_fields_function = ['organizational_unit', 'function_id', 'costcenter_id']
-        allowed_fields_timetable = ['changing_work_pattern', 'days_per_week', 'fte', 'on-call_contract']
+        allowed_fields_function = ['costcarrier_id']
+
+        # Timetable fields
         required_fields_timetable = ['weekly_hours', 'parttime_percentage']
-        allowed_fields_salary = ['step', 'function_scale', 'salary_scale', 'salary_year', 'net_salary', 'apply_timetable', 'salary_amount']
+        allowed_fields_timetable = ['changing_work_pattern', 'days_per_week', 'fte', 'on-call_contract', 'type_of_schedule']
+
+        # Salary fields
         required_fields_salary = ['type_of_salary', 'period_table']
+        allowed_fields_salary = ['step', 'function_scale', 'salary_scale', 'salary_year', 'net_salary', 'apply_timetable', 'salary_amount']
+
         allowed_fields = allowed_fields_contract + allowed_fields_salary + allowed_fields_timetable + allowed_fields_function
         required_fields = required_fields_contract + required_fields_function + required_fields_timetable + required_fields_salary
 
         # Check if there are fields that are not allowed or fields missing that are required
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasContract')
@@ -522,15 +534,15 @@
                         }
                     }
                 }
             }
         }
 
         # Extra JSON objects which are optional at contract creation
-        function = {
+        function_dict = {
             "AfasOrgunitFunction": {
                 "Element": {
                     "@DaBe": data['startdate_contract'],
                     "Fields": {
                     }
                 }
             }
@@ -557,52 +569,53 @@
             }
         }
 
         # If one of the optional fields of a subelement is included, we need to merge the whole JSON object to the basebody
         if any(field in data.keys() for field in allowed_fields_function):
             for field in required_fields_function:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for function are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for function are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"DpId": data['organizational_unit']}) if 'organizational_unit' in data else fields_to_update
             fields_to_update.update({"FuId": data['function_id']}) if 'function_id' in data else fields_to_update
             fields_to_update.update({"CrId": data['costcenter_id']}) if 'costcenter_id' in data else fields_to_update
             fields_to_update.update({"CcId": data['costcarrier_id']}) if 'costcarrier_id' in data else fields_to_update
             # add overload function fields to the body
             if overload_fields is not None and 'function' in overload_fields.keys():
                 fields_to_update.update(overload_fields['function'])
 
             # merge subelement with basebody
-            function['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update)
-            base_body['AfasEmployee']['Element']['Objects'].update(function)
+            function_dict['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update)
+            base_body['AfasEmployee']['Element']['Objects'].update(function_dict)
 
         if any(field in data.keys() for field in allowed_fields_timetable):
             for field in required_fields_timetable:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for timetable are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for timetable are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"StPa": data['changing_work_pattern']}) if 'changing_work_pattern' in data else fields_to_update
             fields_to_update.update({"HrWk": data['weekly_hours']}) if 'weekly_hours' in data else fields_to_update
             fields_to_update.update({"PcPt": data['parttime_percentage']}) if 'parttime_percentage' in data else fields_to_update
             fields_to_update.update({"DyWk": data['days_per_week']}) if 'days_per_week' in data else fields_to_update
             fields_to_update.update({"Ft": data['fte']}) if 'fte' in data else fields_to_update
             fields_to_update.update({"ClAg": data['on-call_contract']}) if 'on-call_contract' in data else fields_to_update
+            fields_to_update.update({"EtTy": data['type_of_schedule']}) if 'type_of_schedule' in data else fields_to_update
             # add overload schedule fields to the body
             if overload_fields is not None and 'schedule' in overload_fields.keys():
                 fields_to_update.update(overload_fields['schedule'])
 
             timetable['AfasTimeTable']['Element']['Fields'].update(fields_to_update)
             base_body['AfasEmployee']['Element']['Objects'].update(timetable)
 
         if any(field in data.keys() for field in allowed_fields_salary):
             for field in required_fields_salary:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for salaries are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for salaries are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"SaSt": data['step']}) if 'step' in data else fields_to_update
             fields_to_update.update({"SaPe": data['type_of_salary']}) if 'type_of_salary' in data else fields_to_update
             fields_to_update.update({"EmSa": data['salary_amount']}) if 'salary_amount' in data else fields_to_update
             fields_to_update.update({"PtId": data['period_table']}) if 'period_table' in data else fields_to_update
             fields_to_update.update({"VaSc": data['salary_scale']}) if 'salary_scale' in data else fields_to_update
@@ -627,14 +640,18 @@
         fields_to_update.update({"DaEt": data['probation_enddate']}) if 'probation_enddate' in data else fields_to_update
         fields_to_update.update({"ClId": data['cao']}) if 'cao' in data else fields_to_update
         fields_to_update.update({"WcId": data['terms_of_employment']}) if 'terms_of_employment' in data else fields_to_update
         fields_to_update.update({"ApCo": data['type_of_contract']}) if 'type_of_contract' in data else fields_to_update
         fields_to_update.update({"CmId": data['employer_number']}) if 'employer_number' in data else fields_to_update
         fields_to_update.update({"EmMt": data['type_of_employee']}) if 'type_of_employee' in data else fields_to_update
         fields_to_update.update({"ViEt": data['employment']}) if 'employment' in data else fields_to_update
+        fields_to_update.update({"StAc": data['seniority_date']}) if 'seniority_date' in data else fields_to_update
+        fields_to_update.update({"DaSc": data['start_date_contract_chain']}) if 'start_date_contract_chain' in data else fields_to_update
+        fields_to_update.update({"ViKe": data['contract_chain_code']}) if 'contract_chain_code' in data else fields_to_update
+        fields_to_update.update({"DbYs": data['date_in_service_original']}) if 'date_in_service_original' in data else fields_to_update
         # add overload contract fields to the body
         if overload_fields is not None and 'contract' in overload_fields.keys():
             fields_to_update.update(overload_fields['contract'])
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['AfasContract']['Element']['Fields'].update(fields_to_update)
 
@@ -650,23 +667,33 @@
         :param data: Dictionary of fields that you want to update in AFAS. Only fields listed in allowed arrays are accepted. Fields listed in required fields array, are mandatory
         :param overload_fields: Dictionary of dictionaries. Specify sub dictionaries for each section you want to update.
         Specify as key which element you want to update, available options are: schedule, salary, contract, function.
         Example: overload_fields = {"employee": {"field": value}}
         :param method: request type
         :return: status code for request and optional error message
         """
-        allowed_fields_contract = ['employee_id', 'type_of_employment', 'enddate_contract', 'termination_reason', 'termination_initiative', 'probation_period',
-                                   'probation_enddate', 'cao', 'terms_of_employment', 'type_of_contract', 'employer_number', 'type_of_employee', 'employment']
+
+        # Contract fields
         required_fields_contract = ['employee_id', 'startdate_contract']
-        allowed_fields_function = ['costcarrier_id']
+        allowed_fields_contract = ['employee_id', 'type_of_employment', 'enddate_contract', 'termination_reason', 'termination_initiative', 'probation_period',
+                                   'probation_enddate', 'cao', 'terms_of_employment', 'type_of_contract', 'employer_number', 'type_of_employee', 'employment'
+                                   'seniority_date', 'contract_chain_code', 'start_date_contract_chain']
+
+        # Function fields
         required_fields_function = ['organizational_unit', 'function_id', 'costcenter_id']
-        allowed_fields_timetable = ['changing_work_pattern', 'days_per_week', 'fte', 'on-call_contract']
+        allowed_fields_function = ['costcarrier_id']
+
+        # Timetable fields
         required_fields_timetable = ['weekly_hours', 'parttime_percentage']
-        allowed_fields_salary = ['step', 'function_scale', 'salary_scale', 'salary_year', 'net_salary', 'apply_timetable', 'salary_amount']
+        allowed_fields_timetable = ['changing_work_pattern', 'days_per_week', 'fte', 'on-call_contract', 'type_of_schedule']
+
+        # Salary fields
         required_fields_salary = ['type_of_salary', 'period_table']
+        allowed_fields_salary = ['step', 'function_scale', 'salary_scale', 'salary_year', 'net_salary', 'apply_timetable', 'salary_amount']
+
         allowed_fields = allowed_fields_contract + allowed_fields_salary + allowed_fields_timetable + allowed_fields_function
         required_fields = required_fields_contract + required_fields_function + required_fields_timetable + required_fields_salary
 
         # Check if there are fields that are not allowed or fields missing that are required
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasContract')
@@ -688,15 +715,15 @@
                         }
                     }
                 }
             }
         }
 
         # Extra JSON objects which are optional at contract creation
-        function = {
+        function_dict = {
             "AfasOrgunitFunction": {
                 "Element": {
                     "@DaBe": data['startdate_contract'],
                     "Fields": {
                     }
                 }
             }
@@ -723,52 +750,53 @@
             }
         }
 
         # If one of the optional fields of a subelement is included, we need to merge the whole JSON object to the basebody
         if any(field in data.keys() for field in allowed_fields_function):
             for field in required_fields_function:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for function are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for function are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"DpId": data['organizational_unit']}) if 'organizational_unit' in data else fields_to_update
             fields_to_update.update({"FuId": data['function_id']}) if 'function_id' in data else fields_to_update
             fields_to_update.update({"CrId": data['costcenter_id']}) if 'costcenter_id' in data else fields_to_update
             fields_to_update.update({"CcId": data['costcarrier_id']}) if 'costcarrier_id' in data else fields_to_update
             # add overload function fields to the body
             if overload_fields is not None and 'function' in overload_fields.keys():
                 fields_to_update.update(overload_fields['function'])
 
             # merge subelement with basebody
-            function['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update)
-            base_body['AfasEmployee']['Element']['Objects'].update(function)
+            function_dict['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update)
+            base_body['AfasEmployee']['Element']['Objects'].update(function_dict)
 
         if any(field in data.keys() for field in allowed_fields_timetable):
             for field in required_fields_timetable:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for timetable are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for timetable are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"StPa": data['changing_work_pattern']}) if 'changing_work_pattern' in data else fields_to_update
             fields_to_update.update({"HrWk": data['weekly_hours']}) if 'weekly_hours' in data else fields_to_update
             fields_to_update.update({"PcPt": data['parttime_percentage']}) if 'parttime_percentage' in data else fields_to_update
             fields_to_update.update({"DyWk": data['days_per_week']}) if 'days_per_week' in data else fields_to_update
             fields_to_update.update({"Ft": data['fte']}) if 'fte' in data else fields_to_update
             fields_to_update.update({"ClAg": data['on-call_contract']}) if 'on-call_contract' in data else fields_to_update
+            fields_to_update.update({"EtTy": data['type_of_schedule']}) if 'type_of_schedule' in data else fields_to_update
             # add overload schedule fields to the body
             if overload_fields is not None and 'schedule' in overload_fields.keys():
                 fields_to_update.update(overload_fields['schedule'])
 
             timetable['AfasTimeTable']['Element']['Fields'].update(fields_to_update)
             base_body['AfasEmployee']['Element']['Objects'].update(timetable)
 
         if any(field in data.keys() for field in allowed_fields_salary):
             for field in required_fields_salary:
                 if field not in data.keys():
-                    return 'Field {field} is required. Required fields for salaries are: {required_fields}'.format(field=field, required_fields=tuple(required_fields))
+                    raise KeyError('Field {field} is required. Required fields for salaries are: {required_fields}'.format(field=field, required_fields=tuple(required_fields)))
 
             fields_to_update = {}
             fields_to_update.update({"SaSt": data['step']}) if 'step' in data else fields_to_update
             fields_to_update.update({"SaPe": data['type_of_salary']}) if 'type_of_salary' in data else fields_to_update
             fields_to_update.update({"EmSa": data['salary_amount']}) if 'salary_amount' in data else fields_to_update
             fields_to_update.update({"PtId": data['period_table']}) if 'period_table' in data else fields_to_update
             fields_to_update.update({"VaSc": data['salary_scale']}) if 'salary_scale' in data else fields_to_update
@@ -793,14 +821,17 @@
         fields_to_update.update({"DaEt": data['probation_enddate']}) if 'probation_enddate' in data else fields_to_update
         fields_to_update.update({"ClId": data['cao']}) if 'cao' in data else fields_to_update
         fields_to_update.update({"WcId": data['terms_of_employment']}) if 'terms_of_employment' in data else fields_to_update
         fields_to_update.update({"ApCo": data['type_of_contract']}) if 'type_of_contract' in data else fields_to_update
         fields_to_update.update({"CmId": data['employer_number']}) if 'employer_number' in data else fields_to_update
         fields_to_update.update({"EmMt": data['type_of_employee']}) if 'type_of_employee' in data else fields_to_update
         fields_to_update.update({"ViEt": data['employment']}) if 'employment' in data else fields_to_update
+        fields_to_update.update({"StAc": data['seniority_date']}) if 'seniority_date' in data else fields_to_update
+        fields_to_update.update({"DaSc": data['start_date_contract_chain']}) if 'start_date_contract_chain' in data else fields_to_update
+        fields_to_update.update({"ViKe": data['contract_chain_code']}) if 'contract_chain_code' in data else fields_to_update
         # add overload contract fields to the body
         if overload_fields is not None and 'contract' in overload_fields.keys():
             fields_to_update.update(overload_fields['contract'])
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['AfasContract']['Element']['Fields'].update(fields_to_update)
 
@@ -812,15 +843,15 @@
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Give the guid and value from a free field if wanted
         :param method: PUT or POST, depending on the case
         :return: status code for request and optional error message
         """
         allowed_fields = ['formation', 'costcarrier']
-        required_fields = ['startdate', 'employee_id', 'organizational_unit', 'function', 'costcentre']
+        required_fields = ['startdate', 'employee_id', 'organizational_unit', 'function', 'costcentre', 'employment_number']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasOrgunitFunction')
 
         base_body = {
             "AfasEmployee": {
@@ -842,14 +873,15 @@
             }
         }
         fields_to_update = {}
 
         # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update.update({"FpId": data['formation']}) if 'formation' in data else fields_to_update
         fields_to_update.update({"CcId": data['costcarrier']}) if 'costcarrier' in data else fields_to_update
+        fields_to_update.update({"DvSn": data['employment_number']}) if 'employment_number' in data else fields_to_update
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
@@ -860,15 +892,15 @@
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Give the guid and value from a free field if wanted
         :param method: PUT or POST, depending on the case
         :return: status code for request and optional error message
         """
         allowed_fields = ['step', 'period_table', 'salary_year', 'function_scale', 'function_scale_type', 'salary_scale',
-                          'salary_scale_type', 'salary_amount', 'net_salary', 'apply_timetable']
+                          'salary_scale_type', 'salary_amount', 'net_salary', 'apply_timetable', 'employment_number']
         required_fields = ['startdate', 'employee_id', 'salary_type']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasSalary')
 
         base_body = {
@@ -897,14 +929,15 @@
         fields_to_update.update({"PtId": data['period_table']}) if 'period_table' in data else fields_to_update.update({"PtId": 5})
         fields_to_update.update({"VaSc": data['salary_scale']}) if 'salary_scale' in data else fields_to_update
         fields_to_update.update({"TaId": data['salary_scale_type']}) if 'salary_scale_type' in data else fields_to_update
         fields_to_update.update({"FuSc": data['function_scale']}) if 'function_scale' in data else fields_to_update
         fields_to_update.update({"FuTa": data['function_scale_type']}) if 'function_scale_type' in data else fields_to_update
         fields_to_update.update({"NtSa": data['net_salary']}) if 'net_salary' in data else fields_to_update
         fields_to_update.update({"TtPy": data['apply_timetable']}) if 'apply_timetable' in data else fields_to_update
+        fields_to_update.update({"DvSn": data['employment_number']}) if 'employment_number' in data else fields_to_update
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['AfasSalary']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
@@ -996,15 +1029,15 @@
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Give the guid and value from a free field if wanted
         :param method: PUT or POST, depending on the case
         :return: status code for request and optional error message
         """
 
-        allowed_fields = ['changing_work_pattern', 'days_per_week', 'fte']
+        allowed_fields = ['changing_work_pattern', 'days_per_week', 'fte', 'employment_number']
         required_fields = ['startdate', 'employee_id', 'weekly_hours', 'parttime_percentage']
 
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
         url = 'https://{}.{}/profitrestservices/connectors/{}'.format(self.environment, self.base_url, 'KnEmployee/AfasTimeTable')
 
         base_body = {
@@ -1028,14 +1061,15 @@
         }
         fields_to_update = {}
 
         # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update.update({"StPa": data['changing_work_pattern']}) if 'changing_work_pattern' in data else fields_to_update
         fields_to_update.update({"DyWk": data['days_per_week']}) if 'days_per_week' in data else fields_to_update
         fields_to_update.update({"Ft": data['fte']}) if 'fte' in data else fields_to_update
+        fields_to_update.update({"DvSn": data['employment_number']}) if 'employment_number' in data else fields_to_update
 
         fields_to_update.update(overload_fields) if overload_fields is not None else ''
 
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['AfasTimeTable']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
@@ -1247,28 +1281,39 @@
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: Any custom fields that are not in the allowed or required fields. Specify sub dictionaries for each section you want to update.
         Available options are: employee, person, contract, function, schedule, salary. Specify like: overload_fields = {"employee": {"field": value}}
         :return: status code for request and optional error message
         """
 
+        # Person fields
         required_fields_person = ['last_name', 'gender', 'first_name', 'date_of_birth', 'country', 'ssn']
+        allowed_fields_person = ['employee_id', 'date_of_death', 'initials', 'email_work', 'email_home', 'country_of_birth', 'place_of_birth', 'prefix',
+                                 'birth_name_separate', 'name_use', 'send_payslip', 'send_annual_statement', 'match_employees_on', 'nickname', 'birthname', 'prefix_birthname', 'prefix_birthname_partner', 'birthname_partner',
+                                 'mail_work', 'mail_private', 'mobile_work', 'mobile_private', 'marital_status', 'date_of_marriage', 'phone_work', 'phone_private', 'nationality', 'auto_number']
+
+        # Address fields
+        required_fields_address = ['house_number', 'street', 'street_number_add', 'postal_code', 'city', 'address_country']
+        allowed_fields_address = ['search_address_by_postal_code']
+
+        # contract fields
         required_fields_contract = ['date_effective', 'type_of_contract', 'collective_agreement', 'terms_of_employment', 'employment', 'type_of_employee', 'employer']
-        required_fields_address = ['house_number', 'street', 'street_number_add', 'postal_code', 'city', 'country']
+        allowed_fields_contract = ['end_date_contract', 'seniority_date', 'date_in_service_original', 'probation_period_code', 'end_date_probation_period', 'contract_chain_code', 'start_date_contract_chain']
+
+        # function fields
         required_fields_function = ['organizational_unit', 'date_effective', 'function_id', 'costcenter', 'costcarrier']
+
+        # schedule fields
         required_fields_schedule = ['weekly_hours', 'parttime_percentage']
+        allowed_fields_schedule = ['changing_work_pattern', 'days_per_week', 'fte', 'type_of_schedule']
+
+        # salary fields
         required_fields_salary = ['type_of_salary']
         allowed_fields_salary = ['step', 'salary_scale', 'salary_scale_type', 'function_scale', 'function_scale_type', 'salary_year',
                                  'net_salary', 'apply_timetable', 'amount']
-        allowed_fields_contract = ['end_date_contract']
-        allowed_fields_schedule = ['changing_work_pattern', 'days_per_week', 'fte', 'type_of_schedule']
-        allowed_fields_person = ['employee_id', 'initials', 'email_work', 'email_home', 'country_of_birth', 'place_of_birth', 'prefix',
-                                 'birth_name_separate', 'name_use', 'send_payslip', 'send_annual_statement', 'match_employees_on', 'nickname',
-                                 'mail_work', 'mail_private', 'mobile_work', 'mobile_private', 'marital_status', 'phone_work', 'phone_private', 'nationality', 'auto_number']
-        allowed_fields_address = ['search_address_by_postal_code']
 
         allowed_fields = allowed_fields_person + allowed_fields_salary + allowed_fields_schedule + allowed_fields_contract + allowed_fields_address
         required_fields = required_fields_contract + required_fields_function + required_fields_schedule + required_fields_salary + required_fields_address + required_fields_person
 
         # Check if there are fields that are not allowed or fields missing that are required
         self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
 
@@ -1298,20 +1343,19 @@
                                     # Gender [{"id":"M","description":"Male"},{"id":"U","description":"Unknown"},{"id":"F","description":"Female"}]
                                     "ViGe": data['gender'],
                                     "PsNa": data['country'],  # Nationality
                                     "DaBi": data['date_of_birth'],  # Birth date
                                     "SoSe": data['ssn']  # SSN
                                 },
                                 "Objects": [
-
                                     {
                                         "KnBasicAddressAdr": {
                                             "Element": {
                                                 "Fields": {
-                                                    "CoId": data['country'],  # Country
+                                                    "CoId": data['address_country'],  # Country
                                                     "PbAd": False,  # Postbusadres
                                                     "Ad": data['street'],  # Street
                                                     "HmNr": data['house_number'],  # Streetnumber
                                                     "HmAd": data['street_number_add'],  # Streetnumber addition
                                                     "ZpCd": data['postal_code'],  # Postal code
                                                     "Rs": data['city'],  # City
                                                     "ResZip": data['search_address_by_postal_code'] if 'search_address_by_postal_code' in data.keys() else True,
@@ -1319,15 +1363,15 @@
                                             }
                                         }
                                     },
                                     {
                                         "KnBasicAddressPad": {
                                             "Element": {
                                                 "Fields": {
-                                                    "CoId": data['country'],  # Country
+                                                    "CoId": data['address_country'],  # Country
                                                     "PbAd": False,  # Postbusadres
                                                     "Ad": data['street'],  # Street
                                                     "HmNr": data['house_number'],  # Streetnumber
                                                     "HmAd": data['street_number_add'],  # Streetnumber addition
                                                     "ZpCd": data['postal_code'],  # Postal code
                                                     "Rs": data['city'],  # City
                                                     "ResZip": data['search_address_by_postal_code'] if 'search_address_by_postal_code' in data.keys() else True,
@@ -1344,15 +1388,14 @@
                                 "Fields": {
                                     "ClId": data['collective_agreement'],  # Cao - fixed
                                     "WcId": data['terms_of_employment'],  # Arbeidsvoorwaarde - Fixed op zoetwarenindustrie - 36 uur
                                     "ApCo": data['type_of_contract'],  # Type of contract
                                     "CmId": data['employer'],  # employer - fixed
                                     "EmMt": data['type_of_employee'],  # Type of employee (1=personeelslid)
                                     "ViEt": data['employment']  # Dienstbetrekking
-
                                 }
                             }
                         },
                         "AfasOrgunitFunction": {
                             "Element": {
                                 "@DaBe": data['date_effective'],  # Startdate organizational unit
                                 "Fields": {
@@ -1385,33 +1428,40 @@
                     }
                 }
             }
         }
 
         # Add overload fields to the base of the employee data
         fields_to_update_employee = {}
+        fields_to_update_employee.update({"DaMa": data['date_of_marriage']}) if 'date_of_marriage' in data else fields_to_update_employee
+        fields_to_update_employee.update({"DaDe": data['date_of_death']}) if 'employee_id' in data else fields_to_update_employee
         fields_to_update_employee.update({"PsPv": data['send_payslip']}) if 'send_payslip' in data else fields_to_update_employee
         fields_to_update_employee.update({"YsPv": data['send_annual_statement']}) if 'send_annual_statement' in data else fields_to_update_employee
         body['AfasEmployee']['Element'].update({"@EmId": data['employee_id'] if "employee_id" in data else {}})
-
         # add overload employee fields to  the body
         if overload_fields is not None and 'employee' in overload_fields.keys():
             fields_to_update_employee.update(overload_fields['employee'])
         body['AfasEmployee']['Element']['Fields'].update(fields_to_update_employee)
 
-        # updatecontract section
+        # Add overload fields to the base of the contract data
         fields_to_update_contract = {}
         fields_to_update_contract.update({"DaEn": data['end_date_contract']}) if 'end_date_contract' in data else fields_to_update_contract
+        fields_to_update_contract.update({"StAc": data['seniority_date']}) if 'seniority_date' in data else fields_to_update_contract
+        fields_to_update_contract.update({"ViTo": data['probation_period_code']}) if 'probation_period_code' in data else fields_to_update_contract
+        fields_to_update_contract.update({"DaEt": data['end_date_probation_period']}) if 'end_date_probation_period' in data else fields_to_update_contract
+        fields_to_update_contract.update({"DaSc": data['start_date_contract_chain']}) if 'start_date_contract_chain' in data else fields_to_update_contract
+        fields_to_update_contract.update({"ViKe": data['contract_chain_code']}) if 'contract_chain_code' in data else fields_to_update_contract
+        fields_to_update_contract.update({"DbYs": data['date_in_service_original']}) if 'date_in_service_original' in data else fields_to_update_contract
         # add overload contract fields to  the body
         if overload_fields is not None and 'contract' in overload_fields.keys():
             fields_to_update_contract.update(overload_fields['contract'])
         body['AfasEmployee']['Element']['Objects']['AfasContract']['Element']['Fields'].update(fields_to_update_contract)
 
+        # Add overload fields to the base of the salary data
         fields_to_update_salary = {}
-        # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update_salary.update({"SaSt": data['step']}) if 'step' in data else fields_to_update_salary
         fields_to_update_salary.update({"SaYe": data['salary_year']}) if 'salary_year' in data else fields_to_update_salary
         fields_to_update_salary.update({"PtId": data['period_table']}) if 'period_table' in data else fields_to_update_salary.update({"PtId": 5})
         fields_to_update_salary.update({"VaSc": data['salary_scale']}) if 'salary_scale' in data else fields_to_update_salary
         fields_to_update_salary.update({"TaId": data['salary_scale_type']}) if 'salary_scale_type' in data else fields_to_update_salary
         fields_to_update_salary.update({"FuSc": data['function_scale']}) if 'function_scale' in data else fields_to_update_salary
         fields_to_update_salary.update({"FuTa": data['function_scale_type']}) if 'function_scale_type' in data else fields_to_update_salary
@@ -1419,19 +1469,23 @@
         fields_to_update_salary.update({"TtPy": data['apply_timetable']}) if 'apply_timetable' in data else fields_to_update_salary
         fields_to_update_salary.update({"EmSa": data['amount']}) if 'amount' in data else fields_to_update_salary
         if overload_fields is not None and 'salary' in overload_fields.keys():
             fields_to_update_salary.update(overload_fields['salary'])
         # Update the request body with update fields
         body['AfasEmployee']['Element']['Objects']['AfasSalary']['Element']['Fields'].update(fields_to_update_salary)
 
+        # Add overload fields to the base of the person data
         fields_to_update_person = {}
-        # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update_person.update({"In": data['initials']}) if 'initials' in data else fields_to_update_person
         fields_to_update_person.update({"CoBi": data['country_of_birth']}) if 'country_of_birth' in data else fields_to_update_person
         fields_to_update_person.update({"RsBi": data['place_of_birth']}) if 'place_of_birth' in data else fields_to_update_person
+        fields_to_update_person.update({"IsBi": data['birthname_prefix']}) if 'birthname_prefix' in data else fields_to_update_person
+        fields_to_update_person.update({"NmBi": data['birthname']}) if 'birthname' in data else fields_to_update_person
+        fields_to_update_person.update({"IsPa": data['prefix_birthname_partner']}) if 'prefix_birthname_partner' in data else fields_to_update_person
+        fields_to_update_person.update({"NmPa": data['birthname_partner']}) if 'birthname_partner' in data else fields_to_update_person
         fields_to_update_person.update({"EmAd": data['email_work']}) if 'email_work' in data else fields_to_update_person
         fields_to_update_person.update({"EmA2": data['email_home']}) if 'email_home' in data else fields_to_update_person
         fields_to_update_person.update({"SpNm": data['birth_name_separate']}) if 'birth_name_separate' in data else fields_to_update_person
         fields_to_update_person.update({"ViUs": data['name_use']}) if 'name_use' in data else fields_to_update_person
         fields_to_update_person.update({"Is": data['prefix']}) if 'prefix' in data else fields_to_update_person
         fields_to_update_person.update({"CaNm": data['nickname']}) if 'nickname' in data else fields_to_update_person
         fields_to_update_person.update({"EmAd": data['mail_work']}) if 'mail_work' in data else fields_to_update_person
@@ -1444,37 +1498,43 @@
         fields_to_update_person.update({"TeNr": data['phone_work']}) if 'phone_work' in data else fields_to_update_person
         fields_to_update_person.update({"TeN2": data['phone_private']}) if 'phone_private' in data else fields_to_update_person
         if overload_fields is not None and 'person' in overload_fields.keys():
             fields_to_update_person.update(overload_fields['person'])
         # Update the request body with update fields
         body['AfasEmployee']['Element']['Objects']['KnPerson']['Element']['Fields'].update(fields_to_update_person)
 
+        # Add overload fields to the base of the schedule data
         fields_to_update_schedule = {}
-        # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update_schedule.update({"StPa": data['changing_work_pattern']}) if 'changing_work_pattern' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"DyWk": data['days_per_week']}) if 'days_per_week' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"Ft": data['fte']}) if 'fte' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"EtTy": data['type_of_schedule']}) if 'type_of_schedule' in data else fields_to_update_schedule
         if overload_fields is not None and 'schedule' in overload_fields.keys():
             fields_to_update_schedule.update(overload_fields['schedule'])
         # Update the request body with update fields
         body['AfasEmployee']['Element']['Objects']['AfasTimeTable']['Element']['Fields'].update(fields_to_update_schedule)
 
+        # Add fields that you want to update a dict (adding to body itself is too much text)
+        fields_to_update_organisational_unit = {}
+        if overload_fields is not None and 'organisational_unit' in overload_fields.keys():
+            fields_to_update_organisational_unit.update(overload_fields['organisational_unit'])
+        # Update the request body with update fields
+        body['AfasEmployee']['Element']['Objects']['AfasOrgunitFunction']['Element']['Fields'].update(fields_to_update_organisational_unit)
+
         if self.debug:
             print(json.dumps(body))
 
         update = requests.request('POST', url, data=json.dumps(body), headers=self.headers)
 
         return update
 
     def create_sickleave(self, data: dict, overload_fields: dict = None) -> requests.Response:
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
-        :param method: request type
         :return: status code for request and optional error message
         """
 
         allowed_fields = {
             'safety_net': 'SfNt',
             'end_date': 'DaEn',
             'end_date_report_date': 'DMeE',
@@ -1523,15 +1583,14 @@
 
         return update
 
     def update_sickleave(self, data: dict, overload_fields: dict = None) -> requests.Response:
         """
         :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
         :param overload_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
-        :param method: request type
         :return: status code for request and optional error message
         """
         allowed_fields = {
             'safety_net': 'SfNt',
             'end_date': 'DaEn',
             'end_date_report_date': 'DMeE',
             'reason_ending': 'ViRs',
```

### Comparing `salure_helpers_profit-1.3.4/setup.py` & `salure_helpers_profit-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.3.4',
+    version='1.3.5',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

