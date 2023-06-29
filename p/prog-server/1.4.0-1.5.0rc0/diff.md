# Comparing `tmp/prog_server-1.4.0.tar.gz` & `tmp/prog_server-1.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_server-1.4.0.tar", last modified: Fri Oct 28 16:22:11 2022, max compression
+gzip compressed data, was "prog_server-1.5.0rc0.tar", last modified: Thu Jun 29 15:29:23 2023, max compression
```

## Comparing `prog_server-1.4.0.tar` & `prog_server-1.5.0rc0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.487996 prog_server-1.4.0/
--rw-r--r--   0 cteubert   (507) staff       (20)     5933 2022-10-28 16:22:11.487841 prog_server-1.4.0/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     3990 2022-10-20 20:13:26.000000 prog_server-1.4.0/README.md
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2022-10-28 16:22:11.488044 prog_server-1.4.0/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2703 2022-10-20 20:15:59.000000 prog_server-1.4.0/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.483593 prog_server-1.4.0/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.484404 prog_server-1.4.0/src/prog_client/
--rw-r--r--   0 cteubert   (507) staff       (20)      211 2022-05-07 22:50:05.000000 prog_server-1.4.0/src/prog_client/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9298 2022-10-20 20:01:59.000000 prog_server-1.4.0/src/prog_client/session.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.485413 prog_server-1.4.0/src/prog_server/
--rw-r--r--   0 cteubert   (507) staff       (20)     1029 2022-10-25 18:10:47.000000 prog_server-1.4.0/src/prog_server/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      418 2022-10-25 18:09:47.000000 prog_server-1.4.0/src/prog_server/__main__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2370 2022-10-20 18:37:00.000000 prog_server-1.4.0/src/prog_server/app.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21604 2022-10-20 18:43:13.000000 prog_server-1.4.0/src/prog_server/controllers.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.487556 prog_server-1.4.0/src/prog_server/models/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2021-12-22 19:21:19.000000 prog_server-1.4.0/src/prog_server/models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2405 2022-10-20 17:46:26.000000 prog_server-1.4.0/src/prog_server/models/load_ests.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1646 2022-01-18 16:47:38.000000 prog_server-1.4.0/src/prog_server/models/prediction_handler.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1811 2022-10-25 18:10:39.000000 prog_server-1.4.0/src/prog_server/models/prog_server.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5631 2022-10-20 17:22:51.000000 prog_server-1.4.0/src/prog_server/models/session.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-10-28 16:22:11.486085 prog_server-1.4.0/src/prog_server.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     5933 2022-10-28 16:22:11.000000 prog_server-1.4.0/src/prog_server.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)      565 2022-10-28 16:22:11.000000 prog_server-1.4.0/src/prog_server.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2022-10-28 16:22:11.000000 prog_server-1.4.0/src/prog_server.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)       33 2022-10-28 16:22:11.000000 prog_server-1.4.0/src/prog_server.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       24 2022-10-28 16:22:11.000000 prog_server-1.4.0/src/prog_server.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.762075 prog_server-1.5.0rc0/
+-rw-r--r--   0 cteubert   (507) staff       (20)     5987 2023-06-29 15:29:23.761921 prog_server-1.5.0rc0/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     3990 2023-06-21 22:21:41.000000 prog_server-1.5.0rc0/README.md
+-rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-29 15:29:23.762113 prog_server-1.5.0rc0/setup.cfg
+-rw-r--r--   0 cteubert   (507) staff       (20)     2731 2023-06-21 22:21:41.000000 prog_server-1.5.0rc0/setup.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.757111 prog_server-1.5.0rc0/src/
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.758117 prog_server-1.5.0rc0/src/prog_client/
+-rw-r--r--   0 cteubert   (507) staff       (20)      215 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_client/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     9298 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_client/session.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.759349 prog_server-1.5.0rc0/src/prog_server/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1033 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      418 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/__main__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2370 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/app.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    21604 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/controllers.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.761580 prog_server-1.5.0rc0/src/prog_server/models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2021-12-22 19:21:19.000000 prog_server-1.5.0rc0/src/prog_server/models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2405 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/load_ests.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1646 2022-01-18 16:47:38.000000 prog_server-1.5.0rc0/src/prog_server/models/prediction_handler.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1811 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/prog_server.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5631 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/session.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.760391 prog_server-1.5.0rc0/src/prog_server.egg-info/
+-rw-------   0 cteubert   (507) staff       (20)     5987 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/PKG-INFO
+-rw-------   0 cteubert   (507) staff       (20)      565 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/SOURCES.txt
+-rw-------   0 cteubert   (507) staff       (20)        1 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/dependency_links.txt
+-rw-------   0 cteubert   (507) staff       (20)       33 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/requires.txt
+-rw-------   0 cteubert   (507) staff       (20)       24 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/top_level.txt
```

### Comparing `prog_server-1.4.0/PKG-INFO` & `prog_server-1.5.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_server
-Version: 1.4.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures
 Home-page: https://nasa.github.com/progpy/prog_server_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_server/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_server_guide.html
