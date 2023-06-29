# Comparing `tmp/aws-cdk.aws-scheduler-alpha-2.85.0a0.tar.gz` & `tmp/aws-cdk.aws-scheduler-alpha-2.86.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.85.0a0.tar", last modified: Wed Jun 21 13:32:06 2023, max compression
+gzip compressed data, was "/codebuild/output/src3755887465/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.86.0a0.tar", last modified: Thu Jun 29 08:23:31 2023, max compression
```

## Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0.tar` & `aws-cdk.aws-scheduler-alpha-2.86.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8262 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7255 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/
--rw-r--r--   0 root         (0) root         (0)    22132 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25662 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.85.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:00.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8262 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:06.000000 aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7255 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/
+-rw-r--r--   0 root         (0) root         (0)    22132 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25662 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:25.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 08:23:31.000000 aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/LICENSE` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.85.0a0
+Version: 2.86.0a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/README.md` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/setup.py` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-scheduler-alpha",
-    "version": "2.85.0.a0",
+    "version": "2.86.0.a0",
     "description": "The CDK Construct Library for Amazon Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_scheduler_alpha",
         "aws_cdk.aws_scheduler_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_scheduler_alpha._jsii": [
-            "aws-scheduler-alpha@2.85.0-alpha.0.jsii.tgz"
+            "aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_scheduler_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.85.0",
+        "aws-cdk-lib==2.86.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.85.0-alpha.0.jsii.tgz` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz`

 * *Files 2% similar despite different names*

#### Comparing `aws-scheduler-alpha@2.85.0-alpha.0.jsii.tgz-content` & `aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9652777777777778%*

 * *Differences: {"'dependencies'": "{'aws-cdk-lib': '2.86.0'}", "'version'": "'2.86.0-alpha.0'"}*

```diff
@@ -4,15 +4,15 @@
         "organization": true,
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "dependencies": {
-        "aws-cdk-lib": "2.85.0",
+        "aws-cdk-lib": "2.86.0",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
                     "namespace": "Amazon.CDK.Asset.AwsCliV1",
@@ -3780,9 +3780,9 @@
                         "fqn": "aws-cdk-lib.TimeZone"
                     }
                 }
             ],
             "symbolId": "lib/schedule-expression:ScheduleExpression"
         }
     },
-    "version": "2.85.0-alpha.0"
+    "version": "2.86.0-alpha.0"
 }
```

##### package/lib/schedule-expression.js

###### js-beautify {}

```diff
@@ -71,15 +71,15 @@
         return new LiteralScheduleExpression(schedule.expressionString, timeZone);
     }
     constructor() {}
 }
 _a = JSII_RTTI_SYMBOL_1;
 ScheduleExpression[_a] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.ScheduleExpression",
-    version: "2.85.0-alpha.0"
+    version: "2.86.0-alpha.0"
 };
 exports.ScheduleExpression = ScheduleExpression;
 const DEFAULT_TIMEZONE = core_1.TimeZone.ETC_UTC;
 class LiteralScheduleExpression extends ScheduleExpression {
     constructor(expressionString, timeZone = DEFAULT_TIMEZONE) {
         super();
         this.expressionString = expressionString;
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9650621118012421%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.86.0-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.86.0-alpha.0', '@aws-cdk/cfn2ts': '2.86.0-alpha.0', '@aws-cdk/pkglint': "*

 * *                      "'2.86.0-alpha.0', 'aws-cdk-lib': '2.86.0'}",*

 * * "'peerDependencies'": "{'aws-cdk-lib': '2.86.0'}",*

 * * "'version'": "'2.86.0-alpha.0'"}*

```diff
@@ -16,20 +16,20 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "The CDK Construct Library for Amazon Scheduler",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.85.0-alpha.0",
-        "@aws-cdk/cfn2ts": "2.85.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.85.0-alpha.0",
-        "@aws-cdk/pkglint": "2.85.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.86.0-alpha.0",
+        "@aws-cdk/cfn2ts": "2.86.0-alpha.0",
+        "@aws-cdk/integ-runner": "2.86.0-alpha.0",
+        "@aws-cdk/pkglint": "2.86.0-alpha.0",
         "@types/jest": "^29.5.1",
-        "aws-cdk-lib": "2.85.0",
+        "aws-cdk-lib": "2.86.0",
         "constructs": "^10.0.0"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
     "homepage": "https://github.com/aws/aws-cdk",
     "jsii": {
@@ -76,15 +76,15 @@
         "aws-scheduler"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-scheduler-alpha",
     "peerDependencies": {
-        "aws-cdk-lib": "2.85.0",
+        "aws-cdk-lib": "2.86.0",
         "constructs": "^10.0.0"
     },
     "pkglint": {
         "exclude": [
             "naming/package-matches-directory",
             "assert/assert-dependency"
         ]
@@ -111,9 +111,9 @@
         "pkglint": "pkglint -f",
         "rosetta:extract": "yarn --silent jsii-rosetta extract",
         "test": "cdk-test",
         "watch": "cdk-watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "2.85.0-alpha.0"
+    "version": "2.86.0-alpha.0"
 }
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.85.0a0
+Version: 2.86.0a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.85.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-scheduler-alpha-2.86.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_scheduler_alpha/__init__.py
 src/aws_cdk/aws_scheduler_alpha/py.typed
 src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
-src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.85.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.86.0-alpha.0.jsii.tgz
```

