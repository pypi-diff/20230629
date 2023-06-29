# Comparing `tmp/chrislab-0.5.3.tar.gz` & `tmp/chrislab-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.3.tar", last modified: Fri May 19 20:53:27 2023, max compression
+gzip compressed data, was "chrislab-0.5.4.tar", last modified: Thu Jun 29 14:12:47 2023, max compression
```

## Comparing `chrislab-0.5.3.tar` & `chrislab-0.5.4.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-14 13:51:34.000000 chrislab-0.5.3/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-19 20:53:27.904633 chrislab-0.5.3/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-14 13:51:34.000000 chrislab-0.5.3/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-14 13:51:34.000000 chrislab-0.5.3/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-19 20:53:27.908633 chrislab-0.5.3/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.900633 chrislab-0.5.3/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.900633 chrislab-0.5.3/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-05-16 05:20:42.000000 chrislab-0.5.3/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13273 2023-05-19 19:44:22.000000 chrislab-0.5.3/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1420 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-19 20:53:27.000000 chrislab-0.5.3/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-05-18 12:07:19.000000 chrislab-0.5.3/src/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8521 2023-05-19 20:24:27.000000 chrislab-0.5.3/src/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/cls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/cls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-05-18 17:57:18.000000 chrislab-0.5.3/src/nlpbook/cls/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5209 2023-05-19 20:51:20.000000 chrislab-0.5.3/src/nlpbook/cls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2674 2023-05-18 17:12:36.000000 chrislab-0.5.3/src/nlpbook/cls/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/data_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3438 2023-05-18 17:45:48.000000 chrislab-0.5.3/src/nlpbook/factory.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-18 08:22:09.000000 chrislab-0.5.3/src/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8942 2023-05-19 20:51:19.000000 chrislab-0.5.3/src/nlpbook/ner/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12626 2023-05-19 20:51:20.000000 chrislab-0.5.3/src/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8534 2023-05-18 18:36:43.000000 chrislab-0.5.3/src/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-18 08:22:04.000000 chrislab-0.5.3/src/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-19 20:53:27.904633 chrislab-0.5.3/src/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-18 08:22:15.000000 chrislab-0.5.3/src/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:51:34.000000 chrislab-0.5.3/src/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8635 2023-05-18 15:44:30.000000 chrislab-0.5.3/src/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-06-29 13:39:49.000000 chrislab-0.5.4/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-06-29 14:12:47.292331 chrislab-0.5.4/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-06-29 13:39:49.000000 chrislab-0.5.4/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-06-29 13:39:49.000000 chrislab-0.5.4/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1129 2023-06-29 14:12:47.296331 chrislab-0.5.4/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11372 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1518 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      132 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      211 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10124 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5209 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2673 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/data_utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/dp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12333 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    19194 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11306 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/model.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3179 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/factory.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5372 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1292 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9886 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18392 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13580 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9960 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2657 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17105 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2071 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10847 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.3/LICENSE` & `chrislab-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/PKG-INFO` & `chrislab-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.3
+Version: 0.5.4
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.3/setup.cfg` & `chrislab-0.5.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.3
+version = 0.5.4
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -19,17 +19,16 @@
 zip_safe = True
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	chrisbase
-	torch>=1.7, <2.0
-	lightning>=1.7, <2.0
-	pytorch-lightning>=1.7, <2.0
+	torch>=1.7
+	lightning>=1.7
 	evaluate
 	datasets
 	tokenizers
 	transformers
 	Flask
 	Flask-Cors
 	Korpora
@@ -48,14 +47,14 @@
 
 [options.package_data]
 * = README.md
 
 [options.entry_points]
 console_scripts = 
 	chrislab.language = chrislab.language.cli:app
