# Comparing `tmp/datamini_toolkits-0.1.0.tar.gz` & `tmp/datamini_toolkits-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamini_toolkits-0.1.0.tar", last modified: Thu Jun 29 15:51:30 2023, max compression
+gzip compressed data, was "datamini_toolkits-0.1.1.tar", last modified: Thu Jun 29 15:55:55 2023, max compression
```

## Comparing `datamini_toolkits-0.1.0.tar` & `datamini_toolkits-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:51:30.274518 datamini_toolkits-0.1.0/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:51:30.274376 datamini_toolkits-0.1.0/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 15:50:56.000000 datamini_toolkits-0.1.0/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:51:30.269206 datamini_toolkits-0.1.0/datamini_toolkits/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.0/datamini_toolkits/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:51:30.269815 datamini_toolkits-0.1.0/datamini_toolkits/cmysql/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.0/datamini_toolkits/cmysql/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:51:30.273714 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6140 2023-06-29 15:30:35.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1614 2023-06-29 15:30:35.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2470 2023-06-29 14:39:45.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/prompts.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/test_tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.0/datamini_toolkits/mock_data/tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.0/datamini_toolkits/tests.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:51:30.269710 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:51:30.000000 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      622 2023-06-29 15:51:30.000000 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-06-29 15:51:30.000000 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-06-29 15:51:30.000000 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-06-29 15:51:30.000000 datamini_toolkits-0.1.0/datamini_toolkits.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-06-29 15:51:30.274549 datamini_toolkits-0.1.0/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-06-29 15:50:56.000000 datamini_toolkits-0.1.0/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.971596 datamini_toolkits-0.1.1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:55:55.971472 datamini_toolkits-0.1.1/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 15:50:56.000000 datamini_toolkits-0.1.1/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.967306 datamini_toolkits-0.1.1/datamini_toolkits/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.1/datamini_toolkits/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.968099 datamini_toolkits-0.1.1/datamini_toolkits/cmysql/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.1/datamini_toolkits/cmysql/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.971212 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6143 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1616 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2472 2023-06-29 15:54:37.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/prompts.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/test_tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.1/datamini_toolkits/mock_data/tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.1/datamini_toolkits/tests.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:55:55.967971 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      622 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-06-29 15:55:55.000000 datamini_toolkits-0.1.1/datamini_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-06-29 15:55:55.971629 datamini_toolkits-0.1.1/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-06-29 15:55:49.000000 datamini_toolkits-0.1.1/setup.py
```

### Comparing `datamini_toolkits-0.1.0/README.md` & `datamini_toolkits-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/agent.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from langchain.callbacks import get_openai_callback
 from langchain.agents import initialize_agent, AgentType
 from langchain.agents.tools import Tool
 from langchain.memory import ConversationBufferMemory
 from langchain.chains import SQLDatabaseChain
 
 
-from prompts import RECORD_CREATOR_PROMPT_TEMPLATE, TABLE_CREATOR_PROMPT_TEMPLATE, SCHEMA_DESIGNER_PROMPT_TEMPLATE
-from base import ChatOpenAIWithLog, SQLDatabaseWithLog
-from logs import log
+from .prompts import RECORD_CREATOR_PROMPT_TEMPLATE, TABLE_CREATOR_PROMPT_TEMPLATE, SCHEMA_DESIGNER_PROMPT_TEMPLATE
+from .base import ChatOpenAIWithLog, SQLDatabaseWithLog
+from .logs import log
 
 
 
 class DataMakerAgentCreator(object):
     def __init__(self, db_uri):
 
         self.db_uri = db_uri
```

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/base.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from langchain.sql_database import SQLDatabase
 from langchain.sql_database import sqlalchemy
 from langchain.chat_models import ChatOpenAI
 
-from tools import parse_sql_script, check_function_creation
-from logs import log
+from .tools import parse_sql_script, check_function_creation
+from .logs import log
 
 class ChatOpenAIWithLog(ChatOpenAI):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def run(self, text: str, **kwargs) -> str:
         rst = super().predict(text=text, **kwargs)
```

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/cli.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from agent import DataMakerAgentCreator
-from logs import log
+from .agent import DataMakerAgentCreator
+from .logs import log
 
 
 def get_args():
     parser = argparse.ArgumentParser(description='SQL Data Maker CLI', add_help=False)
 
 
     # 添加参数选项
```

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/logs.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/prompts.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/test_tools.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/test_tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits/mock_data/tools.py` & `datamini_toolkits-0.1.1/datamini_toolkits/mock_data/tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.0/datamini_toolkits.egg-info/SOURCES.txt` & `datamini_toolkits-0.1.1/datamini_toolkits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

