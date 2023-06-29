# Comparing `tmp/tutor-jupyter-16.0.0.tar.gz` & `tmp/tutor-jupyter-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-jupyter-16.0.0.tar", last modified: Thu Jun 15 08:46:19 2023, max compression
+gzip compressed data, was "tutor-jupyter-16.0.1.tar", last modified: Thu Jun 29 13:48:53 2023, max compression
```

## Comparing `tutor-jupyter-16.0.0.tar` & `tutor-jupyter-16.0.1.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.647487 tutor-jupyter-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 08:46:19.647487 tutor-jupyter-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.640820 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-06-15 08:46:19.000000 tutor-jupyter-16.0.0/tutor_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.640820 tutor-jupyter-16.0.0/tutorjupyter/
--rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/dev-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.634153 tutor-jupyter-16.0.0/tutorjupyter/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.637487 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/hub/
--rw-r--r--   0 ci        (1000) ci        (1000)      410 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/
--rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.637487 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:19.644153 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-06-15 08:46:14.000000 tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6077 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5164 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1786 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.742634 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6077 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1304 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-06-29 13:48:53.000000 tutor-jupyter-16.0.1/tutor_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.742634 tutor-jupyter-16.0.1/tutorjupyter/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.745968 tutor-jupyter-16.0.1/tutorjupyter/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/dev-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     1662 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      558 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      253 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      149 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      490 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.735967 tutor-jupyter-16.0.1/tutorjupyter/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.739301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.745968 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/apps/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)     5088 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/hub/
+-rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/hub/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/lab/
+-rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/lab/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.739301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:53.749301 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/init/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-06-29 13:48:48.000000 tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
```

### Comparing `tutor-jupyter-16.0.0/LICENSE.txt` & `tutor-jupyter-16.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-16.0.0/PKG-INFO` & `tutor-jupyter-16.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 16.0.0
+Version: 16.0.1
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-jupyter/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 This is a plugin for Tutor that makes it easy to integrate `Jupyter <https://jupyter.org/>`__ notebooks in `Open edX <https://openedx.org>`__. It achieves the following:
 
 1. Install the official `jupyter-xblock <https://github.com/overhangio/jupyter-xblock/>`__ in the Open edX LMS and Studio.
 2. Run a Docker-based `JupyterHub <https://jupyterhub.readthedocs.io/en/stable/>`__ instance with a `Docker spawner <https://jupyterhub-dockerspawner.readthedocs.io/en/latest/>`__.
 
 In pratice, it means that students will be allocated Docker containers with limited CPU and memory to run their custom notebooks.
 
-⚠️ This plugin is not compatible with Kubernetes. If you wish to run JupyterHub on Kubernetes, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
+⚠️ Compatibility with Kubernetes was not battle-tested. Please report any issue you face. For a more production-ready Kubernetes environment, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
 
 Installation
 ------------
 
 ::
 
     tutor plugins install jupyter
```

### Comparing `tutor-jupyter-16.0.0/README.rst` & `tutor-jupyter-16.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This is a plugin for Tutor that makes it easy to integrate `Jupyter <https://jupyter.org/>`__ notebooks in `Open edX <https://openedx.org>`__. It achieves the following:
 
 1. Install the official `jupyter-xblock <https://github.com/overhangio/jupyter-xblock/>`__ in the Open edX LMS and Studio.
 2. Run a Docker-based `JupyterHub <https://jupyterhub.readthedocs.io/en/stable/>`__ instance with a `Docker spawner <https://jupyterhub-dockerspawner.readthedocs.io/en/latest/>`__.
 
 In pratice, it means that students will be allocated Docker containers with limited CPU and memory to run their custom notebooks.
 
-⚠️ This plugin is not compatible with Kubernetes. If you wish to run JupyterHub on Kubernetes, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
+⚠️ Compatibility with Kubernetes was not battle-tested. Please report any issue you face. For a more production-ready Kubernetes environment, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
 
 Installation
 ------------
 
 ::
 
     tutor plugins install jupyter