-	ratsnlp.nlpbook.cls = ratsnlp.nlpbook.cls.cli:app
-	ratsnlp.nlpbook.ner = ratsnlp.nlpbook.ner.cli:app
+	nlpbook.cls = nlpbook.cls.cli:app
+	nlpbook.ner = nlpbook.ner.cli:app
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `chrislab-0.5.3/src/chrislab/common/downloader.py` & `chrislab-0.5.4/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.4/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/common/util.py` & `chrislab-0.5.4/src/chrislab/common/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,35 +15,26 @@
 from tabulate import tabulate
 
 from chrisbase.io import load_attrs, merge_dicts
 from chrisbase.io import make_dir, files_info, dirs, exists_or, hr
 from chrisbase.io import prepend_to_global_path
 from chrisbase.io import running_file, run_command
 from chrisbase.time import now
-from chrisbase.util import number_only, NO, tupled, to_dataframe
-
-
-def cuda_visible_devices(gpus=None):
-    if gpus:
-        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
-        os.environ["CUDA_VISIBLE_DEVICES"] = gpus
-    return os.environ.get("CUDA_VISIBLE_DEVICES")
+from chrisbase.util import number_only, NO, to_dataframe
 
 
 def set_tokenizers_parallelism(value=False):
     os.environ["TOKENIZERS_PARALLELISM"] = f"{value}".lower()
 
 
-def num_cuda_devices():
-    from torch.cuda import _device_count_nvml
-    nvml_count = _device_count_nvml()
-    if nvml_count >= 0:
-        return nvml_count
-    else:
-        return torch.cuda.device_count()
+def cuda_visible_devices(devices=None):
+    if torch.cuda.is_available() and devices:
+        os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+        os.environ["CUDA_VISIBLE_DEVICES"] = devices
+    return os.environ.get("CUDA_VISIBLE_DEVICES")
 
 
 def include_cuda_bin_dir(candidate_dirs=None) -> Path:
     if candidate_dirs is None:
         candidate_dirs = sorted(dirs("/usr/local/cuda*"), reverse=True)
     cuda_dir = None
     for candidate_dir in candidate_dirs:
@@ -56,18 +47,14 @@
 
 
 def set_torch_ext_path(dev=1):
     torch_ext_dir = Path(f"cache/torch_extensions/dev={dev}")
     os.environ['TORCH_EXTENSIONS_DIR'] = f"{torch_ext_dir.absolute()}"
 
 
-def set_tokenizers_parallelism(value=False):
-    os.environ["TOKENIZERS_PARALLELISM"] = f"{value}".lower()
-
-
 def copy_ipynb_for_run(infile, run_opts=None):
     infile = Path(infile)
     outdir = infile.with_name(f"{infile.stem}-{now('%m.%d')}")
     run_command("rm", "-rf", outdir, bare=True)
     if run_opts:
         for dst in sorted([make_dir(outdir / f"{s}-{r}") for s, rs in run_opts.items() for r in rs]):
             run_command("cp", infile, dst, bare=True)
@@ -123,58 +110,14 @@
     elif len(_opt.rsplit('-')) >= 2:
         splits = _opt.rsplit('-', maxsplit=2)
         final['strategy'] = splits[-2] if splits[-2] in valid_strategies else default['strategy']
         final['run'] = int(number_only(splits[-1]))
     return final
 
 
-def set_devices_to_runs(runs, use_gpu, have_gpu=num_cuda_devices()):
-    gpus_for_use = {
-        1: {
-            0: [0],
-            1: [0],
-            2: [1],
-            3: [2],
-            4: [3],
-            5: [0] if have_gpu < 8 else [4],
-            6: [1] if have_gpu < 8 else [5],
-            7: [2] if have_gpu < 8 else [6],
-            8: [3] if have_gpu < 8 else [7],
-        },
-        2: {
-            0: [0, 1],
-            1: [0, 1],
-            2: [2, 3],
-            3: [0, 1] if have_gpu < 8 else [4, 5],
-            4: [2, 3] if have_gpu < 8 else [6, 7],
-            5: [0, 1],
-            6: [2, 3],
-            7: [0, 1] if have_gpu < 8 else [4, 5],
-            8: [2, 3] if have_gpu < 8 else [6, 7],
-        },
-        4: {
-            0: [0, 1, 2, 3],
-            1: [0, 1, 2, 3],
-            2: [0, 1, 2, 3] if have_gpu < 8 else [4, 5, 6, 7],
-            3: [0, 1, 2, 3],
-            4: [0, 1, 2, 3] if have_gpu < 8 else [4, 5, 6, 7],
-            5: [0, 1, 2, 3],
-            6: [0, 1, 2, 3] if have_gpu < 8 else [4, 5, 6, 7],
-            7: [0, 1, 2, 3],
-            8: [0, 1, 2, 3] if have_gpu < 8 else [4, 5, 6, 7],
-        },
-    }
-    assert use_gpu in gpus_for_use, f"Not defined {use_gpu} in gpus_for_use: defined for {list(gpus_for_use.keys())}"
-    for r in runs:
-        assert r in gpus_for_use[use_gpu], f"Not defined {r} in gpus_for_use[{use_gpu}]: defined for {list(gpus_for_use[use_gpu].keys())}"
-        for x in tupled(runs[r]):
-            x['devices'] = gpus_for_use[use_gpu][r] if use_gpu in gpus_for_use and r in gpus_for_use[use_gpu] else None
-    return runs
-
-
 class EmptyTqdm:
     """Dummy tqdm which doesn't do anything."""
 
     def __init__(self, *args, **kwargs):
         self._iterator = args[0] if args else None
 
     def __iter__(self):
```

### Comparing `chrislab-0.5.3/src/chrislab/language/cli.py` & `chrislab-0.5.4/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/language/converter.py` & `chrislab-0.5.4/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/language/evaluater.py` & `chrislab-0.5.4/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/language/finetuner.py` & `chrislab-0.5.4/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/language/modeling.py` & `chrislab-0.5.4/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab/language/predictor.py` & `chrislab-0.5.4/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.4/src/chrislab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.3
+Version: 0.5.4
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.3/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.4/src/chrislab.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 src/nlpbook/factory.py
 src/nlpbook/metrics.py
 src/nlpbook/utils.py
 src/nlpbook/cls/__init__.py
 src/nlpbook/cls/cli.py
 src/nlpbook/cls/corpus.py
 src/nlpbook/cls/task.py
+src/nlpbook/dp/__init__.py
+src/nlpbook/dp/cli.py
+src/nlpbook/dp/corpus.py
+src/nlpbook/dp/model.py
 src/nlpbook/generation/__init__.py
 src/nlpbook/generation/arguments.py
 src/nlpbook/generation/corpus.py
 src/nlpbook/generation/deploy.py
 src/nlpbook/generation/task.py
 src/nlpbook/ner/__init__.py
 src/nlpbook/ner/cli.py
```

### Comparing `chrislab-0.5.3/src/nlpbook/arguments.py` & `chrislab-0.5.4/src/nlpbook/arguments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import nlpbook
+import logging
+import math
 import os
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
-from typing import List
+from typing import List, Tuple
 
 import pandas as pd
 from dataclasses_json import DataClassJsonMixin
-from pytorch_lightning.accelerators import Accelerator
-from pytorch_lightning.loggers import CSVLogger
-from pytorch_lightning.strategies import Strategy
+from lightning.fabric.accelerators import Accelerator
+from lightning.fabric.strategies import Strategy
+from lightning.pytorch.loggers import CSVLogger
 
 from chrisbase.io import ProjectEnv, make_dir
 from chrisbase.io import files, make_parent_dir, out_hr, out_table
 from chrisbase.time import now, str_delta
 from chrisbase.util import to_dataframe
 
 
@@ -52,16 +55,17 @@
 
 
 @dataclass
 class DataOption(OptionData):
     name: str | Path = field()
     home: str | Path | None = field(default=None)
     files: DataFiles | None = field(default=None)
-    caching: bool = field(default=True)
+    caching: bool = field(default=False)
     redownload: bool = field(default=False)
+    show_examples: int = field(default=3)
 
     def __post_init__(self):
         if self.home:
             self.home = Path(self.home)
 
 
 @dataclass
@@ -73,49 +77,52 @@
 
     def __post_init__(self):
         self.finetuning_home = Path(self.finetuning_home)
 
 
 @dataclass
 class HardwareOption(OptionData):
+    # cpu_workers: int = field(default=0)
     cpu_workers: int = field(default=os.cpu_count())
     accelerator: str | Accelerator = field(default="auto")  # possbile value: "cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto"
     batch_size: int = field(default=32)
     precision: int | str = field(default=32)  # floating-point precision type
