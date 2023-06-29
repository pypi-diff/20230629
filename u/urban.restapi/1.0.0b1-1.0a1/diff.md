# Comparing `tmp/urban.restapi-1.0.0b1.tar.gz` & `tmp/urban.restapi-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urban.restapi-1.0.0b1.tar", last modified: Thu Jun 29 12:05:32 2023, max compression
+gzip compressed data, was "dist/urban.restapi-1.0a1.tar", last modified: Wed Apr  5 08:44:33 2023, max compression
```

## Comparing `urban.restapi-1.0.0b1.tar` & `urban.restapi-1.0a1.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1926 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/.gitlab-ci.yml
--rw-r--r--   0 mpeeters   (501) staff       (20)      682 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/.travis.yml
--rw-r--r--   0 mpeeters   (501) staff       (20)      334 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/CHANGES.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       70 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/CONTRIBUTORS.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)      297 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/DEVELOP.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/LICENSE.GPL
--rw-r--r--   0 mpeeters   (501) staff       (20)      659 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/LICENSE.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)      104 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/MANIFEST.in
--rw-r--r--   0 mpeeters   (501) staff       (20)     3286 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     1406 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/README.rst
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/docs/
--rw-r--r--   0 mpeeters   (501) staff       (20)       62 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/docs/index.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       39 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/requirements.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      321 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/setup.cfg
--rw-r--r--   0 mpeeters   (501) staff       (20)     1911 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/setup.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/
--rw-r--r--   0 mpeeters   (501) staff       (20)       80 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/
--rw-r--r--   0 mpeeters   (501) staff       (20)      130 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1214 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      569 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/exceptions.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      262 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/interfaces.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/
--rw-r--r--   0 mpeeters   (501) staff       (20)      611 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/README.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/en/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 mpeeters   (501) staff       (20)       28 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/en/LC_MESSAGES/urban.restapi.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/en/LC_MESSAGES/urban.restapi.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     1571 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/update.py
--rwxr-xr-x   0 mpeeters   (501) staff       (20)      476 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/update.sh
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/locales/urban.restapi.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)      260 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/permissions.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/
--rw-r--r--   0 mpeeters   (501) staff       (20)      165 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/browserlayer.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      105 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/catalog.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      195 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)       85 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/registry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      118 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/default/rolemap.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/uninstall/
--rw-r--r--   0 mpeeters   (501) staff       (20)      123 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      205 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/address/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/address/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1380 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/address/base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      367 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/address/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      333 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/elements/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/elements/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    19181 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/elements/base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      371 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/elements/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1593 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      618 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)    12695 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/envclassthree.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    11428 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      267 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/buildlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      280 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/codt_buildlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      292 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/codt_parceloutlicence.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1454 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      356 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/envclassthree.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      489 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/environment_base.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/parcel/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/parcel/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1472 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/parcel/base.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      366 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/parcel/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4175 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/services/content/utils.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      614 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/setuphandlers.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1560 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/testing.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/robot/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1983 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/robot/test_example.robot
--rw-r--r--   0 mpeeters   (501) staff       (20)      869 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/test_robot.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2038 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/tests/test_setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      205 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/upgrades.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      382 2023-06-29 12:05:31.000000 urban.restapi-1.0.0b1/src/urban/restapi/upgrades.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/
--rw-r--r--   0 mpeeters   (501) staff       (20)     3286 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     2977 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/SOURCES.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/dependency_links.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      138 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/entry_points.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        6 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/namespace_packages.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/not-zip-safe
--rw-r--r--   0 mpeeters   (501) staff       (20)      124 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/requires.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        6 2023-06-29 12:05:32.000000 urban.restapi-1.0.0b1/src/urban.restapi.egg-info/top_level.txt
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/docs/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       62 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/docs/index.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      659 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/LICENSE.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      682 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/.travis.yml
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      124 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/requires.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2940 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        6 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        6 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      138 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2919 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban.restapi.egg-info/SOURCES.txt
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      333 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/configure.zcml
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/elements/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      371 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/elements/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/elements/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    19181 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/elements/base.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/address/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      367 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/address/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/address/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      950 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/address/base.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/parcel/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      366 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/parcel/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/parcel/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1472 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/parcel/base.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3852 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/utils.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/__init__.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/esb/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      618 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/esb/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    12695 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/esb/envclassthree.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/esb/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1593 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/esb/base.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1281 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      489 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/environment_base.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      292 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/codt_parceloutlicence.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      356 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/envclassthree.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    10808 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/base.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      280 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/codt_buildlicence.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      267 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/content/licence/buildlicence.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      205 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/services/__init__.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/tests/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      869 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/tests/test_robot.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/tests/robot/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1983 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/tests/robot/test_example.robot
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/tests/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2038 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/tests/test_setup.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      260 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/permissions.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      262 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/interfaces.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/locales/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1571 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/update.py
+-rwxrwxr-x   0 fngaha    (1000) fngaha    (1000)      476 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/update.sh
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/locales/en/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/en/LC_MESSAGES/urban.restapi.po
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/urban.restapi.pot
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      611 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/README.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/locales/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1214 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/configure.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      614 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/setuphandlers.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      382 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/upgrades.zcml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      569 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/exceptions.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1560 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/testing.py
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      165 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      105 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      118 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       85 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/registry.xml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      195 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/default/metadata.xml
+drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/uninstall/
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      123 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      130 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      205 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/restapi/upgrades.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       80 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/src/urban/__init__.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2940 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/PKG-INFO
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      321 2023-04-05 08:44:33.000000 urban.restapi-1.0a1/setup.cfg
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1909 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/setup.py
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      297 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/DEVELOP.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       70 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/CONTRIBUTORS.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      104 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/MANIFEST.in
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       94 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/CHANGES.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       39 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/requirements.txt
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1406 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/README.rst
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1926 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/.gitlab-ci.yml
+-rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    18092 2023-04-05 08:44:32.000000 urban.restapi-1.0a1/LICENSE.GPL
```

### Comparing `urban.restapi-1.0.0b1/.gitlab-ci.yml` & `urban.restapi-1.0a1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/.travis.yml` & `urban.restapi-1.0a1/.travis.yml`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/LICENSE.GPL` & `urban.restapi-1.0a1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/LICENSE.rst` & `urban.restapi-1.0a1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/PKG-INFO` & `urban.restapi-1.0a1/src/urban.restapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urban.restapi
-Version: 1.0.0b1
+Version: 1.0a1
 Summary: specific urban restapi for interoperability
 Home-page: https://pypi.python.org/pypi/urban.restapi
 Author: Julien Jaumotte
 Author-email: julien.jaumotte@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -86,27 +86,14 @@
         - Julien Jaumotte, julien.jaumotte@imio.be
         
         
         Changelog
         =========
         
         
-        1.0.0b1 (2023-06-29)
-        --------------------
-        
-        - Fix POST endpoint for event creation [URB-2730]
-          [jchandelle]
-        
-        - Add utils for getting config object from a path
-          [jchandelle]
-        
-        - Fix address query with parenthesis [URB-2696]
-          [jchandelle]
-        
-        
         1.0a1 (2023-04-05)
         ------------------
         
         - Initial release.
           [jjaumotte]
         
 Keywords: Python Plone
```