@@ -20,16 +20,17 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: Other/Proprietary License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 
 # Prognostics As-A-Service (PaaS) Sandbox
 [![CodeFactor](https://www.codefactor.io/repository/github/nasa/prog_server/badge)](https://www.codefactor.io/repository/github/nasa/prog_server)
 [![GitHub License](https://img.shields.io/badge/License-NOSA-green)](https://github.com/nasa/prog_server/blob/master/license.pdf)
 [![GitHub Releases](https://img.shields.io/github/release/nasa/prog_server.svg)](https://github.com/nasa/prog_server/releases)
 
@@ -43,27 +44,27 @@
 ## [Documentation](https://nasa.github.io/progpy/prog_server_guide.html)
 See documentation [here](https://nasa.github.io/progpy/prog_server_guide.html)
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2021_nasa_prog_models,
+@misc{2023_nasa_prog_models,
     author    = {Christopher Teubert and Jason Watkins and Katelyn Jarvis},
     title     = {Prognostics As-A-Service (PaaS) Sandbox},
-    month     = Oct,
-    year      = 2022,
-    version   = {1.4},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog_server}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.4, Oct 2022. URL https://github.com/nasa/prog_server.
+C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.5, May 2023. URL https://github.com/nasa/prog_server.
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 ## Disclaimers
 No Warranty: THE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED, WILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER, CONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE, SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.  FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE, IF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."
```

### Comparing `prog_server-1.4.0/README.md` & `prog_server-1.5.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 ## [Documentation](https://nasa.github.io/progpy/prog_server_guide.html)
 See documentation [here](https://nasa.github.io/progpy/prog_server_guide.html)
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2021_nasa_prog_models,
+@misc{2023_nasa_prog_models,
     author    = {Christopher Teubert and Jason Watkins and Katelyn Jarvis},
     title     = {Prognostics As-A-Service (PaaS) Sandbox},
-    month     = Oct,
-    year      = 2022,
-    version   = {1.4},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog_server}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.4, Oct 2022. URL https://github.com/nasa/prog_server.
+C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.5, May 2023. URL https://github.com/nasa/prog_server.
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 ## Disclaimers
 No Warranty: THE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED, WILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER, CONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE, SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.  FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE, IF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."
```

### Comparing `prog_server-1.4.0/setup.py` & `prog_server-1.5.0rc0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,49 +6,50 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
-    name = 'prog_server',
-    version = '1.4.0',
-    description = 'The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures',
+    name='prog_server',
+    version='1.5.0-pre',
+    description='The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url = 'https://nasa.github.com/progpy/prog_server_guide.html',
-    author = 'Christopher Teubert',
-    author_email = 'christopher.a.teubert@nasa.gov',
-    classifiers = [
+    url='https://nasa.github.com/progpy/prog_server_guide.html',
+    author='Christopher Teubert',
+    author_email='christopher.a.teubert@nasa.gov',
+    classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Intended Audience :: Manufacturing', 
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: Other/Proprietary License ',   
         'Programming Language :: Python :: 3',     
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only'
     ],
-    keywords = ['prognostics', 'diagnostics', 'fault detection', 'fdir', 'physics modeling', 'prognostics and health management', 'PHM', 'health management', 'prognostics as a service', 'ivhm'],
-    package_dir = {"":"src"},
-    packages = find_packages(where = 'src'),
-    python_requires='>=3.7, <3.11',
-    install_requires = [
+    keywords=['prognostics', 'diagnostics', 'fault detection', 'fdir', 'physics modeling', 'prognostics and health management', 'PHM', 'health management', 'prognostics as a service', 'ivhm'],
+    package_dir={"":"src"},
+    packages=find_packages(where='src'),
+    python_requires='>=3.7, <3.12',
+    install_requires=[
         'prog_algs',
         'requests',
         'urllib3',
         'flask'
     ],
-    license = 'NOSA',
+    license='NOSA',
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/nasa/prog_server/issues',
         'Docs': 'https://nasa.github.io/progpy/prog_server_guide.html',
         'Organization': 'https://www.nasa.gov/content/diagnostics-prognostics',
         'Source': 'https://github.com/nasa/prog_server',
     },
 )
```

### Comparing `prog_server-1.4.0/src/prog_client/session.py` & `prog_server-1.5.0rc0/src/prog_client/session.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/__init__.py` & `prog_server-1.5.0rc0/src/prog_server/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the
 # National Aeronautics and Space Administration.  All Rights Reserved.
 
 from .models.prog_server import server
 
-__version__ = '1.4.0'
+__version__ = '1.5.0-pre'
 
 def run(**kwargs):
     """
     Start the server and block until it is stopped.
 
     Args:
         host (str, optional): Server host. Defaults to '127.0.0.1'.
```

### Comparing `prog_server-1.4.0/src/prog_server/app.py` & `prog_server-1.5.0rc0/src/prog_server/app.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/controllers.py` & `prog_server-1.5.0rc0/src/prog_server/controllers.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/models/load_ests.py` & `prog_server-1.5.0rc0/src/prog_server/models/load_ests.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/models/prediction_handler.py` & `prog_server-1.5.0rc0/src/prog_server/models/prediction_handler.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/models/prog_server.py` & `prog_server-1.5.0rc0/src/prog_server/models/prog_server.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server/models/session.py` & `prog_server-1.5.0rc0/src/prog_server/models/session.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.4.0/src/prog_server.egg-info/PKG-INFO` & `prog_server-1.5.0rc0/src/prog_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-server
-Version: 1.4.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures
 Home-page: https://nasa.github.com/progpy/prog_server_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_server/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_server_guide.html
@@ -20,16 +20,17 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: Other/Proprietary License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 
 # Prognostics As-A-Service (PaaS) Sandbox
 [![CodeFactor](https://www.codefactor.io/repository/github/nasa/prog_server/badge)](https://www.codefactor.io/repository/github/nasa/prog_server)
 [![GitHub License](https://img.shields.io/badge/License-NOSA-green)](https://github.com/nasa/prog_server/blob/master/license.pdf)
 [![GitHub Releases](https://img.shields.io/github/release/nasa/prog_server.svg)](https://github.com/nasa/prog_server/releases)
 
@@ -43,27 +44,27 @@
 ## [Documentation](https://nasa.github.io/progpy/prog_server_guide.html)
 See documentation [here](https://nasa.github.io/progpy/prog_server_guide.html)
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2021_nasa_prog_models,
+@misc{2023_nasa_prog_models,
     author    = {Christopher Teubert and Jason Watkins and Katelyn Jarvis},
     title     = {Prognostics As-A-Service (PaaS) Sandbox},
-    month     = Oct,
-    year      = 2022,
-    version   = {1.4},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog_server}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.4, Oct 2022. URL https://github.com/nasa/prog_server.
+C. Teubert, J. Watkins, K. Jarvis, Prognostics As-A-Service (PaaS) Sandbox, v1.5, May 2023. URL https://github.com/nasa/prog_server.
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 ## Disclaimers
 No Warranty: THE SUBJECT SOFTWARE IS PROVIDED "AS IS" WITHOUT ANY WARRANTY OF ANY KIND, EITHER EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR FREEDOM FROM INFRINGEMENT, ANY WARRANTY THAT THE SUBJECT SOFTWARE WILL BE ERROR FREE, OR ANY WARRANTY THAT DOCUMENTATION, IF PROVIDED, WILL CONFORM TO THE SUBJECT SOFTWARE. THIS AGREEMENT DOES NOT, IN ANY MANNER, CONSTITUTE AN ENDORSEMENT BY GOVERNMENT AGENCY OR ANY PRIOR RECIPIENT OF ANY RESULTS, RESULTING DESIGNS, HARDWARE, SOFTWARE PRODUCTS OR ANY OTHER APPLICATIONS RESULTING FROM USE OF THE SUBJECT SOFTWARE.  FURTHER, GOVERNMENT AGENCY DISCLAIMS ALL WARRANTIES AND LIABILITIES REGARDING THIRD-PARTY SOFTWARE, IF PRESENT IN THE ORIGINAL SOFTWARE, AND DISTRIBUTES IT "AS IS."
```

### Comparing `prog_server-1.4.0/src/prog_server.egg-info/SOURCES.txt` & `prog_server-1.5.0rc0/src/prog_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

