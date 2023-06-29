# Comparing `tmp/wwwpy-0.0.8.tar.gz` & `tmp/wwwpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simone/Documents/python/pynanto2bis/dist/.tmp-55h8isy9/wwwpy-0.0.8.tar", last modified: Sat Mar 11 09:41:57 2023, max compression
+gzip compressed data, was "/home/simone/Documents/python/pynanto2bis/dist/.tmp-0zm0ufue/wwwpy-0.0.9.tar", last modified: Mon Mar 13 18:05:19 2023, max compression
```

## Comparing `wwwpy-0.0.8.tar` & `wwwpy-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/
--rw-rw-r--   0 simone    (1000) simone    (1000)     2642 2023-03-11 09:41:57.000000 wwwpy-0.0.8/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     2015 2023-03-02 23:31:53.000000 wwwpy-0.0.8/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)      147 2023-03-02 14:42:33.000000 wwwpy-0.0.8/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)     1053 2023-03-11 09:41:57.000000 wwwpy-0.0.8/setup.cfg
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/js/
--rw-rw-r--   0 simone    (1000) simone    (1000)       17 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/js/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)   526414 2023-03-05 19:01:29.000000 wwwpy-0.0.8/src/js/__init__.pyi
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/
--rw-rw-r--   0 simone    (1000) simone    (1000)      811 2023-03-11 09:41:41.000000 wwwpy-0.0.8/src/pynanto/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1964 2023-03-02 18:39:53.000000 wwwpy-0.0.8/src/pynanto/bootstrap.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      921 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/bundle.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1710 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/bundles.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/common/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/common/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1806 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/common/bundle.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/common/test/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/common/test/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2851 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/common/test/test_bundle.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4542 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/config.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      242 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/exceptions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      221 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/quickstart.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/remote/
--rw-rw-r--   0 simone    (1000) simone    (1000)      113 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      634 2023-03-10 18:05:06.000000 wwwpy-0.0.8/src/pynanto/remote/asyncjs.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/remote/components/
--rw-rw-r--   0 simone    (1000) simone    (1000)     2098 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/components/ForwardTo.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/components/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      420 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/components/pn_button.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      331 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/components/pn_slider.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      470 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/components/pn_text.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2010 2023-03-10 18:12:53.000000 wwwpy-0.0.8/src/pynanto/remote/components/spinner_widget.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      116 2023-03-09 12:20:09.000000 wwwpy-0.0.8/src/pynanto/remote/components/spinner_widget_test.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      195 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/elements.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      293 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/fetch.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      730 2023-03-10 18:07:47.000000 wwwpy-0.0.8/src/pynanto/remote/hash_args.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1373 2023-03-11 09:41:15.000000 wwwpy-0.0.8/src/pynanto/remote/hotkey.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2648 2023-03-10 18:29:32.000000 wwwpy-0.0.8/src/pynanto/remote/test_widget.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1300 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/unittest_fix.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3498 2023-03-10 18:27:47.000000 wwwpy-0.0.8/src/pynanto/remote/widget.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/remote/widgets/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/widgets/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2545 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/remote/widgets/filesystem_tree_widget.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      516 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/resource.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      439 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/response.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      622 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/routes.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     5499 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/rpc.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/server/
--rw-rw-r--   0 simone    (1000) simone    (1000)       64 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/server/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      809 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/server/fetch.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      649 2023-03-02 17:40:06.000000 wwwpy-0.0.8/src/pynanto/server/find_port.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      346 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/server/wait_url.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1140 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/unasync.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1450 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webserver.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/pynanto/webservers/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1223 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/available_webservers.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      921 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/fastapi.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      902 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/flask.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3696 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/python_embedded.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1826 2023-03-02 14:42:33.000000 wwwpy-0.0.8/src/pynanto/webservers/tornado.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     2642 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1859 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-03-02 14:53:53.000000 wwwpy-0.0.8/src/wwwpy.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)      178 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       11 2023-03-11 09:41:57.000000 wwwpy-0.0.8/src/wwwpy.egg-info/top_level.txt
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-11 09:41:57.000000 wwwpy-0.0.8/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1521 2023-03-02 23:22:17.000000 wwwpy-0.0.8/tests/test_bootstrap.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1543 2023-03-02 18:57:16.000000 wwwpy-0.0.8/tests/test_end2end.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      658 2023-03-02 14:42:33.000000 wwwpy-0.0.8/tests/test_stack_filename.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      258 2023-03-02 14:42:33.000000 wwwpy-0.0.8/tests/test_unsync.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1464 2023-03-02 14:42:33.000000 wwwpy-0.0.8/tests/test_webserver.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2642 2023-03-13 18:05:19.000000 wwwpy-0.0.9/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2015 2023-03-02 23:31:53.000000 wwwpy-0.0.9/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)      147 2023-03-02 14:42:33.000000 wwwpy-0.0.9/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1053 2023-03-13 18:05:19.000000 wwwpy-0.0.9/setup.cfg
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/js/
+-rw-rw-r--   0 simone    (1000) simone    (1000)       17 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/js/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)   526414 2023-03-05 19:01:29.000000 wwwpy-0.0.9/src/js/__init__.pyi
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      811 2023-03-13 18:04:56.000000 wwwpy-0.0.9/src/pynanto/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1964 2023-03-02 18:39:53.000000 wwwpy-0.0.9/src/pynanto/bootstrap.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      921 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/bundle.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1710 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/bundles.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/common/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/common/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1806 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/common/bundle.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/common/test/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/common/test/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2851 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/common/test/test_bundle.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4542 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/config.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      242 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/exceptions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      221 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/quickstart.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/remote/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      113 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      634 2023-03-10 18:05:06.000000 wwwpy-0.0.9/src/pynanto/remote/asyncjs.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/remote/components/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2098 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/components/ForwardTo.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/components/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      420 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/components/pn_button.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      331 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/components/pn_slider.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      470 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/components/pn_text.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2010 2023-03-10 18:12:53.000000 wwwpy-0.0.9/src/pynanto/remote/components/spinner_widget.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      116 2023-03-09 12:20:09.000000 wwwpy-0.0.9/src/pynanto/remote/components/spinner_widget_test.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      195 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/elements.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      293 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/fetch.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      730 2023-03-10 18:07:47.000000 wwwpy-0.0.9/src/pynanto/remote/hash_args.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1373 2023-03-11 09:41:15.000000 wwwpy-0.0.9/src/pynanto/remote/hotkey.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2648 2023-03-10 18:29:32.000000 wwwpy-0.0.9/src/pynanto/remote/test_widget.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1300 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/unittest_fix.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3498 2023-03-10 18:27:47.000000 wwwpy-0.0.9/src/pynanto/remote/widget.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/remote/widgets/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/remote/widgets/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3537 2023-03-13 16:33:56.000000 wwwpy-0.0.9/src/pynanto/remote/widgets/filesystem_tree_widget.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      516 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/resource.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      439 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/response.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      622 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/routes.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     5532 2023-03-13 16:51:48.000000 wwwpy-0.0.9/src/pynanto/rpc.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/server/
+-rw-rw-r--   0 simone    (1000) simone    (1000)       64 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/server/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      809 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/server/fetch.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      649 2023-03-02 17:40:06.000000 wwwpy-0.0.9/src/pynanto/server/find_port.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      346 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/server/wait_url.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1140 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/unasync.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1450 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webserver.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/pynanto/webservers/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1223 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/available_webservers.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      921 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/fastapi.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      902 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/flask.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3696 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/python_embedded.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1826 2023-03-02 14:42:33.000000 wwwpy-0.0.9/src/pynanto/webservers/tornado.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2642 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1859 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-03-02 14:53:53.000000 wwwpy-0.0.9/src/wwwpy.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)      178 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       11 2023-03-13 18:05:19.000000 wwwpy-0.0.9/src/wwwpy.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-03-13 18:05:19.000000 wwwpy-0.0.9/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1521 2023-03-02 23:22:17.000000 wwwpy-0.0.9/tests/test_bootstrap.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1543 2023-03-02 18:57:16.000000 wwwpy-0.0.9/tests/test_end2end.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      658 2023-03-02 14:42:33.000000 wwwpy-0.0.9/tests/test_stack_filename.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      258 2023-03-02 14:42:33.000000 wwwpy-0.0.9/tests/test_unsync.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1464 2023-03-02 14:42:33.000000 wwwpy-0.0.9/tests/test_webserver.py
```

### Comparing `wwwpy-0.0.8/PKG-INFO` & `wwwpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwwpy
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/www-py/wwwpy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: Apache 2.0
 Keywords: wwwpy wasm pyodide web development dom html javascript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wwwpy-0.0.8/README.md` & `wwwpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/setup.cfg` & `wwwpy-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/js/__init__.pyi` & `wwwpy-0.0.9/src/js/__init__.pyi`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/__init__.py` & `wwwpy-0.0.9/src/pynanto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 
 def ws_fastapi() -> WsFastapi:
     from .webservers.fastapi import WsFastapi
     return WsFastapi()
 
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `wwwpy-0.0.8/src/pynanto/bootstrap.py` & `wwwpy-0.0.9/src/pynanto/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/bundle.py` & `wwwpy-0.0.9/src/pynanto/bundle.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/bundles.py` & `wwwpy-0.0.9/src/pynanto/bundles.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/common/bundle.py` & `wwwpy-0.0.9/src/pynanto/common/bundle.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/common/test/test_bundle.py` & `wwwpy-0.0.9/src/pynanto/common/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/config.py` & `wwwpy-0.0.9/src/pynanto/config.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/asyncjs.py` & `wwwpy-0.0.9/src/pynanto/remote/asyncjs.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/components/ForwardTo.py` & `wwwpy-0.0.9/src/pynanto/remote/components/ForwardTo.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/components/spinner_widget.py` & `wwwpy-0.0.9/src/pynanto/remote/components/spinner_widget.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/hash_args.py` & `wwwpy-0.0.9/src/pynanto/remote/hash_args.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/hotkey.py` & `wwwpy-0.0.9/src/pynanto/remote/hotkey.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/test_widget.py` & `wwwpy-0.0.9/src/pynanto/remote/test_widget.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/unittest_fix.py` & `wwwpy-0.0.9/src/pynanto/remote/unittest_fix.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/remote/widget.py` & `wwwpy-0.0.9/src/pynanto/remote/widget.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/resource.py` & `wwwpy-0.0.9/src/pynanto/resource.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/routes.py` & `wwwpy-0.0.9/src/pynanto/routes.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/rpc.py` & `wwwpy-0.0.9/src/pynanto/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,25 +156,26 @@
         yield StringResource(self._module.name.replace('.', '/') + '.py', stub_source)
 
 
 def generate_stub_source(module: Module, rpc_url: str, imports: str):
     module_name = module.name
     # language=python
     stub_header = f"""
+from __future__ import annotations
 from pynanto.rpc import Proxy
 {imports}
 
 rpc_url = '{rpc_url}'
 module_name = '{module_name}'
 proxy = Proxy(module_name, rpc_url, async_fetch_str)
     """
 
     stub_functions = ''
     for f in module.functions:
         parameters = f.sign.parameters.values()
         params_list = ', '.join(p.name for p in parameters)
         args_list = '' if params_list == '' else ', ' + params_list