```

### Comparing `tutor-jupyter-16.0.0/setup.py` & `tutor-jupyter-16.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     install_requires=["tutor>=16.0.0,<17.0.0", "tutor-mfe>=16.0.0,<17.0.0"],
     entry_points={
         "tutor.plugin.v1": [
             "jupyter = tutorjupyter.plugin"
         ]
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `tutor-jupyter-16.0.0/tutor_jupyter.egg-info/PKG-INFO` & `tutor-jupyter-16.0.1/tutor_jupyter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 16.0.0
+Version: 16.0.1
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-jupyter/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 This is a plugin for Tutor that makes it easy to integrate `Jupyter <https://jupyter.org/>`__ notebooks in `Open edX <https://openedx.org>`__. It achieves the following:
 
 1. Install the official `jupyter-xblock <https://github.com/overhangio/jupyter-xblock/>`__ in the Open edX LMS and Studio.
 2. Run a Docker-based `JupyterHub <https://jupyterhub.readthedocs.io/en/stable/>`__ instance with a `Docker spawner <https://jupyterhub-dockerspawner.readthedocs.io/en/latest/>`__.
 
 In pratice, it means that students will be allocated Docker containers with limited CPU and memory to run their custom notebooks.
 
-⚠️ This plugin is not compatible with Kubernetes. If you wish to run JupyterHub on Kubernetes, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
+⚠️ Compatibility with Kubernetes was not battle-tested. Please report any issue you face. For a more production-ready Kubernetes environment, you are encouraged to check the documentation of the `Zero to JupyterHub with Kubernetes <https://z2jh.jupyter.org/en/stable/resources/reference.html>`__ project.
 
 Installation
 ------------
 
 ::
 
     tutor plugins install jupyter
```

### Comparing `tutor-jupyter-16.0.0/tutor_jupyter.egg-info/SOURCES.txt` & `tutor-jupyter-16.0.1/tutor_jupyter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 tutor_jupyter.egg-info/top_level.txt
 tutorjupyter/__about__.py
 tutorjupyter/__init__.py
 tutorjupyter/plugin.py
 tutorjupyter/patches/.gitignore
 tutorjupyter/patches/caddyfile
 tutorjupyter/patches/dev-docker-compose-services
+tutorjupyter/patches/k8s-deployments
+tutorjupyter/patches/k8s-jobs
+tutorjupyter/patches/k8s-services
+tutorjupyter/patches/kustomization-configmapgenerator
 tutorjupyter/patches/local-docker-compose-jobs-services
 tutorjupyter/patches/local-docker-compose-services
 tutorjupyter/patches/openedx-common-settings
 tutorjupyter/patches/openedx-dockerfile-post-python-requirements
 tutorjupyter/templates/jupyter/apps/.gitignore
 tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
 tutorjupyter/templates/jupyter/build/.gitignore
```

### Comparing `tutor-jupyter-16.0.0/tutorjupyter/plugin.py` & `tutor-jupyter-16.0.1/tutorjupyter/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py` & `tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 c.JupyterHub.port = 9045
 # Internal IP and port that spawners connect to
 c.JupyterHub.hub_ip = "0.0.0.0"
 c.JupyterHub.hub_port = 8081
 # Database
 c.JupyterHub.db_url = "mysql+pymysql://{{ JUPYTER_HUB_MYSQL_USERNAME }}:{{ JUPYTER_HUB_MYSQL_PASSWORD }}@{{ MYSQL_HOST }}:{{ MYSQL_PORT }}/{{ JUPYTER_HUB_MYSQL_DATABASE }}"
 c.JupyterHub.cookie_secret = "{{ JUPYTER_HUB_COOKIE_SECRET }}"
+# Don't write pid file to current folder, where we may not have write access
+c.ConfigurableHTTPProxy.pid_file = "/tmp/jupyter-proxy.pid"
 
 # Authorise embedding in some iframes.
 # Add "*" to allow embedding in all iframes (though it's dangerous and you probably
 # shouldn't do it).
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy/frame-ancestors
 frame_ancestors = [
     "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}",
@@ -65,30 +67,42 @@
 # c.LTI13Authenticator.endpoint: "http://localhost:8000/hub/oauth_callback"
 # c.LTI13Authenticator.token_url: "https://canvas.instructure.com/login/oauth2/token"
 
 # nbgitpuller
 c.ServerApp.nbserver_extensions = {"nbgitpuller": True}
 
 # Spawner
-
-# Run as Docker containers
-# https://jupyterhub-dockerspawner.readthedocs.io/en/latest/api/index.html
-c.JupyterHub.spawner_class = "dockerspawner.DockerSpawner"
-c.DockerSpawner.image = "{{ JUPYTER_DOCKER_IMAGE_LAB }}"
-c.DockerSpawner.debug = True
-c.DockerSpawner.remove = True
-c.DockerSpawner.use_internal_ip = True
-c.DockerSpawner.network_name = os.environ.get("NETWORK_NAME")
-c.DockerSpawner.environment = {"CONTENT_SECURITY_POLICY": content_security_policy}
-# Persist user data: this will create a new "jupyterhub-user-{username}" named volume on
-# the host for every Docker container.
-# https://jupyterhub-dockerspawner.readthedocs.io/en/latest/data-persistence.html
-notebook_dir = "/home/jovyan/work"
-c.DockerSpawner.notebook_dir = notebook_dir
-c.DockerSpawner.volumes = {"jupyterhub-user-{username}": notebook_dir}
 # Limit spawner cpu and memory
 {% if JUPYTER_LAB_CPU_LIMIT %}
 c.Spawner.cpu_limit = {{ JUPYTER_LAB_CPU_LIMIT }}
 {% endif %}
 c.Spawner.mem_limit = "{{ JUPYTER_LAB_MEMORY_LIMIT }}"
 
+if os.environ.get("SPAWNER") == "docker":
+    # Run as Docker containers
+    # https://jupyterhub-dockerspawner.readthedocs.io/en/latest/api/index.html
+    c.JupyterHub.spawner_class = "dockerspawner.DockerSpawner"
+    c.DockerSpawner.image = "{{ JUPYTER_DOCKER_IMAGE_LAB }}"
+    c.DockerSpawner.debug = True
+    c.DockerSpawner.remove = True
+    c.DockerSpawner.use_internal_ip = True
+    c.DockerSpawner.network_name = os.environ.get("NETWORK_NAME")
+    c.DockerSpawner.environment = {"CONTENT_SECURITY_POLICY": content_security_policy}
+    # Persist user data: this will create a new "jupyterhub-user-{username}" named volume on
+    # the host for every Docker container.
+    # https://jupyterhub-dockerspawner.readthedocs.io/en/latest/data-persistence.html
+    c.DockerSpawner.notebook_dir = "/home/jovyan/work"
+    c.DockerSpawner.volumes = {"jupyterhub-user-{username}": c.DockerSpawner.notebook_dir}
+elif os.environ.get("SPAWNER") == "kubernetes":
+    # Run as kubernetes pods
+    # https://jupyterhub-kubespawner.readthedocs.io/en/latest/spawner.html
+    # https://z2jh.jupyter.org/en/stable/resources/reference.html#helm-chart-configuration-reference
+    # spoiler: you're in for one hell of a ride...
+    c.JupyterHub.spawner_class = "kubespawner.KubeSpawner"
+    c.KubeSpawner.debug = True
+    c.KubeSpawner.hub_connect_url = "http://jupyterhub:8081"
+    # c.KubeSpawner.port = 8081
+    c.KubeSpawner.service_account = "jupyterhub"
+    c.KubeSpawner.image = "{{ JUPYTER_DOCKER_IMAGE_LAB }}"
+    c.KubeSpawner.environment = {"CONTENT_SECURITY_POLICY": content_security_policy}
+
 {{ patch("jupyterhub-config") }}
```

### Comparing `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile` & `tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-16.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh` & `tutor-jupyter-16.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh`

 * *Files identical despite different names*

