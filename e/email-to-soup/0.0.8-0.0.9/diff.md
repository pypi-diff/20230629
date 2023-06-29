# Comparing `tmp/email_to_soup-0.0.8.tar.gz` & `tmp/email_to_soup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_to_soup-0.0.8.tar", last modified: Tue Jan 31 12:57:00 2023, max compression
+gzip compressed data, was "email_to_soup-0.0.9.tar", last modified: Wed Feb  1 08:49:45 2023, max compression
```

## Comparing `email_to_soup-0.0.8.tar` & `email_to_soup-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.999897 email_to_soup-0.0.8/
--rw-r--r--   0 devtanna   (501) staff       (20)     1819 2022-11-27 19:16:07.000000 email_to_soup-0.0.8/.gitignore
--rw-r--r--   0 devtanna   (501) staff       (20)     1066 2022-11-27 19:11:13.000000 email_to_soup-0.0.8/LICENSE
--rw-r--r--   0 devtanna   (501) staff       (20)      904 2023-01-31 12:57:00.000023 email_to_soup-0.0.8/PKG-INFO
--rw-r--r--   0 devtanna   (501) staff       (20)      278 2022-11-27 19:48:15.000000 email_to_soup-0.0.8/README.md
--rw-r--r--   0 devtanna   (501) staff       (20)      818 2023-01-31 12:55:37.000000 email_to_soup-0.0.8/pyproject.toml
--rw-r--r--   0 devtanna   (501) staff       (20)       58 2022-12-11 20:22:17.000000 email_to_soup-0.0.8/requirements.txt
--rw-r--r--   0 devtanna   (501) staff       (20)      479 2023-01-31 12:57:00.000355 email_to_soup-0.0.8/setup.cfg
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.996076 email_to_soup-0.0.8/src/
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.997859 email_to_soup-0.0.8/src/email_to_soup/
--rw-r--r--   0 devtanna   (501) staff       (20)       33 2022-11-27 19:45:59.000000 email_to_soup-0.0.8/src/email_to_soup/__init__.py
--rw-r--r--   0 devtanna   (501) staff       (20)     2649 2023-01-31 12:54:34.000000 email_to_soup-0.0.8/src/email_to_soup/main.py
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.998723 email_to_soup-0.0.8/src/email_to_soup.egg-info/
--rw-r--r--   0 devtanna   (501) staff       (20)      904 2023-01-31 12:56:59.000000 email_to_soup-0.0.8/src/email_to_soup.egg-info/PKG-INFO
--rw-r--r--   0 devtanna   (501) staff       (20)      449 2023-01-31 12:56:59.000000 email_to_soup-0.0.8/src/email_to_soup.egg-info/SOURCES.txt
--rw-r--r--   0 devtanna   (501) staff       (20)        1 2023-01-31 12:56:59.000000 email_to_soup-0.0.8/src/email_to_soup.egg-info/dependency_links.txt
--rw-r--r--   0 devtanna   (501) staff       (20)       56 2023-01-31 12:56:59.000000 email_to_soup-0.0.8/src/email_to_soup.egg-info/requires.txt
--rw-r--r--   0 devtanna   (501) staff       (20)       20 2023-01-31 12:56:59.000000 email_to_soup-0.0.8/src/email_to_soup.egg-info/top_level.txt
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.998987 email_to_soup-0.0.8/src/tests/
--rw-r--r--   0 devtanna   (501) staff       (20)        0 2022-11-27 19:16:53.000000 email_to_soup-0.0.8/src/tests/__init__.py
-drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-01-31 12:56:59.999422 email_to_soup-0.0.8/src/tests/fixtures/
--rw-r--r--   0 devtanna   (501) staff       (20)        0 2022-11-27 19:28:35.000000 email_to_soup-0.0.8/src/tests/fixtures/__init__.py
--rw-r--r--   0 devtanna   (501) staff       (20)    27609 2022-11-27 19:28:35.000000 email_to_soup-0.0.8/src/tests/fixtures/test_email.eml
--rw-r--r--   0 devtanna   (501) staff       (20)      458 2022-11-27 19:39:31.000000 email_to_soup-0.0.8/src/tests/test_email_to_soup.py
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.823375 email_to_soup-0.0.9/
+-rw-r--r--   0 devtanna   (501) staff       (20)     1819 2022-11-27 19:16:07.000000 email_to_soup-0.0.9/.gitignore
+-rw-r--r--   0 devtanna   (501) staff       (20)     1066 2022-11-27 19:11:13.000000 email_to_soup-0.0.9/LICENSE
+-rw-r--r--   0 devtanna   (501) staff       (20)      904 2023-02-01 08:49:45.823491 email_to_soup-0.0.9/PKG-INFO
+-rw-r--r--   0 devtanna   (501) staff       (20)      278 2022-11-27 19:48:15.000000 email_to_soup-0.0.9/README.md
+-rw-r--r--   0 devtanna   (501) staff       (20)      818 2023-02-01 08:49:19.000000 email_to_soup-0.0.9/pyproject.toml
+-rw-r--r--   0 devtanna   (501) staff       (20)       58 2022-12-11 20:22:17.000000 email_to_soup-0.0.9/requirements.txt
+-rw-r--r--   0 devtanna   (501) staff       (20)      479 2023-02-01 08:49:45.823799 email_to_soup-0.0.9/setup.cfg
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.819340 email_to_soup-0.0.9/src/
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.821282 email_to_soup-0.0.9/src/email_to_soup/
+-rw-r--r--   0 devtanna   (501) staff       (20)       33 2022-11-27 19:45:59.000000 email_to_soup-0.0.9/src/email_to_soup/__init__.py
+-rw-r--r--   0 devtanna   (501) staff       (20)     2661 2023-02-01 08:49:08.000000 email_to_soup-0.0.9/src/email_to_soup/main.py
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.822126 email_to_soup-0.0.9/src/email_to_soup.egg-info/
+-rw-r--r--   0 devtanna   (501) staff       (20)      904 2023-02-01 08:49:45.000000 email_to_soup-0.0.9/src/email_to_soup.egg-info/PKG-INFO
+-rw-r--r--   0 devtanna   (501) staff       (20)      449 2023-02-01 08:49:45.000000 email_to_soup-0.0.9/src/email_to_soup.egg-info/SOURCES.txt
+-rw-r--r--   0 devtanna   (501) staff       (20)        1 2023-02-01 08:49:45.000000 email_to_soup-0.0.9/src/email_to_soup.egg-info/dependency_links.txt
+-rw-r--r--   0 devtanna   (501) staff       (20)       56 2023-02-01 08:49:45.000000 email_to_soup-0.0.9/src/email_to_soup.egg-info/requires.txt
+-rw-r--r--   0 devtanna   (501) staff       (20)       20 2023-02-01 08:49:45.000000 email_to_soup-0.0.9/src/email_to_soup.egg-info/top_level.txt
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.822386 email_to_soup-0.0.9/src/tests/
+-rw-r--r--   0 devtanna   (501) staff       (20)        0 2022-11-27 19:16:53.000000 email_to_soup-0.0.9/src/tests/__init__.py
+drwxr-xr-x   0 devtanna   (501) staff       (20)        0 2023-02-01 08:49:45.822945 email_to_soup-0.0.9/src/tests/fixtures/
+-rw-r--r--   0 devtanna   (501) staff       (20)        0 2022-11-27 19:28:35.000000 email_to_soup-0.0.9/src/tests/fixtures/__init__.py
+-rw-r--r--   0 devtanna   (501) staff       (20)    27609 2022-11-27 19:28:35.000000 email_to_soup-0.0.9/src/tests/fixtures/test_email.eml
+-rw-r--r--   0 devtanna   (501) staff       (20)      458 2022-11-27 19:39:31.000000 email_to_soup-0.0.9/src/tests/test_email_to_soup.py
```

### Comparing `email_to_soup-0.0.8/.gitignore` & `email_to_soup-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `email_to_soup-0.0.8/LICENSE` & `email_to_soup-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `email_to_soup-0.0.8/PKG-INFO` & `email_to_soup-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email_to_soup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Email to HTML-Soup & Soup-Text
 Home-page: https://github.com/devtanna/email-to-soup
 Author-email: Dev Tanna <dev.tanna@gmail.com>
 Project-URL: Homepage, https://github.com/devtanna/soup-to-email
 Project-URL: Bug Tracker, https://github.com/devtanna/soup-to-email/issues
 Keywords: html-soup,soup-text,email-to-soup,email-to-text
 Classifier: Programming Language :: Python :: 3
