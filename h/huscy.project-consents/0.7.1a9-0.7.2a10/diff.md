# Comparing `tmp/huscy.project_consents-0.7.1a9.tar.gz` & `tmp/huscy.project_consents-0.7.2a10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.7.1a9.tar", last modified: Tue Jun  6 10:56:25 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.7.2a10.tar", last modified: Thu Jun 29 09:16:39 2023, max compression
```

## Comparing `huscy.project_consents-0.7.1a9.tar` & `huscy.project_consents-0.7.2a10.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a9/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a9/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.7.1a9/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.328214 huscy.project_consents-0.7.1a9/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-06-06 10:13:14.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      749 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1007 2023-04-27 11:26:24.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1690 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1215 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1923 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/services.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.328214 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     6710 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      737 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent_token.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      379 2023-05-11 13:50:39.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/sign_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      870 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/signed_project_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      287 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4645 2023-06-06 10:13:14.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.7.1a9/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1138 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-06-06 10:56:25.000000 huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-06-01 13:11:47.000000 huscy.project_consents-0.7.1a9/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-06 10:56:25.332213 huscy.project_consents-0.7.1a9/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      440 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      592 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.7.1a9/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      625 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5522 2023-06-06 10:09:08.000000 huscy.project_consents-0.7.1a9/tests/test_viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.930282 huscy.project_consents-0.7.2a10/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.2a10/LICENSE
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       39 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.2a10/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1099 2023-06-29 09:16:39.930282 huscy.project_consents-0.7.2a10/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       19 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.2a10/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.922282 huscy.project_consents-0.7.2a10/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.926282 huscy.project_consents-0.7.2a10/huscy/project_consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       82 2023-06-27 16:00:58.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      749 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      479 2023-01-13 15:29:15.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      194 2022-12-08 10:33:28.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1007 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.926282 huscy.project_consents-0.7.2a10/huscy/project_consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3678 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-12-08 10:34:52.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1690 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1215 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1923 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.922282 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.926282 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6663 2023-06-27 16:00:58.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      737 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/project_consent_token.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      379 2023-05-11 13:38:27.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/sign_project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      902 2023-06-27 16:00:58.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/signed_project_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      287 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4645 2023-06-06 10:11:17.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1527 2023-01-13 15:29:15.000000 huscy.project_consents-0.7.2a10/huscy/project_consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.926282 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1099 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1188 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      115 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-06-29 09:16:39.000000 huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-06-29 09:16:39.930282 huscy.project_consents-0.7.2a10/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1673 2023-04-25 13:22:38.000000 huscy.project_consents-0.7.2a10/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-29 09:16:39.930282 huscy.project_consents-0.7.2a10/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      440 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/tests/test_admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      592 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/tests/test_models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      760 2023-01-30 13:08:18.000000 huscy.project_consents-0.7.2a10/tests/test_project_consent_category_serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      625 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/tests/test_project_consent_serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5522 2023-06-02 13:15:25.000000 huscy.project_consents-0.7.2a10/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.7.1a9/LICENSE` & `huscy.project_consents-0.7.2a10/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/PKG-INFO` & `huscy.project_consents-0.7.2a10/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.7.1a9
+Version: 0.7.2a10
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # project consents
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,12 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# project consents
-
-
```

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/admin.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/forms.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/models.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/serializer.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/services.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent.html` & `huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/project_consent.html`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,14 @@
             .bigskip {margin-top: 1.5cm;}
             .medskip {margin-top: 1cm;}
 
             .contact-data {
                 margin-top: 1.5cm;
             }
 
-            .new_page {
-                page-break-before: always;
-            }
-
             .table-row {display: flex;}
             .table-cell {flex: 1; padding: 5px;}
 
             .btn {visibility: hidden}
 
             {% block extra_css %}{% endblock extra_css %}
         </style>
@@ -79,15 +75,15 @@
             {% endfor %}
 
             <p class="bigskip">
                 Eine Weitergabe, Speicherung, Auswertung und Nutzung der bei wissenschaftlichen Studien erhobenen Daten erfolgt nach gesetzlichen Bestimmungen und setzt vor Teilnahme an der Studie die folgenden freiwilligen Einwilligungen voraus:
             </p>
         </div>
 
-        <div class="page new_page">
+        <div class="page new_page" style="page-break-before: always;">
             <form method="post">
                 {% csrf_token %}
                 <input type="hidden" name="form-TOTAL_FORMS" value="2">
                 <input type="hidden" name="form-INITIAL_FORMS" value="0">
 
                 <h2>Einwilligungserklärung zur Teilnahme an der Studie</h2>
                 <h2>{{ project.title }}</h2>
```

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/project_consent_token.html` & `huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/project_consent_token.html`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/templates/project_consents/signed_project_consent.html` & `huscy.project_consents-0.7.2a10/huscy/project_consents/templates/project_consents/signed_project_consent.html`

 * *Files 10% similar despite different names*

```diff
@@ -27,23 +27,26 @@
 h1.title {color: #7b7d7d; font-size: 18px;}
 h2 {font-size: 20px;}
 h3 {font-size: 19px;}
 
 img.signature {
     border: 1px solid black;
     height: 120px;
+    max-width: 300px;
 }
 {% endblock extra_css %}
 
 
 {% block signature_experimenter %}
+<br>
 <img class="signature" src="{{ form.0.cleaned_data.signature|signature_base64 }}">
 {% endblock signature_experimenter %}
 
 
 {% block signature_subject %}
+<br>
 <img class="signature" src="{{ form.1.cleaned_data.signature|signature_base64 }}">
 {% endblock signature_subject %}
 
 
 {% block submit_button %}
 {% endblock submit_button %}
```

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/views.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.7.2a10/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.7.1a9
+Version: 0.7.2a10
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # project consents
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,12 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-License-File: LICENSE
-
-# project consents
-
-
```

### Comparing `huscy.project_consents-0.7.1a9/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.7.2a10/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 huscy/project_consents/forms.py
 huscy/project_consents/models.py
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
+huscy/project_consents/migrations/0001_initial.py
 huscy/project_consents/migrations/__init__.py
 huscy/project_consents/templates/project_consents/project_consent.html
 huscy/project_consents/templates/project_consents/project_consent_token.html
 huscy/project_consents/templates/project_consents/sign_project_consent.html
 huscy/project_consents/templates/project_consents/signed_project_consent.html
 tests/test_admin.py
 tests/test_models.py
```

### Comparing `huscy.project_consents-0.7.1a9/setup.py` & `huscy.project_consents-0.7.2a10/setup.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/tests/test_models.py` & `huscy.project_consents-0.7.2a10/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.7.2a10/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.7.2a10/tests/test_project_consent_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.7.1a9/tests/test_viewsets.py` & `huscy.project_consents-0.7.2a10/tests/test_viewsets.py`

 * *Files identical despite different names*