-    strategy: str | Strategy | None = field(default=None)  # multi-device strategies
-    devices: List[int] | int | str = field(default=1)  # devices to use
+    strategy: str | Strategy = field(default="auto")  # multi-device strategies
+    devices: List[int] | int | str = field(default="auto")  # devices to use
 
     def __post_init__(self):
         if not self.strategy:
             if self.devices == 1 or isinstance(self.devices, list) and len(self.devices) == 1:
                 self.strategy = "single_device"
             elif isinstance(self.devices, int) and self.devices > 1 or isinstance(self.devices, list) and len(self.devices) > 1:
                 self.strategy = "ddp"
 
 
 @dataclass
 class LearningOption(OptionData):
-    condition: str = field(default="min val_loss")  # monitor condition for num_save
-    log_steps: int = field(default=10)
-    num_save: int = field(default=100)
+    validating_fmt: str | None = field(default=None)
+    validating_on: int | float = field(default=1.0)
+    num_keeping: int = field(default=5)
+    keeping_by: str = field(default="min val_loss")
     epochs: int = field(default=1)
     speed: float = field(default=5e-5)
     seed: int | None = field(default=None)  # random seed
 
+    def __post_init__(self):
+        self.validating_on = math.fabs(self.validating_on)
+
 
 @dataclass
 class JobTimer(ResultData):
+    name: str = field()
     t1 = datetime.now()
     t2 = datetime.now()
-    started: str | None = field(init=False)
-    settled: str | None = field(init=False)
-    elapsed: str | None = field(init=False)
-
-    def __post_init__(self):
-        self.set_started()
+    started: str | None = field(default=None)
+    settled: str | None = field(default=None)
+    elapsed: str | None = field(default=None)
 
     def set_started(self):
         self.started = now()
         self.settled = None
         self.elapsed = None
         self.t1 = datetime.now()
         return self
@@ -128,51 +135,65 @@
 
 
 @dataclass
 class JobOutput(ResultData):
     dir_path: Path | None = field(init=False, default=None)
     csv_out: CSVLogger | None = field(init=False, default=None)
     result: dict = field(init=False, default_factory=dict)
+    global_step: int = field(init=False, default=0)
+    global_epoch: float = field(init=False, default=0.0)
+    epoch_per_step: float = field(init=False, default=0.0)
 
 
 @dataclass
 class CommonArguments(ArgumentGroupData):
     tag = "common"
+    job: JobTimer = field()
     env: ProjectEnv = field()
     data: DataOption | None = field(default=None)
     model: ModelOption | None = field(default=None)
-    timer: JobTimer = field(default=JobTimer())
     output: JobOutput = field(default=JobOutput())
 
     def __post_init__(self):
         super().__post_init__()
+        if not self.env.logging_file.stem.endswith(self.tag):
+            self.env.logging_file = self.env.logging_file.with_stem(f"{self.env.logging_file.stem}-{self.tag}")
         if not self.env.argument_file.stem.endswith(self.tag):
             self.env.argument_file = self.env.argument_file.with_stem(f"{self.env.argument_file.stem}-{self.tag}")
         if self.data and self.model:
             self.output.dir_path = self.model.finetuning_home / self.data.name
         if self.model and self.tag in ("train",):
             self.model.finetuning_home = make_dir(self.model.finetuning_home)
 
     def dataframe(self, columns=None):
         if not columns:
             columns = [self.data_type, "value"]
         return pd.concat([
+            to_dataframe(columns=columns, raw=self.job, data_prefix="job"),
             to_dataframe(columns=columns, raw=self.env, data_prefix="env"),
             to_dataframe(columns=columns, raw=self.data, data_prefix="data"),
             to_dataframe(columns=columns, raw=self.model, data_prefix="model"),
-            to_dataframe(columns=columns, raw=self.timer, data_prefix="timer"),
             to_dataframe(columns=columns, raw=self.output, data_prefix="output"),
         ]).reset_index(drop=True)
 
     def show(self):
         out_hr(c='-')
         out_table(self.dataframe())
         out_hr(c='-')
         return self
 
+    def setup_csv_out(self, version=None):
+        if not version:
+            version = now('%m%d.%H%M%S')
+        self.output.csv_out = CSVLogger(self.model.finetuning_home, name=self.data.name,
+                                        version=f'{self.tag}-{self.job.name}-{version}',
+                                        flush_logs_every_n_steps=1)
+        self.output.dir_path = Path(self.output.csv_out.log_dir)
+        return self
+
     def save(self, to: Path | str = None) -> Path | None:
         if not self.output.dir_path:
             return None
         args_file = to if to else self.output.dir_path / self.env.argument_file
         args_json = self.to_json(default=str, ensure_ascii=False, indent=2)
         make_parent_dir(args_file).write_text(args_json, encoding="utf-8")
         return args_file
@@ -221,29 +242,35 @@
         return pd.concat([
             super().dataframe(columns=columns),
             to_dataframe(columns=columns, raw=self.learning, data_prefix="training"),
         ]).reset_index(drop=True)
 
 
 class ArgumentsUsing:
-    def __init__(self, args: CommonArguments):
+    def __init__(self, args: CommonArguments, logging_level: int = logging.INFO, delete_on_exit: bool = True):
         self.args: CommonArguments = args
+        self.logging_level = logging_level
+        self.delete_on_exit: bool = delete_on_exit
 
-    def __enter__(self) -> Path:
+    def __enter__(self) -> Tuple[Path, logging.Logger]:
         self.args_file: Path | None = self.args.save()
-        return self.args_file
+        self.logger: logging.Logger = nlpbook.new_logger_file(name=f"main.{self.args.env.running_file.stem}",
+                                                              filepath=self.args.output.dir_path / self.args.env.logging_file,
+                                                              filemode="w",
+                                                              level=self.logging_level, )
+        return self.args_file, self.logger
 
     def __exit__(self, *exc_info):
-        if self.args_file:
+        if self.delete_on_exit and self.args_file:
             self.args_file.unlink(missing_ok=True)
 
 
 class RuntimeChecking:
     def __init__(self, args: CommonArguments):
         self.args: CommonArguments = args
 
     def __enter__(self):
-        self.args.timer.set_started()
+        self.args.job.set_started()
 
     def __exit__(self, *exc_info):
-        self.args.timer.set_settled()
+        self.args.job.set_settled()
         self.args.save(self.args.output.dir_path / self.args.env.argument_file)
```

### Comparing `chrislab-0.5.3/src/nlpbook/cls/cli.py` & `chrislab-0.5.4/src/nlpbook/cls/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import logging
 from pathlib import Path
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
+import nlpbook
 import torch
 from Korpora import Korpora
