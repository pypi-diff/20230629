# Comparing `tmp/django_cookie_consent_gutsh-1.0.1-py3-none-any.whl.zip` & `tmp/django_cookie_consent_gutsh-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 8106 bytes, number of entries: 19
+Zip file size: 8952 bytes, number of entries: 20
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 08:39 cookie_consent/__init__.py
 -rw-r--r--  2.0 unx      108 b- defN 23-Apr-15 13:09 cookie_consent/admin.py
 -rw-r--r--  2.0 unx      159 b- defN 23-Apr-14 08:39 cookie_consent/apps.py
 -rw-r--r--  2.0 unx      327 b- defN 23-Apr-15 13:30 cookie_consent/models.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Apr-14 08:39 cookie_consent/tests.py
 -rw-r--r--  2.0 unx      180 b- defN 23-Apr-15 12:36 cookie_consent/urls.py
 -rw-r--r--  2.0 unx     1249 b- defN 23-Apr-15 13:29 cookie_consent/views.py
 -rw-r--r--  2.0 unx      732 b- defN 23-Apr-15 12:52 cookie_consent/migrations/0001_initial.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 08:39 cookie_consent/migrations/__init__.py
 -rw-r--r--  2.0 unx      104 b- defN 23-Jun-21 15:06 cookie_consent/static/cookie_consent/css/README.md
 -rw-r--r--  2.0 unx      470 b- defN 23-Jun-21 11:29 cookie_consent/static/cookie_consent/css/cookie_consent.scss
 -rw-r--r--  2.0 unx      462 b- defN 23-Apr-14 09:46 cookie_consent/static/cookie_consent/css/index.css
 -rw-r--r--  2.0 unx      245 b- defN 23-Apr-14 09:46 cookie_consent/static/cookie_consent/css/index.css.map
+-rw-r--r--  2.0 unx     1938 b- defN 23-Jun-29 05:36 cookie_consent/static/cookie_consent/js/main.js
 -rw-r--r--  2.0 unx      704 b- defN 23-Apr-15 13:27 cookie_consent/templates/cookie_consent/includes/consent.html
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-21 15:23 django_cookie_consent_gutsh-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1778 b- defN 23-Jun-21 15:23 django_cookie_consent_gutsh-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 15:23 django_cookie_consent_gutsh-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-21 15:23 django_cookie_consent_gutsh-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1782 b- defN 23-Jun-21 15:23 django_cookie_consent_gutsh-1.0.1.dist-info/RECORD
-19 files, 9541 bytes uncompressed, 5090 bytes compressed:  46.7%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-29 05:42 django_cookie_consent_gutsh-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-29 05:42 django_cookie_consent_gutsh-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 05:42 django_cookie_consent_gutsh-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 05:42 django_cookie_consent_gutsh-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1886 b- defN 23-Jun-29 05:42 django_cookie_consent_gutsh-1.0.2.dist-info/RECORD
+20 files, 11529 bytes uncompressed, 5766 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -33,26 +33,29 @@
 
 Filename: cookie_consent/static/cookie_consent/css/index.css
 Comment: 
 
 Filename: cookie_consent/static/cookie_consent/css/index.css.map
 Comment: 
 
+Filename: cookie_consent/static/cookie_consent/js/main.js
+Comment: 
+
 Filename: cookie_consent/templates/cookie_consent/includes/consent.html
 Comment: 
 
-Filename: django_cookie_consent_gutsh-1.0.1.dist-info/LICENSE
+Filename: django_cookie_consent_gutsh-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_cookie_consent_gutsh-1.0.1.dist-info/METADATA
+Filename: django_cookie_consent_gutsh-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: django_cookie_consent_gutsh-1.0.1.dist-info/WHEEL
+Filename: django_cookie_consent_gutsh-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_cookie_consent_gutsh-1.0.1.dist-info/top_level.txt
+Filename: django_cookie_consent_gutsh-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_cookie_consent_gutsh-1.0.1.dist-info/RECORD
+Filename: django_cookie_consent_gutsh-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `django_cookie_consent_gutsh-1.0.1.dist-info/LICENSE` & `django_cookie_consent_gutsh-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_cookie_consent_gutsh-1.0.1.dist-info/METADATA` & `django_cookie_consent_gutsh-1.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent-gutsh
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cookie consent component for any Django web-site
 Home-page: https://www.barskiylab.com/
 Author: Artem Barskii
 Author-email: Artem Barskii <artemiy.barskiy@gmail.com>
 License: MIT  # Will be changed later perhaps
 Project-URL: Homepage, https://github.com/gutsh/django-cookie-consent
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,14 @@
   
   For example, I've included that text in my base template:
 
   ```
   {% block cookie_consent %}
     <link rel="stylesheet" href="{% static 'cookie_consent/css/index.css' %}">
     {% include 'cookie_consent/includes/consent.html' %}