### Comparing `urban.restapi-1.0.0b1/README.rst` & `urban.restapi-1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/setup.py` & `urban.restapi-1.0a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='urban.restapi',
-    version='1.0.0b1',
+    version='1.0a1',
     description="specific urban restapi for interoperability",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/configure.zcml` & `urban.restapi-1.0a1/src/urban/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/exceptions.py` & `urban.restapi-1.0a1/src/urban/restapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/locales/README.rst` & `urban.restapi-1.0a1/src/urban/restapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/locales/update.py` & `urban.restapi-1.0a1/src/urban/restapi/locales/update.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/elements/base.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/elements/base.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/base.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/esb/base.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/configure.zcml` & `urban.restapi-1.0a1/src/urban/restapi/services/content/esb/configure.zcml`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/esb/envclassthree.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/esb/envclassthree.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/base.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/licence/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from imio.restapi.services import add
 
 from plone import api
 
 from plone.restapi.deserializer import json_body
 
 from urban.restapi.exceptions import UndefinedPortalType, DefaultFolderManagerNotFoundError
-from urban.restapi.services.content.utils import get_config_object
 
 from Products.urban.utils import getLicenceFolder
 
 import json
 
 
 class AddLicencePost(add.FolderPost):
@@ -207,25 +206,7 @@
             data['description'] = {}
         if 'data' not in data['description']:
             data['description']['data'] = ""
         if 'content-type' not in data['description']:
             data['description']['content-type'] = "text/html"
 
         return data
-
-
-class AddLicenceChildPost(add.FolderPost):
-    def prepare_data(self, data):
-        data = super(AddLicenceChildPost, self).prepare_data(data)
-
-        if u"urbaneventtypes" in data:
-            try:
-                config = get_config_object(
-                    "{0}/eventconfigs/{1}".format(
-                        self.context.portal_type.lower(), data["urbaneventtypes"]
-                    )
-                )
-                data["urbaneventtypes"] = config.UID()
-            except KeyError:
-                return data
-
-        return data
```

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/licence/configure.zcml` & `urban.restapi-1.0a1/src/urban/restapi/services/content/licence/configure.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -39,15 +39,8 @@
     method="POST"
     name="@codt_parceloutlicence"
     for="Products.CMFPlone.interfaces.siteroot.IPloneSiteRoot"
     factory=".codt_parceloutlicence.AddCodtParcelOutLicencePost"
     permission="cmf.AddPortalContent"
     />
 
