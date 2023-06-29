# Comparing `tmp/aws-cdk.app-staging-synthesizer-alpha-2.85.0a0.tar.gz` & `tmp/aws-cdk.app-staging-synthesizer-alpha-2.86.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src913890871/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer-", last modified: Wed Jun 21 13:32:27 2023, max compression
+gzip compressed data, was "/codebuild/output/src3755887465/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer", last modified: Thu Jun 29 08:23:47 2023, max compression
```

## Comparing `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0.tar` & `aws-cdk.app-staging-synthesizer-alpha-2.86.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25678 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24658 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1949 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
--rw-r--r--   0 root         (0) root         (0)   186549 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81210 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:18.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:27.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25678 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 13:32:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-29 08:23:39.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 08:23:39.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15372 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14352 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
+-rw-r--r--   0 root         (0) root         (0)   180441 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81882 2023-06-29 08:23:39.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.86.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:40.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15372 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 08:23:47.000000 aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/LICENSE` & `aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/setup.py` & `aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.app-staging-synthesizer-alpha",
-    "version": "2.85.0.a0",
+    "version": "2.86.0.a0",
     "description": "Cdk synthesizer for with app-scoped staging stack",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.app_staging_synthesizer_alpha",
         "aws_cdk.app_staging_synthesizer_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.app_staging_synthesizer_alpha._jsii": [
-            "app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz"
+            "app-staging-synthesizer-alpha@2.86.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.app_staging_synthesizer_alpha": [
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

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py` & `aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,125 +44,67 @@
 
 If you are migrating from a different version of synthesis your updated CDK App will target
 the resources in the `DefaultStagingStack` and no longer be tied to the bootstrapped resources
 in your account.
 
 ## Bootstrap Model
 
-Our current bootstrap model looks like this, when you run `cdk bootstrap aws://<account>/<region>` :
-
-```text
-┌───────────────────────────────────┐┌────────────────────────┐┌────────────────────────┐
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│          ┌───────────────┐        ││    ┌──────────────┐    ││    ┌──────────────┐    │
-│          │Bootstrap Stack│        ││    │  CDK App 1   │    ││    │  CDK App 2   │    │
-│          └───────────────┘        ││    └──────────────┘    ││    └──────────────┘    │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│   ┌───────────────────────────┐   ││     ┌────────────┐     ││                        │
-│   │IAM Role for CFN execution │   ││┌────│  S3 Asset  │     ││                        │
-│   │    IAM Role for lookup    │   │││    └────────────┘     ││                        │
-│   │  IAM Role for deployment  │   │││                       ││                        │
-│   └───────────────────────────┘   │││                       ││     ┌─────────────┐    │
-│                                   │││            ┌──────────┼┼─────│  S3 Asset   │    │
-│                                   │││            │          ││     └─────────────┘    │
-│ ┌───────────────────────────────┐ │││            │          ││                        │
-│ │ IAM Role for File Publishing  │ │││            │          ││                        │
-│ │ IAM Role for Image Publishing │ │││            │          ││                        │
-│ └───────────────────────────────┘ │││            │          ││                        │
-│                                   │││            │          ││                        │
-│  ┌─────────────────────────────┐  │││            │          ││                        │
-│  │S3 Bucket for Staging Assets │  │││            │          ││                        │
-│  │     KMS Key encryption      │◀─┼┼┴────────────┘          ││      ┌────────────┐    │
-│  └─────────────────────────────┘  ││             ┌──────────┼┼───── │ ECR Asset  │    │
-│                                   ││             │          ││      └────────────┘    │
-│                                   ││             │          ││                        │
-│┌─────────────────────────────────┐││             │          ││                        │
-││ECR Repository for Staging Assets◀┼┼─────────────┘          ││                        │
-│└─────────────────────────────────┘││                        ││                        │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-│                                   ││                        ││                        │
-└───────────────────────────────────┘└────────────────────────┘└────────────────────────┘
-```
-
-Your CDK Application utilizes these resources when deploying. For example, if you have a file asset,
-it gets uploaded to the S3 Staging Bucket using the File Publishing Role when you run `cdk deploy`.
-
-This library introduces an alternate model to bootstrapping, by splitting out essential CloudFormation IAM roles
-and staging resources. There will still be a Bootstrap Stack, but this will only contain IAM roles necessary for
-CloudFormation deployment. Each CDK App will instead be in charge of its own staging resources, including the
-S3 Bucket, ECR Repositories, and associated IAM roles. It works like this:
-
-The Staging Stack will contain, on a per-need basis,
-
-* 1 S3 Bucket with KMS encryption for all file assets in the CDK App.
-* An ECR Repository *per* image (and its revisions).
-* IAM roles with access to the Bucket and Repositories.
-
-```text
-┌─────────────────────────────┐┌───────────────────────────────────────┐┌───────────────────────────────────────┐
-│                             ││                                       ││                                       │
-│      ┌───────────────┐      ││             ┌──────────────┐          ││             ┌──────────────┐          │
-│      │Bootstrap Stack│      ││             │  CDK App 1   │          ││             │  CDK App 2   │          │
-│      └───────────────┘      ││             └──────────────┘          ││             └──────────────┘          │
-│                             ││┌──────────────────┐                   ││┌──────────────────┐                   │
-│                             │││ ┌──────────────┐ │                   │││ ┌──────────────┐ │                   │
-│                             │││ │Staging Stack │ │                   │││ │Staging Stack │ │                   │
-│                             │││ └──────────────┘ │                   │││ └──────────────┘ │                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││┌────────────────┐│     ┌────────────┐│││┌────────────────┐│     ┌────────────┐│
-│                             ││││  IAM Role for  ││ ┌───│  S3 Asset  │││││  IAM Role for  ││ ┌───│  S3 Asset  ││
-│                             ││││File Publishing ││ │   └────────────┘││││File Publishing ││ │   └────────────┘│
-│                             │││└────────────────┘│ │                 ││││  IAM Role for  ││ │                 │
-│                             │││                  │ │                 ││││Image Publishing││ │                 │
-│┌───────────────────────────┐│││                  │ │                 │││└────────────────┘│ │                 │
-││IAM Role for CFN execution ││││                  │ │                 │││                  │ │                 │
-││    IAM Role for lookup    ││││                  │ │                 │││                  │ │                 │
-││  IAM Role for deployment  ││││┌────────────────┐│ │                 │││┌────────────────┐│ │                 │
-│└───────────────────────────┘││││ S3 Bucket for  ││ │                 ││││ S3 Bucket for  ││ │                 │
-│                             ││││ Staging Assets │◀─┘                 ││││ Staging Assets │◀─┘                 │
-│                             │││└────────────────┘│                   │││└────────────────┘│      ┌───────────┐│
-│                             │││                  │                   │││                  │  ┌───│ ECR Asset ││
-│                             │││                  │                   │││┌────────────────┐│  │   └───────────┘│
-│                             │││                  │                   ││││ ECR Repository ││  │                │
-│                             │││                  │                   ││││  for Staging   │◀──┘                │
-│                             │││                  │                   ││││     Assets     ││                   │
-│                             │││                  │                   │││└────────────────┘│                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││                  │                   │││                  │                   │
-│                             │││                  │                   │││                  │                   │
-│                             ││└──────────────────┘                   ││└──────────────────┘                   │
-└─────────────────────────────┘└───────────────────────────────────────┘└───────────────────────────────────────┘
-```
-
-This allows staging resources to be created when needed next to the CDK App. It has the following
-benefits:
+In our default bootstrapping process, when you run `cdk bootstrap aws://<account>/<region>`, the following
+resources are created:
 
+* It creates Roles to assume for cross-account deployments and for Pipeline deployments;
+* It creates staging resources: a global S3 bucket and global ECR repository to hold CDK assets;
+* It creates Roles to write to the S3 bucket and ECR repository;
+
+Because the bootstrapping resources include regional resources, you need to bootstrap
+every region you plan to deploy to individually. All assets of all CDK apps deploying
+to that account and region will be written to the single S3 Bucket and ECR repository.
+
+By using the synthesizer in this library, instead of the
+`DefaultStackSynthesizer`, a different set of staging resources will be created
+for every CDK application, and they will be created automatically as part of a
+regular deployment, in a separate Stack that is deployed before your application
+Stacks. The staging resources will be one S3 bucket, and *one ECR repository per
+image*, and Roles necessary to access those buckets and ECR repositories. The
+Roles from the default bootstrap stack are still used (though their use can be
+turned off).
+
+This has the following advantages:
+
+* Because staging resources are now application-specific, they can be fully cleaned up when you clean up
+  the application.
+* Because there is now one ECR repository per image instead of one ECR repository for all images, it is
+  possible to effectively use ECR life cycle rules (for example, retain only the most recent 5 images)
+  to cut down on storage costs.
 * Resources between separate CDK Apps are separated so they can be cleaned up and lifecycle
   controlled individually.
-* Users have a familiar way to customize staging resources in the CDK Application.
+* Because the only shared bootstrapping resources required are Roles, which are global resources,
+  you now only need to bootstrap every account in one Region (instead of every Region). This makes it
+  easier to do with CloudFormation StackSets.
+
+For the deployment roles, this synthesizer still uses the Roles from the default
+bootstrap stack, and nothing else. The staging resources from that bootstrap
+stack will be unused. You can customize the template to remove those resources
+if you prefer.  In the future, we will provide a bootstrap stack template with
+only those Roles, specifically for use with this synthesizer.
 
 ## Using the Default Staging Stack per Environment
 
 The most common use case will be to use the built-in default resources. In this scenario, the
 synthesizer will create a new Staging Stack in each environment the CDK App is deployed to store
 its staging resources. To use this kind of synthesizer, use `AppStagingSynthesizer.defaultResources()`.
 
 ```python
 app = App(
     default_stack_synthesizer=AppStagingSynthesizer.default_resources(
-        app_id="my-app-id"
+        app_id="my-app-id",
+
+        # The following line is optional. By default it is assumed you have bootstrapped in the same
+        # region(s) as the stack(s) you are deploying.
+        deployment_identities=DeploymentIdentities.default_bootstrap_roles(bootstrap_region="us-east-1")
     )
 )
 ```
 
 Every CDK App that uses the `DefaultStagingStack` must include an `appId`. This should
 be an identifier unique to the app and is used to differentiate staging resources associated
 with the app.
@@ -380,23 +322,23 @@
 ```
 
 ## Known Limitations
 
 Since this module is experimental, there are some known limitations:
 
 * Currently this module does not support CDK Pipelines. You must deploy CDK Apps using this
-  synthesizer via `cdk deploy`.
+  synthesizer via `cdk deploy`. Please upvote [this issue](https://github.com/aws/aws-cdk/issues/26118)
+  to indicate you want this.
 * This synthesizer only needs a bootstrap stack with Roles, without staging resources. We
   haven't written such a bootstrap stack yet; at the moment you can use the existing modern
-  bootstrap stack, the staging resources in them will just go unused.
+  bootstrap stack, the staging resources in them will just go unused. You can customize the
+  template to remove them if desired.
 * Due to limitations on the CloudFormation template size, CDK Applications can have
-  at most 38 independent ECR images.
-* When you run `cdk destroy` (for example during testing), the staging bucket and ECR
-  repositories will be left behind because CloudFormation cannot clean up non-empty resources.
-  You must deploy those resources manually if you want to redeploy again using the same `appId`.
+  at most 38 independent ECR images. Please upvote [this issue](https://github.com/aws/aws-cdk/issues/26119)
+  if you need more than this.
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -1183,14 +1125,76 @@
     def __repr__(self) -> str:
         return "CustomResourcesOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="@aws-cdk/app-staging-synthesizer-alpha.DefaultBootstrapRolesOptions",
+    jsii_struct_bases=[],
+    name_mapping={"bootstrap_region": "bootstrapRegion"},
+)
+class DefaultBootstrapRolesOptions:
+    def __init__(
+        self,
+        *,
+        bootstrap_region: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''(experimental) Options for ``DeploymentIdentities.defaultBootstrappedRoles``.
+
+        :param bootstrap_region: (experimental) The region where the default bootstrap roles have been created. By default, the region in which the stack is deployed is used. Default: - the stack's current region
+
+        :stability: experimental
+        :exampleMetadata: infused
+
+        Example::
+
+            app = App(
+                default_stack_synthesizer=AppStagingSynthesizer.default_resources(
+                    app_id="my-app-id",
+            
+                    # The following line is optional. By default it is assumed you have bootstrapped in the same
+                    # region(s) as the stack(s) you are deploying.
+                    deployment_identities=DeploymentIdentities.default_bootstrap_roles(bootstrap_region="us-east-1")
+                )
+            )
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__04df2201aac14a17d1f202664f0ecfab35edb0a3e63061b1cb8c73c369ae2804)
+            check_type(argname="argument bootstrap_region", value=bootstrap_region, expected_type=type_hints["bootstrap_region"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if bootstrap_region is not None:
+            self._values["bootstrap_region"] = bootstrap_region
+
+    @builtins.property
+    def bootstrap_region(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The region where the default bootstrap roles have been created.
+
+        By default, the region in which the stack is deployed is used.
+
+        :default: - the stack's current region
+
+        :stability: experimental
+        '''
+        result = self._values.get("bootstrap_region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DefaultBootstrapRolesOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@aws-cdk/app-staging-synthesizer-alpha.DefaultStagingStackOptions",
     jsii_struct_bases=[],
     name_mapping={
         "app_id": "appId",
         "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
@@ -1864,32 +1868,48 @@
     :exampleMetadata: infused
 
     Example::
 
         app = App(
             default_stack_synthesizer=AppStagingSynthesizer.default_resources(
                 app_id="my-app-id",
-                deployment_identities=DeploymentIdentities.specify_roles(
-                    cloud_formation_execution_role=BootstrapRole.from_role_arn("arn:aws:iam::123456789012:role/Execute"),
-                    deployment_role=BootstrapRole.from_role_arn("arn:aws:iam::123456789012:role/Deploy"),
-                    lookup_role=BootstrapRole.from_role_arn("arn:aws:iam::123456789012:role/Lookup")
-                )
+        
+                # The following line is optional. By default it is assumed you have bootstrapped in the same
+                # region(s) as the stack(s) you are deploying.
+                deployment_identities=DeploymentIdentities.default_bootstrap_roles(bootstrap_region="us-east-1")
             )
         )
     '''
 
     @jsii.member(jsii_name="cliCredentials")
     @builtins.classmethod
     def cli_credentials(cls) -> "DeploymentIdentities":
         '''(experimental) Use CLI credentials for all deployment identities.
 
         :stability: experimental
         '''
         return typing.cast("DeploymentIdentities", jsii.sinvoke(cls, "cliCredentials", []))
 
+    @jsii.member(jsii_name="defaultBootstrapRoles")
+    @builtins.classmethod
+    def default_bootstrap_roles(
+        cls,
+        *,
+        bootstrap_region: typing.Optional[builtins.str] = None,
+    ) -> "DeploymentIdentities":
+        '''(experimental) Use the Roles that have been created by the default bootstrap stack.
+
+        :param bootstrap_region: (experimental) The region where the default bootstrap roles have been created. By default, the region in which the stack is deployed is used. Default: - the stack's current region
+
+        :stability: experimental
+        '''
+        options = DefaultBootstrapRolesOptions(bootstrap_region=bootstrap_region)
+
+        return typing.cast("DeploymentIdentities", jsii.sinvoke(cls, "defaultBootstrapRoles", [options]))
+
     @jsii.member(jsii_name="specifyRoles")
     @builtins.classmethod
     def specify_roles(
         cls,
         *,
         cloud_formation_execution_role: typing.Optional[BootstrapRole] = None,
         deployment_role: typing.Optional[BootstrapRole] = None,
@@ -1911,21 +1931,41 @@
             deployment_role=deployment_role,
             lookup_role=lookup_role,
         )
 
         return typing.cast("DeploymentIdentities", jsii.sinvoke(cls, "specifyRoles", [roles]))
 
     @builtins.property
-    @jsii.member(jsii_name="roles")
-    def roles(self) -> BootstrapRoles:
-        '''(experimental) roles that are bootstrapped to your account.
+    @jsii.member(jsii_name="cloudFormationExecutionRole")
+    def cloud_formation_execution_role(self) -> typing.Optional[BootstrapRole]:
+        '''(experimental) CloudFormation Execution Role.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[BootstrapRole], jsii.get(self, "cloudFormationExecutionRole"))
+
+    @builtins.property
+    @jsii.member(jsii_name="deploymentRole")
+    def deployment_role(self) -> typing.Optional[BootstrapRole]:
+        '''(experimental) Deployment Action Role.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[BootstrapRole], jsii.get(self, "deploymentRole"))
+
+    @builtins.property
+    @jsii.member(jsii_name="lookupRole")
+    def lookup_role(self) -> typing.Optional[BootstrapRole]:
+        '''(experimental) Lookup Role.
+
+        :default: - use bootstrapped role
 
         :stability: experimental
         '''
-        return typing.cast(BootstrapRoles, jsii.get(self, "roles"))
+        return typing.cast(typing.Optional[BootstrapRole], jsii.get(self, "lookupRole"))
 
 
 @jsii.data_type(
     jsii_type="@aws-cdk/app-staging-synthesizer-alpha.FileStagingLocation",
     jsii_struct_bases=[],
     name_mapping={
         "bucket_name": "bucketName",
@@ -3091,14 +3131,15 @@
 __all__ = [
     "AppStagingSynthesizer",
     "AppStagingSynthesizerOptions",
     "BootstrapRole",
     "BootstrapRoles",
     "CustomFactoryOptions",
     "CustomResourcesOptions",
+    "DefaultBootstrapRolesOptions",
     "DefaultResourcesOptions",
     "DefaultStagingStack",
     "DefaultStagingStackOptions",
     "DefaultStagingStackProps",
     "DeploymentIdentities",
     "FileStagingLocation",
     "IStagingResources",
@@ -3167,14 +3208,21 @@
     bootstrap_qualifier: typing.Optional[builtins.str] = None,
     deployment_identities: typing.Optional[DeploymentIdentities] = None,
     resources: IStagingResources,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__04df2201aac14a17d1f202664f0ecfab35edb0a3e63061b1cb8c73c369ae2804(
+    *,
+    bootstrap_region: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__09dbc6ce5bcfd58fa48337caac574e10727d4bf9a43dc89866fbe7541b026219(
     *,
     app_id: builtins.str,
     auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.85.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt` & `aws-cdk.app-staging-synthesizer-alpha-2.86.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
 src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
 src/aws_cdk/app_staging_synthesizer_alpha/py.typed
 src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
-src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.85.0-alpha.0.jsii.tgz
+src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.86.0-alpha.0.jsii.tgz
```