-    <script type="module" src="/assets/js/toolkit/cookie_consent.js"></script>
+    <script defer src="{% static 'cookie_consent/js/main.js' %}"></script>
   {% endblock %}
   ```
 
-  Don't forget to serve that script and css files! You can find them in distribution, css is in both source and compiled forms and is already fine (as long as you run `collectstatic` command), and javascript is available under `assets/js/tookit`.
+  Don't forget to serve that script and css files! You can find them in distribution, css and js are in both source and compiled forms and is are fine (as long as you run `collectstatic` command).
 
 5. Start the development server and visit necessary pages.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-cookie-consent-gutsh Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: django-cookie-consent-gutsh Version: 1.0.2 Summary:
 Cookie consent component for any Django web-site Home-page: https://
 www.barskiylab.com/ Author: Artem Barskii Author-email: Artem Barskii
 barskiy@gmail.com> License: MIT # Will be changed later perhaps Project-URL:
 Homepage, https://github.com/gutsh/django-cookie-consent Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
@@ -12,11 +12,10 @@
 ..., ] ``` 2. Include the cookie\_consent URLconf in your project urls.py like
 this: ``` path("cookie_consent/", include("cookie_consent.urls")), ``` 3. Run
 `python manage.py migrate` to create the models. 4. Include consent template in
 your web-site templates. For example, I've included that text in my base
 template: ``` {% block cookie_consent %}
  {% include 'cookie_consent/includes/consent.html' %}
  {% endblock %} ``` Don't forget to serve that script and css files! You can
-find them in distribution, css is in both source and compiled forms and is
-already fine (as long as you run `collectstatic` command), and javascript is
-available under `assets/js/tookit`. 5. Start the development server and visit
-necessary pages.
+find them in distribution, css and js are in both source and compiled forms and
+is are fine (as long as you run `collectstatic` command). 5. Start the
+development server and visit necessary pages.
```

## Comparing `django_cookie_consent_gutsh-1.0.1.dist-info/RECORD` & `django_cookie_consent_gutsh-1.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 cookie_consent/views.py,sha256=AyYhCT9xKusivyDK5Sq3qKCqgsQsvr4QhHI11X8ZbTw,1249
 cookie_consent/migrations/0001_initial.py,sha256=RVfOKneBwbLBy9R8j6vV62o8qOGAZLA1sT4_UwIY42I,732
 cookie_consent/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cookie_consent/static/cookie_consent/css/README.md,sha256=mXCWfhLhvT55G6zBywRVf2CjUuIoY8oL3m2NVNpTpoA,104
 cookie_consent/static/cookie_consent/css/cookie_consent.scss,sha256=3RH-e1H3Z06lBsIYlzWLD-1FLf9SoJAXgq3JpwHLaMw,470
 cookie_consent/static/cookie_consent/css/index.css,sha256=6wPNyCl-whNvfZEjhaQbG4HhXOAS_CPEhXet1JrnaM4,462
 cookie_consent/static/cookie_consent/css/index.css.map,sha256=RE2JfSPD76qIKIP3vtdstobVz7Ub54RRSmDv0SBgqh0,245
+cookie_consent/static/cookie_consent/js/main.js,sha256=0DeASO1QIkB8TpNTOM9KACaElBzPuRG43V2iNSG-7io,1938
 cookie_consent/templates/cookie_consent/includes/consent.html,sha256=_eYBGDTwtJFIq3Oq6MACRsqFP55o-24P6VVTWnDhgf4,704
-django_cookie_consent_gutsh-1.0.1.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-django_cookie_consent_gutsh-1.0.1.dist-info/METADATA,sha256=Mt4A8HpM6C_BwRxTzlqmma0ybrDQw3G-f4p2_w1qQNs,1778
-django_cookie_consent_gutsh-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_cookie_consent_gutsh-1.0.1.dist-info/top_level.txt,sha256=wD8Ix58rJguYeYfils_Z40QfVybiRYb1vwRNm09HN4M,15
-django_cookie_consent_gutsh-1.0.1.dist-info/RECORD,,
+django_cookie_consent_gutsh-1.0.2.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+django_cookie_consent_gutsh-1.0.2.dist-info/METADATA,sha256=Gjc8QIIqCwfkTYHP_sjrJDcdq7ODKGVruV7eXWP5QUc,1724
+django_cookie_consent_gutsh-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_cookie_consent_gutsh-1.0.2.dist-info/top_level.txt,sha256=wD8Ix58rJguYeYfils_Z40QfVybiRYb1vwRNm09HN4M,15
+django_cookie_consent_gutsh-1.0.2.dist-info/RECORD,,
```

