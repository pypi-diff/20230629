# Comparing `tmp/django-translatemessages-0.0.4.tar.gz` & `tmp/django-translatemessages-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-translatemessages-0.0.4.tar", last modified: Wed Jun 21 10:30:31 2023, max compression
+gzip compressed data, was "django-translatemessages-0.0.5.tar", last modified: Thu Jun 29 08:24:01 2023, max compression
```

## Comparing `django-translatemessages-0.0.4.tar` & `django-translatemessages-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      125 2023-06-21 10:29:53.000000 django-translatemessages-0.0.4/CHANGELOG.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.4/LICENSE
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.4/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4191 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3077 2023-06-12 15:37:11.000000 django-translatemessages-0.0.4/README.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-21 10:28:43.000000 django-translatemessages-0.0.4/django_translatemessages/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/management/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.4/django_translatemessages/management/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages/management/commands/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.4/django_translatemessages/management/commands/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11579 2023-06-21 10:28:43.000000 django-translatemessages-0.0.4/django_translatemessages/management/commands/translatemessages.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/django_translatemessages.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4191 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-21 10:30:31.000000 django-translatemessages-0.0.4/django_translatemessages.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-21 10:30:31.623843 django-translatemessages-0.0.4/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.4/setup.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      274 2023-06-29 08:23:10.000000 django-translatemessages-0.0.5/CHANGELOG.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.5/LICENSE
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.5/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4340 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3077 2023-06-12 15:37:11.000000 django-translatemessages-0.0.5/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/django_translatemessages/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-29 08:23:10.000000 django-translatemessages-0.0.5/django_translatemessages/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/django_translatemessages/management/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.5/django_translatemessages/management/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/django_translatemessages/management/commands/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.5/django_translatemessages/management/commands/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12392 2023-06-29 08:23:10.000000 django-translatemessages-0.0.5/django_translatemessages/management/commands/translatemessages.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-29 08:24:01.409378 django-translatemessages-0.0.5/django_translatemessages.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4340 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-29 08:24:01.000000 django-translatemessages-0.0.5/django_translatemessages.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-29 08:24:01.413378 django-translatemessages-0.0.5/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.5/setup.py
```

### Comparing `django-translatemessages-0.0.4/LICENSE` & `django-translatemessages-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.4/PKG-INFO` & `django-translatemessages-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.4
+Version: 0.0.5
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -124,14 +124,19 @@
 
 For more options, run ``python ./manage.py translatemessages -h``
 
 
 News
 ----
 
+0.0.5 (2023-06-29)
+------------------
+- Force translation of fuzzy strings except when obsolete or already translated
+  by django-translatemessages
+
 0.0.4 (2023-06-21)
 ------------------
 - Do not translate fuzzy strings
 
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.4/README.rst` & `django-translatemessages-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.4/django_translatemessages/management/commands/translatemessages.py` & `django-translatemessages-0.0.5/django_translatemessages/management/commands/translatemessages.py`

 * *Files 3% similar despite different names*

```diff
@@ -250,34 +250,46 @@
         )
         translator = self.translator_cls(**translator_params)
         if self.do_batch:
             entries = [
                 entry
                 for entry in po
                 if (
-                    (not entry.translated() or self.options["all"])
+                    (
+                        (
+                            not entry.translated()
+                            and not entry.obsolete
+                            and "translatemessages" not in entry.comment
+                        )
+                        or self.options["all"]
+                    )
                     and self.filter_msgid(entry.msgid)
                 )
             ]
             nb_translations += len(entries)
             texts = [entry.msgid for entry in entries]
             translated_texts = self.translate_text_batch(texts, translator)
             for entry, translated_text in zip(entries, translated_texts):
                 entry.msgstr = translated_text
+                if "translatemessages" not in entry.comment:
+                    entry.comment += "-> Translated with django-translatemessages"
                 if self.auto_fuzzy:
-                    entry.flags.append("fuzzy")
+                    if "fuzzy" not in entry.flags:
+                        entry.flags.append("fuzzy")
                 self.stdout.write(
                     colorize(f"{entry.msgid}", fg="blue"),
                     ending="",
                 )
                 self.stdout.write(colorize(f"-> {translated_text}", fg="cyan"))
         else:
             for entry in po:
                 if (
-                    not entry.translated() and "fuzzy" not in entry.flags
+                    not entry.obsolete
+                    and "translatemessages" not in entry.comment
+                    and not entry.translated()
                 ) or self.options["all"]:
                     filtered_msgid = self.filter_msgid(entry.msgid)
                     if filtered_msgid:
                         nb_translations += 1
                         self.stdout.write(
                             colorize(f"{entry.msgid}", fg="blue"),
                             ending="",
@@ -285,16 +297,21 @@
                         if translator.source != translator.target:
                             translated_text = self.translate_text(
                                 filtered_msgid, translator
                             )
                         else:
                             translated_text = filtered_msgid
                         entry.msgstr = translated_text
+                        if "translatemessages" not in entry.comment:
+                            entry.comment += (
+                                "-> Translated with django-translatemessages"
+                            )
                         if self.auto_fuzzy:
-                            entry.flags.append("fuzzy")
+                            if "fuzzy" not in entry.flags:
+                                entry.flags.append("fuzzy")
                         self.stdout.write(colorize(f"-> {translated_text}", fg="cyan"))
 
         if nb_translations:
             self.stdout.write(
                 self.style.SUCCESS(f"{nb_translations} strings translated")
             )
             if self.options["dry_run"]:
```

### Comparing `django-translatemessages-0.0.4/django_translatemessages.egg-info/PKG-INFO` & `django-translatemessages-0.0.5/django_translatemessages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translatemessages
-Version: 0.0.4
+Version: 0.0.5
 Summary: Translate Django .po files
 Home-page: https://github.com/elapouya/django-translatemessages
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: MIT
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
@@ -124,14 +124,19 @@
 
 For more options, run ``python ./manage.py translatemessages -h``
 
 
 News
 ----
 
+0.0.5 (2023-06-29)
+------------------
+- Force translation of fuzzy strings except when obsolete or already translated
+  by django-translatemessages
+
 0.0.4 (2023-06-21)
 ------------------
 - Do not translate fuzzy strings
 
 0.0.2 (2023-06-11)
 ------------------
 - First commit
```

### Comparing `django-translatemessages-0.0.4/django_translatemessages.egg-info/SOURCES.txt` & `django-translatemessages-0.0.5/django_translatemessages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.4/setup.py` & `django-translatemessages-0.0.5/setup.py`

 * *Files identical despite different names*

