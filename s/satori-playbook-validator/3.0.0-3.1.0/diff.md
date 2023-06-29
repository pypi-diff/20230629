# Comparing `tmp/satori_playbook_validator-3.0.0.tar.gz` & `tmp/satori_playbook_validator-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-3.0.0.tar", last modified: Thu Jun 22 03:46:32 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.1.0.tar", last modified: Thu Jun 29 15:56:33 2023, max compression
```

## Comparing `satori_playbook_validator-3.0.0.tar` & `satori_playbook_validator-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2023-06-22 03:46:18.452247 satori_playbook_validator-3.0.0/README.md
--rw-r--r--   0        0        0      474 2023-06-22 03:46:32.880395 satori_playbook_validator-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      301 2023-06-22 03:46:18.452247 satori_playbook_validator-3.0.0/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5706 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      298 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2361 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      100 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/src/satorici/validator/warnings.py
--rw-r--r--   0        0        0     1613 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-22 03:46:18.456248 satori_playbook_validator-3.0.0/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/README.md
+-rw-r--r--   0        0        0      474 2023-06-29 15:56:33.446518 satori_playbook_validator-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5920 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      298 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1906 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     2467 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-29 15:56:15.898237 satori_playbook_validator-3.1.0/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.0/PKG-INFO
```

### Comparing `satori_playbook_validator-3.0.0/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.1.0/src/satorici/validator/_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,14 +92,18 @@
 def validate_settings(settings: dict):
     _validate(settings_schema, settings)
 
     if "cron" in settings or "rate" in settings:
         if not any(k.startswith("log") for k in settings):
             warnings.warn(NoLogMonitorWarning("Monitor without notifications."))
 
+    if "timeout" in settings and "commandTimeout" in settings:
+        if settings["timeout"] < settings["commandTimeout"]:
+            raise PlaybookValidationError("timeout must be greater than commandTimeout")
+
 
 def is_settings(settings: dict):
     return _is(validate_settings, settings)
 
 
 def has_input(d: dict[str]):
     stack = [v for k, v in d.items() if "^" not in k]
```

### Comparing `satori_playbook_validator-3.0.0/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.1.0/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.0.0/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.1.0/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.0.0/tests/test_playbook_validator.py` & `satori_playbook_validator-3.1.0/tests/test_playbook_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,7 +79,52 @@
         "cmd": [
             ["echo"],
         ],
     }
 
     with pytest.warns(NoLogMonitorWarning):
         validate_playbook(playbook)
+
+
+def test_cron_monitor():
+    playbook = {
+        "settings": {
+            "name": "aaaa",
+            "cron": "0 0 0 0 0",
+            "rate": "0 minutes",
+        },
+        "cmd": [
+            ["echo"],
+        ],
+    }
+
+    with pytest.raises(PlaybookValidationError):
+        validate_playbook(playbook)
+
+
+def test_unnamed_monitor():
+    playbook = {
+        "settings": {
+            "rate": "0 minutes",
+        },
+        "cmd": [
+            ["echo"],
+        ],
+    }
+
+    with pytest.raises(PlaybookValidationError):
+        validate_playbook(playbook)
+
+
+def test_bad_timeout_settings():
+    playbook = {
+        "settings": {
+            "timeout": 1,
+            "commandTimeout": 2,
+        },
+        "cmd": [
+            ["echo"],
+        ],
+    }
+
+    with pytest.raises(PlaybookValidationError):
+        validate_playbook(playbook)
```

### Comparing `satori_playbook_validator-3.0.0/tests/test_reference_finder.py` & `satori_playbook_validator-3.1.0/tests/test_reference_finder.py`

 * *Files identical despite different names*

