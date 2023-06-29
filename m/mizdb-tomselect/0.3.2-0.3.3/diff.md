# Comparing `tmp/mizdb-tomselect-0.3.2.tar.gz` & `tmp/mizdb-tomselect-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb-tomselect-0.3.2.tar", last modified: Wed Jun 28 08:27:39 2023, max compression
+gzip compressed data, was "mizdb-tomselect-0.3.3.tar", last modified: Thu Jun 29 09:26:43 2023, max compression
```

## Comparing `mizdb-tomselect-0.3.2.tar` & `mizdb-tomselect-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.472917 mizdb-tomselect-0.3.2/
--rw-r--r--   0 philip    (1000) philip    (1000)     1064 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.2/LICENSE
--rw-r--r--   0 philip    (1000) philip    (1000)    10529 2023-06-28 08:27:39.472917 mizdb-tomselect-0.3.2/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)    10128 2023-06-20 11:54:49.000000 mizdb-tomselect-0.3.2/README.md
--rw-r--r--   0 philip    (1000) philip    (1000)     1600 2023-06-28 08:27:16.000000 mizdb-tomselect-0.3.2/pyproject.toml
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-06-28 08:27:39.472917 mizdb-tomselect-0.3.2/setup.cfg
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.469916 mizdb-tomselect-0.3.2/src/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.470917 mizdb-tomselect-0.3.2/src/mizdb_tomselect/
--rw-r--r--   0 philip    (1000) philip    (1000)      123 2023-05-18 12:38:24.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/__init__.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.469916 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.469916 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.471917 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/css/
--rw-r--r--   0 philip    (1000) philip    (1000)      430 2023-06-15 10:00:33.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.471917 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/js/
--rw-r--r--   0 philip    (1000) philip    (1000)   145941 2023-06-28 08:27:36.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.469916 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.469916 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.471917 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/css/
--rw-r--r--   0 philip    (1000) philip    (1000)    17697 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
--rw-r--r--   0 philip    (1000) philip    (1000)    23112 2023-05-26 08:49:37.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
--rw-r--r--   0 philip    (1000) philip    (1000)     4360 2023-06-27 12:22:49.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     5743 2023-06-20 11:43:52.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect/widgets.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.471917 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)    10529 2023-06-28 08:27:39.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      672 2023-06-28 08:27:39.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-06-28 08:27:39.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        7 2023-06-28 08:27:39.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/requires.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       16 2023-06-28 08:27:39.000000 mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/top_level.txt
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-28 08:27:39.472917 mizdb-tomselect-0.3.2/tests/
--rw-r--r--   0 philip    (1000) philip    (1000)    13937 2023-06-20 06:55:07.000000 mizdb-tomselect-0.3.2/tests/test_e2e.py
--rw-r--r--   0 philip    (1000) philip    (1000)    16071 2023-06-27 12:22:49.000000 mizdb-tomselect-0.3.2/tests/test_views.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2718 2023-06-15 09:59:55.000000 mizdb-tomselect-0.3.2/tests/test_widgets.py
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     1064 2023-05-24 06:41:14.000000 mizdb-tomselect-0.3.3/LICENSE
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10848 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/PKG-INFO
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10446 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/README.md
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     1601 2023-06-29 09:26:26.000000 mizdb-tomselect-0.3.3/pyproject.toml
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)       38 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/setup.cfg
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.989368 mizdb-tomselect-0.3.3/src/
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.012369 mizdb-tomselect-0.3.3/src/mizdb_tomselect/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      123 2023-05-24 06:41:14.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/__init__.py
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/css/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      430 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/css/mizselect.css
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)   145839 2023-06-29 09:26:40.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:42.990368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.013368 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    17697 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    23112 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     4360 2023-06-29 08:29:14.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/views.py
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     6229 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect/widgets.py
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.012369 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    10848 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/PKG-INFO
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)      672 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/SOURCES.txt
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)        1 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/dependency_links.txt
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)        7 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/requires.txt
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)       16 2023-06-29 09:26:42.000000 mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/top_level.txt
+drwxr-xr-x   0 philip-f37  (1000) philip-f37  (1000)        0 2023-06-29 09:26:43.022369 mizdb-tomselect-0.3.3/tests/
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    14349 2023-06-29 09:22:17.000000 mizdb-tomselect-0.3.3/tests/test_e2e.py
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)    16071 2023-06-29 07:01:47.000000 mizdb-tomselect-0.3.3/tests/test_views.py
+-rw-r--r--   0 philip-f37  (1000) philip-f37  (1000)     5000 2023-06-29 09:22:01.000000 mizdb-tomselect-0.3.3/tests/test_widgets.py
```

### Comparing `mizdb-tomselect-0.3.2/LICENSE` & `mizdb-tomselect-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.2/PKG-INFO` & `mizdb-tomselect-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.2
+Version: 0.3.3
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
-Project-URL: Source, https://github.com/Actionb/mizdb-tomselet
+Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TomSelect for Django (MIZDB)
@@ -122,45 +122,45 @@
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
 
 Base autocomplete widget. The arguments of MIZSelect are:
 
