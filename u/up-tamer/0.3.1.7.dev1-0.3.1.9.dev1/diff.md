# Comparing `tmp/up_tamer-0.3.1.7.dev1.tar.gz` & `tmp/up_tamer-0.3.1.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_tamer-0.3.1.7.dev1.tar", last modified: Tue Mar 14 15:48:02 2023, max compression
+gzip compressed data, was "up_tamer-0.3.1.9.dev1.tar", last modified: Wed Mar 15 10:35:52 2023, max compression
```

## Comparing `up_tamer-0.3.1.7.dev1.tar` & `up_tamer-0.3.1.9.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:48:02.924463 up_tamer-0.3.1.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-14 15:48:02.924463 up_tamer-0.3.1.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 15:48:02.924463 up_tamer-0.3.1.7.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:48:02.924463 up_tamer-0.3.1.7.dev1/up_tamer/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/up_tamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/up_tamer/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-03-14 15:47:37.000000 up_tamer-0.3.1.7.dev1/up_tamer/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:48:02.924463 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-14 15:48:02.000000 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-14 15:48:02.000000 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:48:02.000000 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-14 15:48:02.000000 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-14 15:48:02.000000 up_tamer-0.3.1.7.dev1/up_tamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:35:52.152294 up_tamer-0.3.1.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-15 10:35:52.152294 up_tamer-0.3.1.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 10:35:52.152294 up_tamer-0.3.1.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:35:52.152294 up_tamer-0.3.1.9.dev1/up_tamer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/up_tamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/up_tamer/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28163 2023-03-15 10:35:49.000000 up_tamer-0.3.1.9.dev1/up_tamer/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 10:35:52.152294 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-15 10:35:52.000000 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-15 10:35:52.000000 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 10:35:52.000000 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-15 10:35:52.000000 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-15 10:35:52.000000 up_tamer-0.3.1.9.dev1/up_tamer.egg-info/top_level.txt
```

### Comparing `up_tamer-0.3.1.7.dev1/LICENSE` & `up_tamer-0.3.1.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `up_tamer-0.3.1.7.dev1/README.md` & `up_tamer-0.3.1.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `up_tamer-0.3.1.7.dev1/setup.py` & `up_tamer-0.3.1.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `up_tamer-0.3.1.7.dev1/up_tamer/__init__.py` & `up_tamer-0.3.1.9.dev1/up_tamer/__init__.py`

 * *Files identical despite different names*

### Comparing `up_tamer-0.3.1.7.dev1/up_tamer/converter.py` & `up_tamer-0.3.1.9.dev1/up_tamer/converter.py`

 * *Files identical despite different names*

### Comparing `up_tamer-0.3.1.7.dev1/up_tamer/engine.py` & `up_tamer-0.3.1.9.dev1/up_tamer/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         else:
             if self._heuristic is not None:
                 pytamer.tamer_env_set_string_option(self._env, 'tsimple-heuristic', self._heuristic)
             else:
                 pytamer.tamer_env_set_string_option(self._env, 'tsimple-heuristic', "hadd")
             ttplan = self._solve_classical_problem(tproblem, heuristic_fun)
         plan = self._to_up_plan(problem, ttplan)
-        return up.engines.PlanGenerationResult(PlanGenerationResultStatus.UNSOLVABLE_PROVEN if plan is None else PlanGenerationResultStatus.SOLVED_SATISFICING, plan, self.name)
+        return up.engines.PlanGenerationResult(PlanGenerationResultStatus.UNSOLVABLE_INCOMPLETELY if plan is None else PlanGenerationResultStatus.SOLVED_SATISFICING, plan, self.name)
 
     def _convert_type(self, typename: 'up.model.Type',
                       user_types_map: Dict['up.model.Type', pytamer.tamer_type]) -> pytamer.tamer_type:
         if typename.is_bool_type():
             ttype = self._bool_type
         elif typename.is_user_type():
             ttype = user_types_map[typename]
```