```

### Comparing `email_to_soup-0.0.8/pyproject.toml` & `email_to_soup-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email_to_soup"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dev Tanna", email="dev.tanna@gmail.com" },
 ]
 dependencies = [
     "beautifulsoup4==4.11.1",
     "lxml==4.9.1",
     "html2text==2020.1.16",
```

### Comparing `email_to_soup-0.0.8/src/email_to_soup/main.py` & `email_to_soup-0.0.9/src/email_to_soup/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         An EmailSoup object representing the email html-soup, html-body, soup-text.
     """
     email = Parser(policy=default_policy).parsestr(email)
     html_body = email.get_body(preferencelist=('html', 'plain')).get_content()
 
     # Oh, the wonders of HTML emails. Some emails have multiple <html> tags. Let's the one with more content.
     if html_body:
-        html_body = max(re.findall(r"<html .*?</html>", html_body, re.M|re.S|re.I), key=len)
+        html_body = max(re.findall(r"<html.*?</html>", html_body, re.M|re.S|re.I), key=len) or html_body
 
     html_soup = BeautifulSoup(html_body, features="lxml")
     xml_tree = html.fromstring(html_body)
     email_soup = EmailSoup(
         html_soup = html_soup,
         soup_text = _extract_soup_text(html_soup),
         html_body = html_body,
```

### Comparing `email_to_soup-0.0.8/src/email_to_soup.egg-info/PKG-INFO` & `email_to_soup-0.0.9/src/email_to_soup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-to-soup
-Version: 0.0.8
+Version: 0.0.9
 Summary: Email to HTML-Soup & Soup-Text
 Home-page: https://github.com/devtanna/email-to-soup
 Author-email: Dev Tanna <dev.tanna@gmail.com>
 Project-URL: Homepage, https://github.com/devtanna/soup-to-email
 Project-URL: Bug Tracker, https://github.com/devtanna/soup-to-email/issues
 Keywords: html-soup,soup-text,email-to-soup,email-to-text
 Classifier: Programming Language :: Python :: 3
```

### Comparing `email_to_soup-0.0.8/src/tests/fixtures/test_email.eml` & `email_to_soup-0.0.9/src/tests/fixtures/test_email.eml`

 * *Files identical despite different names*