-| Argument       | Default value       | Description                                                                                    |
-|----------------|---------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**        | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
-| search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
-| value_field    | `"id"`              | model field that provides the value of an option                                               |
-| label_field    | `"name"`            | model field that provides the label of an option                                               |
-| create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False               | if True, allow selecting multiple options                                                      |
-| changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
+| Argument       | Default value                          | Description                                                                                    |
+|----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
+| model          | **required**                           | the model class that provides the choices                                                      |
+| url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
+| value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
+| label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
+| search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
+| create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
+| multiple       | False                                  | if True, allow selecting multiple options                                                      |
+| changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
+| add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
 ![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
-| Argument           | Default value | Description                         |
-|--------------------|---------------|-------------------------------------|
-| extra_columns      |               | a mapping for additional columns    |
-| value_field_label  | `"ID"`        | table header for the value column   |
-| label_field_label  | `"Object"`    | table header for the label column   |
+| Argument           | Default value                   | Description                         |
+|--------------------|---------------------------------|-------------------------------------|
+| extra_columns      |                                 | a mapping for additional columns    |
+| value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
+| label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
 #### Adding more columns 
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
 argument `extra_columns`.
 
 The column label is the table header label for a given column.
```

### Comparing `mizdb-tomselect-0.3.2/README.md` & `mizdb-tomselect-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -110,45 +110,45 @@
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
 
 Base autocomplete widget. The arguments of MIZSelect are:
 
-| Argument       | Default value       | Description                                                                                    |
-|----------------|---------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**        | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
-| search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
-| value_field    | `"id"`              | model field that provides the value of an option                                               |
-| label_field    | `"name"`            | model field that provides the label of an option                                               |
-| create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False               | if True, allow selecting multiple options                                                      |
-| changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
+| Argument       | Default value                          | Description                                                                                    |
+|----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
+| model          | **required**                           | the model class that provides the choices                                                      |
+| url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
+| value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
+| label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
+| search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
+| create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
+| multiple       | False                                  | if True, allow selecting multiple options                                                      |
+| changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
+| add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
 ![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
-| Argument           | Default value | Description                         |
-|--------------------|---------------|-------------------------------------|
-| extra_columns      |               | a mapping for additional columns    |
-| value_field_label  | `"ID"`        | table header for the value column   |
-| label_field_label  | `"Object"`    | table header for the label column   |
+| Argument           | Default value                   | Description                         |
+|--------------------|---------------------------------|-------------------------------------|
+| extra_columns      |                                 | a mapping for additional columns    |
+| value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
+| label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
 #### Adding more columns 
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
 argument `extra_columns`.
 
 The column label is the table header label for a given column.
```

### Comparing `mizdb-tomselect-0.3.2/pyproject.toml` & `mizdb-tomselect-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mizdb-tomselect"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Philip Becker", email="yummytea1@gmail.com" },
 ]
 description = "Django autocomplete widgets and views using TomSelect"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -16,15 +16,15 @@
 ]
 classifiers = [
     "Framework :: Django",
     "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
-Source = "https://github.com/Actionb/mizdb-tomselet"
+Source = "https://github.com/Actionb/mizdb-tomselect"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/mizdb_tomselect/js/mizselect.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4430,26 +4430,24 @@
         const changelistURL = elem.dataset.changelistUrl;
         const addURL = elem.dataset.addUrl;
         if (changelistURL || addURL) {
             const footer = document.createElement("div");
             footer.classList.add("d-flex", "mt-1", "dropdown-footer");
             if (addURL) {
                 const addBtn = document.createElement("a");
-                addBtn.classList.add("btn", "btn-success", "invisible", "add-btn");
+                addBtn.classList.add("btn", "btn-success", "add-btn", "d-none");
                 addBtn.href = addURL;
                 addBtn.target = "_blank";
                 addBtn.innerHTML = "Hinzuf\xFCgen";
                 footer.appendChild(addBtn);
                 ts.on("load", () => {
                     if (ts.settings.showCreateOption) {
-                        addBtn.classList.remove("invisible");
-                        addBtn.classList.add("visible");
+                        addBtn.classList.remove("d-none");
                     } else {
-                        addBtn.classList.remove("visible");
-                        addBtn.classList.add("invisible");
+                        addBtn.classList.add("d-none");
                     }
                 });
                 ts.on("type", (query) => {
                     if (query) {
                         addBtn.innerHTML = `'${query}' hinzuf\xFCgen...`;
                     } else {
                         addBtn.innerHTML = "Hinzuf\xFCgen";
```

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect/static/vendor/tom-select/css/tom-select.bootstrap5.css.map`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect/views.py` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect/views.py`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect/widgets.py` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect/widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,54 +12,57 @@
     the select element, which are provided by the widget's `build_attrs` method.
     """
 
     def __init__(
         self,
         model,
         url="autocomplete",
-        search_lookup="name__icontains",
-        value_field="id",
-        label_field="name",
+        value_field="",
+        label_field="",
+        search_lookup="",
         create_field="",
         multiple=False,
         changelist_url="",
         add_url="",
         filter_by=(),
         **kwargs,
     ):
         """
         Instantiate a MIZSelect widget.
 
         Args:
             model: the django model that the choices are derived from
             url: the URL pattern name of the view that serves the choices and
               handles requests from the TomSelect element
-            search_lookup: a Django field lookup to use with the given search
-              term to filter the results
             value_field: the name of the model field that corresponds to the
-              choice value of an option (f.ex. 'id')
+              choice value of an option (f.ex. 'id'). Defaults to the name of
+              the model's primary key field.
             label_field: the name of the model field that corresponds to the
-              human-readable value of an option (f.ex. 'name')
+              human-readable value of an option (f.ex. 'name'). Defaults to the
+              value of the model's `name_field` attribute. If the model has no
+              `name_field` attribute, it defaults to 'name'.
+            search_lookup: a Django field lookup to use with the given search
+              term to filter the results
             create_field: the name of the model field used to create new
               model objects with
             multiple: if True, allow selecting multiple options
             changelist_url: URL name of the changelist view for this model
             add_url: URL name of the add view for this model
             filter_by: a 2-tuple (form_field_name, field_lookup) to filter the
               results against the value of the form field using the given
               Django field lookup. For example:
                ('foo', 'bar__id') => results.filter(bar__id=data['foo'])
             kwargs: additional keyword arguments passed to forms.Select
         """
         self.model = model
         self.url = url
-        self.search_lookup = search_lookup
+        self.value_field = value_field or self.model._meta.pk.name
+        self.label_field = label_field or getattr(self.model, "name_field", "name")
+        self.search_lookup = search_lookup or f"{self.label_field}__icontains"
         self.create_field = create_field
-        self.value_field = value_field
-        self.label_field = label_field
         self.multiple = multiple
         self.changelist_url = changelist_url
         self.add_url = add_url
         self.filter_by = filter_by
         super().__init__(**kwargs)
 
     def optgroups(self, name, value, attrs=None):
@@ -106,31 +109,33 @@
         }
         js = ["mizdb_tomselect/js/mizselect.js"]
 
 
 class MIZSelectTabular(MIZSelect):
     """A MIZSelect widget that displays results in a table with a table header."""
 
-    def __init__(self, *args, extra_columns=None, value_field_label="ID", label_field_label="Object", **kwargs):
+    def __init__(self, *args, extra_columns=None, value_field_label="", label_field_label="", **kwargs):
         """
         Instantiate a MIZSelectTabular widget.
 
         Args:
             extra_columns: a mapping of <model field names> to <column labels>
               for additional columns. The field name tells TomSelect what
               values to look up on a model object result for a given column.
               The label is the table header label for a given column.
-            value_field_label: table header label for the value field column
-            label_field_label: table header label for the label field column
+            value_field_label: table header label for the value field column.
+              Defaults to value_field.title().
+            label_field_label: table header label for the label field column.
+              Defaults to the verbose_name of the model.
             args: additional positional arguments passed to MIZSelect
             kwargs: additional keyword arguments passed to MIZSelect
         """
         super().__init__(*args, **kwargs)
-        self.value_field_label = value_field_label
-        self.label_field_label = label_field_label
+        self.value_field_label = value_field_label or self.value_field.title()
+        self.label_field_label = label_field_label or self.model._meta.verbose_name or "Object"
         self.extra_columns = extra_columns or {}
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         """Build HTML attributes for the widget."""
         attrs = super().build_attrs(base_attrs, extra_attrs)
         attrs.update(
             {
```

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/PKG-INFO` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mizdb-tomselect
-Version: 0.3.2
+Version: 0.3.3
 Summary: Django autocomplete widgets and views using TomSelect
 Author-email: Philip Becker <yummytea1@gmail.com>
-Project-URL: Source, https://github.com/Actionb/mizdb-tomselet
+Project-URL: Source, https://github.com/Actionb/mizdb-tomselect
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TomSelect for Django (MIZDB)
@@ -122,45 +122,45 @@
 HTML element via the dataset property. The TomSelect element is then initialized
 from the attributes in the dataset property.
 
 ### MIZSelect
 
 Base autocomplete widget. The arguments of MIZSelect are:
 
-| Argument       | Default value       | Description                                                                                    |
-|----------------|---------------------|------------------------------------------------------------------------------------------------|
-| model          | **required**        | the model class that provides the choices                                                      |
-| url            | `"autocomplete"`    | URL pattern name of the autocomplete view                                                      |
-| search_lookup  | `"name__icontains"` | the lookup to use when filtering the results                                                   |
-| value_field    | `"id"`              | model field that provides the value of an option                                               |
-| label_field    | `"name"`            | model field that provides the label of an option                                               |
-| create_field   |                     | model field to create new objects with ([see below](#ajax-request))                            |
-| multiple       | False               | if True, allow selecting multiple options                                                      |
-| changelist_url |                     | URL name of the changelist view for this model ([see below](#changelist-link))                 |
-| add_url        |                     | URL name of the add view for this model([see below](#option-creation))                         |
-| filter_by      |                     | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
+| Argument       | Default value                          | Description                                                                                    |
+|----------------|----------------------------------------|------------------------------------------------------------------------------------------------|
+| model          | **required**                           | the model class that provides the choices                                                      |
+| url            | `"autocomplete"`                       | URL pattern name of the autocomplete view                                                      |
+| value_field    | `f"{model._meta.pk.name}"`             | model field that provides the value of an option                                               |
+| label_field    | `getattr(model, "name_field", "name")` | model field that provides the label of an option                                               |
+| search_lookup  | `f"{label_field}__icontains"`          | the lookup to use when filtering the results                                                   |
+| create_field   |                                        | model field to create new objects with ([see below](#ajax-request))                            |
+| multiple       | False                                  | if True, allow selecting multiple options                                                      |
+| changelist_url |                                        | URL name of the changelist view for this model ([see below](#changelist-link))                 |
+| add_url        |                                        | URL name of the add view for this model([see below](#option-creation))                         |
+| filter_by      |                                        | a 2-tuple defining an additional filter ([see below](#filter-against-values-of-another-field)) |
 
 
 ### MIZSelectTabular
 
 
 This widget displays the results in tabular form. A table header will be added
 to the dropdown. By default, the table contains two columns: one column for the choice 
 value (commonly the "ID" of the option) and one column for the choice label (the 
 human-readable part of the choice).
 
 ![Tabular select preview](./assets/mizselect_tabular.png "Tabular select preview")
 
 MIZSelectTabular has the following additional arguments:
 
-| Argument           | Default value | Description                         |
-|--------------------|---------------|-------------------------------------|
-| extra_columns      |               | a mapping for additional columns    |
-| value_field_label  | `"ID"`        | table header for the value column   |
-| label_field_label  | `"Object"`    | table header for the label column   |
+| Argument           | Default value                   | Description                         |
+|--------------------|---------------------------------|-------------------------------------|
+| extra_columns      |                                 | a mapping for additional columns    |
+| value_field_label  | `f"{value_field.title()}"`      | table header for the value column   |
+| label_field_label  | `f"{model._meta.verbose_name}"` | table header for the label column   |
 
 #### Adding more columns 
 
 To add more columns, pass a `result attribute name: column label` mapping to the widget
 argument `extra_columns`.
 
 The column label is the table header label for a given column.
```

### Comparing `mizdb-tomselect-0.3.2/src/mizdb_tomselect.egg-info/SOURCES.txt` & `mizdb-tomselect-0.3.3/src/mizdb_tomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizdb-tomselect-0.3.2/tests/test_e2e.py` & `mizdb-tomselect-0.3.3/tests/test_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         expect(dropdown_header).to_be_attached()
 
     def test_header_columns(self, _page, header_columns):
         """Assert that the dropdown header has the expected columns."""
         expect(header_columns).to_have_count(5)
         id_col, label_col, jahr_col, num_col, lnum_col = header_columns.all()
         expect(id_col).to_have_class("col-1")
-        expect(id_col).to_have_text("ID")
+        expect(id_col).to_have_text("Id")
         expect(label_col).to_have_class("col-5")
         expect(label_col).to_have_text("Ausgabe")
         expect(jahr_col).to_have_class("col")
         expect(jahr_col).to_have_text("Jahr")
         expect(num_col).to_have_class("col")
         expect(num_col).to_have_text("Nummer")
         expect(lnum_col).to_have_class("col")
@@ -335,15 +335,15 @@
     def test_add_button_click_with_search_term(self, logged_in, _page, add_button, search_input, live_server):
         """
         Assert that clicking the add button with a search term given starts a
         POST request to create a new object instead of opening the 'add' _page.
         """
         with _page.expect_request_finished():
             search_input.fill("2022-99")
-        with _page.expect_response(live_server.url + reverse("ac"), timeout=1000) as response_info:
+        with _page.expect_response(live_server.url + reverse("ac")) as response_info:
             add_button.click()
         response = response_info.value
         data = response.json()
         assert data["text"] == "2022-99"
         assert data["pk"]
 
     def test_add_button_successful_creation(self, logged_in, _page, add_button, search_input):
@@ -354,14 +354,22 @@
         with _page.expect_request_finished():
             search_input.fill("2022-99")
         with _page.expect_request_finished():
             add_button.click()
         expect(_page.locator(".ts-control .item")).to_have_text("2022-99")
         expect(_page.locator(".dropdown-content")).not_to_be_visible()
 
+    def test_add_button_hidden_for_unauthenticated_user(self, username, add_button):
+        """The 'add' button should be hidden if the user is not logged in."""
+        expect(add_button).to_be_hidden()
+
+    def test_footer_not_shown_when_add_btn_invisible(self, username, dropdown_footer):
+        """The footer div should not be shown when the 'add' button is invisible."""
+        expect(dropdown_footer).to_be_hidden()
+
 
 @pytest.mark.django_db
 @pytest.mark.parametrize("view_name", ["changelist"])
 class TestFooterChangelistButton:
     def test_has_visible_changelist_button(self, changelist_button):
         """Assert that the dropdown footer contains a visible 'changelist' button."""
         expect(changelist_button).to_be_visible()
```

### Comparing `mizdb-tomselect-0.3.2/tests/test_views.py` & `mizdb-tomselect-0.3.3/tests/test_views.py`

 * *Files identical despite different names*