-  <plone:service
-    method="POST"
-    for="Products.urban.interfaces.IGenericLicence"
-    factory=".base.AddLicenceChildPost"
-    permission="cmf.AddPortalContent"
-    />
-
 </configure>
```

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/parcel/base.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/parcel/base.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/services/content/utils.py` & `urban.restapi-1.0a1/src/urban/restapi/services/content/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,20 +104,7 @@
         returned_value = method(self, *args, **kwargs)
         self._benchmark[method.__name__]['elapsed_time'] += time.time() - start_time
         self._benchmark[method.__name__]['average_time'] = \
             self._benchmark[method.__name__]['elapsed_time'] / self._benchmark[method.__name__]['counter']
         return returned_value
 
     return replacement
-
-
-def get_config_object(path):
-    """
-    Get a config object from a path
-
-    :param str path: Path slash separeted from root of portal_urban to the config
-    :return: Config object
-    :rtype: LicenceConfig
-    """
-    portal_urban = api.portal.get_tool('portal_urban')
-
-    return portal_urban.restrictedTraverse(path)
```

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/setuphandlers.py` & `urban.restapi-1.0a1/src/urban/restapi/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/testing.py` & `urban.restapi-1.0a1/src/urban/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/tests/robot/test_example.robot` & `urban.restapi-1.0a1/src/urban/restapi/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/tests/test_robot.py` & `urban.restapi-1.0a1/src/urban/restapi/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban/restapi/tests/test_setup.py` & `urban.restapi-1.0a1/src/urban/restapi/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `urban.restapi-1.0.0b1/src/urban.restapi.egg-info/PKG-INFO` & `urban.restapi-1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urban.restapi
-Version: 1.0.0b1
+Version: 1.0a1
 Summary: specific urban restapi for interoperability
 Home-page: https://pypi.python.org/pypi/urban.restapi
 Author: Julien Jaumotte
 Author-email: julien.jaumotte@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -86,27 +86,14 @@
         - Julien Jaumotte, julien.jaumotte@imio.be
         
         
         Changelog
         =========
         
         
-        1.0.0b1 (2023-06-29)
-        --------------------
-        
-        - Fix POST endpoint for event creation [URB-2730]
-          [jchandelle]
-        
-        - Add utils for getting config object from a path
-          [jchandelle]
-        
-        - Fix address query with parenthesis [URB-2696]
-          [jchandelle]
-        
-        
         1.0a1 (2023-04-05)
         ------------------
         
         - Initial release.
           [jjaumotte]
         
 Keywords: Python Plone
```

### Comparing `urban.restapi-1.0.0b1/src/urban.restapi.egg-info/SOURCES.txt` & `urban.restapi-1.0a1/src/urban.restapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 src/urban/restapi/upgrades.py
 src/urban/restapi/upgrades.zcml
 src/urban/restapi/locales/README.rst
 src/urban/restapi/locales/__init__.py
 src/urban/restapi/locales/update.py
 src/urban/restapi/locales/update.sh
 src/urban/restapi/locales/urban.restapi.pot
-src/urban/restapi/locales/en/LC_MESSAGES/urban.restapi.mo
 src/urban/restapi/locales/en/LC_MESSAGES/urban.restapi.po
 src/urban/restapi/profiles/default/browserlayer.xml
 src/urban/restapi/profiles/default/catalog.xml
 src/urban/restapi/profiles/default/metadata.xml
 src/urban/restapi/profiles/default/registry.xml
 src/urban/restapi/profiles/default/rolemap.xml
 src/urban/restapi/profiles/uninstall/browserlayer.xml
```