-        fun_stub = f'\nasync def {f.name}({params_list}):\n' + \
+        fun_stub = f'\nasync def {f.name}{f.signature}:\n' + \
                    f'    return await proxy.dispatch("{f.name}"{args_list})\n'
         stub_functions += fun_stub
 
     return stub_header + stub_functions
```

### Comparing `wwwpy-0.0.8/src/pynanto/server/fetch.py` & `wwwpy-0.0.9/src/pynanto/server/fetch.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/server/find_port.py` & `wwwpy-0.0.9/src/pynanto/server/find_port.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/unasync.py` & `wwwpy-0.0.9/src/pynanto/unasync.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webserver.py` & `wwwpy-0.0.9/src/pynanto/webserver.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webservers/available_webservers.py` & `wwwpy-0.0.9/src/pynanto/webservers/available_webservers.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webservers/fastapi.py` & `wwwpy-0.0.9/src/pynanto/webservers/fastapi.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webservers/flask.py` & `wwwpy-0.0.9/src/pynanto/webservers/flask.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webservers/python_embedded.py` & `wwwpy-0.0.9/src/pynanto/webservers/python_embedded.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/pynanto/webservers/tornado.py` & `wwwpy-0.0.9/src/pynanto/webservers/tornado.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/src/wwwpy.egg-info/PKG-INFO` & `wwwpy-0.0.9/src/wwwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwwpy
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/www-py/wwwpy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: Apache 2.0
 Keywords: wwwpy wasm pyodide web development dom html javascript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wwwpy-0.0.8/src/wwwpy.egg-info/SOURCES.txt` & `wwwpy-0.0.9/src/wwwpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/tests/test_bootstrap.py` & `wwwpy-0.0.9/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/tests/test_end2end.py` & `wwwpy-0.0.9/tests/test_end2end.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/tests/test_stack_filename.py` & `wwwpy-0.0.9/tests/test_stack_filename.py`

 * *Files identical despite different names*

### Comparing `wwwpy-0.0.8/tests/test_webserver.py` & `wwwpy-0.0.9/tests/test_webserver.py`

 * *Files identical despite different names*

