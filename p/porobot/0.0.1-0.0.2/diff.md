# Comparing `tmp/porobot-0.0.1.tar.gz` & `tmp/porobot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porobot-0.0.1.tar", last modified: Thu Jun 29 14:39:32 2023, max compression
+gzip compressed data, was "porobot-0.0.2.tar", last modified: Thu Jun 29 15:08:53 2023, max compression
```

## Comparing `porobot-0.0.1.tar` & `porobot-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.154336 porobot-0.0.1/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 porobot-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4156 2023-06-29 14:39:32.155337 porobot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3613 2023-06-28 15:39:38.000000 porobot-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.139696 porobot-0.0.1/pofinance/
--rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 porobot-0.0.1/pofinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.143214 porobot-0.0.1/pofinance/api/
--rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 porobot-0.0.1/pofinance/api/__init__.py
--rw-rw-rw-   0        0        0     4986 2023-06-06 17:35:03.000000 porobot-0.0.1/pofinance/api/shares.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.145225 porobot-0.0.1/pofinance/core/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.1/pofinance/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.146224 porobot-0.0.1/pofinance/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.1/pofinance/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:39:32.153329 porobot-0.0.1/porobot.egg-info/
--rw-rw-rw-   0        0        0     4156 2023-06-29 14:39:31.000000 porobot-0.0.1/porobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-29 14:39:32.000000 porobot-0.0.1/porobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:39:31.000000 porobot-0.0.1/porobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 14:39:31.000000 porobot-0.0.1/porobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-29 14:39:31.000000 porobot-0.0.1/porobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      706 2023-06-29 14:39:32.156338 porobot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 porobot-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.030921 porobot-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-29 14:40:45.000000 porobot-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      565 2023-06-29 15:08:53.030921 porobot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-06-29 14:40:45.000000 porobot-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.011276 porobot-0.0.2/porobot/
+-rw-rw-rw-   0        0        0       32 2023-06-29 15:02:34.000000 porobot-0.0.2/porobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/api/
+-rw-rw-rw-   0        0        0       15 2023-06-29 15:02:05.000000 porobot-0.0.2/porobot/api/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-06-29 15:06:53.000000 porobot-0.0.2/porobot/api/normal.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/core/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.2/porobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.2/porobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot.egg-info/
+-rw-rw-rw-   0        0        0      565 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 14:59:29.000000 porobot-0.0.2/porobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-06-29 15:08:53.030921 porobot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 porobot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/tests/
+-rw-rw-rw-   0        0        0      268 2023-06-29 15:04:12.000000 porobot-0.0.2/tests/test.py
```

### Comparing `porobot-0.0.1/setup.cfg` & `porobot-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f72 6f62 6f74 0d0a 7665 7273   = porobot..vers
-00000020: 696f 6e20 3d20 302e 302e 310d 0a64 6573  ion = 0.0.1..des
+00000020: 696f 6e20 3d20 302e 302e 320d 0a64 6573  ion = 0.0.2..des
 00000030: 6372 6970 7469 6f6e 203d 2070 6970 2069  cription = pip i
