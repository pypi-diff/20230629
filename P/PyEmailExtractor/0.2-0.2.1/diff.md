# Comparing `tmp/PyEmailExtractor-0.2.tar.gz` & `tmp/PyEmailExtractor-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailExtractor-0.2.tar", last modified: Fri Jun 23 08:40:11 2023, max compression
+gzip compressed data, was "PyEmailExtractor-0.2.1.tar", last modified: Thu Jun 29 09:17:19 2023, max compression
```

## Comparing `PyEmailExtractor-0.2.tar` & `PyEmailExtractor-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/
--rw-rw-r--   0 karki     (1000) karki     (1000)     1525 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/PKG-INFO
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.396879 PyEmailExtractor-0.2/PyEmailExtractor/
--rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtractor-0.2/PyEmailExtractor/__init__.py
--rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtractor-0.2/PyEmailExtractor/driver.py
--rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtractor-0.2/PyEmailExtractor/helper.py
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/
--rw-rw-r--   0 karki     (1000) karki     (1000)     1525 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/PKG-INFO
--rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/SOURCES.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/dependency_links.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       76 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/requires.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/top_level.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)     1275 2023-06-23 08:39:32.000000 PyEmailExtractor-0.2/README.md
--rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/setup.cfg
--rw-rw-r--   0 karki     (1000) karki     (1000)      648 2023-06-23 08:40:09.000000 PyEmailExtractor-0.2/setup.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-29 09:17:19.365390 PyEmailExtractor-0.2.1/
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1649 2023-06-29 09:17:19.365390 PyEmailExtractor-0.2.1/PKG-INFO
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-29 09:17:19.365390 PyEmailExtractor-0.2.1/PyEmailExtractor/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtractor-0.2.1/PyEmailExtractor/__init__.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1085 2023-06-29 09:12:07.000000 PyEmailExtractor-0.2.1/PyEmailExtractor/driver.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     2528 2023-06-29 09:12:39.000000 PyEmailExtractor-0.2.1/PyEmailExtractor/helper.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-29 09:17:19.365390 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1649 2023-06-29 09:17:19.000000 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/PKG-INFO
+-rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-29 09:17:19.000000 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-29 09:17:19.000000 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       88 2023-06-29 09:17:19.000000 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/requires.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-29 09:17:19.000000 PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/top_level.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1398 2023-06-29 09:16:21.000000 PyEmailExtractor-0.2.1/README.md
+-rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-29 09:17:19.365390 PyEmailExtractor-0.2.1/setup.cfg
+-rw-rw-r--   0 karki     (1000) karki     (1000)      655 2023-06-29 09:17:15.000000 PyEmailExtractor-0.2.1/setup.py
```

### Comparing `PyEmailExtractor-0.2/PKG-INFO` & `PyEmailExtractor-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyEmailExtractor
-Version: 0.2
+Version: 0.2.1
 Summary: Tool for extracting emails from pdf and docx files. (Designed especially for resumes)
 Author: Bidut Karki
 Author-email: bidutjava3@gmail.com
 Description-Content-Type: text/markdown
 
-# PyEmailExtractor
+# PyEmailExtractor [![Downloads](https://static.pepy.tech/badge/pyemailextractor)](https://pepy.tech/project/pyemailextractor)
 
 PyEmailExtractor is a tool designed specifically for extracting emails from PDF and DOCX files, with a focus on resumes. It provides a convenient way to extract email addresses from these document formats, which can be useful for various applications, such as recruitment, data analysis, or contact management.
 
 ## Features
 
 - Extract email addresses from PDF files.
 - Extract email addresses from DOCX files.
@@ -41,14 +41,15 @@
 
 PyEmailExtractor requires the following dependencies:
 - docx2txt==0.8
 - lxml==4.9.2
 - PyPDF2==3.0.1
 - python-docx==0.8.11
 - PyMuPDF==1.22.5
+- pytesseract
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the GitHub repository.
 License
 
 `PyEmailExtractor is released under the MIT License. See the LICENSE file for more details.`
```

### Comparing `PyEmailExtractor-0.2/PyEmailExtractor/driver.py` & `PyEmailExtractor-0.2.1/PyEmailExtractor/driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 def extract_emails(dir=""):
     # Example: "/home/user_name/some_directory/resumes"
     # directory = str(
     #     input("Paste the absolute path of the directory and press enter.\n")
     # )
     directory = str(dir)
