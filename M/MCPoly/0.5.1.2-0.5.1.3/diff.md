# Comparing `tmp/MCPoly-0.5.1.2.tar.gz` & `tmp/MCPoly-0.5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.5.1.2.tar", last modified: Wed Jun 28 14:07:49 2023, max compression
+gzip compressed data, was "MCPoly-0.5.1.3.tar", last modified: Thu Jun 29 15:19:39 2023, max compression
```

## Comparing `MCPoly-0.5.1.2.tar` & `MCPoly-0.5.1.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.044466 MCPoly-0.5.1.2/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.5.1.2/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.5.1.2/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.027628 MCPoly-0.5.1.2/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    12292 2023-06-27 16:00:50.000000 MCPoly-0.5.1.2/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.5.1.2/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.031524 MCPoly-0.5.1.2/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)     5719 2023-06-18 16:08:00.000000 MCPoly-0.5.1.2/MCPoly/lmpset/DATAtoXYZ.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.5.1.2/MCPoly/lmpset/DATAtomolTXT.py
--rw-r--r--   0 cxs454     (503) staff       (20)      169 2023-06-17 16:42:13.000000 MCPoly-0.5.1.2/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.5.1.2/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.5.1.2/MCPoly/lmpset/infchain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    53042 2023-06-18 16:59:51.000000 MCPoly-0.5.1.2/MCPoly/lmpset/mould.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5402 2023-06-19 16:17:41.000000 MCPoly-0.5.1.2/MCPoly/lmpset/rebuild.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.034328 MCPoly-0.5.1.2/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.5.1.2/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.5.1.2/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.5.1.2/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.5.1.2/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.5.1.2/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.5.1.2/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.037340 MCPoly-0.5.1.2/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)    10729 2023-06-24 15:26:07.000000 MCPoly-0.5.1.2/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.5.1.2/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    20688 2023-06-27 14:13:27.000000 MCPoly-0.5.1.2/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7792 2023-06-27 14:07:19.000000 MCPoly-0.5.1.2/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.5.1.2/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2310 2023-06-27 14:02:40.000000 MCPoly-0.5.1.2/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24591 2023-06-28 14:04:56.000000 MCPoly-0.5.1.2/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.5.1.2/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.5.1.2/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.039362 MCPoly-0.5.1.2/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.5.1.2/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)      133 2023-06-27 15:58:50.000000 MCPoly-0.5.1.2/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-06-22 12:33:27.000000 MCPoly-0.5.1.2/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12736 2023-06-27 15:58:34.000000 MCPoly-0.5.1.2/MCPoly/sscurve/gui2.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.5.1.2/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5162 2023-06-27 15:58:01.000000 MCPoly-0.5.1.2/MCPoly/sscurve/multiple2.py
--rw-r--r--   0 cxs454     (503) staff       (20)    13033 2023-06-27 15:58:20.000000 MCPoly-0.5.1.2/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.040733 MCPoly-0.5.1.2/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.5.1.2/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6192 2023-06-18 16:33:35.000000 MCPoly-0.5.1.2/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.5.1.2/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24351 2023-06-27 13:59:56.000000 MCPoly-0.5.1.2/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.041575 MCPoly-0.5.1.2/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.5.1.2/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-28 14:05:03.000000 MCPoly-0.5.1.2/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.042059 MCPoly-0.5.1.2/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.5.1.2/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.5.1.2/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.042739 MCPoly-0.5.1.2/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.5.1.2/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2112 2023-06-27 13:59:22.000000 MCPoly-0.5.1.2/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.028625 MCPoly-0.5.1.2/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     4201 2023-06-28 14:07:49.000000 MCPoly-0.5.1.2/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1330 2023-06-28 14:07:49.000000 MCPoly-0.5.1.2/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-28 14:07:49.000000 MCPoly-0.5.1.2/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-28 14:07:49.000000 MCPoly-0.5.1.2/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-28 14:07:49.000000 MCPoly-0.5.1.2/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     4201 2023-06-28 14:07:49.044275 MCPoly-0.5.1.2/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3837 2023-06-28 14:06:17.000000 MCPoly-0.5.1.2/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-28 14:07:49.044531 MCPoly-0.5.1.2/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-28 14:05:11.000000 MCPoly-0.5.1.2/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-28 14:07:49.043926 MCPoly-0.5.1.2/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     9627 2023-06-18 17:38:10.000000 MCPoly-0.5.1.2/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.5.1.2/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3931 2023-06-24 15:32:23.000000 MCPoly-0.5.1.2/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.5.1.2/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-24 15:37:07.000000 MCPoly-0.5.1.2/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.734040 MCPoly-0.5.1.3/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.5.1.3/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.5.1.3/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.726254 MCPoly-0.5.1.3/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    12292 2023-06-29 15:19:33.000000 MCPoly-0.5.1.3/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.5.1.3/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.728041 MCPoly-0.5.1.3/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     5719 2023-06-18 16:08:00.000000 MCPoly-0.5.1.3/MCPoly/lmpset/DATAtoXYZ.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.5.1.3/MCPoly/lmpset/DATAtomolTXT.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      169 2023-06-17 16:42:13.000000 MCPoly-0.5.1.3/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.5.1.3/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.5.1.3/MCPoly/lmpset/infchain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    53042 2023-06-18 16:59:51.000000 MCPoly-0.5.1.3/MCPoly/lmpset/mould.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5402 2023-06-19 16:17:41.000000 MCPoly-0.5.1.3/MCPoly/lmpset/rebuild.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.729076 MCPoly-0.5.1.3/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.5.1.3/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.5.1.3/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.5.1.3/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.5.1.3/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.5.1.3/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.5.1.3/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.730484 MCPoly-0.5.1.3/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)    10729 2023-06-24 15:26:07.000000 MCPoly-0.5.1.3/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.5.1.3/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    20688 2023-06-27 14:13:27.000000 MCPoly-0.5.1.3/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7792 2023-06-27 14:07:19.000000 MCPoly-0.5.1.3/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.5.1.3/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2310 2023-06-27 14:02:40.000000 MCPoly-0.5.1.3/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24620 2023-06-29 15:10:43.000000 MCPoly-0.5.1.3/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.5.1.3/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.5.1.3/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.731467 MCPoly-0.5.1.3/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.5.1.3/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      133 2023-06-27 15:58:50.000000 MCPoly-0.5.1.3/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-06-22 12:33:27.000000 MCPoly-0.5.1.3/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12736 2023-06-27 15:58:34.000000 MCPoly-0.5.1.3/MCPoly/sscurve/gui2.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.5.1.3/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5162 2023-06-27 15:58:01.000000 MCPoly-0.5.1.3/MCPoly/sscurve/multiple2.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    13033 2023-06-27 15:58:20.000000 MCPoly-0.5.1.3/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.732020 MCPoly-0.5.1.3/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.5.1.3/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6192 2023-06-18 16:33:35.000000 MCPoly-0.5.1.3/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.5.1.3/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24351 2023-06-29 14:46:46.000000 MCPoly-0.5.1.3/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.732313 MCPoly-0.5.1.3/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.5.1.3/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-28 15:45:03.000000 MCPoly-0.5.1.3/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.732588 MCPoly-0.5.1.3/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.5.1.3/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.5.1.3/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.732858 MCPoly-0.5.1.3/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.5.1.3/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2112 2023-06-27 13:59:22.000000 MCPoly-0.5.1.3/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.726974 MCPoly-0.5.1.3/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     4201 2023-06-29 15:19:39.000000 MCPoly-0.5.1.3/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1330 2023-06-29 15:19:39.000000 MCPoly-0.5.1.3/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-29 15:19:39.000000 MCPoly-0.5.1.3/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-29 15:19:39.000000 MCPoly-0.5.1.3/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-29 15:19:39.000000 MCPoly-0.5.1.3/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     4201 2023-06-29 15:19:39.733869 MCPoly-0.5.1.3/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3837 2023-06-29 14:06:33.000000 MCPoly-0.5.1.3/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-29 15:19:39.734093 MCPoly-0.5.1.3/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-29 15:19:26.000000 MCPoly-0.5.1.3/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-29 15:19:39.733631 MCPoly-0.5.1.3/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     9627 2023-06-18 17:38:10.000000 MCPoly-0.5.1.3/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.5.1.3/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3931 2023-06-24 15:32:23.000000 MCPoly-0.5.1.3/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.5.1.3/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-24 15:37:07.000000 MCPoly-0.5.1.3/tests/test_status.py
```

### Comparing `MCPoly-0.5.1.2/LICENSE` & `MCPoly-0.5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/.DS_Store` & `MCPoly-0.5.1.3/MCPoly/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
 00001070: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00001080: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00001090: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000010a0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000010b0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000010c0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 000010d0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000010e0: 7208 0908 095f 1018 7b7b 3131 352c 2031  r...._..{{115, 1
-000010f0: 3837 7d2c 207b 3932 302c 2034 3336 7d7d  87}, {920, 436}}
+000010e0: 7208 0908 095f 1018 7b7b 3637 342c 2033  r...._..{{674, 3
+000010f0: 3832 7d2c 207b 3932 302c 2034 3336 7d7d  82}, {920, 436}}
 00001100: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 00001110: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 00001120: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 00001130: 0007 006f 0072 0063 0061 0073 0065 0074  ...o.r.c.a.s.e.t
 00001140: 6963 7670 626c 6f62 0000 0194 6270 6c69  icvpblob....bpli
 00001150: 7374 3030 de01 0203 0405 0607 0809 0a0b  st00............
 00001160: 0c0d 0e0f 1011 0f12 0f13 1314 1516 1718  ................
