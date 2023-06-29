# Comparing `tmp/bullmq-1.2.0.tar.gz` & `tmp/bullmq-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.2.0.tar", last modified: Sat Jun 24 16:26:41 2023, max compression
+gzip compressed data, was "bullmq-1.3.0.tar", last modified: Thu Jun 29 15:32:02 2023, max compression
```

## Comparing `bullmq-1.2.0.tar` & `bullmq-1.3.0.tar`

### file list

```diff
@@ -1,62 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-24 16:26:41.742303 bullmq-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 16:25:13.000000 bullmq-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.734303 bullmq-1.2.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-24 16:26:39.000000 bullmq-1.2.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-24 16:26:09.000000 bullmq-1.2.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-24 16:26:10.000000 bullmq-1.2.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.742303 bullmq-1.2.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-24 16:25:13.000000 bullmq-1.2.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:26:41.734303 bullmq-1.2.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 16:26:41.000000 bullmq-1.2.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-24 16:26:41.742303 bullmq-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-24 16:25:13.000000 bullmq-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:32:02.333591 bullmq-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-29 15:32:02.333591 bullmq-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 15:30:02.000000 bullmq-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:32:02.329591 bullmq-1.3.0/bullmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:32:02.329591 bullmq-1.3.0/bullmq/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-29 15:32:02.000000 bullmq-1.3.0/bullmq/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-29 15:32:02.000000 bullmq-1.3.0/bullmq/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:32:02.000000 bullmq-1.3.0/bullmq/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 15:32:02.000000 bullmq-1.3.0/bullmq/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 15:32:02.000000 bullmq-1.3.0/bullmq/bullmq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:32:02.333591 bullmq-1.3.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 15:30:02.000000 bullmq-1.3.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-29 15:31:59.000000 bullmq-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:32:02.333591 bullmq-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 15:30:02.000000 bullmq-1.3.0/setup.py
```

### Comparing `bullmq-1.2.0/PKG-INFO` & `bullmq-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.2.0
+Version: 1.3.0
 Summary: BullMQ for Python
-Home-page: https://bullmq.io
-Author: Taskforce.sh Inc.
-Author-email: manast@taskforce.sh
-License: MIT
+Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
+Project-URL: Homepage, https://bullmq.io
+Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
+Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bullmq-1.2.0/README.md` & `bullmq-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.2.0/bullmq/types/job_options.py` & `bullmq-1.3.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.2.0/bullmq/types/worker_options.py` & `bullmq-1.3.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.2.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.3.0/bullmq/bullmq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.2.0
+Version: 1.3.0
 Summary: BullMQ for Python
-Home-page: https://bullmq.io
-Author: Taskforce.sh Inc.
-Author-email: manast@taskforce.sh
-License: MIT
+Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
+Project-URL: Homepage, https://bullmq.io
+Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
+Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bullmq-1.2.0/setup.py` & `bullmq-1.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,59 @@
-from setuptools import setup
-from bullmq import __version__
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-# To use a consistent encoding
-from codecs import open
-from os import path
-
-# Get the long description from the README file
-with open(path.join(".", 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='bullmq',
-    version=__version__,
-    description='BullMQ for Python',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://bullmq.io',
-    author='Taskforce.sh Inc.',
-    author_email='manast@taskforce.sh',
-    license='MIT',
-    packages=['bullmq'],
-    package_data={'bullmq': ['commands/*.lua', 'types/*']},
-    install_requires=[
-        'redis',
-        'msgpack',
-        'semver',
-    ],
-    extras_require={
-        "dev": [
-            "pre-commit==3.3.3",
-            "python-semantic-release==7.34.3",
-        ]
-    },
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',  
-        'Operating System :: POSIX :: Linux',        
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-    ],
-)
+[project]
+name = "bullmq"
+version = "1.3.0"
+description='BullMQ for Python'
+readme="README.md"
+authors = [
+    {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
+]
+classifiers=[
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: POSIX :: Linux',
+    'Programming Language :: Python :: 2',
+    'Programming Language :: Python :: 2.7',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.4',
+    'Programming Language :: Python :: 3.5',
+]
+keywords = ["python", "bullmq", "queues"]
+dependencies = [
+    "redis >= 4.5.0, < 5",
+    "msgpack >= 1.0.0, < 2",
+    "semver >= 2.13.0, < 3"
+]
+
+[project.optional-dependencies]
+dev = [
+    "setuptools==63.1.0",
+    "pre-commit==3.3.3",
+    "build==0.8.0",
+    "python-semantic-release==7.28.1",
+    "types-redis==4.5.5.0"
+]
+
+[project.urls]
+"Homepage" = "https://bullmq.io"
+"Bug Tracker" = "https://github.com/taskforcesh/bullmq/issues"
+
+[tool.setuptools.packages.find]
+where = ["bullmq"]
+exclude = ["tests*"]
+
+[tool.setuptools.package-data]
+bullmq = ["commands/*.lua", "types/*"]
+
+[tool.semantic_release]
+branch = "master"
+version_variable = "bullmq/__init__.py:__version__"
+version_toml = "pyproject.toml:project.version"
+build_command = "python3 setup.py sdist"
+tag_format = "vpy{version}"
+version_source = "commit"
+changelog_file = "../docs/gitbook/python/changelog.md"
+upload_to_pypi = true
```

