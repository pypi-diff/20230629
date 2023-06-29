# Comparing `tmp/JestingLang-0.0.0a7.tar.gz` & `tmp/JestingLang-0.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JestingLang-0.0.0a7.tar", last modified: Sun Jun 25 11:52:14 2023, max compression
+gzip compressed data, was "JestingLang-0.0.0a8.tar", last modified: Thu Jun 29 09:19:51 2023, max compression
```

## Comparing `JestingLang-0.0.0a7.tar` & `JestingLang-0.0.0a8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.430865 JestingLang-0.0.0a7/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a7/LICENSE
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-25 11:52:14.430865 JestingLang-0.0.0a7/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5048 2023-06-24 06:31:03.000000 JestingLang-0.0.0a7/README.md
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-25 11:52:14.446556 JestingLang-0.0.0a7/setup.cfg
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1564 2023-06-25 11:51:20.000000 JestingLang-0.0.0a7/setup.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.391610 JestingLang-0.0.0a7/src/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.731538 JestingLang-0.0.0a7/src/JestingLang/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.951585 JestingLang-0.0.0a7/src/JestingLang/Core/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.219187 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      338 2023-06-17 12:27:43.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/AbstractDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1962 2023-06-23 14:00:27.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1097 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1311 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.329064 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4766 2023-06-22 15:16:12.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/JestingAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.596683 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1458 2023-06-11 13:16:25.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1528 2023-06-19 14:48:18.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3014 2023-06-24 03:02:41.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2593 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 12:31:05.000000 JestingLang-0.0.0a7/src/JestingLang/Core/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.643602 JestingLang-0.0.0a7/src/JestingLang/JestingScript/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.801075 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      660 2023-06-21 14:08:54.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/AbstractScriptDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4913 2023-06-23 14:12:13.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.910500 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2150 2023-06-21 14:08:54.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.021545 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3340 2023-06-21 14:23:12.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 13:09:13.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)    13162 2023-06-23 13:58:27.000000 JestingLang-0.0.0a7/src/JestingLang/LexerParser.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)    11414 2023-06-23 14:12:21.000000 JestingLang-0.0.0a7/src/JestingLang/LexerParser_cachedParseTable.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.068786 JestingLang-0.0.0a7/src/JestingLang/Misc/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.226034 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2082 2023-06-23 13:58:27.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/LogicFunctions.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2919 2023-06-22 15:28:50.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/OperationMapping.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.396830 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      688 2023-06-17 13:17:53.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/DereferencerHelper.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      349 2023-06-18 00:00:43.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/LexerParserHelpers.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a7/src/JestingLang/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3037 2023-06-17 13:52:56.000000 JestingLang-0.0.0a7/src/JestingLang/main.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.904662 JestingLang-0.0.0a7/src/JestingLang.egg-info/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1830 2023-06-25 11:52:12.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/SOURCES.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/dependency_links.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/requires.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/top_level.txt
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:51.046224 JestingLang-0.0.0a8/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a8/LICENSE
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 09:19:51.047254 JestingLang-0.0.0a8/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5263 2023-06-29 09:14:50.000000 JestingLang-0.0.0a8/README.md
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-29 09:19:51.056241 JestingLang-0.0.0a8/setup.cfg
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1564 2023-06-29 09:14:58.000000 JestingLang-0.0.0a8/setup.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.108373 JestingLang-0.0.0a8/src/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.432034 JestingLang-0.0.0a8/src/JestingLang/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.650813 JestingLang-0.0.0a8/src/JestingLang/Core/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.904025 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      338 2023-06-17 12:27:43.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/AbstractDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2027 2023-06-27 11:59:14.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1097 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1311 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.004673 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4813 2023-06-29 07:06:24.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/JestingAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.258545 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1561 2023-06-29 00:03:40.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1528 2023-06-19 14:48:18.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3014 2023-06-24 03:02:41.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2593 2023-06-17 13:10:33.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 12:31:05.000000 JestingLang-0.0.0a8/src/JestingLang/Core/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.302727 JestingLang-0.0.0a8/src/JestingLang/JestingScript/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.400545 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     6024 2023-06-29 05:30:35.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.502179 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2419 2023-06-29 06:38:18.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.601722 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3242 2023-06-29 06:38:18.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 13:09:13.000000 JestingLang-0.0.0a8/src/JestingLang/JestingScript/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    16076 2023-06-29 09:04:57.000000 JestingLang-0.0.0a8/src/JestingLang/LexerParser.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    14904 2023-06-29 07:06:25.000000 JestingLang-0.0.0a8/src/JestingLang/LexerParser_cachedParseTable.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.645722 JestingLang-0.0.0a8/src/JestingLang/Misc/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:50.799425 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2391 2023-06-28 12:22:45.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/LogicFunctions.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3540 2023-06-29 07:03:12.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/OperationMapping.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:51.005069 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      688 2023-06-17 13:17:53.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/DereferencerHelper.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      349 2023-06-18 00:00:43.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/LexerParserHelpers.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      342 2023-06-27 11:06:51.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/NonFileExternalFileLoader.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a8/src/JestingLang/Misc/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a8/src/JestingLang/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3037 2023-06-17 13:52:56.000000 JestingLang-0.0.0a8/src/JestingLang/main.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-29 09:19:49.610886 JestingLang-0.0.0a8/src/JestingLang.egg-info/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1815 2023-06-29 09:19:49.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/requires.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-29 09:19:48.000000 JestingLang-0.0.0a8/src/JestingLang.egg-info/top_level.txt
```

### Comparing `JestingLang-0.0.0a7/LICENSE` & `JestingLang-0.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/PKG-INFO` & `JestingLang-0.0.0a8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a7/README.md` & `JestingLang-0.0.0a8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 It can be considered a subset of the core languages used 
 in those programs, but lacking many of the rich syntax and 
 functions they use.
 
 It was created for the JESTING APP, a Python-based 
 Spreadsheet program used to emulate behaviours similar 
 to those Spreadsheet Applications. Mostly to test 
