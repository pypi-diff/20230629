# Comparing `tmp/nmbu.rinex-1.0.0.tar.gz` & `tmp/nmbu.rinex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Foxxxy/Desktop/masteroppgave/rinex-reader/dist/.tmp-0_m80hou/nmbu.rinex-1.0.0.tar", last modified: Mon Jun  5 21:07:02 2023, max compression
+gzip compressed data, was "/Users/Foxxxy/Desktop/masteroppgave/rinex-reader/dist/.tmp-kjg02afh/nmbu.rinex-1.0.1.tar", last modified: Thu Jun 29 12:16:02 2023, max compression
```

## Comparing `nmbu.rinex-1.0.0.tar` & `nmbu.rinex-1.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.313624 nmbu.rinex-1.0.0/
--rw-r--r--   0 Foxxxy     (501) staff       (20)    35128 2023-02-14 19:23:55.000000 nmbu.rinex-1.0.0/COPYING
--rw-r--r--   0 Foxxxy     (501) staff       (20)    15670 2023-06-05 21:07:02.315483 nmbu.rinex-1.0.0/PKG-INFO
--rw-r--r--   0 Foxxxy     (501) staff       (20)    15064 2023-06-05 20:53:45.000000 nmbu.rinex-1.0.0/README.md
--rw-r--r--   0 Foxxxy     (501) staff       (20)      680 2023-06-05 21:06:44.000000 nmbu.rinex-1.0.0/pyproject.toml
--rw-r--r--   0 Foxxxy     (501) staff       (20)      149 2023-06-05 21:07:02.317310 nmbu.rinex-1.0.0/setup.cfg
--rw-r--r--   0 Foxxxy     (501) staff       (20)      594 2023-02-14 19:52:00.000000 nmbu.rinex-1.0.0/setup.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.183353 nmbu.rinex-1.0.0/src/
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.196439 nmbu.rinex-1.0.0/src/nmbu/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:21:55.000000 nmbu.rinex-1.0.0/src/nmbu/__init__.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.204362 nmbu.rinex-1.0.0/src/nmbu/rinex/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:21:55.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/__init__.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.208892 nmbu.rinex-1.0.0/src/nmbu/rinex/common/
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2296 2023-04-21 14:43:57.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/common/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     7375 2023-04-26 17:57:19.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/common/rinex_data.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.213325 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/__init__.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.216846 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     6968 2023-05-03 17:25:53.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/header.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.237741 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2779 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/BDS.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3146 2023-04-15 00:15:14.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GAL.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     1891 2023-04-11 07:35:23.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_04.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2056 2023-02-14 19:26:14.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_05.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2708 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GPS.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2700 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/IRN.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2706 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/QZS.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     1898 2023-02-14 19:26:14.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/SBAS.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)    12092 2023-04-17 21:36:11.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/navigation.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.245406 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2276 2023-02-14 19:23:27.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/header.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.290630 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3542 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV1.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3514 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV2.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3259 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV3.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3116 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_D1_D2.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2194 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/EOP.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3555 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GAL_INAV_FNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2733 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GLO_FDMA.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3150 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3307 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV2.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3012 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_LNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2159 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_BDGIM.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2157 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Klobuchar.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     1929 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Nequick.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2961 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/IRN_LNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3150 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3307 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV2.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     3000 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_LNAV.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2588 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/SBAS.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2085 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/STO.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)    13801 2023-04-23 11:27:59.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/navigation.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.295033 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/__init__.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.298934 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     8407 2023-04-11 11:17:35.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/header.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)    10189 2023-04-11 11:17:35.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/observation.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.303141 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/
--rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/__init__.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     7668 2023-04-11 11:17:35.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/header.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)    10189 2023-02-14 19:23:27.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/observation.py
--rw-r--r--   0 Foxxxy     (501) staff       (20)     9243 2023-04-11 07:32:21.000000 nmbu.rinex-1.0.0/src/nmbu/rinex/reader.py
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.202737 nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/
--rw-r--r--   0 Foxxxy     (501) staff       (20)    15670 2023-06-05 21:07:02.000000 nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/PKG-INFO
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2610 2023-06-05 21:07:02.000000 nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/SOURCES.txt
--rw-r--r--   0 Foxxxy     (501) staff       (20)        1 2023-06-05 21:07:02.000000 nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/dependency_links.txt
--rw-r--r--   0 Foxxxy     (501) staff       (20)        5 2023-06-05 21:07:02.000000 nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/top_level.txt
-drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-05 21:07:02.304860 nmbu.rinex-1.0.0/tests/
--rw-r--r--   0 Foxxxy     (501) staff       (20)     2558 2023-02-13 10:27:19.000000 nmbu.rinex-1.0.0/tests/test_reader_pytest.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.606824 nmbu.rinex-1.0.1/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    35128 2023-02-14 19:23:55.000000 nmbu.rinex-1.0.1/COPYING
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    15670 2023-06-29 12:16:02.607297 nmbu.rinex-1.0.1/PKG-INFO
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    15064 2023-06-29 12:11:26.000000 nmbu.rinex-1.0.1/README.md
+-rw-r--r--   0 Foxxxy     (501) staff       (20)      680 2023-06-29 11:59:03.000000 nmbu.rinex-1.0.1/pyproject.toml
+-rw-r--r--   0 Foxxxy     (501) staff       (20)      149 2023-06-29 12:16:02.608814 nmbu.rinex-1.0.1/setup.cfg
+-rw-r--r--   0 Foxxxy     (501) staff       (20)      594 2023-02-14 19:52:00.000000 nmbu.rinex-1.0.1/setup.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.491796 nmbu.rinex-1.0.1/src/
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.500070 nmbu.rinex-1.0.1/src/nmbu/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:21:55.000000 nmbu.rinex-1.0.1/src/nmbu/__init__.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.510397 nmbu.rinex-1.0.1/src/nmbu/rinex/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:21:55.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/__init__.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.513668 nmbu.rinex-1.0.1/src/nmbu/rinex/common/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2296 2023-04-21 14:43:57.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/common/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     7375 2023-04-26 17:57:19.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/common/rinex_data.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.514739 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/__init__.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.516938 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     6968 2023-05-03 17:25:53.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/header.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.535829 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2779 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/BDS.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3146 2023-04-15 00:15:14.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GAL.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     1891 2023-04-11 07:35:23.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_04.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2056 2023-02-14 19:26:14.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_05.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2708 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GPS.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2700 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/IRN.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2706 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/QZS.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     1898 2023-02-14 19:26:14.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/SBAS.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    12092 2023-04-17 21:36:11.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/navigation.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.538659 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2276 2023-02-14 19:23:27.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/header.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.587516 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3542 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV1.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3514 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV2.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3259 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV3.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3116 2023-04-18 11:47:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_D1_D2.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2194 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/EOP.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3555 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GAL_INAV_FNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2733 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GLO_FDMA.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3150 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3307 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV2.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3012 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_LNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2159 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_BDGIM.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2157 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Klobuchar.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     1929 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Nequick.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2961 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/IRN_LNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3150 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3307 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV2.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     3000 2023-04-14 21:46:06.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_LNAV.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2588 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/SBAS.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2085 2023-02-12 15:20:36.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/STO.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    13801 2023-04-23 11:27:59.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/navigation.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.588369 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/__init__.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.591957 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     8407 2023-04-11 11:17:35.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/header.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    10318 2023-06-29 12:12:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/observation.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.604361 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        0 2023-02-13 10:23:31.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/__init__.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     7668 2023-04-11 11:17:35.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/header.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    10318 2023-06-29 12:12:07.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/observation.py
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     9243 2023-04-11 07:32:21.000000 nmbu.rinex-1.0.1/src/nmbu/rinex/reader.py
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.502421 nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)    15670 2023-06-29 12:16:02.000000 nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/PKG-INFO
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2610 2023-06-29 12:16:02.000000 nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/SOURCES.txt
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        1 2023-06-29 12:16:02.000000 nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/dependency_links.txt
+-rw-r--r--   0 Foxxxy     (501) staff       (20)        5 2023-06-29 12:16:02.000000 nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/top_level.txt
+drwxr-xr-x   0 Foxxxy     (501) staff       (20)        0 2023-06-29 12:16:02.605739 nmbu.rinex-1.0.1/tests/
+-rw-r--r--   0 Foxxxy     (501) staff       (20)     2558 2023-02-13 10:27:19.000000 nmbu.rinex-1.0.1/tests/test_reader_pytest.py
```

### Comparing `nmbu.rinex-1.0.0/COPYING` & `nmbu.rinex-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/PKG-INFO` & `nmbu.rinex-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbu.rinex
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reader for RINEX v3 and v4 formats for both observation and navigation files
 Author: Liudmila Sherstnyakova
 Project-URL: Homepage, https://github.com/liudmila-sherstnyakova/rinex-reader
 Project-URL: Bug Tracker, https://github.com/liudmila-sherstnyakova/rinex-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `nmbu.rinex-1.0.0/README.md` & `nmbu.rinex-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/pyproject.toml` & `nmbu.rinex-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nmbu.rinex"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Liudmila Sherstnyakova" },
 ]
 description = "Reader for RINEX v3 and v4 formats for both observation and navigation files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nmbu.rinex-1.0.0/setup.py` & `nmbu.rinex-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/common/__init__.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/common/rinex_data.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/common/rinex_data.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/header.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/header.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/BDS.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/BDS.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GAL.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GAL.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_04.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_04.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_05.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GLOv3_05.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/GPS.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/GPS.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/IRN.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/IRN.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/QZS.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/QZS.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/nav_message_type/SBAS.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/nav_message_type/SBAS.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v3/navigation.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v3/navigation.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/header.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/header.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV1.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV1.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV2.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV2.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV3.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_CNAV3.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_D1_D2.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/BDS_D1_D2.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/EOP.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/EOP.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GAL_INAV_FNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GAL_INAV_FNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GLO_FDMA.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GLO_FDMA.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV2.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_CNAV2.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_LNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/GPS_LNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_BDGIM.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_BDGIM.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Klobuchar.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Klobuchar.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Nequick.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/ION_Nequick.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/IRN_LNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/IRN_LNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV2.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_CNAV2.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_LNAV.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/QZS_LNAV.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/SBAS.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/SBAS.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/nav_message_type/STO.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/nav_message_type/STO.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/navigation/v4/navigation.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/navigation/v4/navigation.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/header.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/header.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v3/observation.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v3/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,18 @@
             print("For GNSS '{gnss:s}' only following obs types are included: {types:s}".format(
                 gnss=system,
                 types=str(list_of_obs_types)))
         result = result[list_of_obs_types]  # reduce result to only the selection of obs types
         for i in range(len(sv_names)):
             if sv_names[i] not in observations.satellites.keys():
                 observations.satellites[sv_names[i]] = {block_name: np.nan}