@@ -302,108 +302,108 @@
 000012d0: 0000 0000 0000 0000 0000 0000 0000 0140  ...............@
 000012e0: 0000 0007 006f 0072 0063 0061 0073 0065  .....o.r.c.a.s.e
 000012f0: 0074 7653 726e 6c6f 6e67 0000 0001 0000  .tvSrnlong......
 00001300: 0007 0073 0073 0063 0075 0072 0076 0065  ...s.s.c.u.r.v.e
 00001310: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
 00001320: 0000 002e ffff ffff ffff 0000 0000 0007  ................
 00001330: 0073 0073 0063 0075 0072 0076 0065 6277  .s.s.c.u.r.v.ebw
-00001340: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
+00001340: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
 00001350: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00001360: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00001370: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00001380: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00001390: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 000013a0: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-000013b0: 6465 6261 7208 0908 095f 1017 7b7b 3436  debar...._..{{46
-000013c0: 2c20 3430 317d 2c20 7b39 3230 2c20 3433  , 401}, {920, 43
-000013d0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000013e0: 8900 0000 0000 0001 0100 0000 0000 0000  ................
-000013f0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-00001400: 8a00 0000 0700 7300 7300 6300 7500 7200  ......s.s.c.u.r.
-00001410: 7600 6576 5372 6e6c 6f6e 6700 0000 0100  v.evSrnlong.....
-00001420: 0000 0600 7300 7400 6100 7400 7500 7349  ....s.t.a.t.u.sI
-00001430: 6c6f 6362 6c6f 6200 0000 1000 0002 6700  locblob.......g.
-00001440: 0000 2eff ffff ffff ff00 0000 0000 0600  ................
-00001450: 7300 7400 6100 7400 7500 7362 7773 7062  s.t.a.t.u.sbwspb
-00001460: 6c6f 6200 0000 b862 706c 6973 7430 30d6  lob....bplist00.
-00001470: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
-00001480: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
-00001490: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-000014a0: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-000014b0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-000014c0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-000014d0: 6172 0809 0809 5f10 187b 7b36 3734 2c20  ar...._..{{674, 
-000014e0: 3338 327d 2c20 7b39 3230 2c20 3433 367d  382}, {920, 436}
-000014f0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8a00  }...#/;R_klmno..
-00001500: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
-00001510: 0000 0000 0000 0000 0000 0000 0000 8b00  ................
-00001520: 0000 0600 7300 7400 6100 7400 7500 7376  ....s.t.a.t.u.sv
-00001530: 5372 6e6c 6f6e 6700 0000 0100 0000 0700  Srnlong.........
-00001540: 7600 6500 7200 7300 6900 6f00 6e49 6c6f  v.e.r.s.i.o.nIlo
-00001550: 6362 6c6f 6200 0000 1000 0002 d500 0000  cblob...........
-00001560: 2eff ffff ffff ff00 0000 0000 0700 7600  ..............v.
-00001570: 6500 7200 7300 6900 6f00 6e62 7773 7062  e.r.s.i.o.nbwspb
-00001580: 6c6f 6200 0000 b762 706c 6973 7430 30d6  lob....bplist00.
-00001590: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
-000015a0: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
-000015b0: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-000015c0: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-000015d0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-000015e0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-000015f0: 6172 0809 0809 5f10 177b 7b34 362c 2034  ar...._..{{46, 4
-00001600: 3031 7d2c 207b 3932 302c 2034 3336 7d7d  01}, {920, 436}}
-00001610: 0908 1523 2f3b 525f 6b6c 6d6e 6f89 0000  ...#/;R_klmno...
-00001620: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-00001630: 0000 0000 0000 0000 0000 0000 008a 0000  ................
-00001640: 0007 0076 0065 0072 0073 0069 006f 006e  ...v.e.r.s.i.o.n
-00001650: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
-00001660: 0000 0007 0076 0065 0072 0073 0069 006f  .....v.e.r.s.i.o
-00001670: 006e 6d6f 4444 626c 6f62 0000 0008 f66e  .nmoDDblob.....n
-00001680: a121 cf01 c541 0000 0007 0076 0065 0072  .!...A.....v.e.r
-00001690: 0073 0069 006f 006e 6d6f 6444 626c 6f62  .s.i.o.nmodDblob
-000016a0: 0000 0008 f66e a121 cf01 c541 0000 0007  .....n.!...A....
-000016b0: 0076 0065 0072 0073 0069 006f 006e 7068  .v.e.r.s.i.o.nph
-000016c0: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
-000016d0: 0007 0076 0065 0072 0073 0069 006f 006e  ...v.e.r.s.i.o.n
-000016e0: 7653 726e 6c6f 6e67 0000 0001 0000 0006  vSrnlong........
-000016f0: 0076 0069 0065 0077 0033 0064 496c 6f63  .v.i.e.w.3.dIloc
-00001700: 626c 6f62 0000 0010 0000 0041 0000 009e  blob.......A....
-00001710: ffff ffff ffff 0000 0000 0006 0076 0069  .............v.i
-00001720: 0065 0077 0033 0064 6277 7370 626c 6f62  .e.w.3.dbwspblob
-00001730: 0000 00b7 6270 6c69 7374 3030 d601 0203  ....bplist00....
-00001740: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
-00001750: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00001760: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00001770: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00001780: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00001790: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000017a0: 0908 095f 1017 7b7b 3436 2c20 3430 317d  ..._..{{46, 401}
-000017b0: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-000017c0: 232f 3b52 5f6b 6c6d 6e6f 8900 0000 0000  #/;R_klmno......
-000017d0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-000017e0: 0000 0000 0000 0000 0000 8a00 0000 0600  ................
-000017f0: 7600 6900 6500 7700 3300 6476 5372 6e6c  v.i.e.w.3.dvSrnl
-00001800: 6f6e 6700 0000 0100 0000 0300 7600 6900  ong.........v.i.
-00001810: 7349 6c6f 6362 6c6f 6200 0000 1000 0000  sIlocblob.......
-00001820: af00 0000 9eff ffff ffff ff00 0000 0000  ................
-00001830: 0300 7600 6900 7362 7773 7062 6c6f 6200  ..v.i.sbwspblob.
-00001840: 0000 b762 706c 6973 7430 30d6 0102 0304  ...bplist00.....
-00001850: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
-00001860: 7475 7342 6172 5b53 686f 7754 6f6f 6c62  tusBar[ShowToolb
-00001870: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00001880: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00001890: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-000018a0: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
-000018b0: 0809 5f10 177b 7b34 362c 2034 3031 7d2c  .._..{{46, 401},
-000018c0: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
-000018d0: 2f3b 525f 6b6c 6d6e 6f89 0000 0000 0000  /;R_klmno.......
-000018e0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-000018f0: 0000 0000 0000 0000 008a 0000 0003 0076  ...............v
-00001900: 0069 0073 7653 726e 6c6f 6e67 0000 0001  .i.svSrnlong....
-00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000013b0: 6465 6261 7208 0908 095f 1018 7b7b 3637  debar...._..{{67
+000013c0: 332c 2031 3330 7d2c 207b 3932 302c 2034  3, 130}, {920, 4
+000013d0: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+000013e0: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+000013f0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00001400: 008b 0000 0007 0073 0073 0063 0075 0072  .......s.s.c.u.r
+00001410: 0076 0065 7653 726e 6c6f 6e67 0000 0001  .v.evSrnlong....
+00001420: 0000 0006 0073 0074 0061 0074 0075 0073  .....s.t.a.t.u.s
+00001430: 496c 6f63 626c 6f62 0000 0010 0000 0267  Ilocblob.......g
+00001440: 0000 002e ffff ffff ffff 0000 0000 0006  ................
+00001450: 0073 0074 0061 0074 0075 0073 6277 7370  .s.t.a.t.u.sbwsp
+00001460: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00001470: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00001480: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001490: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+000014a0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+000014b0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+000014c0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+000014d0: 6261 7208 0908 095f 1018 7b7b 3637 342c  bar...._..{{674,
+000014e0: 2033 3832 7d2c 207b 3932 302c 2034 3336   382}, {920, 436
+000014f0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00001500: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001510: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00001520: 0000 0006 0073 0074 0061 0074 0075 0073  .....s.t.a.t.u.s
+00001530: 7653 726e 6c6f 6e67 0000 0001 0000 0007  vSrnlong........
+00001540: 0076 0065 0072 0073 0069 006f 006e 496c  .v.e.r.s.i.o.nIl
+00001550: 6f63 626c 6f62 0000 0010 0000 02d5 0000  ocblob..........
+00001560: 002e ffff ffff ffff 0000 0000 0007 0076  ...............v
+00001570: 0065 0072 0073 0069 006f 006e 6277 7370  .e.r.s.i.o.nbwsp
+00001580: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00001590: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+000015a0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+000015b0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+000015c0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+000015d0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+000015e0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+000015f0: 6261 7208 0908 095f 1018 7b7b 3637 332c  bar...._..{{673,
+00001600: 2031 3330 7d2c 207b 3932 302c 2034 3336   130}, {920, 436
+00001610: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00001620: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001630: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00001640: 0000 0007 0076 0065 0072 0073 0069 006f  .....v.e.r.s.i.o
+00001650: 006e 6c67 3153 636f 6d70 0000 0000 0000  .nlg1Scomp......
+00001660: 0000 0000 0007 0076 0065 0072 0073 0069  .......v.e.r.s.i
+00001670: 006f 006e 6d6f 4444 626c 6f62 0000 0008  .o.nmoDDblob....
+00001680: f66e a121 cf01 c541 0000 0007 0076 0065  .n.!...A.....v.e
+00001690: 0072 0073 0069 006f 006e 6d6f 6444 626c  .r.s.i.o.nmodDbl
+000016a0: 6f62 0000 0008 f66e a121 cf01 c541 0000  ob.....n.!...A..
+000016b0: 0007 0076 0065 0072 0073 0069 006f 006e  ...v.e.r.s.i.o.n
+000016c0: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
+000016d0: 0000 0007 0076 0065 0072 0073 0069 006f  .....v.e.r.s.i.o
+000016e0: 006e 7653 726e 6c6f 6e67 0000 0001 0000  .nvSrnlong......
+000016f0: 0006 0076 0069 0065 0077 0033 0064 496c  ...v.i.e.w.3.dIl
+00001700: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
+00001710: 009e ffff ffff ffff 0000 0000 0006 0076  ...............v
+00001720: 0069 0065 0077 0033 0064 6277 7370 626c  .i.e.w.3.dbwspbl
+00001730: 6f62 0000 00b7 6270 6c69 7374 3030 d601  ob....bplist00..
+00001740: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00001750: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00001760: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00001770: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00001780: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00001790: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+000017a0: 7208 0908 095f 1017 7b7b 3436 2c20 3430  r...._..{{46, 40
+000017b0: 317d 2c20 7b39 3230 2c20 3433 367d 7d09  1}, {920, 436}}.
+000017c0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
+000017d0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+000017e0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
+000017f0: 0600 7600 6900 6500 7700 3300 6476 5372  ..v.i.e.w.3.dvSr
+00001800: 6e6c 6f6e 6700 0000 0100 0000 0300 7600  nlong.........v.
+00001810: 6900 7349 6c6f 6362 6c6f 6200 0000 1000  i.sIlocblob.....
+00001820: 0000 af00 0000 9eff ffff ffff ff00 0000  ................
+00001830: 0000 0300 7600 6900 7362 7773 7062 6c6f  ....v.i.sbwspblo
+00001840: 6200 0000 b762 706c 6973 7430 30d6 0102  b....bplist00...
+00001850: 0304 0506 0708 0708 0b08 5d53 686f 7753  ..........]ShowS
+00001860: 7461 7475 7342 6172 5b53 686f 7754 6f6f  tatusBar[ShowToo
+00001870: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00001880: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00001890: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+000018a0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+000018b0: 0809 0809 5f10 177b 7b34 362c 2034 3031  ...._..{{46, 401
+000018c0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
+000018d0: 1523 2f3b 525f 6b6c 6d6e 6f89 0000 0000  .#/;R_klmno.....
+000018e0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
+000018f0: 0000 0000 0000 0000 0000 008a 0000 0003  ................
+00001900: 0076 0069 0073 7653 726e 6c6f 6e67 0000  .v.i.svSrnlong..
+00001910: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -625,24 +625,24 @@
 00002700: 019f 01a1 01a2 01ab 01b0 01b9 0000 0000  ................
 00002710: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00002720: 0000 0000 0000 0000 0000 01ba 0000 0006  ................
 00002730: 006c 006d 0070 0073 0065 0074 7653 726e  .l.m.p.s.e.tvSrn
 00002740: 6c6f 6e67 0000 0001 0000 0007 006d 006f  long.........m.o
 00002750: 006c 0064 0072 0061 0077 496c 6f63 626c  .l.d.r.a.wIlocbl
 00002760: 6f62 0000 0010 0000 011d 0000 002e ffff  ob..............
-00002770: ffff ffff 0000 6169 6e65 7253 686f 7753  ......ainerShowS
-00002780: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002790: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000027a0: 0908 095f 1017 7b7b 3436 2c20 3430 317d  ..._..{{46, 401}
-000027b0: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-000027c0: 232f 3b52 5f6b 6c6d 6e6f 8900 0000 0000  #/;R_klmno......
-000027d0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-000027e0: 0000 0000 0000 0000 0000 8a00 0000 0600  ................
-000027f0: 7600 6900 6500 7700 3300 6476 5372 6e6c  v.i.e.w.3.dvSrnl
-00002800: 6f6e 6700 0000 0005 0000 0000 0000 280b  ong...........(.
+00002770: ffff ffff 0000 6e74 6169 6e65 7253 686f  ......ntainerSho
+00002780: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00002790: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+000027a0: 7208 0908 095f 1017 7b7b 3436 2c20 3430  r...._..{{46, 40
+000027b0: 317d 2c20 7b39 3230 2c20 3433 367d 7d09  1}, {920, 436}}.
+000027c0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
+000027d0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+000027e0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
+000027f0: 0600 7600 6900 6500 7700 3300 6476 5372  ..v.i.e.w.3.dvSr
+00002800: 6e6c 6f6e 0000 0005 0000 0000 0000 280b  nlon..........(.
 00002810: 0000 0045 0000 100c 0000 0108 0000 200b  ...E.......... .
 00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -753,17 +753,17 @@
 00002f00: 019f 01a1 01a2 01ab 01b0 01b9 0000 0000  ................
 00002f10: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00002f20: 0000 0000 0000 0000 0000 01ba 0000 0006  ................
 00002f30: 006c 006d 0070 0073 0065 0074 7653 726e  .l.m.p.s.e.tvSrn
 00002f40: 6c6f 6e67 0000 0001 0000 0007 006d 006f  long.........m.o
 00002f50: 006c 0064 0072 0061 0077 496c 6f63 626c  .l.d.r.a.wIlocbl
 00002f60: 6f62 0000 0010 0000 011d 0000 002e ffff  ob..............
-00002f70: ffff ffff 0000 6169 6e65 7253 686f 7753  ......ainerShowS
-00002f80: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002f90: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002fa0: 0908 095f 1017 7b7b 3436 2c20 3430 317d  ..._..{{46, 401}
-00002fb0: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-00002fc0: 232f 3b52 5f6b 6c6d 6e6f 8900 0000 0000  #/;R_klmno......
-00002fd0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-00002fe0: 0000 0000 0000 0000 0000 8a00 0000 0600  ................
-00002ff0: 7600 6900 6500 7700 3300 6476 5372 6e6c  v.i.e.w.3.dvSrnl
-00003000: 6f6e 6700                                ong.
+00002f70: ffff ffff 0000 6e74 6169 6e65 7253 686f  ......ntainerSho
+00002f80: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00002f90: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00002fa0: 7208 0908 095f 1017 7b7b 3436 2c20 3430  r...._..{{46, 40
+00002fb0: 317d 2c20 7b39 3230 2c20 3433 367d 7d09  1}, {920, 436}}.
+00002fc0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
+00002fd0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+00002fe0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
+00002ff0: 0600 7600 6900 6500 7700 3300 6476 5372  ..v.i.e.w.3.dvSr
+00003000: 6e6c 6f6e                                nlon
```

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/DATAtoXYZ.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/DATAtoXYZ.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/DATAtomolTXT.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/DATAtomolTXT.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/chain.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/infchain.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/infchain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/mould.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/mould.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/lmpset/rebuild.py` & `MCPoly-0.5.1.3/MCPoly/lmpset/rebuild.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/moldraw/C_selection.py` & `MCPoly-0.5.1.3/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.5.1.3/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/moldraw/gui.py` & `MCPoly-0.5.1.3/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/moldraw/molecule.py` & `MCPoly-0.5.1.3/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.5.1.3/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/XYZtoINP.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/gui.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/mgui.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/mgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/multiorca.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/orca.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/orca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/ssgui.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/ssgui.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,14 @@
         num=len(atomsx)
         if aim1.value>=num:
             aim1.valu10e=num-1
         if aim2.value>=num:
             aim2.value=num-1
         output.clear_output()
         case.clear_output()
-        output2.clear_output()
         if aa.value==404:
             with output2:
                 if roomox.value==False and coreox.value==False:
                     XYZtoINP(file.value+'_{0:.3f}'.format(strain.value),inpname=file.value+'_{0:.3f}'.format(strain.value+forcestep[key]),\
                                  method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
                                  external_force=True,aim=[aim1.value,aim2.value],strain=strain.value+forcestep[key],\
                                  maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value)
@@ -200,29 +199,30 @@
                 forcestep={strain.value: addforce.value, strain2.value: addforce2.value, strain3.value: addforce3.value}
             for key in forcestep:
                 keys.append(key)
             keys.reverse()
             key=keys[0]
             ii=2
         else:
+            output2.clear_output()
             with output2:
                 display(widgets.Label('File: {0}.xyz'.format(file.value),style=dict(font_weight='bold')))
                 if roomox.value==False and coreox.value==False:
                     XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
                      external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxiter=maxiter.value,maxcore=room.value*1024,corenum=corenum.value)
                 elif roomox.value==True and coreox.value==True:
                     XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
                      external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value)
                 elif roomox.value==False and coreox.value==True:
                     XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
                      external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value,maxcore=room.value*1024)
                 elif roomox.value==True and coreox.value==False:
                     XYZtoINP(file.value,fileloc=loc.value,method=method.value,basis_set=bs.value,opt=True,freq=freq.value,\
                      external_force=True,aim=[aim1.value,aim2.value],maxiter=maxiter.value,strain=strain.value,corenum=corenum.value)
-            if strain==0.000:
+            if strain.value==0.000:
                 os.system('cp {0}.inp {0}_0.000.inp'.format(file.value))
             keys=[]
             if addforce.value==0:
                 raise ValueError("You can't set the force add per step zero!")
             forcestep={strain.value:addforce.value}
             if addox1.value==True:
                 if addforce2.value==0:
@@ -246,20 +246,20 @@
                 display(widgets.HBox([widgets.Label(file.value+'_{0:.3f}'.format(strain.value)), widgets.Label('  Processing...'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
             orca(file.value+'_{0:.3f}'.format(strain.value),orcaloc.value,loc.value,loc.value)
             ii=ii+1
             s=status(file.value+'_{0:.3f}'.format(strain.value),loc.value).status(statusonly=True)
             the_atoms=read(file.value+'_{0:.3f}.xyz'.format(strain.value))
             d=the_atoms.get_distance(aim1.value,aim2.value)
             case.clear_output()
-            if s==4:
+            if s==4 or s==41:
                 aa.value=0
                 distances.append(d)
                 force.append(strain.value)
                 xoy=checkbroken(distances,force)
-                if xoy==1:
+                if xoy==1 and s!=41:
                     with output2:
                         display(widgets.HBox([widgets.Valid(description=file.value+'_{0:.3f}'.format(strain.value),value=True),\
                                       widgets.Label('Broken.'), widgets.Label('[{0}]'.format(t.ctime(t.time())))]))
                     fromoutput.clear_output()
                     with fromoutput:
                         for i,poly in enumerate(polys):
                             print(poly+': {0:.6f} Hartree'.format(status(poly,loc.value).status(figureonly=True)[-1]))
```

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/ssorca.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/ssorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.5.1.3/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/YModulus.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/gui.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/gui2.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/gui2.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/multiple.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/multiple2.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/multiple2.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/sscurve/single.py` & `MCPoly-0.5.1.3/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/status/echart.py` & `MCPoly-0.5.1.3/MCPoly/status/echart.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/status/gui.py` & `MCPoly-0.5.1.3/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/status/status.py` & `MCPoly-0.5.1.3/MCPoly/status/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 if alls[0]=='0':
                     energy.append(eval(alls[-1]))
                 else:
                     if eval(alls[0])%gap==0:
                         energy.append(eval(alls[-3]))
     f.close()
     if statusonly==True:
-        if s2==1:
+        if s1==1:
             return 2
         else:
             return s1
     if figureonly==False and MD==False:
         print('{0} turns have been calculated.'.format(term))
         status_judge(s1,s2,converge)
         statusfig(energy,choose)
```

### Comparing `MCPoly-0.5.1.2/MCPoly/view3d/view3d.py` & `MCPoly-0.5.1.3/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly/vis/vis.py` & `MCPoly-0.5.1.3/MCPoly/vis/vis.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.5.1.3/MCPoly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.5.1.2
+Version: 0.5.1.3
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.5.1.2(28.06.23)
+## Updated in v0.5.1.3(29.06.23)
 1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
 2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
 3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
 4. All these functions can be used by lmpset.mould().XXX() now.
 5. Fix some bugs about ORCA Calculations Settings
 6. Fix some bugs about ORCA GUI display
 7. Fix some bugs about judging the maximum iteration of atoms
```

### Comparing `MCPoly-0.5.1.2/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.5.1.3/MCPoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/PKG-INFO` & `MCPoly-0.5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.5.1.2
+Version: 0.5.1.3
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.5.1.2(28.06.23)
+## Updated in v0.5.1.3(29.06.23)
 1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
 2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
 3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
 4. All these functions can be used by lmpset.mould().XXX() now.
 5. Fix some bugs about ORCA Calculations Settings
 6. Fix some bugs about ORCA GUI display
 7. Fix some bugs about judging the maximum iteration of atoms
```

### Comparing `MCPoly-0.5.1.2/README.md` & `MCPoly-0.5.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MCPoly
 Some methods to deal with some manipulation of computational chemistry, mostly about mechanical properties of polymers.
 ![](./reference/function.png)
 
 ## Overview
 `MCPoly` is a Python library to make some steps of computational chemistry easier. It includes some functions of drawing molecule structures, creating proper .xyz , .inp , .mol and .data file, which specialised for using ORCA and LAMMPS, and some functions for researching the mechanical property of some polymers.
 
-## Updated in v0.5.1.2(28.06.23)
+## Updated in v0.5.1.3(29.06.23)
 1. Add 'rebuild' in 'lmpset' package. You can now use it to rebuild geometry structure of LAMMPS input data now.
 2. Add 'DATAtoXYZ' in 'lmpset' package to convert LAMMPS Data File into XYZ File
 3. Add 'DATAtomolTXT' to convert LAMMPS Data File into LAMMPS Molecule Text File.
 4. All these functions can be used by lmpset.mould().XXX() now.
 5. Fix some bugs about ORCA Calculations Settings
 6. Fix some bugs about ORCA GUI display
 7. Fix some bugs about judging the maximum iteration of atoms
```

### Comparing `MCPoly-0.5.1.2/setup.py` & `MCPoly-0.5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.5.1.2',
+    version='0.5.1.3',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.5.1.2/tests/test_lmpset.py` & `MCPoly-0.5.1.3/tests/test_lmpset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/tests/test_moldraw.py` & `MCPoly-0.5.1.3/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/tests/test_orcaset.py` & `MCPoly-0.5.1.3/tests/test_orcaset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/tests/test_sscurve.py` & `MCPoly-0.5.1.3/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.5.1.2/tests/test_status.py` & `MCPoly-0.5.1.3/tests/test_status.py`

 * *Files identical despite different names*