-esoteric programs created for those applications.
+esoteric code created to work on those applications.
 
 ## Syntax and AST
 
 The Jesting Lang syntax follows the standard used by most
 spreadsheets programs, allowing simple operations (+, -, *
 , /, =, & ), the **IF token** (to allow branching), the use of 
 indirections to other cells such as A2 (key behaviour or
@@ -46,21 +46,21 @@
   compiling/parsing process without any interpretation. 
 
 
 * **Visitors** explore the trees and do something with them, 
   which could be as trivial as printing its data. The ones
   we will actually care about are those that take care of 
   doing the interpretations/execution of the AST. The idea 
-  is to keep them "technology-agnostic", so these visitors 
+  is to keep them "application-agnostic", so these visitors 
   do not manipulate memory directly on their own, and 
   have no way of directly resolving any reference.
 
 
 * **De-referencers** can access memory and resolve the
-  references used in the visitors. They exists to abstract
+  references used in the visitors. They exist to abstract
   the behaviour with secondary effect of "of real components" 
   such as databases. Most of the examples of this repo will
   be constrained to python structures, such as simple
   arrays or key-value maps.
 
 ## Fixed vs Volatile Visitors
 
@@ -117,14 +117,25 @@
 
     // Output the value of [BOOK_A]Sheet_A!A2 
     !A2
 
     // Output all of the values 
     !!
 
+    // Import code from other File
+    #INCLUDE imported_in_example.jestScript
+
+    // Create an Alias
+    FIRST_CELL ? A1
+
+    // Use the Alias as a regular cell name
+    FIRST_CELL @ 12
+    A2 @= FIRST_CELL + 1
+    !FIRST_CELL
+
     // Close a file
     { BOOK_A
 
 We could compile it in Python with:
 
     lexerparser = LexerParser(multilineScript=True)
     parser = lexerparser.parser
@@ -136,10 +147,9 @@
 add a handful of test to make sure the language is working 
 as expected. In the future, running this (or some derivation
 of this) will probably be the main goal of this library.
 
 ## TODO
 
 * Finish dates as datatypes
-* Finish the Script visitor
 * Add function for readall
 * Use the script visitor to create more test cases
```

### Comparing `JestingLang-0.0.0a7/setup.py` & `JestingLang-0.0.0a8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='JestingLang',
-    version='0.0.0a7',
+    version='0.0.0a8',
     author='itrufat',
     description='A compiler for the minimalist spreadsheet language Jesting',
     long_description='A compiler + a few node navigators (including an interpreter) for a minimalist language intended to copy the most basic functionalities found in spreadsheet-applications called JestingLang. It was created to be used with Jesting, a spreadsheet terminal tool.',
     long_description_content_type='text/markdown',
     url='https://github.com/itruffat/JestingLang',
     packages=['JestingLang',
               'JestingLang.Core',
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from JestingLang.Misc.JLogic.LogicFunctions import extract_address
 
 
 class CachedCellDereferencer(CachedDereferencer):
     """Same as CachedDeferencer but parsing the key to emulate workbooks, worksheets and cells.
     """
 
+    def _parse(self, name):
+        return extract_address(name)
+
     def resolveReference(self, name):
-        _, book, sheet, cell, _ = extract_address(name)
+        _, book, sheet, cell, _ = self._parse(name)
         if (book not in self.cache.keys() or self.cache[book] is None) or \
             (sheet not in self.cache[book].keys() or self.cache[book][sheet] is None) or \
             (cell not in self.cache[book][sheet].keys() or self.cache[book][sheet][cell] is None):
             return EmptyValueNode()
         return self.cache[book][sheet][cell]
 
     def write(self, key, formula, value=None):
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedDereferencer.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/CachedDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/JestingAST.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JParsing/JestingAST.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 
-operations = {"+","-","*","/","&","=",'>','NOT','AND','OR', "u-", 'MOD'}
+operations = {"PLUS", "MINUS", "NEGATE", "TIMES", "DIVIDE", "AMPERSAND", "EQUALS", 'BIGGER', 'NOT', 'AND', 'OR', 'MOD'}
 
 class Node(ABC):
     def __init__(self):
         self.children = {}
 
     @abstractmethod
     def accept(self, visitor):
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
     def visitIndirect(self, node):
         return None
 
     def visitTick(self, node):
         raise Exception("Not implemented outside of ScriptJester")
 
+    def visitAlias(self, node):
+        raise Exception("Not implemented outside of ScriptJester")
+
     def visitRawInput(self, node):
         raise Exception("Not implemented outside of ScriptJester")
 
     def visitAssign(self, node):
         raise Exception("Not implemented outside of ScriptJester")
 
     def visitSetDefaults(self, node):
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py` & `JestingLang-0.0.0a8/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py` & `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from JestingLang.Core.JParsing.JestingAST import EmptyValueNode
-from JestingLang.JestingScript.JDereferencer.AbstractScriptDereferencer import AbstractScriptDereferencer
+from JestingLang.Core.JDereferencer.CachedCellDereferencer import CachedCellDereferencer
+from JestingLang.JestingScript.JScriptManager.AbstractScriptManager import AbstractScriptManager
 from JestingLang.Misc.JLogic.LogicFunctions import extract_address
 
 
 class SDException(BaseException):
     def __init__(self,msg):
         super().__init__()
         self.msg = msg
@@ -13,63 +14,72 @@
 
 class SDWritingUnopenedException(SDException):
     pass
 
 class SDClosingUnopenedException(SDException):
     pass
 
-class ScriptDereferencer(AbstractScriptDereferencer):
+class SDCantResolveAliasException(SDException):
+    pass
+
+class ScriptDereferencer(CachedCellDereferencer, AbstractScriptManager):
     """
     """
 
     def __init__(self, memory = None, cache = None, require_open = True):
         super().__init__(memory, cache)
-        self.open_files = {}
+        self.open_files = set()
+        self.aliases = {}
+        self.reverse_aliases = {}
         self.default_book = None
         self.default_sheet = None
         self.default_cell = None
         self.local_book = None
         self.local_sheet = None
         self.require_open = require_open
 
-    def _parse(self, name):
-        path, book, sheet, cell, final = extract_address(name)
-        if cell is None:
-            return None, None, None, None, None
+    def _parse(self, _name, check_aliases = True):
+        if _name in self.aliases.keys() and check_aliases:
+            path, book, sheet, cell, final = self.aliases[_name]
         else:
-            book = book if book is not None else self.local_book
-            book = book if book is not None else self.default_book
-            sheet = sheet if sheet is not None else self.local_sheet
-            sheet = sheet if sheet is not None else self.default_sheet
-            cell = cell if cell is not None else self.default_cell
-            return path, book, sheet, cell, final
+            path, book, sheet, cell, final = extract_address(_name)
+            if cell is None:
+                path, book, sheet, cell, final = None, None, None, None, None
+            else:
+                book = book if book is not None else self.local_book
+                book = book if book is not None else self.default_book
+                sheet = sheet if sheet is not None else self.local_sheet
+                sheet = sheet if sheet is not None else self.default_sheet
+                cell = cell if cell is not None else self.default_cell
+        return path, book, sheet, cell, final
 
     def tick(self, visitor):
         new_cache = {}
         for book in self.memory.keys():
             new_cache[book] = {}
             for sheet in self.memory[book].keys():
                 new_cache[book][sheet] = {}
                 for cell in self.memory[book][sheet].keys():
                     if type(self.memory[book][sheet][cell]) is not EmptyValueNode:
                         self._set_local_defaults(book=book, sheet=sheet) # Each node is resolved with itself as local
                         new_cache[book][sheet][cell] = visitor.visit(self.memory[book][sheet][cell])
                     else:
                         if book in self.cache.keys() and sheet in self.cache[book].keys():
                             new_cache[book][sheet][cell] = self.cache[book][sheet].get(cell, EmptyValueNode())
-        self._unset_local_defaults() # Remove the local
+
+        self._unset_local_defaults()  # Remove the local
         keys = list(self.cache.keys())
         for k in keys:
             del self.cache[k]
         for k in new_cache.keys():
             self.cache[k] = new_cache[k]
 
     def parse_key(self, key, require_open):
         _, book, sheet, cell, _ = self._parse(key)
-        if require_open and book not in self.open_files.keys():
+        if require_open and book not in self.open_files:
             raise SDWritingUnopenedException(book)
         return book, sheet, cell
 
     def write_formula(self, key, value):
         book, sheet, cell = self.parse_key(key, require_open=self.require_open)
         self.write_cell(book, sheet, cell, value, None)
         self._unset_local_defaults()
@@ -102,28 +112,42 @@
         self.local_sheet = sheet
 
     def _unset_local_defaults(self):
         self.local_book = None
         self.local_sheet = None
 
     def open_file(self, _filename):
-        if _filename not in self.open_files.keys():
-            self.open_files[_filename] = 0
+        if _filename not in self.open_files:
+            self.open_files.add(_filename)
             if _filename not in self.memory.keys():
                 self.memory[_filename] = {}
             if _filename not in self.cache.keys():
                 self.cache[_filename] = {}
         else:
             raise SDOpenFileException(_filename)
 
     def close_file(self, _filename):
-        if _filename in self.open_files.keys():
-            del self.open_files[_filename]
+        if _filename in self.open_files:
+            self.open_files.remove(_filename)
         else:
             raise SDClosingUnopenedException(_filename)
 
+    def make_alias(self, alias, cell):
+        parsed_cell = self._parse(cell, check_aliases = False)
+
+        if None in parsed_cell[1:4]:  # Doesn't have a book, a sheet or a initial cell
+            pb, ps, pc = parsed_cell[1:4]
+            raise SDCantResolveAliasException(f"Either book ({pb}), sheet ({ps}) or cell ({pc}) are not defined")
+
+        if parsed_cell in self.reverse_aliases.keys():
+            previous_cell_alias = self.reverse_aliases[parsed_cell]
+            del self.aliases[previous_cell_alias]
+            del self.reverse_aliases[parsed_cell]
+
+        self.aliases[alias] = parsed_cell
+        self.reverse_aliases[parsed_cell] = alias
 
 if __name__ == "__main__":
     #c = CachedCellDereferencer()
     pass
     #c.write("A1", StrValueNode("12"), StrValueNode("12"))
     #print(c.cache)
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py` & `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,30 @@
 
     def accept(self, visitor):
         return visitor.visitAssign(self)
 
     def volatile(self):
         return False
 
+class AliasNode(Node):
+    def __init__(self, alias, cell):
+        super().__init__()
+        self.target = alias
+        self.source = cell
+
+    def accept(self, visitor):
+        return visitor.visitAlias(self)
+
+    def volatile(self):
+        return False
+
 class SetDefaultsNode(Node):
     def __init__(self, cell):
         super().__init__()
-        self.children = {0: cell}
+        self.reference = cell
 
     def accept(self, visitor):
         return visitor.visitSetDefaults(self)
 
     def volatile(self):
         return False
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py` & `JestingLang-0.0.0a8/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,77 @@
 from JestingLang.Core.JVisitors.ContextfreeInterpreterVisitor import renodify
 from JestingLang.Core.JVisitors.ContextBoundInterpreterVisitor import ContextBoundInterpreterVisitor
 from JestingLang.Misc.JLogic.LogicFunctions import label_data
 from JestingLang.Core.JParsing.JestingAST import EmptyValueNode
 from JestingLang.JestingScript.JParsing.JestingScriptAST import RawInputNode
-from JestingLang.JestingScript.JDereferencer.AbstractScriptDereferencer import AbstractScriptDereferencer
+from JestingLang.JestingScript.JScriptManager.AbstractScriptManager import AbstractScriptManager
+from JestingLang.Core.JDereferencer.AbstractDereferencer import AbstractDereferencer
 from sys import stdout
 
 class ScriptInterpreterVisitor(ContextBoundInterpreterVisitor):
 
-    def __init__(self, dereferencer: AbstractScriptDereferencer, resolveVolatile, insertionUpdate= True, output = None):
-
-        try:
-            for required_call in ['tick', 'write_formula', 'write_value', 'read', 'read_all',
-                              'set_default', 'open_file', 'close_file']:
-                assert(required_call in dir(dereferencer))
-
-        except AssertionError as e:
-            print("INVALID dereferencer FOR SCRIPT INTERPRETER")
-            raise e
+    def __init__(self,
+                 dereferencer: AbstractDereferencer,
+                 resolveVolatile,
+                 scriptManager: AbstractScriptManager = None,
+                 insertionUpdate = True,
+                 output = None):
 
         super().__init__(dereferencer, resolveVolatile)
-        self.scriptManager = dereferencer
+        self.scriptManager = scriptManager if scriptManager is not None else dereferencer
         self.insertionUpdate = insertionUpdate
         self.default_book = None
         self.default_sheet = None
         self.default_cell = None
         self.output = output if output is not None else stdout
 
     def visitScript(self, node):
         for n, sub_node in node.children.items():
             self.visit(sub_node)
 
     def visitTick(self, node):
         for _ in range(node.ticks):
             self.scriptManager.tick(self)
 
+    def visitAlias(self, node):
+        self.scriptManager.make_alias(node.target, node.source)
+
     def visitRawInput(self, node):
         data = node.value
         label = label_data(data)
         return renodify(data, label)
 
     def visitAssign(self, node):
         cell = node.target
         self.scriptManager.set_local_defaults(cell)
-        #cell = node.children[0].accept(self)
         if type(node.children[0]) is RawInputNode:
             data = node.children[0].accept(self)
             self.scriptManager.write_formula(cell, EmptyValueNode())
             self.scriptManager.write_value(cell, data)
         else:
             child = node.children[0]
             self.scriptManager.write_formula(cell, child)
             if (not child.volatile()) or (self.resolveVolatile and self.insertionUpdate):
                 self.scriptManager.write_value(cell, child.accept(self))
             else:
                 self.scriptManager.write_value(cell, EmptyValueNode())
 
     def visitSetDefaults(self, node):
-        cell = node.children[0].accept(self)
+        cell = node.reference
         self.scriptManager.set_default(cell)
 
     def visitPrintValue(self, node):
         if node.print_all:
             self.output.write(self.scriptManager.read_all())
         else:
-                cell = node.children[0]
-                if node.print_value:
-                    self.output.write(str(self.scriptManager.read(cell, True)))
-                else:
-                    self.output.write(str(self.scriptManager.read(cell, False)))
+            cell = node.children[0]
+            if node.print_value:
+                self.output.write(str(self.scriptManager.read(cell, True)))
+            else:
+                self.output.write(str(self.scriptManager.read(cell, False)))
         self.output.write("\n")
 
     def visitOpenCloseFile(self, node):
         file_name = node.value
         if node.do_open:
             self.scriptManager.open_file(file_name)
         else:
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/LexerParser.py` & `JestingLang-0.0.0a8/src/JestingLang/LexerParser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 import ply.yacc as yacc
 import ply.lex as lex
 from JestingLang.Core.JParsing.JestingAST import *
 from JestingLang.JestingScript.JParsing.JestingScriptAST import *
-from JestingLang.Misc.JLogic.LogicFunctions import address_regex_str
+from JestingLang.JestingScript.JFileLoader.ExternalFileLoader import ExternalFileLoader
+from JestingLang.Misc.JLogic.LogicFunctions import address_regex_str, address
 
-def subtokenIsType(tokens, position, checkType):
-    return tokens.slice[position].type == checkType
+def getTokenType(tokens, position):
+    return tokens.slice[position].type
 
+def subtokenIsType(tokens, position, checkType):
+    return getTokenType(tokens, position) == checkType
 
 class LexerParser:
 
-    def __init__(self, *, multilineScript = False):
+    def __init__(self, *, multilineScript = False, useCellToken=False, external_file_loader = None):
 
         self.multilineScript = multilineScript
-        self.spreadsheet_function_set = ( 'MOD' , )
-        self.implemented_functions = ('IF', 'INDIRECT', 'NOT', 'AND', 'OR')
+        self.useCellToken = useCellToken
+        self.spreadsheet_function_set = {'MOD': 2}  # second value is amount of operands it receives
+        self.fixed_implementations = ('IF', 'INDIRECT',)
+        self.logic_functions = ('NOT', 'AND', 'OR',)
+        self.fixed_operations = ('PLUS', 'MINUS', 'TIMES',
+                                      'DIVIDE', 'EQUALS', 'BIGGER', 'AMPERSAND',)
+        self.indirect_fixed_operations = ('SMALLER',)
         self.tokens = (
                      'CELL_ADDRESS', 'NUMBER', 'BOOLEAN',
-                     'PLUS', 'MINUS', 'TIMES', 'DIVIDE', 'EQUALS', 'BIGGER', 'SMALLER',
-                     'LPAREN', 'RPAREN', 'AMPERSAND', 'STRING', 'COMMA'
-                 ) + self.implemented_functions + self.spreadsheet_function_set + ('TEXT',)
+                     'LPAREN', 'RPAREN', 'STRING', 'COMMA'
+                 ) + self.fixed_implementations + self.logic_functions \
+                      + self.indirect_fixed_operations + self.fixed_operations + ('TEXT',)
         if self.multilineScript:
-            self.tokens += ('ASSIGN_FORMULA', 'ASSIGN_VALUE', 'UNASSIGN', 'TICK',
-                            'SETDEFAULTS', 'PRINT', 'PRINTALL', 'NEWLINE', 'COMMENT','OPEN', 'CLOSE', )
+            self.tokens += ('ASSIGN_FORMULA', 'ASSIGN_VALUE', 'UNASSIGN', 'ASSIGN_ALIAS', 'TICK',
+                            'SETDEFAULTS', 'PRINT', 'NEWLINE', 'COMMENT',
+                            'OPEN', 'CLOSE', 'INCLUDE_EXTERNAL_FILE', )
+            self.external_file_loader = \
+                external_file_loader if external_file_loader is not None else ExternalFileLoader()
         self.setup_tokens()
         self.lexer = self.jesting_lexer()
         self.parser = self.jesting_parser()
         self.clearup_tokens()
 
     def setup_tokens(self):
         global tokens
@@ -51,36 +62,33 @@
             r'("[^"]*")|(\'[^\']*\')'
             t.value = t.value[1:-1]
             return t
 
         # ~~~ START OF MULTILINE
 
         if self.multilineScript:
+            t_INCLUDE_EXTERNAL_FILE = r'\#INCLUDE'
+            t_ASSIGN_ALIAS=r'\?'
             t_ASSIGN_FORMULA = r'@='
-            #t_ASSIGN_VALUE = r'@\s[^\n]+'
             def t_ASSIGN_VALUE(t):
                 r'@\s[^\n]+'
                 t.value = t.value[2:]
                 return t
             t_UNASSIGN = r'@'
             t_TICK = r'~+'
             t_SETDEFAULTS=r':'
-            t_PRINTALL=r'!!'
             t_PRINT=r'!'
-            #t_COMMENT=r'//[^\n]*'
             def t_COMMENT(t):
                 r'//[^\n]*'
                 t.value = t.value[2:]
                 return t
-            #t_OPEN=r'}[^\n]*'
             def t_OPEN(t):
                 r'}[^\n]*'
                 t.value = f"[{t.value[1:].strip()}]"
                 return t
-            #t_CLOSE=r'{[^\n]*'
             def t_CLOSE(t):
                 r'{[^\n]*'
                 t.value = f"[{t.value[1:].strip()}]"
                 return t
 
         # ~~~ END OF MULTILINE
 
@@ -91,38 +99,40 @@
         t_EQUALS = r'='
         t_BIGGER = r'>'
         t_SMALLER= r'<'
         t_LPAREN = r'\('
         t_RPAREN = r'\)'
         t_AMPERSAND = r'&'
         t_COMMA = r'\,'
-        t_MOD = r'MOD'
 
-        def t_CELL_ADDRESS(t):
-            return t
-
-        t_CELL_ADDRESS.__doc__ = address_regex_str  # This needs to be shared from another file
+        if self.useCellToken:
+            def t_CELL_ADDRESS(t):
+                return t
+            t_CELL_ADDRESS.__doc__ = address_regex_str  # This needs to be shared from another file
 
         def t_NUMBER(t):
             r'\d+'
             try:
                 t.value = int(t.value)
             except ValueError:
                 print("Integer value too large %d", t.value)
                 t.value = 0
             return t
 
         def t_TEXT(t):
-            r'[a-zA-Z_][a-zA-Z_0-9]*'
-            if t.value in self.implemented_functions:
+            r'[a-zA-Z_\.][a-zA-Z_0-9\.]*'
+            if t.value in self.logic_functions + self.fixed_implementations:
                 t.type = t.value
             if t.value in ('TRUE', 'FALSE'):
                 t.type = 'BOOLEAN'
             return t
 
+        if not self.useCellToken:
+            t_TEXT.__doc__ = r'[a-zA-Z_\.\[\]!][a-zA-Z_0-9\.\[\]!]*'
+
         def t_NEWLINE(t):
             r'\n[\n 	]*'
             t.lexer.lineno += t.value.count("\n")
             if self.multilineScript:
                 t.value = "\n"
             else:
                 t = None
@@ -151,139 +161,166 @@
 
         # ~~~ START OF MULTILINE
 
         if self.multilineScript:
 
             def p_start(t):
                 '''start : lines
+                        | lines NEWLINE
                         | NEWLINE lines
+                        | NEWLINE lines NEWLINE
                 '''
 
                 if len(t) == 2:
                     t[0] = t[1]
+                elif len(t) == 3 and subtokenIsType(t, 1, "NEWLINE"):
+                    t[0] = t[2]
                 elif len(t) == 3:
+                    t[0] = t[1]
+                else:
                     t[0] = t[2]
                 if t[0] is None:
                     raise Exception("Empty program")
                 return t[0]
 
             def p_lines(t):
                 '''lines : line
                          | lines NEWLINE line
                 '''
 
                 if len(t) == 2:
                     if t[1] is None:
                         t[0] = None
                     else:
-                        t[0] = ScriptNode(t[1])
+                        if type(t[1]) is ScriptNode:
+                            t[0] = t[1]
+                        else:
+                            t[0] = ScriptNode(t[1])
                 elif len(t) == 4:
                     if t[3] is None:
                         t[0] = t[1]
                     elif t[1] is None:
-                        t[0] = ScriptNode(t[3])
+                        if type(t[3]) is ScriptNode:
+                            t[0] = t[3]
+                        else:
+                            t[0] = ScriptNode(t[3])
                     else:
-                        t[0] = t[1].addChild(t[3])
+                        if type(t[3]) is ScriptNode:
+                            t[0] = t[1]
+                            for child in t[3].children:
+                                t[0] = t[0].addChild(t[3].children[child])
+                        else:
+                            t[0] = t[1].addChild(t[3])
                 return t[0]
 
             def p_line(t):
-                '''line :
-                        | COMMENT
+                '''line : COMMENT
                         | TICK
-                        | PRINTALL
-                        | PRINT CELL_ADDRESS
                         | OPEN
                         | CLOSE
+                        | PRINT PRINT
+                        | PRINT CELL_ADDRESS
                         | SETDEFAULTS CELL_ADDRESS
                         | CELL_ADDRESS UNASSIGN
                         | CELL_ADDRESS ASSIGN_VALUE
+                        | INCLUDE_EXTERNAL_FILE TEXT
                         | PRINT EQUALS CELL_ADDRESS
                         | CELL_ADDRESS ASSIGN_FORMULA statement
+                        | TEXT ASSIGN_ALIAS CELL_ADDRESS
                 '''
 
                 if len(t) == 2:
 
-                    if subtokenIsType(t,1,"PRINTALL"):
-                    #if t[1] == "!!":
-                        t[0] = PrintValueNode(print_all=True)
-                    elif subtokenIsType(t, 1, "TICK"):
-                    #elif t[1] == "~":
+                    if subtokenIsType(t, 1, "TICK"):
                         t[0] = TickNode(len(t[1]))
                     elif subtokenIsType(t, 1, "OPEN"):
-                    #elif t[1][0] == "}":
                         t[0] = OpenCloseFileNode(t[1], do_open=True)
                     elif subtokenIsType(t, 1, "CLOSE"):
-                    #elif t[1][0] == "{":
                         t[0] = OpenCloseFileNode(t[1], do_open=False)
                     else:
                         t[0] = None
 
                 elif len(t) == 3:
                     if subtokenIsType(t,1,"SETDEFAULTS"):
-                    #if t[1] == ":":
                         t[0] = SetDefaultsNode(t[2])
                     elif subtokenIsType(t, 1, "PRINT"):
-                    #elif t[1] == "!":
-                        t[0] = PrintValueNode(cell=t[2], print_value=True)
+                        if subtokenIsType(t, 2, "PRINT"):
+                            t[0] = PrintValueNode(print_all=True)
+                        else:
+                            t[0] = PrintValueNode(cell=t[2], print_value=True)
                     elif subtokenIsType(t, 2, "UNASSIGN"):
-                    #elif t[2] == "@":
                         t[0] = AssignNode(t[1], EmptyValueNode())
-                    else:
+                    elif subtokenIsType(t, 2, "ASSIGN_VALUE"):
                         t[0] = AssignNode(t[1], RawInputNode(t[2]))
+                    elif subtokenIsType(t, 1, "INCLUDE_EXTERNAL_FILE"):
+                        tmp_lexer = self.lexer.clone()  # Due to how ply work, we need a different lexer
+                        external_code = self.external_file_loader.load(t[2])
+                        t[0] = self.parser.parse(external_code, lexer=tmp_lexer)
+                        self.external_file_loader.unload(t[2])
+                    else:
+                        t[0] = None
 
                 elif len(t) == 4:
-                    if subtokenIsType(t,2,"EQUALS"):
+                    if subtokenIsType(t,2,"ASSIGN_ALIAS"):
+                        if not self.useCellToken:
+                            assert(address.match(t[1]) is None)
+                            assert(address.match(t[3]) is not None)
+                        t[0] = AliasNode(alias=t[1], cell=t[3])
+                    elif subtokenIsType(t, 1, "PRINT"):
                         t[0] = PrintValueNode(cell=t[3], print_value=False)
                     else:
                         t[0] = AssignNode(t[1], t[3])
 
                 return t[0]
 
+            if not self.useCellToken:
+                p_line.__doc__ = p_line.__doc__.replace("CELL_ADDRESS", "TEXT")
+
         # ~~~ END OF MULTILINE
 
         def p_statement(t):
             '''statement    : parameter
                             | callable_operation
                             | fixed_operation
             '''
             t[0] = t[1]
             return t[0]
 
+        def p_statement_list(t):
+            '''statement_list    : statement
+                            | statement COMMA statement_list
+            '''
+            t[0] = [t[1]]
+            if len(t) == 4:
+                t[0] += t[3]
+            return t[0]
+
         def p_callable_opereation(t):
             '''callable_operation   : IF LPAREN statement COMMA  statement COMMA statement RPAREN
                                     | NOT LPAREN statement RPAREN
                                     | AND LPAREN statement COMMA statement RPAREN
                                     | OR LPAREN statement COMMA statement RPAREN
                                     | INDIRECT LPAREN statement RPAREN
-                                    | TEXT LPAREN statement RPAREN
-                                    | TEXT LPAREN statement COMMA statement RPAREN
-                                    | TEXT LPAREN statement COMMA statement COMMA statement RPAREN '''
+                                    | TEXT LPAREN statement_list RPAREN'''
             if subtokenIsType(t, 1, "NOT"):
-            #if t[1] == 'NOT':
                 t[0] = OperationNode(t[1], {0: t[3]})
             if subtokenIsType(t, 1, "AND") or subtokenIsType(t, 1, "OR"):
-            #if t[1] in ('AND', 'OR'):
                 t[0] = OperationNode(t[1], {0: t[3], 1: t[5]})
             if subtokenIsType(t, 1, "IF"):
-            #if t[1] == 'IF':
                 t[0] = IfNode(t[3], t[5], t[7])
             if subtokenIsType(t, 1, "INDIRECT"):
-            #if t[1] == 'INDIRECT':
                 t[0] = IndirectNode(t[3])
             if subtokenIsType(t, 1, "TEXT"):
-                if t[1] not in self.spreadsheet_function_set:
+                if t[1] not in self.spreadsheet_function_set.keys():
                     raise Exception("unknown text")
-                if len(t) == 5:
-                    t[0] = OperationNode(t[1], {0: t[3]})
-                elif len(t) == 7:
-                    t[0] = OperationNode(t[1], {0: t[3], 1: t[5]})
-                elif len(t) == 9:
-                    t[0] = OperationNode(t[1], {0: t[3], 1: t[5], 2: t[7]})
                 else:
-                    raise Exception("unknown call")
+                    operands = self.spreadsheet_function_set[t[1]]
+                    children = {k: v for k, v in enumerate(t[3])}
+                    assert(len(children) == operands)
+                    t[0] = OperationNode(t[1], children)
             return t[0]
 
 
         def p_statement_paren(t):
             '''statement    :  LPAREN statement RPAREN '''
             t[0] = t[2]
             return t[0]
@@ -298,71 +335,82 @@
                                 | statement DIVIDE statement
                                 | statement SMALLER BIGGER statement
                                 | statement BIGGER statement
                                 | statement SMALLER statement
                                 | statement BIGGER EQUALS statement
                                 | statement SMALLER EQUALS statement
                                 | MINUS statement %prec UMINUS '''
-            if t[1] == "-":
-                t[0] = OperationNode("u-", {0: t[2]})
-            elif t[2] in ['<', '>']:
-                if t[2] == '<' and t[3] == '>':
-                    equals = OperationNode('=', {0: t[1], 1: t[4]})
+            if subtokenIsType(t, 1, "MINUS"):
+            #if t[1] == "-":
+                #t[0] = OperationNode("u-", {0: t[2]})
+                t[0] = OperationNode("NEGATE", {0: t[2]})
+            #elif t[2] in ['<', '>']:
+            elif subtokenIsType(t, 2, "SMALLER") or subtokenIsType(t, 2, "BIGGER"):
+                #if t[2] == '<' and t[3] == '>':
+                if subtokenIsType(t, 2, "SMALLER") and subtokenIsType(t, 3, "BIGGER"):
+                    equals = OperationNode('EQUALS', {0: t[1], 1: t[4]})
+                    #equals = OperationNode('=', {0: t[1], 1: t[4]})
                     t[0] = OperationNode('NOT', {0: equals})
                 else:
-                    second = t[4] if t[3] == '=' else t[3]
-                    if t[2] == '>':
+                    second = t[4] if subtokenIsType(t, 3, "EQUALS") else t[3]
+                    #second = t[4] if t[3] == '=' else t[3]
+                    #if t[2] == '>':
+                    if subtokenIsType(t, 2, "BIGGER"):
                         bg, sm = (t[1], second)
                     else:
                         bg, sm = (second, t[1])  # IN CASE ITS SMALLER JUST REVERSE THE ORDER
-                    bigger = OperationNode('>', {0: bg, 1: sm})
-                    if t[3] == '=':
-                        equals = OperationNode('=', {0: bg, 1: sm})
+                    bigger = OperationNode('BIGGER', {0: bg, 1: sm})
+                    #bigger = OperationNode('>', {0: bg, 1: sm})
+                    #if t[3] == '=':
+                    if subtokenIsType(t, 3, "EQUALS"):
+                        equals = OperationNode('EQUALS', {0: bg, 1: sm})
+                        #equals = OperationNode('=', {0: bg, 1: sm})
                         t[0] = OperationNode('OR', {0: equals, 1: bigger})
                     else:
                         t[0] = bigger
             else:
-                t[0] = OperationNode(t[2], {0: t[1], 1: t[3]})
+                t[0] = OperationNode(getTokenType(t,2) , {0: t[1], 1: t[3]})
+                #t[0] = OperationNode(t[2], {0: t[1], 1: t[3]})
             return t[0]
 
 
         def p_parameter_int(t):
             '''parameter    : NUMBER'''
             t[0] = IntValueNode(t[1])
             return t[0]
 
 
         def p_parameter_STR(t):
             '''parameter    : STRING'''
             t[0] = StrValueNode(t[1])
             return t[0]
 
-
-        def p_parameter_ADDRESS(t):
-            '''parameter    : CELL_ADDRESS'''
-            t[0] = ReferenceValueNode(t[1])
-            return t[0]
-
-
         def p_parameter_BOOL(t):
             '''parameter    : BOOLEAN'''
             t[0] = BoolValueNode(t[1])
             return t[0]
 
+        def p_parameter_ADDRESS_OR_TEXT(t):
+            '''parameter    : address'''
+            t[0] = t[1]
+            return t[0]
 
-        def p_text_parameter_text(t):
-            '''statement     : TEXT'''
-            text = t[1]
-            text = text.upper()
-            text = text.replace(".", "_")
-            text = text if text != "error" else "_error"
-            if text in self.spreadsheet_function_set:
-                raise Exception(f"FUNCTION '{t[1]}' NOT IMPLEMENTED")
-            else:
+        def p_parameter_ADDRESS(t):
+            '''address    : CELL_ADDRESS'''
+            t[0] = ReferenceValueNode(t[1])
+            return t[0]
+
+        def p_parameter_TEXT(t):
+            '''address  : TEXT'''
+            if self.useCellToken:
                 raise Exception(f"'{t[1]}' is Unknown")
+            else:
+                t[0] = ReferenceValueNode(t[1])
+            return t[0]
 
 
         def p_error(t):
             print("Syntax error at '%s'" % t.value)
 
         parser = yacc.yacc(tabmodule="LexerParser_cachedParseTable", debug=False)
+
         return parser
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/LogicFunctions.py` & `JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/LogicFunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import re
 
-address_regex_str =  r'(?P<path>(?P<workbook>\[[a-zA-Z0-9\.\(\)]+\])?(?P<worksheet>[a-zA-Z][a-zA-Z0-9]*!))?\$?(?P<initial>([a-z]+|[A-Z]+)\$?[0-9]+)(?P<final>:\$?[a-zA-Z]+\$?[0-9]+)?'
+b_rgx = r'\[[a-zA-Z0-9\.\(\)]+\]'  # book
+s_rgx = r'[a-zA-Z][a-zA-Z0-9]*!'  # sheet
+c_rgx = r'\$?([a-z][a-z]?[a-z]?|[A-Z][A-Z]?[A-Z]?)\$?[1-9][0-9]?[0-9]?[0-9]?[0-9]?[0-9]?[0-9]?'  # cell
+# Regex with excel limits'
+c_rgx_xl = r'\$?([x-zX-Z][a-zA-Z]?|[a-wA-W][a-zA-Z]?[a-zA-Z]?|[xX]([a-eA-E][a-zA-Z]|[fF][a-dA-D]))\$?[0-9][0-9]?[0-9]?[0-9]?[0-9]?[0-9]?[0-9]?'  # cell
+address_regex_str = fr'(?P<path>(?P<workbook>{b_rgx})?(?P<worksheet>{s_rgx}))?(?P<initial>{c_rgx})(?P<final>:{c_rgx})?'
 
-digit = re.compile(r' *-?\d+ *')
 address = re.compile(address_regex_str)
+digit = re.compile(r' *-?\d+ *')
 boolean_true = re.compile(r'TRUE|true')
 boolean_false = re.compile(r'FALSE|false')
 #numeric = re.compile(r'[0-9]+')
 
 def extract_address(t):
     match = address.match(t)
     if match is None:
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/OperationMapping.py` & `JestingLang-0.0.0a8/src/JestingLang/Misc/JLogic/OperationMapping.py`

 * *Files 20% similar despite different names*

```diff
@@ -66,23 +66,40 @@
         answer = variables_int[0] > variables_int[1]
     return errors, answer, "BOOL"
 
 
 def operationNot(variables):
     return [], not(variables[0]), "BOOL"
 
+# operations = {
+#                 "+": operationPlus,
+#                 "-": operationMinus,
+#                 "u-": operationMinus,
+#                 "*": operationTimes,
+#                 "/": operationDivide,
+#                 "&": operationConcat,
+#                 "=": operationEquals,
+#                 '>': operationBigger,
+#                 'NOT': operationNot,
+#                 'AND': operationAnd,
+#                 'OR': operationOr,
+#                 'MOD': operationModulo,
+# }
+
 operations = {
-                "+": operationPlus,
-                "-": operationMinus,
-                "u-": operationMinus,
-                "*": operationTimes,
-                "/": operationDivide,
-                "&": operationConcat,
-                "=": operationEquals,
-                '>': operationBigger,
+                "PLUS": operationPlus,
+                "MINUS": operationMinus,
+                "NEGATE": operationMinus,
+                "TIMES": operationTimes,
+                "DIVIDE": operationDivide,
+                "AMPERSAND": operationConcat,
+                "EQUALS": operationEquals,
+                'BIGGER': operationBigger,
                 'NOT': operationNot,
                 'AND': operationAnd,
                 'OR': operationOr,
                 'MOD': operationModulo,
 }
 
+('PLUS', 'MINUS', 'TIMES','DIVIDE', 'EQUALS', 'BIGGER', 'AMPERSAND',)
+
 assert(astOperations == set(operations.keys()))
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/DereferencerHelper.py` & `JestingLang-0.0.0a8/src/JestingLang/Misc/JTesting/DereferencerHelper.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang/main.py` & `JestingLang-0.0.0a8/src/JestingLang/main.py`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a7/src/JestingLang.egg-info/PKG-INFO` & `JestingLang-0.0.0a8/src/JestingLang.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a7/src/JestingLang.egg-info/SOURCES.txt` & `JestingLang-0.0.0a8/src/JestingLang.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 src/JestingLang/Core/JParsing/__init__.py
 src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
 src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
 src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
 src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
 src/JestingLang/Core/JVisitors/__init__.py
 src/JestingLang/JestingScript/__init__.py
-src/JestingLang/JestingScript/JDereferencer/AbstractScriptDereferencer.py
 src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
 src/JestingLang/JestingScript/JDereferencer/__init__.py
 src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
 src/JestingLang/JestingScript/JParsing/__init__.py
 src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
 src/JestingLang/JestingScript/JVisitors/__init__.py
 src/JestingLang/Misc/__init__.py
 src/JestingLang/Misc/JLogic/LogicFunctions.py
 src/JestingLang/Misc/JLogic/OperationMapping.py
 src/JestingLang/Misc/JLogic/__init__.py
 src/JestingLang/Misc/JTesting/DereferencerHelper.py
 src/JestingLang/Misc/JTesting/LexerParserHelpers.py
+src/JestingLang/Misc/JTesting/NonFileExternalFileLoader.py
 src/JestingLang/Misc/JTesting/__init__.py
```

