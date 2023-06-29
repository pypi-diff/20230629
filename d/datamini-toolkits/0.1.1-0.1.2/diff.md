# Comparing `tmp/datamini_toolkits-0.1.1.tar.gz` & `tmp/datamini_toolkits-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamini_toolkits-0.1.1.tar", last modified: Thu Jun 29 15:55:55 2023, max compression
+gzip compressed data, was "datamini_toolkits-0.1.2.tar", last modified: Thu Jun 29 16:05:58 2023, max compression
```

## Comparing `datamini_toolkits-0.1.1.tar` & `datamini_toolkits-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.971596 datamini_toolkits-0.1.1/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:55:55.971472 datamini_toolkits-0.1.1/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 15:50:56.000000 datamini_toolkits-0.1.1/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.967306 datamini_toolkits-0.1.1/datamini_toolkits/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.1/datamini_toolkits/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.968099 datamini_toolkits-0.1.1/datamini_toolkits/cmysql/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.1/datamini_toolkits/cmysql/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.971212 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6143 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2472 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/prompts.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/test_tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.1/datamini_toolkits/tests.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.967971 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      622 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-06-29 15:55:55.971629 datamini_toolkits-0.1.1/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-06-29 15:55:49.000000 datamini_toolkits-0.1.1/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 16:05:58.365271 datamini_toolkits-0.1.2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 16:05:58.365161 datamini_toolkits-0.1.2/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 15:50:56.000000 datamini_toolkits-0.1.2/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 16:05:58.362072 datamini_toolkits-0.1.2/datamini_toolkits/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.2/datamini_toolkits/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 16:05:58.362882 datamini_toolkits-0.1.2/datamini_toolkits/cmysql/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.2/datamini_toolkits/cmysql/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 16:05:58.364780 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6143 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2498 2023-06-29 16:02:35.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/prompts.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/test_tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.2/datamini_toolkits/mock_data/tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.2/datamini_toolkits/tests.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 16:05:58.362773 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 16:05:58.000000 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      622 2023-06-29 16:05:58.000000 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-06-29 16:05:58.000000 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-06-29 16:05:58.000000 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-06-29 16:05:58.000000 datamini_toolkits-0.1.2/datamini_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-06-29 16:05:58.365300 datamini_toolkits-0.1.2/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-06-29 16:04:15.000000 datamini_toolkits-0.1.2/setup.py
```

### Comparing `datamini_toolkits-0.1.1/README.md` & `datamini_toolkits-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/agent.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/agent.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/base.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/base.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/cli.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     db_user = args.user or "root"
     db_password = args.password or ""
     db_name = args.database or "test"
 
     db_uri = f"mysql+pymysql://{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
     return db_uri
 
-if __name__ == "__main__":
 
+
+def main():
     args = get_args()
     db_uri = get_db_uri_from_args(args)
 
     creator = DataMakerAgentCreator(db_uri)
 
     while True:
 
@@ -55,8 +56,12 @@
      根据 user 和 product 表的数据，生成 1000 条 order 表的数据
 
 请输入命令：""")
 
 
         with creator.get_llm_callback() as cb:
             creator.agent.run(request)
-            log.llm_billing(request, cb)
+            log.llm_billing(request, cb)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/logs.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/prompts.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/test_tools.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/test_tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/tools.py` & `datamini_toolkits-0.1.2/datamini_toolkits/mock_data/tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.1/datamini_toolkits.egg-info/SOURCES.txt` & `datamini_toolkits-0.1.2/datamini_toolkits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