-00000040: 6e73 7461 6c6c 2070 6f66 696e 616e 6365  nstall pofinance
-00000050: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000060: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-00000070: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-00000080: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000090: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-000000a0: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-000000b0: 3a2f 2f77 7777 2e70 7974 686f 6e2d 6f66  ://www.python-of
-000000c0: 6669 6365 2e63 6f6d 2f0d 0a61 7574 686f  fice.com/..autho
-000000d0: 7220 3d20 436f 6465 7257 616e 4665 6e67  r = CoderWanFeng
-000000e0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-000000f0: 2031 3935 3738 3735 3037 3340 7171 2e63   1957875073@qq.c
-00000100: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
-00000110: 540d 0a6c 6963 656e 7365 5f66 696c 6520  T..license_file 
-00000120: 3d20 4c49 4345 4e53 450d 0a70 6c61 7466  = LICENSE..platf
-00000130: 6f72 6d73 203d 2061 6e79 0d0a 7072 6f6a  orms = any..proj
-00000140: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
-00000150: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
-00000160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
-00000170: 6f64 6572 5761 6e46 656e 672f 706f 6669  oderWanFeng/pofi
-00000180: 6e61 6e63 652f 6973 7375 6573 0d0a 0944  nance/issues...D
-00000190: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
-000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001b0: 6d2f 436f 6465 7257 616e 4665 6e67 2f70  m/CoderWanFeng/p
-000001c0: 6f66 696e 616e 6365 2f62 6c6f 622f 6d61  ofinance/blob/ma
-000001d0: 7374 6572 2f52 4541 444d 452e 6d64 0d0a  ster/README.md..
-000001e0: 0953 6f75 7263 6520 436f 6465 203d 2068  .Source Code = h
-000001f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000200: 6d2f 436f 6465 7257 616e 4665 6e67 2f70  m/CoderWanFeng/p
-00000210: 6f66 696e 616e 6365 0d0a 0d0a 5b6f 7074  ofinance....[opt
-00000220: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
-00000230: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
-00000240: 5f72 6571 7569 7265 7320 3d20 0d0a 7079  _requires = ..py
-00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000260: 3e3d 332e 350d 0a69 6e63 6c75 6465 5f70  >=3.5..include_p
-00000270: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-00000280: 7565 0d0a 7a69 705f 7361 6665 203d 2046  ue..zip_safe = F
-00000290: 616c 7365 0d0a 0d0a 5b65 6767 5f69 6e66  alse....[egg_inf
-000002a0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002b0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002c0: 0d0a                                     ..
+00000040: 6e73 7461 6c6c 2070 6f72 6f62 6f74 0d0a  nstall porobot..
+00000050: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000060: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000070: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+00000080: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000090: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+000000a0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+000000b0: 2f77 7777 2e70 7974 686f 6e2d 6f66 6669  /www.python-offi
+000000c0: 6365 2e63 6f6d 2f0d 0a61 7574 686f 7220  ce.com/..author 
+000000d0: 3d20 436f 6465 7257 616e 4665 6e67 0d0a  = CoderWanFeng..
+000000e0: 6175 7468 6f72 5f65 6d61 696c 203d 2031  author_email = 1
+000000f0: 3935 3738 3735 3037 3340 7171 2e63 6f6d  957875073@qq.com
+00000100: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
+00000110: 0a6c 6963 656e 7365 5f66 696c 6520 3d20  .license_file = 
+00000120: 4c49 4345 4e53 450d 0a70 6c61 7466 6f72  LICENSE..platfor
+00000130: 6d73 203d 2061 6e79 0d0a 7072 6f6a 6563  ms = any..projec
+00000140: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
+00000150: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000160: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6f64  //github.com/Cod
+00000170: 6572 5761 6e46 656e 672f 706f 726f 626f  erWanFeng/porobo
+00000180: 742f 6973 7375 6573 0d0a 0944 6f63 756d  t/issues...Docum
+00000190: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
+000001a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 436f  ://github.com/Co
+000001b0: 6465 7257 616e 4665 6e67 2f70 6f72 6f62  derWanFeng/porob
+000001c0: 6f74 2f62 6c6f 622f 6d61 7374 6572 2f52  ot/blob/master/R
+000001d0: 4541 444d 452e 6d64 0d0a 0953 6f75 7263  EADME.md...Sourc
+000001e0: 6520 436f 6465 203d 2068 7474 7073 3a2f  e Code = https:/
+000001f0: 2f67 6974 6875 622e 636f 6d2f 436f 6465  /github.com/Code
+00000200: 7257 616e 4665 6e67 2f70 6f72 6f62 6f74  rWanFeng/porobot
+00000210: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000220: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000230: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000240: 7320 3d20 0d0a 7079 7468 6f6e 5f72 6571  s = ..python_req
+00000250: 7569 7265 7320 3d20 3e3d 332e 350d 0a69  uires = >=3.5..i
+00000260: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000270: 6174 6120 3d20 5472 7565 0d0a 7a69 705f  ata = True..zip_
+00000280: 7361 6665 203d 2046 616c 7365 0d0a 0d0a  safe = False....
+00000290: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000002a0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002b0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

