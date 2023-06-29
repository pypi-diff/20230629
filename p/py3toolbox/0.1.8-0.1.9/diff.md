# Comparing `tmp/py3toolbox-0.1.8.tar.gz` & `tmp/py3toolbox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\py3toolbox-0.1.8.tar", last modified: Mon Jan 25 13:26:45 2021, max compression
+gzip compressed data, was "dist\py3toolbox-0.1.9.tar", last modified: Mon Jan 25 13:30:38 2021, max compression
```

## Comparing `py3toolbox-0.1.8.tar` & `py3toolbox-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/
--rw-rw-rw-   0        0        0      377 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/docs/
--rw-rw-rw-   0        0        0        0 2019-02-15 08:58:46.000000 py3toolbox-0.1.8/docs/usages.txt
-drwxrwxrwx   0        0        0        0 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/py3toolbox/
--rw-rw-rw-   0        0        0      598 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/py3toolbox/__init__.py
--rw-rw-rw-   0        0        0     2796 2020-06-28 23:31:15.000000 py3toolbox-0.1.8/py3toolbox/constants.py
--rw-rw-rw-   0        0        0     3332 2020-07-13 04:35:06.000000 py3toolbox-0.1.8/py3toolbox/daemon_tools.py
--rw-rw-rw-   0        0        0      240 2019-08-12 03:15:44.000000 py3toolbox-0.1.8/py3toolbox/dict_tools.py
--rw-rw-rw-   0        0        0    20272 2021-01-25 05:05:16.000000 py3toolbox-0.1.8/py3toolbox/fs_tools.py
--rw-rw-rw-   0        0        0    16891 2020-07-02 04:02:47.000000 py3toolbox-0.1.8/py3toolbox/gdrive_tools.py
--rw-rw-rw-   0        0        0      903 2020-07-10 08:36:32.000000 py3toolbox-0.1.8/py3toolbox/helper.py
--rw-rw-rw-   0        0        0      408 2019-02-15 08:58:47.000000 py3toolbox-0.1.8/py3toolbox/html_tools.py
--rw-rw-rw-   0        0        0      333 2020-01-02 06:49:56.000000 py3toolbox-0.1.8/py3toolbox/img_tools.py
--rw-rw-rw-   0        0        0      712 2019-08-12 03:44:13.000000 py3toolbox-0.1.8/py3toolbox/json_tools.py
--rw-rw-rw-   0        0        0     3015 2020-08-07 03:33:17.000000 py3toolbox-0.1.8/py3toolbox/mail_tools.py
--rw-rw-rw-   0        0        0     1986 2019-09-21 12:06:51.000000 py3toolbox-0.1.8/py3toolbox/media_tools.py
--rw-rw-rw-   0        0        0     2552 2020-01-16 23:44:21.000000 py3toolbox-0.1.8/py3toolbox/net_tools.py
--rw-rw-rw-   0        0        0      806 2020-07-07 00:57:03.000000 py3toolbox-0.1.8/py3toolbox/os_tools.py
--rw-rw-rw-   0        0        0     6589 2020-07-09 14:34:06.000000 py3toolbox-0.1.8/py3toolbox/print_tools.py
--rw-rw-rw-   0        0        0        0 2020-07-09 01:42:15.000000 py3toolbox-0.1.8/py3toolbox/security_tools.py
--rw-rw-rw-   0        0        0      693 2020-12-20 00:59:51.000000 py3toolbox-0.1.8/py3toolbox/text_tools.py
--rw-rw-rw-   0        0        0     4839 2020-07-09 02:51:11.000000 py3toolbox-0.1.8/py3toolbox/time_tools.py
--rw-rw-rw-   0        0        0     2177 2019-02-15 08:58:47.000000 py3toolbox-0.1.8/py3toolbox/xml_tools.py
--rw-rw-rw-   0        0        0       44 2019-02-15 08:58:47.000000 py3toolbox-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      547 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-25 13:26:45.000000 py3toolbox-0.1.8/test/
--rw-rw-rw-   0        0        0     1453 2019-02-15 08:58:47.000000 py3toolbox-0.1.8/test/test.py
+drwxrwxrwx   0        0        0        0 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/
+-rw-rw-rw-   0        0        0      377 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/docs/
+-rw-rw-rw-   0        0        0        0 2019-02-15 08:58:46.000000 py3toolbox-0.1.9/docs/usages.txt
+drwxrwxrwx   0        0        0        0 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/py3toolbox/
+-rw-rw-rw-   0        0        0      598 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/py3toolbox/__init__.py
+-rw-rw-rw-   0        0        0     2796 2020-06-28 23:31:15.000000 py3toolbox-0.1.9/py3toolbox/constants.py
+-rw-rw-rw-   0        0        0     3332 2020-07-13 04:35:06.000000 py3toolbox-0.1.9/py3toolbox/daemon_tools.py
+-rw-rw-rw-   0        0        0      240 2019-08-12 03:15:44.000000 py3toolbox-0.1.9/py3toolbox/dict_tools.py
+-rw-rw-rw-   0        0        0    20272 2021-01-25 05:05:16.000000 py3toolbox-0.1.9/py3toolbox/fs_tools.py
+-rw-rw-rw-   0        0        0    16891 2020-07-02 04:02:47.000000 py3toolbox-0.1.9/py3toolbox/gdrive_tools.py
+-rw-rw-rw-   0        0        0      903 2020-07-10 08:36:32.000000 py3toolbox-0.1.9/py3toolbox/helper.py
+-rw-rw-rw-   0        0        0      408 2019-02-15 08:58:47.000000 py3toolbox-0.1.9/py3toolbox/html_tools.py
+-rw-rw-rw-   0        0        0      333 2020-01-02 06:49:56.000000 py3toolbox-0.1.9/py3toolbox/img_tools.py
+-rw-rw-rw-   0        0        0      712 2019-08-12 03:44:13.000000 py3toolbox-0.1.9/py3toolbox/json_tools.py
+-rw-rw-rw-   0        0        0     3015 2020-08-07 03:33:17.000000 py3toolbox-0.1.9/py3toolbox/mail_tools.py
+-rw-rw-rw-   0        0        0     1986 2019-09-21 12:06:51.000000 py3toolbox-0.1.9/py3toolbox/media_tools.py
+-rw-rw-rw-   0        0        0     2552 2020-01-16 23:44:21.000000 py3toolbox-0.1.9/py3toolbox/net_tools.py
+-rw-rw-rw-   0        0        0      806 2020-07-07 00:57:03.000000 py3toolbox-0.1.9/py3toolbox/os_tools.py
+-rw-rw-rw-   0        0        0     6589 2020-07-09 14:34:06.000000 py3toolbox-0.1.9/py3toolbox/print_tools.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 01:42:15.000000 py3toolbox-0.1.9/py3toolbox/security_tools.py
+-rw-rw-rw-   0        0        0      693 2020-12-20 00:59:51.000000 py3toolbox-0.1.9/py3toolbox/text_tools.py
+-rw-rw-rw-   0        0        0     4839 2020-07-09 02:51:11.000000 py3toolbox-0.1.9/py3toolbox/time_tools.py
+-rw-rw-rw-   0        0        0     2177 2019-02-15 08:58:47.000000 py3toolbox-0.1.9/py3toolbox/xml_tools.py
+-rw-rw-rw-   0        0        0       44 2019-02-15 08:58:47.000000 py3toolbox-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      547 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-01-25 13:30:38.000000 py3toolbox-0.1.9/test/
+-rw-rw-rw-   0        0        0     1453 2019-02-15 08:58:47.000000 py3toolbox-0.1.9/test/test.py
```

### Comparing `py3toolbox-0.1.8/py3toolbox/__init__.py` & `py3toolbox-0.1.9/py3toolbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__  = "Great Tomorrow(gr82morozr@gmail.com)"
 __license__ = "MIT"
