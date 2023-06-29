# Comparing `tmp/cirq-1.2.0.dev20230628175157-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230629173323-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8377 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/LICENSE
--rw-r--r--  2.0 unx     7834 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jun-28 17:52 cirq-1.2.0.dev20230628175157.dist-info/RECORD
-6 files, 20139 bytes uncompressed, 7339 bytes compressed:  63.6%
+Zip file size: 8391 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7850 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jun-29 17:33 cirq-1.2.0.dev20230629173323.dist-info/RECORD
+6 files, 20155 bytes uncompressed, 7353 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.2.0.dev20230628175157.dist-info/AUTHORS
+Filename: cirq-1.2.0.dev20230629173323.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.2.0.dev20230628175157.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230629173323.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230628175157.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230629173323.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230628175157.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230629173323.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230628175157.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230629173323.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230628175157.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230629173323.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230628175157.dist-info/LICENSE` & `cirq-1.2.0.dev20230629173323.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230628175157.dist-info/METADATA` & `cirq-1.2.0.dev20230629173323.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230628175157
+Version: 1.2.0.dev20230629173323
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
-Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-core (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-ft (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-google (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230628175157)
-Requires-Dist: cirq-web (==1.2.0.dev20230628175157)
+Requires-Python: >=3.9.0
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: cirq-aqt (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-core (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-ft (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-google (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230629173323)
+Requires-Dist: cirq-web (==1.2.0.dev20230629173323)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
@@ -31,30 +33,30 @@
 Requires-Dist: pytest-xdist (~=2.2.0) ; extra == 'dev_env'
 Requires-Dist: filelock (~=3.0.12) ; extra == 'dev_env'
 Requires-Dist: freezegun (~=0.3.15) ; extra == 'dev_env'
 Requires-Dist: importlib-metadata ; extra == 'dev_env'
 Requires-Dist: virtualenv ; extra == 'dev_env'
 Requires-Dist: virtualenv-clone ; extra == 'dev_env'
 Requires-Dist: flynt (~=0.60) ; extra == 'dev_env'
-Requires-Dist: black (==22.3.0) ; extra == 'dev_env'
+Requires-Dist: black (==23.3.0) ; extra == 'dev_env'
 Requires-Dist: pylint (~=2.13.0) ; extra == 'dev_env'
 Requires-Dist: grpcio-tools (~=1.37.0) ; extra == 'dev_env'
 Requires-Dist: mypy-protobuf (==1.10) ; extra == 'dev_env'
 Requires-Dist: ipython (>=7.34.0) ; extra == 'dev_env'
 Requires-Dist: notebook (<=6.4.7,>=6.4.1) ; extra == 'dev_env'
 Requires-Dist: ipykernel (==5.3.4) ; extra == 'dev_env'
 Requires-Dist: papermill (~=2.3.2) ; extra == 'dev_env'
 Requires-Dist: seaborn (~=0.11.1) ; extra == 'dev_env'
 Requires-Dist: setuptools ; extra == 'dev_env'
 Requires-Dist: wheel ; extra == 'dev_env'
 Requires-Dist: twine ; extra == 'dev_env'
 Requires-Dist: asv ; extra == 'dev_env'
 Requires-Dist: qiskit-aer (~=0.10.4) ; extra == 'dev_env'
 Requires-Dist: rstcheck (~=3.3.1) ; extra == 'dev_env'
-Requires-Dist: codeowners ; (python_version >= "3.7" and platform_system != "Windows") and extra == 'dev_env'
+Requires-Dist: codeowners ; (platform_system != "Windows") and extra == 'dev_env'
 
 **This is a development version of Cirq and may be unstable.**
 
 **For the latest stable release of Cirq see**
 `here <https://pypi.org/project/cirq>`__.
 
 .. image:: https://raw.githubusercontent.com/quantumlib/Cirq/master/docs/images/Cirq_logo_color.png
```

## Comparing `cirq-1.2.0.dev20230628175157.dist-info/RECORD` & `cirq-1.2.0.dev20230629173323.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-cirq-1.2.0.dev20230628175157.dist-info/AUTHORS,sha256=FyiF0gaNIILE_9q7HDCtKOsTlwNwu0qsTbOAXF67F9A,292
-cirq-1.2.0.dev20230628175157.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-cirq-1.2.0.dev20230628175157.dist-info/METADATA,sha256=6I73u6QrGerte6Etcg7t7jgJ2QM2gavhkBiC9-XnoIk,7834
-cirq-1.2.0.dev20230628175157.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cirq-1.2.0.dev20230628175157.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-cirq-1.2.0.dev20230628175157.dist-info/RECORD,,
+cirq-1.2.0.dev20230629173323.dist-info/AUTHORS,sha256=FyiF0gaNIILE_9q7HDCtKOsTlwNwu0qsTbOAXF67F9A,292
+cirq-1.2.0.dev20230629173323.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+cirq-1.2.0.dev20230629173323.dist-info/METADATA,sha256=iGDsqXddFCt3wpfURBQb44RWW66wrAcZTMuyZpjwyWA,7850
+cirq-1.2.0.dev20230629173323.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cirq-1.2.0.dev20230629173323.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+cirq-1.2.0.dev20230629173323.dist-info/RECORD,,
```