-from flask import Flask
-from torch.utils.data import DataLoader, RandomSampler
-from torch.utils.data import SequentialSampler
-from typer import Typer
-
-import nlpbook
 from chrisbase.io import JobTimer, err_hr
+from flask import Flask
 from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
 from nlpbook.cls.corpus import NsmcCorpus, ClassificationDataset
 from nlpbook.cls.task import ClassificationTask
+from torch.utils.data import DataLoader, RandomSampler
+from torch.utils.data import SequentialSampler
 from transformers import BertConfig, BertForSequenceClassification, BertTokenizer
 from transformers.modeling_outputs import SequenceClassifierOutput
+from typer import Typer
 
 app = Typer()
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
 
 
 @app.command()
 def train(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
```

### Comparing `chrislab-0.5.3/src/nlpbook/cls/corpus.py` & `chrislab-0.5.4/src/nlpbook/cls/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
 from nlpbook.arguments import TrainerArguments, TesterArguments
 from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
 
 
 @dataclass
 class ClassificationExample:
     text_a: str
     text_b: Optional[str] = None
     label: Optional[str] = None
@@ -110,15 +110,15 @@
         assert args.data.home, f"No data_home: {args.data.home}"
         assert args.data.name, f"No data_name: {args.data.name}"
         data_file_dict: dict = args.data.files.to_dict()
         assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
         assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
         text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
         cache_data_path = text_data_path \
-            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-as-{args.model.max_seq_length}seq") \
+            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
             .with_suffix(".cache")
         cache_lock_path = cache_data_path.with_suffix(".lock")
 
         with FileLock(cache_lock_path):
             if os.path.exists(cache_data_path) and args.data.caching:
                 start = time.time()
                 self.features = torch.load(cache_data_path)
```

### Comparing `chrislab-0.5.3/src/nlpbook/cls/task.py` & `chrislab-0.5.4/src/nlpbook/cls/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import pytorch_lightning as pl
-from pytorch_lightning import LightningModule
-from torch.optim import AdamW
-from torch.optim.lr_scheduler import ExponentialLR
-
+import lightning.pytorch as pl
+from lightning.pytorch import LightningModule
 from nlpbook.arguments import TrainerArguments, TesterArguments
 from nlpbook.metrics import accuracy
+from torch.optim import AdamW
+from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel
 from transformers.modeling_outputs import SequenceClassifierOutput
 
 
 class ClassificationTask(LightningModule):
     def __init__(self, model: PreTrainedModel,
                  args: TrainerArguments | TesterArguments,
```

### Comparing `chrislab-0.5.3/src/nlpbook/data_utils.py` & `chrislab-0.5.4/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/factory.py` & `chrislab-0.5.4/src/nlpbook/factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from pathlib import Path
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 import torch
-from flask import Flask, request, jsonify, render_template
-from pytorch_lightning.callbacks import ModelCheckpoint
-from pytorch_lightning.loggers import CSVLogger
-
 from chrisbase.io import merge_dicts
 from chrisbase.time import now
-from nlpbook.arguments import TrainerArguments, TesterArguments, ServerArguments
+from flask import Flask, request, jsonify, render_template
+from lightning.pytorch.loggers import CSVLogger
+from lightning.pytorch.callbacks import ModelCheckpoint
+from nlpbook.arguments import TrainerArguments, TesterArguments, CommonArguments
 
 
-def setup_csv_out(args: ServerArguments, version=None) -> ServerArguments:
+def setup_csv_out(args: CommonArguments, version=None) -> CommonArguments:
     if not version:
-        version = now(f'{args.tag}-%m%d.%H%M')
+        version = now(f'{args.tag}-{args.job.name}-%m%d.%H%M')
     csv_out: CSVLogger = CSVLogger(args.model.finetuning_home, args.data.name, version)
     args.output.dir_path = Path(csv_out.log_dir)
     args.output.csv_out = csv_out
     return args
 
 
 class LoggingCallback(pl.Callback):
@@ -36,41 +35,42 @@
 
 
 def make_trainer(args: TrainerArguments) -> pl.Trainer:
     logging_callback = LoggingCallback()
     checkpoint_callback = ModelCheckpoint(
         dirpath=args.output.dir_path,
         filename=args.model.finetuning_name,
-        save_top_k=args.learning.num_save,
-        monitor=args.learning.condition.split()[1],
-        mode=args.learning.condition.split()[0],
+        save_top_k=args.learning.num_keeping,
+        monitor=args.learning.keeping_by.split()[1],
+        mode=args.learning.keeping_by.split()[0],
     )
     trainer = pl.Trainer(
         logger=args.output.csv_out,
-        devices=args.hardware.devices if not args.hardware.devices else None,
-        strategy=args.hardware.strategy if not args.hardware.strategy else None,
-        precision=args.hardware.precision if args.hardware.precision else 32,
-        accelerator=args.hardware.accelerator if args.hardware.accelerator else None,
+        devices=args.hardware.devices,
+        strategy=args.hardware.strategy,
+        precision=args.hardware.precision,
+        accelerator=args.hardware.accelerator,
         deterministic=torch.cuda.is_available() and args.learning.seed is not None,
+        # enable_progress_bar=False,
         num_sanity_val_steps=0,
-        val_check_interval=args.learning.log_steps,
-        log_every_n_steps=args.learning.log_steps,
+        val_check_interval=args.learning.validating_on,
         max_epochs=args.learning.epochs,
         callbacks=[logging_callback, checkpoint_callback],
     )
     return trainer
 
 
 def make_tester(args: TesterArguments) -> pl.Trainer:
     tester = pl.Trainer(
         logger=args.output.csv_out,
-        devices=args.hardware.devices if not args.hardware.devices else None,
-        strategy=args.hardware.strategy if not args.hardware.strategy else None,
-        precision=args.hardware.precision if args.hardware.precision else 32,
-        accelerator=args.hardware.accelerator if args.hardware.accelerator else None,
+        devices=args.hardware.devices,
+        strategy=args.hardware.strategy,
+        precision=args.hardware.precision,
+        accelerator=args.hardware.accelerator,
+        # enable_progress_bar=False,
     )
     return tester
 
 
 def make_server(inference_fn, template_file, ngrok_home=None):
     app = Flask(__name__, template_folder='')
     if ngrok_home:
```

### Comparing `chrislab-0.5.3/src/nlpbook/generation/arguments.py` & `chrislab-0.5.4/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/generation/corpus.py` & `chrislab-0.5.4/src/nlpbook/generation/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
 from nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedTokenizerFast
 
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
 
 
 @dataclass
 class GenerationExample:
     text: str
```

### Comparing `chrislab-0.5.3/src/nlpbook/generation/deploy.py` & `chrislab-0.5.4/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/generation/task.py` & `chrislab-0.5.4/src/nlpbook/generation/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from pytorch_lightning import LightningModule
+from lightning.pytorch import LightningModule
+from nlpbook.generation.arguments import GenerationTrainArguments
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
-
-from nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedModel
 
 
 class GenerationTask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
```

### Comparing `chrislab-0.5.3/src/nlpbook/ner/corpus.py` & `chrislab-0.5.4/src/nlpbook/ner/corpus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 import logging
-import os
 import re
-import time
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Optional, ClassVar
+from typing import List, Optional, ClassVar, Dict
 
 import torch
 from dataclasses_json import DataClassJsonMixin
-from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from chrisbase.io import make_parent_dir, files, merge_dicts
+from chrisbase.io import make_parent_dir, files, merge_dicts, out_hr
 from nlpbook.arguments import TesterArguments
-from transformers import PreTrainedTokenizerFast
-from transformers.tokenization_utils_base import CharSpan
-from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy, BatchEncoding
-
-logger = logging.getLogger("nlpbook")
-
-NER_CLS_TOKEN = "[CLS]"
-NER_SEP_TOKEN = "[SEP]"
-NER_PAD_TOKEN = "[PAD]"
-NER_MASK_TOKEN = "[MASK]"
-NER_PAD_ID = 2
+from transformers import PreTrainedTokenizerFast, BatchEncoding, CharSpan
+from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
+
+logger = logging.getLogger("chrislab")
 
 
 @dataclass
 class EntityInText(DataClassJsonMixin):
     pattern: ClassVar[re.Pattern] = re.compile('<([^<>]+?):([A-Z]{2,3})>')
     text: str
     label: str
@@ -38,187 +28,209 @@
         x = m.group(1)
         y = m.group(2)
         z = (m.start(), m.start() + len(x))
         e = EntityInText(text=x, label=y, offset=z)
         s = s[:m.start()] + m.group(1) + s[m.end():]
         return e, s
 
-    def to_offset_lable_dict(self) -> dict[int, str]:
+    def to_offset_lable_dict(self) -> Dict[int, str]:
         offset_list = [(self.offset[0], f"B-{self.label}")]
         for i in range(self.offset[0] + 1, self.offset[1]):
             offset_list.append((i, f"I-{self.label}"))
         return dict(offset_list)
 
 
 @dataclass
-class NERExampleForKLUE(DataClassJsonMixin):
+class NERRawExample(DataClassJsonMixin):
     origin: str = field(default_factory=str)
-    entity_list: list[EntityInText] = field(default_factory=list)
-    character_list: list[tuple[str, str]] = field(default_factory=list)
+    entity_list: List[EntityInText] = field(default_factory=list)
+    character_list: List[tuple[str, str]] = field(default_factory=list)
+
+    def get_offset_label_dict(self):
+        return {i: y for i, (_, y) in enumerate(self.character_list)}
 
 
 @dataclass
-class NERFeatures:
-    input_ids: List[int]
-    attention_mask: Optional[List[int]] = None
-    token_type_ids: Optional[List[int]] = None
+class NEREncodedExample:
+    idx: int
+    raw: NERRawExample
+    encoded: BatchEncoding
     label_ids: Optional[List[int]] = None
 
 
+def ner_encoded_examples_to_batch(examples: List[NEREncodedExample]) -> Dict[str, torch.Tensor]:
+    first = examples[0]
+    batch = {}
+    for k, v in first.encoded.items():
+        if k not in ("label", "label_ids") and v is not None and not isinstance(v, str):
+            if isinstance(v, torch.Tensor):
+                batch[k] = torch.stack([ex.encoded[k] for ex in examples])
+            else:
+                batch[k] = torch.tensor([ex.encoded[k] for ex in examples], dtype=torch.long)
+    batch["labels"] = torch.tensor([ex.label_ids for ex in examples],
+                                   dtype=torch.long if type(first.label_ids[0]) is int else torch.float)
+    batch["example_ids"] = torch.tensor([ex.idx for ex in examples], dtype=torch.int)
+    return batch
+
+
 class NERCorpus:
     def __init__(self, args: TesterArguments):
         self.args = args
 
-    def get_examples(self, data_path: Path) -> List[NERExampleForKLUE]:
+    def read_raw_examples(self, data_path: Path) -> List[NERRawExample]:
         examples = []
         with data_path.open(encoding="utf-8") as inp:
             for line in inp.readlines():
-                examples.append(NERExampleForKLUE.from_json(line))
-        logger.info(f"Loaded {len(examples)} {examples[0].__class__.__name__} from {data_path}")
+                examples.append(NERRawExample.from_json(line))
+        logger.info(f"Loaded {len(examples)} examples from {data_path}")
         return examples
 
-    def get_labels(self):
+    def get_labels(self) -> List[str]:
         label_map_path = make_parent_dir(self.args.output.dir_path / "label_map.txt")
         if not label_map_path.exists():
             ner_tags = []
-            train_data_path: Path = self.args.data.home / self.args.data.name / self.args.data.files.train
+            train_data_path = self.args.data.home / self.args.data.name / self.args.data.files.train
+            logger.info(f"Extracting labels from {train_data_path}")
             with train_data_path.open(encoding="utf-8") as inp:
                 for line in inp.readlines():
-                    for x in NERExampleForKLUE.from_json(line).entity_list:
+                    for x in NERRawExample.from_json(line).entity_list:
                         if x.label not in ner_tags:
                             ner_tags.append(x.label)
             b_tags = [f"B-{ner_tag}" for ner_tag in ner_tags]
             i_tags = [f"I-{ner_tag}" for ner_tag in ner_tags]
-            labels = [NER_CLS_TOKEN, NER_SEP_TOKEN, NER_PAD_TOKEN, NER_MASK_TOKEN, "O"] + b_tags + i_tags
+            labels = ["O"] + b_tags + i_tags
+            logger.info(f"Saved {len(labels)} labels to {label_map_path}")
             with label_map_path.open("w", encoding="utf-8") as f:
                 f.writelines([x + "\n" for x in labels])
         else:
-            labels = [label.strip() for label in label_map_path.open(encoding="utf-8").readlines()]
-        logger.info(f"Loaded {len(labels)} labels from {label_map_path}")
+            labels = label_map_path.read_text(encoding="utf-8").splitlines()
         return labels
 
     @property
     def num_labels(self):
         return len(self.get_labels())
 
 
-def _decide_span_label(span: CharSpan, offset_to_label: dict[int, str]):
+def _decide_span_label(span: CharSpan, offset_to_label: Dict[int, str]):
     for x in [offset_to_label[i] for i in range(span.start, span.end)]:
         if x.startswith("B-") or x.startswith("I-"):
             return x
     return "O"
 
 
-def _convert_examples_to_ner_features(
-        examples: List[NERExampleForKLUE],
+def _convert_to_encoded_examples(
+        raw_examples: List[NERRawExample],
         tokenizer: PreTrainedTokenizerFast,
         args: TesterArguments,
         label_list: List[str],
-        cls_token_at_end: Optional[bool] = False,
-        num_show_example: int = 3,
-):
-    """
-    `cls_token_at_end` define the location of the CLS token:
-            - False (Default, BERT/XLM pattern): [CLS] + A + [SEP] + B + [SEP]
-            - True (XLNet/GPT pattern): A + [SEP] + B + [SEP] + [CLS]
-    """
-    label_to_id = {label: i for i, label in enumerate(label_list)}
-    id_to_label = {i: label for i, label in enumerate(label_list)}
-
-    features: list[NERFeatures] = []
-    for example in examples:
-        example: NERExampleForKLUE = example
-        offset_to_label: dict[int, str] = {i: y for i, (_, y) in enumerate(example.character_list)}
-        inputs: BatchEncoding = tokenizer.encode_plus(example.origin,
-                                                      max_length=args.model.max_seq_length,
-                                                      truncation=TruncationStrategy.LONGEST_FIRST,
-                                                      padding=PaddingStrategy.MAX_LENGTH)
-        input_tokens: List[str] = inputs.tokens()
-        # out_hr()
-        # print(f"offset_to_label        = {offset_to_label}")
-        # out_hr()
-        # print(f"input_tokens           = {inputs.tokens()}")
-        # out_hr()
-        # for key in inputs.keys():
-        #     print(f"inputs[{key:14s}] = {inputs[key]}")
-        # out_hr()
-
-        label_list: list[str] = []
-        for i in range(args.model.max_seq_length):
-            token = input_tokens[i]
-            token_span: CharSpan = inputs.token_to_chars(i)
+) -> List[NEREncodedExample]:
+    label_to_id: Dict[str, int] = {label: i for i, label in enumerate(label_list)}
+    id_to_label: Dict[int, str] = {i: label for i, label in enumerate(label_list)}
+    if args.env.off_debugging:
+        print(f"label_to_id = {label_to_id}")
+        print(f"id_to_label = {id_to_label}")
+
+    encoded_examples: List[NEREncodedExample] = []
+    for idx, raw_example in enumerate(raw_examples):
+        raw_example: NERRawExample = raw_example
+        offset_to_label: Dict[int, str] = raw_example.get_offset_label_dict()
+        if args.env.off_tracing:
+            out_hr()
+            print(f"offset_to_label = {offset_to_label}")
+        encoded: BatchEncoding = tokenizer.encode_plus(raw_example.origin,
+                                                       max_length=args.model.max_seq_length,
+                                                       truncation=TruncationStrategy.LONGEST_FIRST,
+                                                       padding=PaddingStrategy.MAX_LENGTH)
+        encoded_tokens: List[str] = encoded.tokens()
+        if args.env.off_debugging:
+            out_hr()
+            print(f"encoded.tokens()           = {encoded.tokens()}")
+            for key in encoded.keys():
+                print(f"encoded[{key:14s}]    = {encoded[key]}")
+
+        if args.env.off_tracing:
+            out_hr()
+        label_list: List[str] = []
+        for token_id in range(args.model.max_seq_length):
+            token_repr: str = encoded_tokens[token_id]
+            token_span: CharSpan = encoded.token_to_chars(token_id)
             if token_span:
                 token_label = _decide_span_label(token_span, offset_to_label)
                 label_list.append(token_label)
-                # token_str = example.origin[token_span.start:token_span.end]
-                # print('\t'.join(map(str, [i, token, token_span, token_str, token_label])))
+                if args.env.off_tracing:
+                    token_sstr = raw_example.origin[token_span.start:token_span.end]
+                    print('\t'.join(map(str, [token_id, token_repr, token_span, token_sstr, token_label])))
             else:
-                label_list.append(token)
-                # print('\t'.join(map(str, [i, token, token_span])))
-        label_ids: list[int] = [label_to_id[label] for label in label_list]
-        features.append(NERFeatures(**inputs, label_ids=label_ids))
-        # print(f"label_list             = {label_list}")
-        # out_hr()
-        # print(f"label_ids              = {label_ids}")
-        # print(f"features               = {features[-1]}")
-
-    for i, example in enumerate(examples[:num_show_example]):
-        logger.info("  === [Example %d] ===" % (i + 1))
-        logger.info("  = sentence : %s" % example.origin)
-        logger.info("  = entities : %s" % example.entity_list)
-        logger.info("  = tokens   : %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
-        logger.info("  = labels   : %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
-        logger.info("  = features : %s" % features[i])
+                label_list.append('O')
+                if args.env.off_tracing:
+                    print('\t'.join(map(str, [token_id, token_repr, token_span])))
+        label_ids: List[int] = [label_to_id[label] for label in label_list]
+        encoded_example = NEREncodedExample(idx=idx, raw=raw_example, encoded=encoded, label_ids=label_ids)
+        encoded_examples.append(encoded_example)
+        if args.env.off_debugging:
+            out_hr()
+            print(f"label_list                = {label_list}")
+            print(f"label_ids                 = {label_ids}")
+            out_hr()
+            print(f"encoded_example.idx       = {encoded_example.idx}")
+            print(f"encoded_example.raw       = {encoded_example.raw}")
+            print(f"encoded_example.encoded   = {encoded_example.encoded}")
+            print(f"encoded_example.label_ids = {encoded_example.label_ids}")
+
+    if args.env.off_debugging:
+        out_hr()
+    for encoded_example in encoded_examples[:args.data.show_examples]:
+        logger.info("  === [Example %d] ===" % encoded_example.idx)
+        logger.info("  = sentence   : %s" % encoded_example.raw.origin)
+        logger.info("  = characters : %s" % " | ".join(f"{x}/{y}" for x, y in encoded_example.raw.character_list))
+        logger.info("  = tokens     : %s" % " ".join(encoded_example.encoded.tokens()))
+        logger.info("  = labels     : %s" % " ".join([id_to_label[x] for x in encoded_example.label_ids]))
         logger.info("  === ")
 
-    return features
+    logger.info(f"Converted {len(raw_examples)} raw examples to {len(encoded_examples)} encoded examples")
+    return encoded_examples
 
 
 class NERDataset(Dataset):
     def __init__(self, split: str, args: TesterArguments, tokenizer: PreTrainedTokenizerFast, corpus: NERCorpus):
         assert corpus, "corpus is not valid"
-        self.corpus = corpus
-
         assert args.data.home, f"No data_home: {args.data.home}"
         assert args.data.name, f"No data_name: {args.data.name}"
+        self.corpus: NERCorpus = corpus
         data_file_dict: dict = args.data.files.to_dict()
         assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
         assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
         text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
-        cache_data_path = text_data_path \
-            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
-            .with_suffix(".cache")
-        cache_lock_path = cache_data_path.with_suffix(".lock")
-
-        with FileLock(cache_lock_path):
-            if os.path.exists(cache_data_path) and args.data.caching:
-                start = time.time()
-                self.features = torch.load(cache_data_path)
-                logger.info(f"Loading features from cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
-            else:
-                assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
-                logger.info(f"Creating features from dataset file at {text_data_path}")
-                examples = self.corpus.get_examples(text_data_path)
-                self.features = _convert_examples_to_ner_features(examples, tokenizer, args, label_list=self.corpus.get_labels())
-                start = time.time()
-                torch.save(self.features, cache_data_path)
-                logger.info(f"Saving features into cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
+        assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
+        logger.info(f"Creating features from dataset file at {text_data_path}")
+        examples: List[NERRawExample] = self.corpus.read_raw_examples(text_data_path)
+        self.label_list: List[str] = self.corpus.get_labels()
+        self._label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self.label_list)}
+        self._id_to_label: Dict[int, str] = {i: label for i, label in enumerate(self.label_list)}
+        self.features: List[NEREncodedExample] = \
+            _convert_to_encoded_examples(examples, tokenizer, args, label_list=self.label_list)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.features)
 
-    def __getitem__(self, i):
+    def __getitem__(self, i) -> NEREncodedExample:
         return self.features[i]
 
-    def get_labels(self):
-        return self.corpus.get_labels()
+    def get_labels(self) -> List[str]:
+        return self.label_list
+
+    def label_to_id(self, label: str) -> int:
+        return self._label_to_id[label]
+
+    def id_to_label(self, label_id: int) -> str:
+        return self._id_to_label[label_id]
 
 
-def _parse_tagged(origin: str, tagged: str, debug: bool = False) -> Optional[NERExampleForKLUE]:
-    entity_list: list[EntityInText] = []
+def parse_tagged(origin: str, tagged: str, debug: bool = False) -> Optional[NERRawExample]:
+    entity_list: List[EntityInText] = []
     if debug:
         print(f"* origin: {origin}")
         print(f"  tagged: {tagged}")
     restored = tagged[:]
     no_problem = True
     offset_labels = {i: "O" for i in range(len(origin))}
     while True:
@@ -236,22 +248,22 @@
             print(f"  = {entity} -> {extracted}")
             # print(f"    {offset_labels}")
     if debug:
         print(f"  --------------------")
     character_list = [(origin[i], offset_labels[i]) for i in range(len(origin))]
     if restored != origin:
         no_problem = False
-    return NERExampleForKLUE(origin, entity_list, character_list) if no_problem else None
+    return NERRawExample(origin, entity_list, character_list) if no_problem else None
 
 
 def convert_kmou_format(infile: str | Path, outfile: str | Path, debug: bool = False):
     with Path(infile).open(encoding="utf-8") as inp, Path(outfile).open("w", encoding="utf-8") as out:
         for line in inp.readlines():
             origin, tagged = line.strip().split("\u241E")
-            parsed: Optional[NERExampleForKLUE] = _parse_tagged(origin, tagged, debug=debug)
+            parsed: Optional[NERRawExample] = parse_tagged(origin, tagged, debug=debug)
             if parsed:
                 out.write(parsed.to_json(ensure_ascii=False) + "\n")
 
 
 def convert_klue_format(infile: str | Path, outfile: str | Path, debug: bool = False):
     with Path(infile) as inp, Path(outfile).open("w", encoding="utf-8") as out:
         raw_text = inp.read_text(encoding="utf-8").strip()
@@ -264,15 +276,15 @@
                     break
                 num_header += 1
             head_lines = raw_lines[:num_header]
             body_lines = raw_lines[num_header:]
 
             origin = ''.join(x.split("\t")[0] for x in body_lines)
             tagged = head_lines[-1].split("\t")[1].strip()
-            parsed: Optional[NERExampleForKLUE] = _parse_tagged(origin, tagged, debug=debug)
+            parsed: Optional[NERRawExample] = parse_tagged(origin, tagged, debug=debug)
             if parsed:
                 character_list_from_head = parsed.character_list
                 character_list_from_body = [tuple(x.split("\t")) for x in body_lines]
                 if character_list_from_head == character_list_from_body:
                     out.write(parsed.to_json(ensure_ascii=False) + "\n")
                 elif debug:
                     print(f"* origin: {origin}")
```

### Comparing `chrislab-0.5.3/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.4/src/nlpbook/paircls/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 import logging
 from nlpbook.cls.corpus import ClassificationExample
 
 
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
 
 
 class KlueNLICorpus:
 
     def __init__(self):
         pass
```

### Comparing `chrislab-0.5.3/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.4/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/qa/arguments.py` & `chrislab-0.5.4/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/qa/corpus.py` & `chrislab-0.5.4/src/nlpbook/qa/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 from tqdm import tqdm
 
 from nlpbook.qa import QATrainArguments
 from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
 
 
 @dataclass
 class QAExample:
     # 질문 : 임종석이 여의도 농민 폭력 시위를 주도한 혐의로 지명수배 된 날은?
     question_text: str
     # (답 찾는 대상인)지문 : 1989년 2월 15일 여의도 농민 폭력 시위를 주도한 혐의 ... 서울지방경찰청 공안분실로 인계되었다.
```

### Comparing `chrislab-0.5.3/src/nlpbook/qa/deploy.py` & `chrislab-0.5.4/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.3/src/nlpbook/qa/task.py` & `chrislab-0.5.4/src/nlpbook/qa/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from pytorch_lightning import LightningModule
-from torch.optim import AdamW
-from torch.optim.lr_scheduler import ExponentialLR
-
+from lightning.pytorch import LightningModule
 from nlpbook.metrics import accuracy
 from nlpbook.qa import QATrainArguments
+from torch.optim import AdamW
+from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel
 
 
 class QATask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
```

### Comparing `chrislab-0.5.3/src/nlpbook/utils.py` & `chrislab-0.5.4/src/nlpbook/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
 import os
+import re
 import sys
+from pathlib import Path
+from typing import List, Tuple
 
 import requests
 import tqdm
-
 from transformers import HfArgumentParser
+
+from chrisbase.io import sys_stdout
 from .arguments import TrainerArguments, TesterArguments
 
 REMOTE_DATA_MAP = {
     "nsmc": {
         "train": {
             "web_url": "https://github.com/e9t/nsmc/raw/master/ratings_train.txt",
             "fname": "train.txt",
@@ -68,15 +72,16 @@
         "config": {
             "googledrive_file_id": "1z6obNRWPHoVrMzT9THElblebdovuDLUZ",
             "fname": "config.json",
         },
     },
 }
 GOOGLE_DRIVE_URL = "https://docs.google.com/uc?export=download"
-logger = logging.getLogger("nlpbook")
+logger = logging.getLogger("chrislab")
+TERM_IN_NAME_FORMAT = re.compile(re.escape("{") + "(.+?)(:.+?)?" + re.escape("}"))
 
 
 def save_response_content(response, save_path):
     with open(save_path, "wb") as f:
         content_length = response.headers.get("Content-Length")
         total = int(content_length) if content_length is not None else None
         progress = tqdm.tqdm(
@@ -211,32 +216,67 @@
         raise ValueError(f"not valid model name({pretrained_model_name}), cannot download resources")
 
 
 def set_seed(args: TrainerArguments):
     if args.learning.seed is not None:
         from transformers import set_seed
         set_seed(args.learning.seed)
-        from pytorch_lightning import seed_everything
+        from lightning.pytorch import seed_everything
         seed_everything(args.learning.seed)
     else:
         print("not fixed seed", file=sys.stderr)
 
 
-def set_logger(level=logging.INFO):
-    import torch
-    if torch.cuda.is_available():
-        stream_handler = logging.StreamHandler()
-        formatter = logging.Formatter(fmt="%(levelname)s:%(name)s:%(message)s")
-        stream_handler.setFormatter(formatter)
-        logger.addHandler(stream_handler)
-    logger.setLevel(level)
+def new_logger(name="chrislab", stream=sys_stdout, level=logging.INFO, fmt="%(levelname)s\t%(name)s\t%(message)s") -> logging.Logger:
+    stream_handler = logging.StreamHandler(stream=stream)
+    stream_handler.setFormatter(logging.Formatter(fmt=fmt))
+    new_logger = logging.getLogger(name)
+    new_logger.addHandler(stream_handler)
+    new_logger.setLevel(level)
+    return new_logger
+
+
+def new_logger_file(name="chrislab", filepath="running.log", filemode="a",
+                    stream=sys_stdout, level=logging.INFO, fmt="%(levelname)s\t%(name)s\t%(message)s") -> logging.Logger:
+    stream_handler = logging.StreamHandler(stream=stream)
+    file_handler = logging.FileHandler(filename=filepath, mode=filemode, encoding="utf-8")
+
+    stream_handler.setFormatter(logging.Formatter(fmt=fmt))
+    file_handler.setFormatter(logging.Formatter(fmt=fmt))
+
+    new_logger = logging.getLogger(name)
+    new_logger.addHandler(stream_handler)
+    new_logger.addHandler(file_handler)
+    new_logger.setLevel(level)
+    return new_logger
 
 
 def load_arguments(argument_class, json_file_path=None):
     parser = HfArgumentParser(argument_class)
     if json_file_path is not None:
         args, = parser.parse_json_file(json_file=json_file_path)
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         args, = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         args, = parser.parse_args_into_dataclasses()
     return args
+
+
+# https://lightning.ai/docs/fabric/stable/guide/checkpoint.html
+def save_checkpoint(fabric, args, metric_values, model, optimizer,
+                    sorted_checkpoints: List[Tuple[float, Path]], sorting_reverse, sorting_metric):
+    checkpoint_state = {"model": model, "optimizer": optimizer, "args": args}
+    terms = [m.group(1) for m in TERM_IN_NAME_FORMAT.finditer(args.model.finetuning_name)]
+    terms = {term: metric_values[term] for term in terms}
+    checkpoint_stem = args.model.finetuning_name.format(**terms)
+    checkpoint_path: Path = (args.output.dir_path / "model.out").with_stem(checkpoint_stem).with_suffix(".ckpt")
+
+    sorted_checkpoints.append((metric_values[sorting_metric], checkpoint_path))
+    sorted_checkpoints.sort(key=lambda x: x[0], reverse=sorting_reverse)
+    for _, path in sorted_checkpoints[args.learning.num_keeping:]:
+        path.unlink(missing_ok=True)
+    sorted_checkpoints = [(value, path) for value, path in sorted_checkpoints[:args.learning.num_keeping] if path.exists()]
+    if len(sorted_checkpoints) < args.learning.num_keeping:
+        fabric.save(checkpoint_path, checkpoint_state)
+        sorted_checkpoints.append((metric_values[sorting_metric], checkpoint_path))
+        sorted_checkpoints.sort(key=lambda x: x[0], reverse=sorting_reverse)
+    return sorted_checkpoints
```