-    file_extensions = [".docx", ".pdf"]
+    file_extensions = [".docx", ".pdf", ".jpg", ".png"]
     files = fetch_files(directory, file_extensions)
 
     # with open("total_files.txt", "a") as f:
     #     f.write("Total files fetched: \n" + str(len(files)) + "\n")
     arr = []
 
     for file in files:
         current_ext = str(file).split(".")[1]
         if current_ext == "pdf":
             emails = extract_email_from_pdf(file)
         elif current_ext == "docx":
             emails = extract_email_from_docx(file)
+        elif current_ext == "jpg" or current_ext == "png":
+            emails = extract_email_from_image(file)
         else:
             print("Currently we dont support ", str(current_ext))
         for email in emails:
             arr.append(email)
             # with open("email_list.txt", "a") as f:
             #     f.write(str(email) + "\n")\
     return arr
```

### Comparing `PyEmailExtractor-0.2/PyEmailExtractor/helper.py` & `PyEmailExtractor-0.2.1/PyEmailExtractor/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 import os
 import PyPDF2
 import docx2txt
 from docx import Document
 import fitz
+import pytesseract
+from PIL import Image
 
 
 def fetch_files(directory, file_extensions):
     """To fetches all the file with the given ext in the given directory"""
     files = []
     try:
         for dirpath, dirnames, filenames in os.walk(directory):
@@ -49,7 +51,24 @@
         if not email:
             with open("no_email_logs.txt", "a") as f:
                 f.write(str(docx_file) + "\n")
     except Exception as e:
         with open("error_logs.txt", "a") as f:
             f.write("Error from extract_email_from_docx function: \n" + str(e) + "\n")
     return email
+
+
+def extract_email_from_image(image_file):
+    email_pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b"
+    email = ""
+    try:
+        image = Image.open(str(image_file))
+
+        text = pytesseract.image_to_string(image)
+        email = re.findall(email_pattern, text)
+        if not email:
+            with open("no_email_logs.txt", "a") as f:
+                f.write(str(image_file) + "\n")
+    except Exception as e:
+        with open("error_logs.txt", "a") as f:
+            f.write("Error from extract_email_from_image function: \n" + str(e) + "\n")
+    return email
```

### Comparing `PyEmailExtractor-0.2/PyEmailExtractor.egg-info/PKG-INFO` & `PyEmailExtractor-0.2.1/PyEmailExtractor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyEmailExtractor
-Version: 0.2
+Version: 0.2.1
 Summary: Tool for extracting emails from pdf and docx files. (Designed especially for resumes)
 Author: Bidut Karki
 Author-email: bidutjava3@gmail.com
 Description-Content-Type: text/markdown
 
-# PyEmailExtractor
+# PyEmailExtractor [![Downloads](https://static.pepy.tech/badge/pyemailextractor)](https://pepy.tech/project/pyemailextractor)
 
 PyEmailExtractor is a tool designed specifically for extracting emails from PDF and DOCX files, with a focus on resumes. It provides a convenient way to extract email addresses from these document formats, which can be useful for various applications, such as recruitment, data analysis, or contact management.
 
 ## Features
 
 - Extract email addresses from PDF files.
 - Extract email addresses from DOCX files.
@@ -41,14 +41,15 @@
 
 PyEmailExtractor requires the following dependencies:
 - docx2txt==0.8
 - lxml==4.9.2
 - PyPDF2==3.0.1
 - python-docx==0.8.11
 - PyMuPDF==1.22.5
+- pytesseract
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the GitHub repository.
 License
 
 `PyEmailExtractor is released under the MIT License. See the LICENSE file for more details.`
```

### Comparing `PyEmailExtractor-0.2/README.md` & `PyEmailExtractor-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PyEmailExtractor
+# PyEmailExtractor [![Downloads](https://static.pepy.tech/badge/pyemailextractor)](https://pepy.tech/project/pyemailextractor)
 
 PyEmailExtractor is a tool designed specifically for extracting emails from PDF and DOCX files, with a focus on resumes. It provides a convenient way to extract email addresses from these document formats, which can be useful for various applications, such as recruitment, data analysis, or contact management.
 
 ## Features
 
 - Extract email addresses from PDF files.
 - Extract email addresses from DOCX files.
@@ -33,14 +33,15 @@
 
 PyEmailExtractor requires the following dependencies:
 - docx2txt==0.8
 - lxml==4.9.2
 - PyPDF2==3.0.1
 - python-docx==0.8.11
 - PyMuPDF==1.22.5
+- pytesseract
 
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the GitHub repository.
 License
 
-`PyEmailExtractor is released under the MIT License. See the LICENSE file for more details.`
+`PyEmailExtractor is released under the MIT License. See the LICENSE file for more details.`
```