-            observations.satellites[sv_names[i]][block_name] = result[i]
+            if result.ndim == 0:
+                observations.satellites[sv_names[i]][block_name] = result
+            else:
+                observations.satellites[sv_names[i]][block_name] = result[i]
 
 
 def read_observation_blocks_v3(
         file: IO,
         header: ObservationHeaderV3,
         start_epoch: Optional[datetime],
         end_epoch: Optional[datetime],
```

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/header.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/header.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/observation/v4/observation.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/observation/v4/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,18 @@
             print("For GNSS '{gnss:s}' only following obs types are included: {types:s}".format(
                 gnss=system,
                 types=str(list_of_obs_types)))
         result = result[list_of_obs_types]  # reduce result to only the selection of obs types
         for i in range(len(sv_names)):
             if sv_names[i] not in observations.satellites.keys():
                 observations.satellites[sv_names[i]] = {block_name: np.nan}
-            observations.satellites[sv_names[i]][block_name] = result[i]
+            if result.ndim == 0:
+                observations.satellites[sv_names[i]][block_name] = result
+            else:
+                observations.satellites[sv_names[i]][block_name] = result[i]
 
 
 def read_observation_blocks_v4(
         file: IO,
         header: ObservationHeaderV4,
         start_epoch: Optional[datetime],
         end_epoch: Optional[datetime],
```

### Comparing `nmbu.rinex-1.0.0/src/nmbu/rinex/reader.py` & `nmbu.rinex-1.0.1/src/nmbu/rinex/reader.py`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/PKG-INFO` & `nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmbu.rinex
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reader for RINEX v3 and v4 formats for both observation and navigation files
 Author: Liudmila Sherstnyakova
 Project-URL: Homepage, https://github.com/liudmila-sherstnyakova/rinex-reader
 Project-URL: Bug Tracker, https://github.com/liudmila-sherstnyakova/rinex-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `nmbu.rinex-1.0.0/src/nmbu.rinex.egg-info/SOURCES.txt` & `nmbu.rinex-1.0.1/src/nmbu.rinex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmbu.rinex-1.0.0/tests/test_reader_pytest.py` & `nmbu.rinex-1.0.1/tests/test_reader_pytest.py`

 * *Files identical despite different names*