-__version__ = "0.1.8",
+__version__ = "0.1.9",
 
 from .fs_tools        import  *
 from .img_tools       import  *
 from .net_tools       import  *
 from .print_tools     import  *
 from .time_tools      import  *
 from .json_tools      import  *
```

### Comparing `py3toolbox-0.1.8/py3toolbox/constants.py` & `py3toolbox-0.1.9/py3toolbox/constants.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/daemon_tools.py` & `py3toolbox-0.1.9/py3toolbox/daemon_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/fs_tools.py` & `py3toolbox-0.1.9/py3toolbox/fs_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/gdrive_tools.py` & `py3toolbox-0.1.9/py3toolbox/gdrive_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/helper.py` & `py3toolbox-0.1.9/py3toolbox/helper.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/json_tools.py` & `py3toolbox-0.1.9/py3toolbox/json_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/mail_tools.py` & `py3toolbox-0.1.9/py3toolbox/mail_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/media_tools.py` & `py3toolbox-0.1.9/py3toolbox/media_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/net_tools.py` & `py3toolbox-0.1.9/py3toolbox/net_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/os_tools.py` & `py3toolbox-0.1.9/py3toolbox/os_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/print_tools.py` & `py3toolbox-0.1.9/py3toolbox/print_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/text_tools.py` & `py3toolbox-0.1.9/py3toolbox/text_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/time_tools.py` & `py3toolbox-0.1.9/py3toolbox/time_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/py3toolbox/xml_tools.py` & `py3toolbox-0.1.9/py3toolbox/xml_tools.py`

 * *Files identical despite different names*

### Comparing `py3toolbox-0.1.8/setup.py` & `py3toolbox-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name          = 'py3toolbox',
   packages      = ['py3toolbox'],
-  version       = '0.1.8',
+  version       = '0.1.9',
   description   = 'A Python3 tools and utilities collection',
   author        = 'Great Tomorrow',
   author_email  = 'gr82morozr@gmail.com',
   url           = 'https://github.com/gr82morozr/py3toolbox.git',  
   download_url  = 'https://github.com/gr82morozr/py3toolbox.git', 
   keywords      = ['Python3', 'Utility', 'Tools' ], 
   classifiers   = [],
```

### Comparing `py3toolbox-0.1.8/test/test.py` & `py3toolbox-0.1.9/test/test.py`

 * *Files identical despite different names*

