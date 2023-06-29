# Comparing `tmp/mona-openai-0.0.7.tar.gz` & `tmp/mona-openai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.7.tar", last modified: Thu Jun  8 11:20:51 2023, max compression
+gzip compressed data, was "mona-openai-0.0.8.tar", last modified: Thu Jun 29 11:38:06 2023, max compression
```

## Comparing `mona-openai-0.0.7.tar` & `mona-openai-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)    11356 2023-06-08 10:06:42.000000 mona-openai-0.0.7/LICENSE
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     9757 2023-06-08 11:20:51.585634 mona-openai-0.0.7/PKG-INFO
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     9162 2023-06-08 10:06:42.000000 mona-openai-0.0.7/README.md
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/mona_openai/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)       77 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/__init__.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/mona_openai/analysis/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     3613 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/analysis/privacy.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      304 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/analysis/profanity.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     3121 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/analysis/textual.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/mona_openai/endpoints/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     7675 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/endpoints/chat_completion.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     5165 2023-06-08 10:28:57.000000 mona-openai-0.0.7/mona_openai/endpoints/completion.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     4792 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/endpoints/endpoint_wrapping.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      792 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/endpoints/wrapping_getter.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      167 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/exceptions.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     1379 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/mona_client.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)    17096 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/mona_openai.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/mona_openai/util/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      946 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/async_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      675 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/func_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     1177 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/oop_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      364 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/openai_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     3788 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/stream_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      776 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/tokens_util.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      971 2023-06-08 10:06:42.000000 mona-openai-0.0.7/mona_openai/util/validation_util.py
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/mona_openai.egg-info/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     9757 2023-06-08 11:20:51.000000 mona-openai-0.0.7/mona_openai.egg-info/PKG-INFO
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      925 2023-06-08 11:20:51.000000 mona-openai-0.0.7/mona_openai.egg-info/SOURCES.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)        1 2023-06-08 11:20:51.000000 mona-openai-0.0.7/mona_openai.egg-info/dependency_links.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)       51 2023-06-08 11:20:51.000000 mona-openai-0.0.7/mona_openai.egg-info/requires.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)       12 2023-06-08 11:20:51.000000 mona-openai-0.0.7/mona_openai.egg-info/top_level.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      818 2023-06-08 11:20:41.000000 mona-openai-0.0.7/pyproject.toml
--rw-rw-r--   0 nemo      (1000) nemo      (1000)       50 2023-06-08 10:06:42.000000 mona-openai-0.0.7/requirements.txt
--rw-rw-r--   0 nemo      (1000) nemo      (1000)       38 2023-06-08 11:20:51.585634 mona-openai-0.0.7/setup.cfg
-drwxrwxr-x   0 nemo      (1000) nemo      (1000)        0 2023-06-08 11:20:51.585634 mona-openai-0.0.7/tests/
--rw-rw-r--   0 nemo      (1000) nemo      (1000)    17351 2023-06-08 10:39:38.000000 mona-openai-0.0.7/tests/test_chat_completion.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)    20103 2023-06-08 10:39:38.000000 mona-openai-0.0.7/tests/test_completion.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)     1607 2023-06-08 10:06:42.000000 mona-openai-0.0.7/tests/test_privacy_analyzer.py
--rw-rw-r--   0 nemo      (1000) nemo      (1000)      852 2023-06-08 10:06:42.000000 mona-openai-0.0.7/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.832827 mona-openai-0.0.8/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.8/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-29 11:38:06.832620 mona-openai-0.0.8/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10208 2023-06-29 11:01:14.000000 mona-openai-0.0.8/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.827551 mona-openai-0.0.8/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      100 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.829093 mona-openai-0.0.8/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3148 2023-06-29 11:36:56.000000 mona-openai-0.0.8/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.829898 mona-openai-0.0.8/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7749 2023-06-29 11:07:35.000000 mona-openai-0.0.8/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5165 2023-06-20 04:36:07.000000 mona-openai-0.0.8/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.0.8/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17565 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.831143 mona-openai-0.0.8/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.0.8/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.8/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.8/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.828384 mona-openai-0.0.8/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-06-29 11:37:26.000000 mona-openai-0.0.8/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.8/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-06-29 11:38:06.832862 mona-openai-0.0.8/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.832335 mona-openai-0.0.8/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.8/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20103 2023-06-22 09:34:20.000000 mona-openai-0.0.8/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.8/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:07:35.000000 mona-openai-0.0.8/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.7/LICENSE` & `mona-openai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/PKG-INFO` & `mona-openai-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e61  : 2.1.Name: mona
 00000020: 2d6f 7065 6e61 690a 5665 7273 696f 6e3a  -openai.Version:
-00000030: 2030 2e30 2e37 0a53 756d 6d61 7279 3a20   0.0.7.Summary: 
+00000030: 2030 2e30 2e38 0a53 756d 6d61 7279 3a20   0.0.8.Summary: 
 00000040: 496e 7465 6772 6174 696f 6e20 636c 6965  Integration clie
 00000050: 6e74 2066 6f72 206d 6f6e 6974 6f72 696e  nt for monitorin
 00000060: 6720 4f70 656e 4149 2075 7361 6765 2077  g OpenAI usage w
 00000070: 6974 6820 4d6f 6e61 0a41 7574 686f 722d  ith Mona.Author-
 00000080: 656d 6169 6c3a 2049 7461 6920 4261 7220  email: Itai Bar 
 00000090: 5369 6e61 6920 3c69 7461 6940 6d6f 6e61  Sinai <itai@mona
 000000a0: 6c61 6273 2e69 6f3e 0a50 726f 6a65 6374  labs.io>.Project
@@ -41,570 +41,636 @@
 00000280: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
 00000290: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
 000002a0: 2e63 6f6d 2f6d 6f6e 616c 6162 732f 6d6f  .com/monalabs/mo
 000002b0: 6e61 2d73 646b 2f62 6c6f 622f 6d61 696e  na-sdk/blob/main
 000002c0: 2f6d 6f6e 615f 6c6f 676f 2e70 6e67 3f72  /mona_logo.png?r
 000002d0: 6177 3d74 7275 6522 2061 6c74 3d22 4d6f  aw=true" alt="Mo
 000002e0: 6e61 2773 206c 6f67 6f22 2077 6964 7468  na's logo" width
-000002f0: 3d22 3138 3022 2f3e 0a3c 2f70 3e0a 0a0a  ="180"/>.</p>...
-00000300: 5573 6520 6f6e 6520 6c69 6e65 206f 6620  Use one line of 
-00000310: 636f 6465 2074 6f20 6765 7420 696e 7374  code to get inst
-00000320: 616e 7420 6c69 7665 206d 6f6e 6974 6f72  ant live monitor
-00000330: 696e 6720 666f 7220 796f 7572 204f 7065  ing for your Ope
-00000340: 6e41 4920 7573 6167 6520 696e 636c 7564  nAI usage includ
-00000350: 696e 673a 0a2a 2054 6f6b 656e 7320 7573  ing:.* Tokens us
-00000360: 6167 650a 2a20 4861 6c6c 7563 696e 6174  age.* Hallucinat
-00000370: 696f 6e20 616c 6572 7473 0a2a 2050 726f  ion alerts.* Pro
-00000380: 6661 6e69 7479 2061 6e64 2070 7269 7661  fanity and priva
-00000390: 6379 2061 6e61 6c79 7365 730a 2a20 4265  cy analyses.* Be
-000003a0: 6861 7669 6f72 616c 2064 7269 6674 7320  havioral drifts 
-000003b0: 616e 6420 616e 6f6d 616c 6965 730a 2a20  and anomalies.* 
-000003c0: 4d75 6368 206d 7563 6820 6d6f 7265 2e0a  Much much more..
-000003d0: 0a23 2320 5365 7474 696e 6720 5570 0a0a  .## Setting Up..
-000003e0: 2d20 544f 444f 3a20 4164 6420 7061 7274  - TODO: Add part
-000003f0: 2061 626f 7574 204d 6f6e 6120 7265 6769   about Mona regi
-00000400: 7374 7261 7469 6f6e 2077 6974 6820 6120  stration with a 
-00000410: 6c69 6e6b 2074 6f20 7468 6520 7265 6c65  link to the rele
-00000420: 7661 6e74 206c 616e 6469 6e67 2070 6167  vant landing pag
-00000430: 6520 7768 6572 6520 7468 6520 7265 6164  e where the read
-00000440: 6572 2063 616e 2073 6967 6e20 7570 2e0a  er can sign up..
-00000450: 6060 6063 6f6e 736f 6c65 0a24 2070 6970  ```console.$ pip
-00000460: 2069 6e73 7461 6c6c 206d 6f6e 615f 6f70   install mona_op
-00000470: 656e 6169 0a60 6060 0a0a 2323 2051 7569  enai.```..## Qui
-00000480: 636b 2053 7461 7274 2061 6e64 2045 7861  ck Start and Exa
-00000490: 6d70 6c65 0a0a 4578 616d 706c 6520 626f  mple..Example bo
-000004a0: 696c 6572 706c 6174 6520 636f 6465 2066  ilerplate code f
-000004b0: 6f72 2062 6f74 6820 7379 6e63 2061 6e64  or both sync and
-000004c0: 2061 7379 6e63 2075 7361 6765 2069 7320   async usage is 
-000004d0: 6769 7665 6e20 696e 2074 6865 2066 696c  given in the fil
-000004e0: 6520 2265 7861 6d70 6c65 5f75 7361 6765  e "example_usage
-000004f0: 2e70 7922 2061 6e64 2068 6572 653a 0a60  .py" and here:.`
-00000500: 6060 7079 0a66 726f 6d20 6f73 2069 6d70  ``py.from os imp
-00000510: 6f72 7420 656e 7669 726f 6e0a 696d 706f  ort environ.impo
-00000520: 7274 2061 7379 6e63 696f 0a69 6d70 6f72  rt asyncio.impor
-00000530: 7420 6f70 656e 6169 0a0a 6672 6f6d 206d  t openai..from m
-00000540: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
-00000550: 7420 6d6f 6e69 746f 720a 0a6f 7065 6e61  t monitor..opena
-00000560: 692e 6170 695f 6b65 7920 3d20 656e 7669  i.api_key = envi
-00000570: 726f 6e2e 6765 7428 224f 5045 4e5f 4149  ron.get("OPEN_AI
-00000580: 5f4b 4559 2229 0a0a 4d4f 4e41 5f41 5049  _KEY")..MONA_API
-00000590: 5f4b 4559 203d 2065 6e76 6972 6f6e 2e67  _KEY = environ.g
-000005a0: 6574 2822 4d4f 4e41 5f41 5049 5f4b 4559  et("MONA_API_KEY
-000005b0: 2229 0a4d 4f4e 415f 5345 4352 4554 203d  ").MONA_SECRET =
-000005c0: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
-000005d0: 4e41 5f53 4543 5245 5422 290a 4d4f 4e41  NA_SECRET").MONA
-000005e0: 5f43 5245 4453 203d 207b 0a20 2020 2022  _CREDS = {.    "
-000005f0: 6b65 7922 3a20 4d4f 4e41 5f41 5049 5f4b  key": MONA_API_K
-00000600: 4559 2c0a 2020 2020 2273 6563 7265 7422  EY,.    "secret"
-00000610: 3a20 4d4f 4e41 5f53 4543 5245 542c 0a7d  : MONA_SECRET,.}
-00000620: 0a43 4f4e 5445 5854 5f43 4c41 5353 5f4e  .CONTEXT_CLASS_N
-00000630: 414d 4520 3d20 2253 4f4d 455f 4d4f 4e49  AME = "SOME_MONI
-00000640: 544f 5249 4e47 5f43 4f4e 5445 5854 5f4e  TORING_CONTEXT_N
-00000650: 414d 4522 0a0a 0a6d 6f6e 6974 6f72 6564  AME"...monitored
-00000660: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
-00000670: 6e69 746f 7228 0a20 2020 206f 7065 6e61  nitor(.    opena
-00000680: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
-00000690: 2020 4d4f 4e41 5f43 5245 4453 2c0a 2020    MONA_CREDS,.  
-000006a0: 2020 434f 4e54 4558 545f 434c 4153 535f    CONTEXT_CLASS_
-000006b0: 4e41 4d45 2c0a 290a 0a0a 7072 6f6d 7074  NAME,.)...prompt
-000006c0: 203d 2022 4920 7761 6e74 2074 6f20 6765   = "I want to ge
-000006d0: 6e65 7261 7465 2073 6f6d 6520 7465 7874  nerate some text
-000006e0: 2061 626f 7574 2022 0a6d 6f64 656c 203d   about ".model =
-000006f0: 2022 7465 7874 2d61 6461 2d30 3031 220a   "text-ada-001".
-00000700: 7465 6d70 6572 6174 7572 6520 3d20 302e  temperature = 0.
-00000710: 360a 6d61 785f 746f 6b65 6e73 203d 2035  6.max_tokens = 5
-00000720: 0a6e 203d 2031 0a0a 2320 5265 6775 6c61  .n = 1..# Regula
-00000730: 7220 2873 796e 6329 2075 7361 6765 0a72  r (sync) usage.r
-00000740: 6573 706f 6e73 6520 3d20 6d6f 6e69 746f  esponse = monito
-00000750: 7265 645f 636f 6d70 6c65 7469 6f6e 2e63  red_completion.c
-00000760: 7265 6174 6528 0a20 2020 2065 6e67 696e  reate(.    engin
-00000770: 653d 6d6f 6465 6c2c 0a20 2020 2070 726f  e=model,.    pro
-00000780: 6d70 743d 7072 6f6d 7074 2c0a 2020 2020  mpt=prompt,.    
-00000790: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
-000007a0: 6f6b 656e 732c 0a20 2020 206e 3d6e 2c0a  okens,.    n=n,.
-000007b0: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
-000007c0: 7465 6d70 6572 6174 7572 652c 0a20 2020  temperature,.   
-000007d0: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
-000007e0: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
-000007f0: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
-00000800: 2c0a 290a 7072 696e 7428 7265 7370 6f6e  ,.).print(respon
-00000810: 7365 2e63 686f 6963 6573 5b30 5d2e 7465  se.choices[0].te
-00000820: 7874 290a 0a23 2041 7379 6e63 2075 7361  xt)..# Async usa
-00000830: 6765 0a72 6573 706f 6e73 6520 3d20 6173  ge.response = as
-00000840: 796e 6369 6f2e 7275 6e28 6d6f 6e69 746f  yncio.run(monito
-00000850: 7265 645f 636f 6d70 6c65 7469 6f6e 2e61  red_completion.a
-00000860: 6372 6561 7465 280a 2020 2020 656e 6769  create(.    engi
-00000870: 6e65 3d6d 6f64 656c 2c0a 2020 2020 7072  ne=model,.    pr
-00000880: 6f6d 7074 3d70 726f 6d70 742c 0a20 2020  ompt=prompt,.   
-00000890: 206d 6178 5f74 6f6b 656e 733d 6d61 785f   max_tokens=max_
-000008a0: 746f 6b65 6e73 2c0a 2020 2020 6e3d 6e2c  tokens,.    n=n,
-000008b0: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
-000008c0: 3d74 656d 7065 7261 7475 7265 2c0a 2020  =temperature,.  
-000008d0: 2020 4d4f 4e41 5f61 6464 6974 696f 6e61    MONA_additiona
-000008e0: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
-000008f0: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
-00000900: 7d2c 0a29 290a 0a70 7269 6e74 2872 6573  },.))..print(res
-00000910: 706f 6e73 652e 6368 6f69 6365 735b 305d  ponse.choices[0]
-00000920: 2e74 6578 7429 0a60 6060 0a23 2320 5375  .text).```.## Su
-00000930: 7070 6f72 7465 6420 4f70 656e 4149 2041  pported OpenAI A
-00000940: 5049 730a 4375 7272 656e 746c 7920 7468  PIs.Currently th
-00000950: 6973 2063 6c69 656e 7420 7375 7070 6f72  is client suppor
-00000960: 7473 2060 6f70 656e 6169 2e43 6f6d 706c  ts `openai.Compl
-00000970: 6574 696f 6e60 2061 6e64 2060 6f70 656e  etion` and `open
-00000980: 6169 2e43 6861 7443 6f6d 706c 6574 696f  ai.ChatCompletio
-00000990: 6e60 2e20 4d6f 6e61 2063 616e 2073 7570  n`. Mona can sup
-000009a0: 706f 7274 2070 726f 6365 7373 6573 2062  port processes b
-000009b0: 6173 6564 206f 6e20 6f74 6865 7220 4150  ased on other AP
-000009c0: 4973 2061 6e64 2061 6c73 6f20 6e6f 6e2d  Is and also non-
-000009d0: 4f70 656e 4149 2d62 6173 6564 2061 7070  OpenAI-based app
-000009e0: 732e 0a49 6620 796f 7520 6861 7665 2061  s..If you have a
-000009f0: 2064 6966 6665 7272 656e 7420 7573 652d   differrent use-
-00000a00: 6361 7365 2c20 7765 2764 206c 6f76 6520  case, we'd love 
-00000a10: 746f 2068 6561 7220 6162 6f75 7420 6974  to hear about it
-00000a20: 2120 506c 6561 7365 2065 6d61 696c 2075  ! Please email u
-00000a30: 7320 6174 2073 7570 706f 7274 406d 6f6e  s at support@mon
-00000a40: 616c 6162 732e 696f 2e0a 0a23 2320 5573  alabs.io...## Us
-00000a50: 6167 650a 2323 2320 496e 6974 6961 6c69  age.### Initiali
-00000a60: 7a61 7469 6f6e 0a0a 5468 6520 6d61 696e  zation..The main
-00000a70: 2061 6e64 206f 6e6c 7920 6675 6e63 7469   and only functi
-00000a80: 6f6e 2065 7870 6f73 6564 2069 6e20 7468  on exposed in th
-00000a90: 6973 2070 6163 6b61 6765 2069 7320 606d  is package is `m
-00000aa0: 6f6e 6974 6f72 602e 0a60 6060 7079 0a69  onitor`..```py.i
-00000ab0: 6d70 6f72 7420 6f70 656e 6169 0a0a 6672  mport openai..fr
-00000ac0: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
-00000ad0: 6d70 6f72 7420 6d6f 6e69 746f 720a 0a6f  mport monitor..o
-00000ae0: 7065 6e61 692e 6170 695f 6b65 7920 3d20  penai.api_key = 
-00000af0: 656e 7669 726f 6e2e 6765 7428 224f 5045  environ.get("OPE
-00000b00: 4e5f 4149 5f4b 4559 2229 0a0a 6d6f 6e69  N_AI_KEY")..moni
-00000b10: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00000b20: 203d 206d 6f6e 6974 6f72 280a 2020 2020   = monitor(.    
-00000b30: 6f70 656e 6169 2e43 6f6d 706c 6574 696f  openai.Completio
-00000b40: 6e2c 0a20 2020 2028 0a20 2020 2020 2020  n,.    (.       
-00000b50: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
-00000b60: 4e41 5f41 5049 5f4b 4559 2229 2c0a 2020  NA_API_KEY"),.  
-00000b70: 2020 2020 2020 656e 7669 726f 6e2e 6765        environ.ge
-00000b80: 7428 224d 4f4e 415f 5345 4352 4554 2229  t("MONA_SECRET")
-00000b90: 2c0a 2020 2020 292c 0a20 2020 2022 534f  ,.    ),.    "SO
-00000ba0: 4d45 5f4d 4f4e 4954 4f52 494e 475f 434f  ME_MONITORING_CO
-00000bb0: 4e54 4558 545f 4e41 4d45 222c 0a20 2020  NTEXT_NAME",.   
-00000bc0: 207b 2261 6e61 6c79 7369 7322 3a20 7b22   {"analysis": {"
-00000bd0: 7072 6f66 616e 6974 7922 3a20 4661 6c73  profanity": Fals
-00000be0: 657d 7d0a 290a 0a2e 2e2e 0a0a 6d6f 6e69  e}}.).......moni
-00000bf0: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00000c00: 2e63 7265 6174 6528 2e2e 2e29 0a60 6060  .create(...).```
-00000c10: 0a0a 5468 6520 606d 6f6e 6974 6f72 6020  ..The `monitor` 
-00000c20: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-00000c30: 2074 6f20 796f 7520 6120 636c 6173 7320   to you a class 
-00000c40: 7468 6174 2077 7261 7073 2074 6865 206f  that wraps the o
-00000c50: 7269 6769 6e61 6c20 6f70 656e 6169 2065  riginal openai e
-00000c60: 6e64 706f 696e 7420 636c 6173 7320 796f  ndpoint class yo
-00000c70: 7520 7072 6f76 6964 652c 2077 6974 6820  u provide, with 
-00000c80: 616e 2065 7175 6976 616c 656e 7420 4150  an equivalent AP
-00000c90: 4920 2862 6573 6964 6573 2073 6f6d 6520  I (besides some 
-00000ca0: 6164 6469 7469 6f6e 7320 6c69 7374 6564  additions listed
-00000cb0: 2062 656c 6f77 292e 0a59 6f75 2063 616e   below)..You can
-00000cc0: 2074 6865 6e20 7573 6520 7468 6520 7265   then use the re
-00000cd0: 7475 726e 6564 2063 6c61 7373 2720 2263  turned class' "c
-00000ce0: 7265 6174 6522 2061 6e64 2022 6163 7265  reate" and "acre
-00000cf0: 6174 6522 2066 756e 6374 696f 6e73 206a  ate" functions j
-00000d00: 7573 7420 6173 2079 6f75 2077 6f75 6c64  ust as you would
-00000d10: 2062 6566 6f72 652c 206f 6e6c 7920 6e6f   before, only no
-00000d20: 772c 2062 6573 6964 6573 2067 6574 7469  w, besides getti
-00000d30: 6e67 2074 6865 2072 6571 7565 7374 6564  ng the requested
-00000d40: 206f 7065 6e41 4920 6675 6e63 7469 6f6e   openAI function
-00000d50: 616c 6974 792c 2074 6869 7320 636c 6965  ality, this clie
-00000d60: 6e74 2077 696c 6c20 6c6f 6720 6f75 7420  nt will log out 
-00000d70: 746f 204d 6f6e 6127 7320 7365 7276 6572  to Mona's server
-00000d80: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-00000d90: 796f 7520 7573 6564 2028 652e 672e 2c20  you used (e.g., 
-00000da0: 7465 6d70 6572 6174 7572 6529 2c20 6461  temperature), da
-00000db0: 7461 2061 626f 7574 2074 6865 2072 6573  ta about the res
-00000dc0: 706f 6e73 6520 6672 6f6d 204f 7065 6e41  ponse from OpenA
-00000dd0: 4927 7320 7365 7276 6572 2c20 616e 6420  I's server, and 
-00000de0: 6375 7374 6f6d 2061 6e61 6c79 7365 7320  custom analyses 
-00000df0: 6162 6f75 7420 7468 6520 6361 6c6c 2028  about the call (
-00000e00: 652e 672e 2c20 7072 6f66 616e 6974 7920  e.g., profanity 
-00000e10: 7363 6f72 6573 2c20 7072 6976 6163 7920  scores, privacy 
-00000e20: 6368 6563 6b73 2066 6f72 2065 6d61 696c  checks for email
-00000e30: 732f 7068 6f6e 6520 6e75 6d62 6572 7320  s/phone numbers 
-00000e40: 666f 756e 6420 696e 2074 6865 2074 6578  found in the tex
-00000e50: 7473 2c20 7465 7874 7561 6c20 616e 616c  ts, textual anal
-00000e60: 7973 6573 2c20 6574 632e 2e2e 290a 0a54  yses, etc...)..T
-00000e70: 6865 2060 6d6f 6e69 746f 7260 2066 756e  he `monitor` fun
-00000e80: 6374 696f 6e20 7265 6365 6976 6573 2074  ction receives t
-00000e90: 6865 2066 6f6c 6c6f 7769 6e67 2061 7267  he following arg
-00000ea0: 756d 656e 7473 3a0a 6f70 656e 6169 5f63  uments:.openai_c
-00000eb0: 6c61 7373 3a20 416e 204f 7065 6e41 4920  lass: An OpenAI 
-00000ec0: 4150 4920 636c 6173 7320 746f 2077 7261  API class to wra
-00000ed0: 7020 7769 7468 206d 6f6e 6974 6f72 696e  p with monitorin
-00000ee0: 6720 6361 7061 6269 6c74 6965 732e 0a6d  g capabilties..m
-00000ef0: 6f6e 615f 6372 6564 733a 2041 2064 6963  ona_creds: A dic
-00000f00: 7420 2863 6f6e 7461 696e 696e 6720 226b  t (containing "k
-00000f10: 6579 2220 616e 6420 2273 6563 7265 7422  ey" and "secret"
-00000f20: 2920 6f72 2070 6169 7220 2874 7570 6c65  ) or pair (tuple
-00000f30: 2920 6f66 204d 6f6e 6120 4150 4920 6b65  ) of Mona API ke
-00000f40: 7920 616e 6420 7365 6372 6574 2074 6f20  y and secret to 
-00000f50: 7365 7420 7570 204d 6f6e 6127 7320 636c  set up Mona's cl
-00000f60: 6965 6e74 7320 6672 6f6d 2069 7473 2053  ients from its S
-00000f70: 444b 2e0a 636f 6e74 6578 745f 636c 6173  DK..context_clas
-00000f80: 733a 2054 6865 204d 6f6e 6120 636f 6e74  s: The Mona cont
-00000f90: 6578 7420 636c 6173 7320 6e61 6d65 2074  ext class name t
-00000fa0: 6f20 7573 6520 666f 7220 6d6f 6e69 746f  o use for monito
-00000fb0: 7269 6e67 2e20 5573 6520 6120 636f 6e73  ring. Use a cons
-00000fc0: 7461 6e74 206e 616d 6520 6f66 2079 6f75  tant name of you
-00000fd0: 7220 6368 6f69 6365 2e0a 7370 6563 733a  r choice..specs:
-00000fe0: 2041 2064 6963 7469 6f6e 6172 7920 6f66   A dictionary of
-00000ff0: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
-00001000: 7375 6368 2061 7320 6d6f 6e69 746f 7269  such as monitori
-00001010: 6e67 2073 616d 706c 696e 6720 7261 7469  ng sampling rati
-00001020: 6f2e 0a0a 2323 2323 2053 7065 6373 0a54  o...#### Specs.T
-00001030: 6865 2073 7065 6373 2061 7267 2061 6c6c  he specs arg all
-00001040: 6f77 7320 796f 7520 746f 2063 6f6e 6669  ows you to confi
-00001050: 6775 7265 2077 6861 7420 7368 6f75 6c64  gure what should
-00001060: 2062 6520 6d6f 6e69 746f 7265 642e 2049   be monitored. I
-00001070: 7420 6578 7065 6374 7320 6120 7079 7468  t expects a pyth
-00001080: 6f6e 2064 6963 7420 7769 7468 2074 6865  on dict with the
-00001090: 2066 6f6c 6c77 6f69 6e67 2070 6f73 7369   follwoing possi
-000010a0: 626c 6520 6b65 7973 3a0a 2a20 7361 6d70  ble keys:.* samp
-000010b0: 6c69 6e67 5f72 6174 696f 2028 3129 3a20  ling_ratio (1): 
-000010c0: 4120 6e75 6d62 6572 2062 6574 7765 656e  A number between
-000010d0: 2030 2061 6e64 2031 2066 6f72 2068 6f77   0 and 1 for how
-000010e0: 206f 6674 656e 2073 686f 756c 6420 7468   often should th
-000010f0: 6520 6361 6c6c 2062 6520 6c6f 6767 6564  e call be logged
-00001100: 2e0a 2a20 6176 6f69 645f 6d6f 6e69 746f  ..* avoid_monito
-00001110: 7269 6e67 5f65 7863 6570 7469 6f6e 7320  ring_exceptions 
-00001120: 2846 616c 7365 293a 2057 6865 7468 6572  (False): Whether
-00001130: 206f 7220 6e6f 7420 746f 206c 6f67 206f   or not to log o
-00001140: 7574 2074 6f20 4d6f 6e61 2077 6865 6e20  ut to Mona when 
-00001150: 7468 6572 6520 6973 2061 6e20 4f70 656e  there is an Open
-00001160: 4149 2065 7863 6570 7469 6f6e 2e20 4465  AI exception. De
-00001170: 6661 756c 7420 6973 2074 6f20 7472 6163  fault is to trac
-00001180: 6b20 6578 6365 7074 696f 6e73 202d 2061  k exceptions - a
-00001190: 6e64 204d 6f6e 6120 7769 6c6c 2061 6c65  nd Mona will ale
-000011a0: 7274 2079 6f75 206f 6e20 7468 696e 6773  rt you on things
-000011b0: 206c 696b 6520 6120 6a75 6d70 2069 6e20   like a jump in 
-000011c0: 6e75 6d62 6572 206f 6620 6578 6365 7074  number of except
-000011d0: 696f 6e73 0a2a 2065 7870 6f72 745f 7072  ions.* export_pr
-000011e0: 6f6d 7074 2028 4661 6c73 6529 3a20 5768  ompt (False): Wh
-000011f0: 6574 6865 7220 4d6f 6e61 2073 686f 756c  ether Mona shoul
-00001200: 6420 6578 706f 7274 2074 6865 2061 6374  d export the act
-00001210: 7561 6c20 7072 6f6d 7074 2074 6578 742e  ual prompt text.
-00001220: 2042 6520 6465 6661 756c 7420 7365 7420   Be default set 
-00001230: 746f 2046 616c 7365 2074 6f20 6176 6f69  to False to avoi
-00001240: 6420 7072 6976 6163 7920 636f 6e63 6572  d privacy concer
-00001250: 6e73 2e0a 2a20 6578 706f 7274 5f72 6573  ns..* export_res
-00001260: 706f 6e73 655f 7465 7874 7320 2846 616c  ponse_texts (Fal
-00001270: 7365 293a 2057 6865 7468 6572 204d 6f6e  se): Whether Mon
-00001280: 6120 7368 6f75 6c64 2065 7870 6f72 7420  a should export 
-00001290: 7468 6520 6163 7475 616c 2072 6573 706f  the actual respo
-000012a0: 6e73 6520 7465 7874 732e 2042 6520 6465  nse texts. Be de
-000012b0: 6661 756c 7420 7365 7420 746f 2046 616c  fault set to Fal
-000012c0: 7365 2074 6f20 6176 6f69 6420 7072 6976  se to avoid priv
-000012d0: 6163 7920 636f 6e63 6572 6e73 2e0a 2a20  acy concerns..* 
-000012e0: 616e 616c 7973 6973 3a20 4120 6469 6374  analysis: A dict
-000012f0: 696f 6e61 7279 206d 6170 7069 6e67 2065  ionary mapping e
-00001300: 6163 6820 616e 616c 7973 6973 2074 7970  ach analysis typ
-00001310: 6520 746f 2061 2062 6f6f 6c65 616e 2076  e to a boolean v
-00001320: 616c 7565 2074 656c 6c69 6e67 2074 6865  alue telling the
-00001330: 2063 6c69 656e 7420 7768 6574 6865 7220   client whether 
-00001340: 6f72 206e 6f74 2074 6f20 7275 6e20 7361  or not to run sa
-00001350: 6964 2061 6e61 6c79 7369 7320 616e 6420  id analysis and 
-00001360: 6c6f 6720 6974 2074 6f20 4d6f 6e61 2e20  log it to Mona. 
-00001370: 506f 7373 6962 6c65 206f 7074 696f 6e73  Possible options
-00001380: 2063 7572 7265 6e74 6c79 2061 7265 2022   currently are "
-00001390: 7072 6976 6163 7922 2c20 2270 726f 6661  privacy", "profa
-000013a0: 6e69 7479 222c 2061 6e64 2022 7465 7874  nity", and "text
-000013b0: 7561 6c22 2e20 4279 2064 6566 6175 6c74  ual". By default
-000013c0: 2c20 616c 6c20 616e 616c 7973 6573 2074  , all analyses t
-000013d0: 616b 6520 706c 6163 6520 616e 6420 6172  ake place and ar
-000013e0: 6520 6c6f 6767 6564 206f 7574 2074 6f20  e logged out to 
-000013f0: 4d6f 6e61 2e0a 0a23 2323 2043 6170 6162  Mona...### Capab
-00001400: 696c 6974 6965 7320 6475 7269 6e67 2041  ilities during A
-00001410: 5049 2063 616c 6c73 0a0a 4166 7465 7220  PI calls..After 
-00001420: 7772 6170 7069 6e67 2079 6f75 7220 656e  wrapping your en
-00001430: 6470 6f69 6e74 2077 6974 6820 606d 6f6e  dpoint with `mon
-00001440: 6974 6f72 602c 2079 6f75 2072 6561 6c6c  itor`, you reall
-00001450: 7920 646f 6e27 7420 6e65 6564 2074 6f20  y don't need to 
-00001460: 646f 2061 6e79 7468 696e 6720 656c 7365  do anything else
-00001470: 2e20 5768 656e 2075 7369 6e67 2060 6372  . When using `cr
-00001480: 6561 7465 6020 6f72 2060 6163 7265 6174  eate` or `acreat
-00001490: 6560 2064 6174 6120 7769 6c6c 2062 6520  e` data will be 
-000014a0: 7472 6163 6b65 6420 616e 6420 6d6f 6e69  tracked and moni
-000014b0: 746f 7269 6e67 2077 696c 6c20 7461 6b65  toring will take
-000014c0: 2070 6c61 6365 2e0a 0a54 6865 7265 2061   place...There a
-000014d0: 7265 2c20 686f 7765 7665 722c 2073 6576  re, however, sev
-000014e0: 6572 616c 2063 6170 6162 696c 6974 6965  eral capabilitie
-000014f0: 7320 7468 6174 2061 7265 2061 6464 6564  s that are added
-00001500: 2074 6f20 7468 6573 6520 6675 6e63 7469   to these functi
-00001510: 6f6e 732e 2053 7065 6369 6669 6361 6c6c  ons. Specificall
-00001520: 792c 2079 6f75 2063 616e 2061 6464 2074  y, you can add t
-00001530: 6865 2066 6f6c 6c6f 7769 6e67 2061 7267  he following arg
-00001540: 756d 656e 7473 2074 6f20 616e 7920 6372  uments to any cr
-00001550: 6561 7465 2063 616c 6c3a 0a2a 204d 4f4e  eate call:.* MON
-00001560: 415f 636f 6e74 6578 745f 6964 3a20 5468  A_context_id: Th
-00001570: 6520 756e 6971 7565 2069 6420 6f66 2074  e unique id of t
-00001580: 6865 2063 6f6e 7465 7874 2069 6e20 7768  he context in wh
-00001590: 6963 6820 7468 6520 6361 6c6c 2069 7320  ich the call is 
-000015a0: 6d61 6465 2e20 4279 2075 7369 6e67 2074  made. By using t
-000015b0: 6869 7320 4944 2079 6f75 2063 616e 2065  his ID you can e
-000015c0: 7870 6f72 7420 6d6f 7265 2064 6174 6120  xport more data 
-000015d0: 746f 204d 6f6e 6120 746f 2074 6865 2073  to Mona to the s
-000015e0: 616d 6520 636f 6e74 6578 7420 6672 6f6d  ame context from
-000015f0: 206f 7468 6572 2070 6c61 6365 732e 2049   other places. I
-00001600: 6620 6e6f 7420 7375 7070 6c69 6564 2c20  f not supplied, 
-00001610: 7468 6520 2269 6422 2066 6965 6c64 206f  the "id" field o
-00001620: 6620 7468 6520 4f70 656e 4149 2045 6e64  f the OpenAI End
-00001630: 706f 696e 7427 7320 7265 7370 6f6e 7365  point's response
-00001640: 2077 696c 6c20 6265 2075 7365 6420 6173   will be used as
-00001650: 2074 6865 204d 6f6e 6120 636f 6e74 6578   the Mona contex
-00001660: 7420 4944 2061 7574 6f6d 6174 6963 616c  t ID automatical
-00001670: 6c79 2e0a 2a20 4d4f 4e41 5f65 7870 6f72  ly..* MONA_expor
-00001680: 745f 7469 6d65 7374 616d 703a 2043 616e  t_timestamp: Can
-00001690: 2062 6520 7573 6564 2074 6f20 7369 6d75   be used to simu
-000016a0: 6c61 7465 2061 7320 6966 2074 6865 2063  late as if the c
-000016b0: 7572 7265 6e74 2063 616c 6c20 7761 7320  urrent call was 
-000016c0: 6d61 6465 2069 6e20 6120 6469 6666 6572  made in a differ
-000016d0: 656e 7420 7469 6d65 2c20 6173 2066 6172  ent time, as far
-000016e0: 2061 7320 4d6f 6e61 2069 7320 636f 6e63   as Mona is conc
-000016f0: 6572 6e65 642e 0a2a 204d 4f4e 415f 6164  erned..* MONA_ad
-00001700: 6469 7469 6f6e 616c 5f64 6174 613a 2041  ditional_data: A
-00001710: 204a 534f 4e2d 7365 7269 616c 697a 6162   JSON-serializab
-00001720: 6c65 2064 6963 7420 7769 7468 2061 6e79  le dict with any
-00001730: 206f 7468 6572 2064 6174 6120 796f 7520   other data you 
-00001740: 7761 6e74 2074 6f20 6164 6420 746f 2074  want to add to t
-00001750: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
-00001760: 6e74 6578 742e 2054 6869 7320 636f 6d65  ntext. This come
-00001770: 7320 696e 2068 616e 6479 2069 6620 796f  s in handy if yo
-00001780: 7520 7761 6e74 2074 6f20 6164 6420 6d6f  u want to add mo
-00001790: 7265 2069 6e66 6f72 6d61 7469 6f6e 2074  re information t
-000017a0: 6f20 7468 6520 6d6f 6e69 746f 7269 6e67  o the monitoring
-000017b0: 2063 6f6e 7465 7820 7468 6174 2069 736e   contex that isn
-000017c0: 2774 2070 6172 7420 6f66 2074 6865 2062  't part of the b
-000017d0: 6173 6963 204f 7065 6e41 4920 4150 4920  asic OpenAI API 
-000017e0: 6361 6c6c 2069 6e66 6f72 6d61 7469 6f6e  call information
-000017f0: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
-00001800: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-00001810: 6120 7370 6563 6966 6963 2074 656d 706c  a specific templ
-00001820: 6174 6520 4944 206f 7220 6966 2074 6869  ate ID or if thi
-00001830: 7320 6361 6c6c 2069 7320 6265 696e 6720  s call is being 
-00001840: 6d61 6465 2066 6f72 2061 2073 7065 6369  made for a speci
-00001850: 6669 6320 6375 7374 6f6d 6572 2049 442c  fic customer ID,
-00001860: 2074 6865 7365 2061 7265 2066 6965 6c64   these are field
-00001870: 7320 796f 7520 6361 6e20 6164 6420 7468  s you can add th
-00001880: 6572 6520 746f 2068 656c 7020 6765 7420  ere to help get 
-00001890: 6675 6c6c 2063 6f6e 7465 7874 2077 6865  full context whe
-000018a0: 6e20 6d6f 6e69 746f 7269 6e67 2077 6974  n monitoring wit
-000018b0: 6820 4d6f 6e61 2e0a 0a45 7861 6d70 6c65  h Mona...Example
-000018c0: 3a0a 6060 6070 790a 7265 7370 6f6e 7365  :.```py.response
-000018d0: 203d 2061 7379 6e63 696f 2e72 756e 286d   = asyncio.run(m
-000018e0: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
-000018f0: 696f 6e2e 6163 7265 6174 6528 0a20 2020  ion.acreate(.   
-00001900: 2065 6e67 696e 653d 6d6f 6465 6c2c 0a20   engine=model,. 
-00001910: 2020 2070 726f 6d70 743d 7072 6f6d 7074     prompt=prompt
-00001920: 2c0a 2020 2020 6d61 785f 746f 6b65 6e73  ,.    max_tokens
-00001930: 3d6d 6178 5f74 6f6b 656e 732c 0a20 2020  =max_tokens,.   
-00001940: 206e 3d6e 2c0a 2020 2020 7465 6d70 6572   n=n,.    temper
-00001950: 6174 7572 653d 7465 6d70 6572 6174 7572  ature=temperatur
-00001960: 652c 0a20 2020 204d 4f4e 415f 6164 6469  e,.    MONA_addi
-00001970: 7469 6f6e 616c 5f64 6174 613d 7b22 6375  tional_data={"cu
-00001980: 7374 6f6d 6572 5f69 6422 3a20 2241 3533  stomer_id": "A53
-00001990: 3132 3531 227d 2c0a 2929 0a70 7269 6e74  1251"},.)).print
-000019a0: 2872 6573 706f 6e73 652e 6368 6f69 6365  (response.choice
-000019b0: 735b 305d 2e74 6578 7429 0a60 6060 0a0a  s[0].text).```..
-000019c0: 2323 2320 5573 696e 6720 4f70 656e 4149  ### Using OpenAI
-000019d0: 2077 6974 6820 5245 5354 2063 616c 6c73   with REST calls
-000019e0: 2069 6e73 7465 6164 206f 6620 4f70 656e   instead of Open
-000019f0: 4149 2773 2050 7974 686f 6e20 636c 6965  AI's Python clie
-00001a00: 6e74 0a49 6e20 736f 6d65 2063 6173 6573  nt.In some cases
-00001a10: 2079 6f75 206d 6179 2063 686f 6f73 6520   you may choose 
-00001a20: 746f 2075 7365 204f 7065 6e41 4927 7320  to use OpenAI's 
-00001a30: 4150 4920 6469 7265 6374 6c79 2077 6974  API directly wit
-00001a40: 6820 5245 5354 2063 616c 6c73 2061 6e64  h REST calls and
-00001a50: 206e 6f74 2075 7369 6e67 204f 7065 6e41   not using OpenA
-00001a60: 4927 7320 5344 4b2e 2046 6f72 2074 6865  I's SDK. For the
-00001a70: 7365 2063 6173 6573 2077 6520 616c 6c6f  se cases we allo
-00001a80: 7720 6120 6d6f 7265 2064 6972 6563 7420  w a more direct 
-00001a90: 6170 7072 6f61 6368 2066 6f72 206c 6f67  approach for log
-00001aa0: 6769 6e67 2074 6f20 4d6f 6e61 2061 7320  ging to Mona as 
-00001ab0: 7765 6c6c 2c20 6279 2075 7369 6e67 2074  well, by using t
-00001ac0: 6865 2022 6765 745f 7265 7374 5f6d 6f6e  he "get_rest_mon
-00001ad0: 6974 6f72 2220 6675 6e63 7469 6f6e 2e20  itor" function. 
-00001ae0: 5365 6520 6578 616d 706c 6520 6265 6c6f  See example belo
-00001af0: 772e 0a0a 6060 6070 790a 2320 4469 7265  w...```py.# Dire
-00001b00: 6374 2052 4553 5420 7573 6167 652c 2077  ct REST usage, w
-00001b10: 6974 686f 7574 204f 7065 6e41 4920 636c  ithout OpenAI cl
-00001b20: 6965 6e74 0a69 6d70 6f72 7420 7265 7175  ient.import requ
-00001b30: 6573 7473 0a66 726f 6d20 6f73 2069 6d70  ests.from os imp
-00001b40: 6f72 7420 656e 7669 726f 6e0a 6672 6f6d  ort environ.from
-00001b50: 206d 6f6e 615f 6f70 656e 6169 2069 6d70   mona_openai imp
-00001b60: 6f72 7420 6765 745f 7265 7374 5f6d 6f6e  ort get_rest_mon
-00001b70: 6974 6f72 0a0a 0a4d 4f4e 415f 4150 495f  itor...MONA_API_
-00001b80: 4b45 5920 3d20 656e 7669 726f 6e2e 6765  KEY = environ.ge
-00001b90: 7428 224d 4f4e 415f 4150 495f 4b45 5922  t("MONA_API_KEY"
-00001ba0: 290a 4d4f 4e41 5f53 4543 5245 5420 3d20  ).MONA_SECRET = 
-00001bb0: 656e 7669 726f 6e2e 6765 7428 224d 4f4e  environ.get("MON
-00001bc0: 415f 5345 4352 4554 2229 0a4d 4f4e 415f  A_SECRET").MONA_
-00001bd0: 4352 4544 5320 3d20 7b0a 2020 2020 226b  CREDS = {.    "k
-00001be0: 6579 223a 204d 4f4e 415f 4150 495f 4b45  ey": MONA_API_KE
-00001bf0: 592c 0a20 2020 2022 7365 6372 6574 223a  Y,.    "secret":
-00001c00: 204d 4f4e 415f 5345 4352 4554 2c0a 7d0a   MONA_SECRET,.}.
-00001c10: 434f 4e54 4558 545f 434c 4153 535f 4e41  CONTEXT_CLASS_NA
-00001c20: 4d45 203d 2022 534f 4d45 5f4d 4f4e 4954  ME = "SOME_MONIT
-00001c30: 4f52 494e 475f 434f 4e54 4558 545f 4e41  ORING_CONTEXT_NA
-00001c40: 4d45 220a 0a23 2047 6574 204d 6f6e 6120  ME"..# Get Mona 
-00001c50: 6c6f 6767 6572 0a6d 6f6e 615f 6c6f 6767  logger.mona_logg
-00001c60: 6572 203d 2067 6574 5f72 6573 745f 6d6f  er = get_rest_mo
-00001c70: 6e69 746f 7228 0a20 2020 2022 436f 6d70  nitor(.    "Comp
-00001c80: 6c65 7469 6f6e 222c 0a20 2020 204d 4f4e  letion",.    MON
-00001c90: 415f 4352 4544 532c 0a20 2020 2043 4f4e  A_CREDS,.    CON
-00001ca0: 5445 5854 5f43 4c41 5353 5f4e 414d 452c  TEXT_CLASS_NAME,
-00001cb0: 0a29 0a0a 2320 5365 7420 7570 2074 6865  .)..# Set up the
-00001cc0: 2041 5049 2065 6e64 706f 696e 7420 5552   API endpoint UR
-00001cd0: 4c20 616e 6420 6175 7468 656e 7469 6361  L and authentica
-00001ce0: 7469 6f6e 2068 6561 6465 7273 0a75 726c  tion headers.url
-00001cf0: 203d 2022 6874 7470 733a 2f2f 6170 692e   = "https://api.
-00001d00: 6f70 656e 6169 2e63 6f6d 2f76 312f 636f  openai.com/v1/co
-00001d10: 6d70 6c65 7469 6f6e 7322 0a68 6561 6465  mpletions".heade
-00001d20: 7273 203d 207b 0a20 2020 2022 436f 6e74  rs = {.    "Cont
-00001d30: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-00001d40: 6963 6174 696f 6e2f 6a73 6f6e 222c 0a20  ication/json",. 
-00001d50: 2020 2022 4175 7468 6f72 697a 6174 696f     "Authorizatio
-00001d60: 6e22 3a20 6622 4265 6172 6572 207b 656e  n": f"Bearer {en
-00001d70: 7669 726f 6e2e 6765 7428 274f 5045 4e5f  viron.get('OPEN_
-00001d80: 4149 5f4b 4559 2729 7d22 2c0a 7d0a 0a23  AI_KEY')}",.}..#
-00001d90: 2053 6574 2075 7020 7468 6520 7265 7175   Set up the requ
-00001da0: 6573 7420 6461 7461 0a64 6174 6120 3d20  est data.data = 
-00001db0: 7b0a 2020 2020 2270 726f 6d70 7422 3a20  {.    "prompt": 
-00001dc0: 7072 6f6d 7074 2c0a 2020 2020 226d 6178  prompt,.    "max
-00001dd0: 5f74 6f6b 656e 7322 3a20 6d61 785f 746f  _tokens": max_to
-00001de0: 6b65 6e73 2c0a 2020 2020 2274 656d 7065  kens,.    "tempe
-00001df0: 7261 7475 7265 223a 2074 656d 7065 7261  rature": tempera
-00001e00: 7475 7265 2c0a 2020 2020 226d 6f64 656c  ture,.    "model
-00001e10: 223a 206d 6f64 656c 2c0a 2020 2020 226e  ": model,.    "n
-00001e20: 223a 206e 2c0a 7d0a 0a23 2054 6865 206c  ": n,.}..# The l
-00001e30: 6f67 5f72 6571 7565 7374 2066 756e 6374  og_request funct
-00001e40: 696f 6e20 7265 7475 726e 7320 7477 6f20  ion returns two 
-00001e50: 6f74 6865 7220 6675 6e63 7469 6f6e 2066  other function f
-00001e60: 6f72 206c 6174 6572 206c 6f67 6769 6e67  or later logging
-00001e70: 0a23 2074 6865 2072 6573 706f 6e73 6520  .# the response 
-00001e80: 6f72 2074 6865 2065 7863 6570 7469 6f6e  or the exception
-00001e90: 2e20 5768 656e 2077 6520 6c61 7465 7220  . When we later 
-00001ea0: 646f 2074 6861 742c 2074 6865 206c 6f67  do that, the log
-00001eb0: 6765 7220 7769 6c6c 0a23 2061 6374 7561  ger will.# actua
-00001ec0: 6c6c 7920 6361 6c63 756c 6174 6520 616c  lly calculate al
-00001ed0: 6c20 7468 6520 7265 6c65 7661 6e74 206d  l the relevant m
-00001ee0: 6574 7269 6373 2061 6e64 2077 696c 6c20  etrics and will 
-00001ef0: 7365 6e64 2074 6865 6d20 746f 0a23 204d  send them to.# M
-00001f00: 6f6e 612e 0a72 6573 706f 6e73 655f 6c6f  ona..response_lo
-00001f10: 6767 6572 2c20 6578 6365 7074 696f 6e5f  gger, exception_
-00001f20: 6c6f 6767 6572 203d 206d 6f6e 615f 6c6f  logger = mona_lo
-00001f30: 6767 6572 2e6c 6f67 5f72 6571 7565 7374  gger.log_request
-00001f40: 280a 2020 2020 6461 7461 2c20 6164 6469  (.    data, addi
-00001f50: 7469 6f6e 616c 5f64 6174 613d 7b22 6375  tional_data={"cu
-00001f60: 7374 6f6d 6572 5f69 6422 3a20 2241 3533  stomer_id": "A53
-00001f70: 3132 3531 227d 0a29 0a0a 7472 793a 0a20  1251"}.)..try:. 
-00001f80: 2020 2023 2053 656e 6420 7468 6520 7265     # Send the re
-00001f90: 7175 6573 7420 746f 2074 6865 2041 5049  quest to the API
-00001fa0: 0a20 2020 2072 6573 706f 6e73 6520 3d20  .    response = 
-00001fb0: 7265 7175 6573 7473 2e70 6f73 7428 7572  requests.post(ur
-00001fc0: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
-00001fd0: 7273 2c20 6a73 6f6e 3d64 6174 6129 0a0a  rs, json=data)..
-00001fe0: 2020 2020 2320 4368 6563 6b20 666f 7220      # Check for 
-00001ff0: 4854 5450 2065 7272 6f72 730a 2020 2020  HTTP errors.    
-00002000: 7265 7370 6f6e 7365 2e72 6169 7365 5f66  response.raise_f
-00002010: 6f72 5f73 7461 7475 7328 290a 0a20 2020  or_status()..   
-00002020: 2023 204c 6f67 2072 6573 706f 6e73 6520   # Log response 
-00002030: 746f 204d 6f6e 610a 2020 2020 7265 7370  to Mona.    resp
-00002040: 6f6e 7365 5f6c 6f67 6765 7228 7265 7370  onse_logger(resp
-00002050: 6f6e 7365 2e6a 736f 6e28 2929 0a20 2020  onse.json()).   
-00002060: 2070 7269 6e74 2872 6573 706f 6e73 652e   print(response.
-00002070: 6a73 6f6e 2829 5b22 6368 6f69 6365 7322  json()["choices"
-00002080: 5d5b 305d 5b22 7465 7874 225d 290a 0a65  ][0]["text"])..e
-00002090: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-000020a0: 6173 2065 7272 3a0a 2020 2020 2320 4c6f  as err:.    # Lo
-000020b0: 6720 6578 6365 7074 696f 6e20 746f 204d  g exception to M
-000020c0: 6f6e 610a 2020 2020 6578 6365 7074 696f  ona.    exceptio
-000020d0: 6e5f 6c6f 6767 6572 2829 0a60 6060 0a0a  n_logger().```..
-000020e0: 2323 2320 5374 7265 616d 2073 7570 706f  ### Stream suppo
-000020f0: 7274 0a0a 4f70 656e 4149 2061 6c6c 6f77  rt..OpenAI allow
-00002100: 7320 7265 6365 6976 696e 6720 7265 7370  s receiving resp
-00002110: 6f6e 7365 7320 6173 2061 2073 7472 6561  onses as a strea
-00002120: 6d20 6f66 2074 6f6b 656e 7320 7573 696e  m of tokens usin
-00002130: 6720 7468 6520 2273 7472 6561 6d22 2070  g the "stream" p
-00002140: 6172 616d 6574 6572 2e20 5768 656e 2074  arameter. When t
-00002150: 6869 7320 6973 2064 6f6e 652c 204d 6f6e  his is done, Mon
-00002160: 6120 7769 6c6c 2063 6f6c 6c65 6374 2061  a will collect a
-00002170: 6c6c 2074 6865 2074 6f6b 656e 7320 696e  ll the tokens in
-00002180: 206d 656d 6f72 7920 616e 6420 7769 6c6c   memory and will
-00002190: 2063 7265 6174 6520 7468 6520 616e 616c   create the anal
-000021a0: 7973 6973 2061 6e64 206c 6f67 206f 7574  ysis and log out
-000021b0: 2074 6865 2064 6174 6120 7468 6520 6d6f   the data the mo
-000021c0: 6d65 6e74 2074 6865 2073 7472 6561 6d20  ment the stream 
-000021d0: 6973 206f 7665 722e 2059 6f75 2064 6f6e  is over. You don
-000021e0: 2774 206e 6565 6420 746f 2064 6f20 616e  't need to do an
-000021f0: 7974 6869 6e67 2074 6f20 6d61 6b65 2074  ything to make t
-00002200: 6869 7320 6861 7070 656e 2e0a 0a53 696e  his happen...Sin
-00002210: 6365 2066 6f72 2073 7472 6561 6d69 6e67  ce for streaming
-00002220: 2072 6573 706f 6e73 6573 204f 7065 6e41   responses OpenA
-00002230: 4920 646f 6573 6e27 7420 7375 7070 6c79  I doesn't supply
-00002240: 2074 6865 2066 756c 6c20 7573 6167 6520   the full usage 
-00002250: 746f 6b65 6e73 2073 756d 6d61 7279 2c20  tokens summary, 
-00002260: 4d6f 6e61 2075 7365 7320 7468 6520 7469  Mona uses the ti
-00002270: 6b74 6f6b 656e 2070 6163 6b61 6765 2074  ktoken package t
-00002280: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00002290: 746f 6b65 6e73 206f 6620 7468 6520 7072  tokens of the pr
-000022a0: 6f6d 7074 2061 6e64 2063 6f6d 706c 6574  ompt and complet
-000022b0: 696f 6e20 616e 6420 6c6f 6720 7468 656d  ion and log them
-000022c0: 2066 6f72 206d 6f6e 6974 6f72 696e 672e   for monitoring.
-000022d0: 0a0a 4e4f 5445 3a20 5374 7265 616d 2069  ..NOTE: Stream i
-000022e0: 7320 6375 7272 656e 746c 7920 6f6e 6c79  s currently only
-000022f0: 2073 7570 706f 7274 6564 2077 6974 6820   supported with 
-00002300: 5344 4b20 7573 6167 652c 2061 6e64 206e  SDK usage, and n
-00002310: 6f74 2077 6974 6820 7573 696e 6720 5245  ot with using RE
-00002320: 5354 2064 6972 6563 746c 792e 0a0a 0a23  ST directly....#
-00002330: 2320 4d6f 6e61 2053 444b 0a0a 5468 6973  # Mona SDK..This
-00002340: 2070 6163 6b61 6765 2075 7365 7320 7468   package uses th
-00002350: 6520 6d6f 6e61 5f73 646b 2070 6163 6b61  e mona_sdk packa
-00002360: 6765 2074 6f20 6578 706f 7274 2074 6865  ge to export the
-00002370: 2072 656c 6576 616e 7420 6461 7461 2074   relevant data t
-00002380: 6f20 4d6f 6e61 2e20 5468 6572 6520 6172  o Mona. There ar
-00002390: 6520 7365 7665 7261 6c20 656e 7669 726f  e several enviro
-000023a0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-000023b0: 796f 7520 6361 6e20 7573 6520 746f 2063  you can use to c
-000023c0: 6f6e 6669 6775 7265 2074 6865 2053 444b  onfigure the SDK
-000023d0: 2773 2062 6568 6176 696f 722e 2046 6f72  's behavior. For
-000023e0: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
-000023f0: 6e20 7365 7420 6974 2075 7020 746f 2072  n set it up to r
-00002400: 6169 7365 2065 7863 6570 7469 6f6e 7320  aise exceptions 
-00002410: 7768 656e 2065 7870 6f72 7469 6e67 2064  when exporting d
-00002420: 6174 6120 746f 204d 6f6e 6120 6661 696c  ata to Mona fail
-00002430: 7320 2869 7420 646f 6573 6e27 7420 646f  s (it doesn't do
-00002440: 2074 6861 7420 6279 2064 6566 6175 6c74   that by default
-00002450: 292e 0a0a 2323 204d 6f6e 6974 6f72 696e  )...## Monitorin
-00002460: 6720 666f 7220 7072 6f66 616e 6974 790a  g for profanity.
-00002470: 0a4d 6f6e 6120 7573 6573 2074 6865 2061  .Mona uses the a
-00002480: 6c74 2d70 726f 6661 6e69 7479 2d63 6865  lt-profanity-che
-00002490: 636b 2070 6163 616b 6765 2028 6874 7470  ck pacakge (http
-000024a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000024b0: 6a65 6374 2f61 6c74 2d70 726f 6661 6e69  ject/alt-profani
-000024c0: 7479 2d63 6865 636b 2f29 2074 6f20 6372  ty-check/) to cr
-000024d0: 6561 7465 2062 6f74 6820 626f 6f6c 6561  eate both boolea
-000024e0: 6e20 7072 6564 6963 7469 6f6e 7320 616e  n predictions an
-000024f0: 6420 7072 6f62 6162 696c 7479 2073 636f  d probabilty sco
-00002500: 7265 7320 666f 7220 7468 6520 6578 6973  res for the exis
-00002510: 7465 6e63 6520 6f66 2070 726f 6661 6e69  tence of profani
-00002520: 7479 2062 6f74 6820 696e 2074 6865 2070  ty both in the p
-00002530: 726f 6d70 7420 616e 6420 696e 2074 6865  rompt and in the
-00002540: 2072 6573 706f 6e73 6573 2e20 5765 2075   responses. We u
-00002550: 7365 2074 6865 2062 7569 6c74 2069 6e20  se the built in 
-00002560: 7061 636b 6167 6520 6d65 7468 6f64 7320  package methods 
-00002570: 666f 7220 7468 6174 2e20 4966 2079 6f75  for that. If you
-00002580: 2077 616e 742c 2066 6f72 2065 7861 6d70   want, for examp
-00002590: 6c65 2c20 746f 2075 7365 2061 2064 6966  le, to use a dif
-000025a0: 6665 7265 6e74 2070 726f 6261 6269 6c69  ferent probabili
-000025b0: 7479 2074 6872 6573 686f 6c64 2066 6f72  ty threshold for
-000025c0: 2074 6865 2062 6f6f 6c65 616e 2070 7265   the boolean pre
-000025d0: 6469 6374 696f 6e2c 2079 6f75 2063 616e  diction, you can
-000025e0: 2064 6f20 7468 6174 2062 7920 6368 616e   do that by chan
-000025f0: 6769 6e67 2079 6f75 7220 4d6f 6e61 2063  ging your Mona c
-00002600: 6f6e 6669 6720 6f6e 2074 6865 204d 6f6e  onfig on the Mon
-00002610: 6120 6461 7368 626f 6172 642e 0a         a dashboard..
+000002f0: 3d22 3138 3022 2f3e 0a3c 2f70 3e0a 0a3c  ="180"/>.</p>..<
+00000300: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000310: 3e3c 6120 7461 7267 6574 3d22 5f62 6c61  ><a target="_bla
+00000320: 6e6b 2220 6872 6566 3d22 6874 7470 733a  nk" href="https:
+00000330: 2f2f 6d6f 6e61 6c61 6273 2e77 6973 7469  //monalabs.wisti
+00000340: 612e 636f 6d2f 6d65 6469 6173 2f6c 3678  a.com/medias/l6x
+00000350: 6d64 6a33 6364 363f 7776 6964 656f 3d6c  mdj3cd6?wvideo=l
+00000360: 3678 6d64 6a33 6364 3622 3e3c 696d 6720  6xmdj3cd6"><img 
+00000370: 7372 633d 2268 7474 7073 3a2f 2f65 6d62  src="https://emb
+00000380: 6564 2d73 736c 2e77 6973 7469 612e 636f  ed-ssl.wistia.co
+00000390: 6d2f 6465 6c69 7665 7269 6573 2f63 3135  m/deliveries/c15
+000003a0: 6262 3631 3661 3338 3966 6137 6437 3532  bb616a389fa7d752
+000003b0: 3936 3863 6362 3361 6632 6162 342e 6a70  968ccb3af2ab4.jp
+000003c0: 673f 7769 7374 6961 2d6c 3678 6d64 6a33  g?wistia-l6xmdj3
+000003d0: 6364 362d 312d 6c36 786d 646a 3363 6436  cd6-1-l6xmdj3cd6
+000003e0: 2d76 6964 656f 2d74 6875 6d62 6e61 696c  -video-thumbnail
+000003f0: 3d31 2661 6d70 3b69 6d61 6765 5f70 6c61  =1&amp;image_pla
+00000400: 795f 6275 7474 6f6e 5f73 697a 653d 3278  y_button_size=2x
+00000410: 2661 6d70 3b69 6d61 6765 5f63 726f 705f  &amp;image_crop_
+00000420: 7265 7369 7a65 643d 3936 3078 3534 3026  resized=960x540&
+00000430: 616d 703b 696d 6167 655f 706c 6179 5f62  amp;image_play_b
+00000440: 7574 746f 6e3d 3126 616d 703b 696d 6167  utton=1&amp;imag
+00000450: 655f 706c 6179 5f62 7574 746f 6e5f 636f  e_play_button_co
+00000460: 6c6f 723d 3636 6337 6431 6530 2220 7769  lor=66c7d1e0" wi
+00000470: 6474 683d 2234 3030 2220 6865 6967 6874  dth="400" height
+00000480: 3d22 3232 3522 2073 7479 6c65 3d22 7769  ="225" style="wi
+00000490: 6474 683a 2034 3030 7078 3b20 6865 6967  dth: 400px; heig
+000004a0: 6874 3a20 3232 3570 783b 223e 3c2f 613e  ht: 225px;"></a>
+000004b0: 3c2f 703e 3c70 2061 6c69 676e 3d22 6365  </p><p align="ce
+000004c0: 6e74 6572 223e 3c61 2068 7265 663d 2268  nter"><a href="h
+000004d0: 7474 7073 3a2f 2f6d 6f6e 616c 6162 732e  ttps://monalabs.
+000004e0: 7769 7374 6961 2e63 6f6d 2f6d 6564 6961  wistia.com/media
+000004f0: 732f 6c36 786d 646a 3363 6436 3f77 7669  s/l6xmdj3cd6?wvi
+00000500: 6465 6f3d 6c36 786d 646a 3363 6436 223e  deo=l6xmdj3cd6">
+00000510: 4f70 656e 4149 2047 5054 2049 6e74 6567  OpenAI GPT Integ
+00000520: 7261 7469 6f6e 2054 7574 6f72 6961 6c3c  ration Tutorial<
+00000530: 2f61 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e  /a></p>...Use on
+00000540: 6520 6c69 6e65 206f 6620 636f 6465 2074  e line of code t
+00000550: 6f20 6765 7420 696e 7374 616e 7420 6c69  o get instant li
+00000560: 7665 206d 6f6e 6974 6f72 696e 6720 666f  ve monitoring fo
+00000570: 7220 796f 7572 204f 7065 6e41 4920 7573  r your OpenAI us
+00000580: 6167 6520 696e 636c 7564 696e 673a 0a2a  age including:.*
+00000590: 2054 6f6b 656e 7320 7573 6167 650a 2a20   Tokens usage.* 
+000005a0: 4861 6c6c 7563 696e 6174 696f 6e20 616c  Hallucination al
+000005b0: 6572 7473 0a2a 2050 726f 6661 6e69 7479  erts.* Profanity
+000005c0: 2061 6e64 2070 7269 7661 6379 2061 6e61   and privacy ana
+000005d0: 6c79 7365 730a 2a20 4265 6861 7669 6f72  lyses.* Behavior
+000005e0: 616c 2064 7269 6674 7320 616e 6420 616e  al drifts and an
+000005f0: 6f6d 616c 6965 730a 2a20 4c61 6e67 4368  omalies.* LangCh
+00000600: 6169 6e20 7375 7070 6f72 740a 2a20 4d75  ain support.* Mu
+00000610: 6368 206d 7563 6820 6d6f 7265 0a0a 2323  ch much more..##
+00000620: 2053 6574 7469 6e67 2055 700a 0a2d 2054   Setting Up..- T
+00000630: 4f44 4f3a 2041 6464 2070 6172 7420 6162  ODO: Add part ab
+00000640: 6f75 7420 4d6f 6e61 2072 6567 6973 7472  out Mona registr
+00000650: 6174 696f 6e20 7769 7468 2061 206c 696e  ation with a lin
+00000660: 6b20 746f 2074 6865 2072 656c 6576 616e  k to the relevan
+00000670: 7420 6c61 6e64 696e 6720 7061 6765 2077  t landing page w
+00000680: 6865 7265 2074 6865 2072 6561 6465 7220  here the reader 
+00000690: 6361 6e20 7369 676e 2075 702e 0a60 6060  can sign up..```
+000006a0: 636f 6e73 6f6c 650a 2420 7069 7020 696e  console.$ pip in
+000006b0: 7374 616c 6c20 6d6f 6e61 5f6f 7065 6e61  stall mona_opena
+000006c0: 690a 6060 600a 0a23 2320 5175 6963 6b20  i.```..## Quick 
+000006d0: 5374 6172 7420 616e 6420 4578 616d 706c  Start and Exampl
+000006e0: 650a 0a45 7861 6d70 6c65 2062 6f69 6c65  e..Example boile
+000006f0: 7270 6c61 7465 2063 6f64 6520 666f 7220  rplate code for 
+00000700: 626f 7468 2073 796e 6320 616e 6420 6173  both sync and as
+00000710: 796e 6320 7573 6167 6520 6973 2067 6976  ync usage is giv
+00000720: 656e 2069 6e20 7468 6520 6669 6c65 2022  en in the file "
+00000730: 6578 616d 706c 655f 7573 6167 652e 7079  example_usage.py
+00000740: 2220 616e 6420 6865 7265 3a0a 6060 6070  " and here:.```p
+00000750: 790a 6672 6f6d 206f 7320 696d 706f 7274  y.from os import
+00000760: 2065 6e76 6972 6f6e 0a69 6d70 6f72 7420   environ.import 
+00000770: 6173 796e 6369 6f0a 696d 706f 7274 206f  asyncio.import o
+00000780: 7065 6e61 690a 0a66 726f 6d20 6d6f 6e61  penai..from mona
+00000790: 5f6f 7065 6e61 6920 696d 706f 7274 206d  _openai import m
+000007a0: 6f6e 6974 6f72 0a0a 6f70 656e 6169 2e61  onitor..openai.a
+000007b0: 7069 5f6b 6579 203d 2065 6e76 6972 6f6e  pi_key = environ
+000007c0: 2e67 6574 2822 4f50 454e 5f41 495f 4b45  .get("OPEN_AI_KE
+000007d0: 5922 290a 0a4d 4f4e 415f 4150 495f 4b45  Y")..MONA_API_KE
+000007e0: 5920 3d20 656e 7669 726f 6e2e 6765 7428  Y = environ.get(
+000007f0: 224d 4f4e 415f 4150 495f 4b45 5922 290a  "MONA_API_KEY").
+00000800: 4d4f 4e41 5f53 4543 5245 5420 3d20 656e  MONA_SECRET = en
+00000810: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
+00000820: 5345 4352 4554 2229 0a4d 4f4e 415f 4352  SECRET").MONA_CR
+00000830: 4544 5320 3d20 7b0a 2020 2020 226b 6579  EDS = {.    "key
+00000840: 223a 204d 4f4e 415f 4150 495f 4b45 592c  ": MONA_API_KEY,
+00000850: 0a20 2020 2022 7365 6372 6574 223a 204d  .    "secret": M
+00000860: 4f4e 415f 5345 4352 4554 2c0a 7d0a 434f  ONA_SECRET,.}.CO
+00000870: 4e54 4558 545f 434c 4153 535f 4e41 4d45  NTEXT_CLASS_NAME
+00000880: 203d 2022 534f 4d45 5f4d 4f4e 4954 4f52   = "SOME_MONITOR
+00000890: 494e 475f 434f 4e54 4558 545f 4e41 4d45  ING_CONTEXT_NAME
+000008a0: 220a 0a0a 6d6f 6e69 746f 7265 645f 636f  "...monitored_co
+000008b0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
+000008c0: 6f72 280a 2020 2020 6f70 656e 6169 2e43  or(.    openai.C
+000008d0: 6f6d 706c 6574 696f 6e2c 0a20 2020 204d  ompletion,.    M
+000008e0: 4f4e 415f 4352 4544 532c 0a20 2020 2043  ONA_CREDS,.    C
+000008f0: 4f4e 5445 5854 5f43 4c41 5353 5f4e 414d  ONTEXT_CLASS_NAM
+00000900: 452c 0a29 0a0a 0a70 726f 6d70 7420 3d20  E,.)...prompt = 
+00000910: 2249 2077 616e 7420 746f 2067 656e 6572  "I want to gener
+00000920: 6174 6520 736f 6d65 2074 6578 7420 6162  ate some text ab
+00000930: 6f75 7420 220a 6d6f 6465 6c20 3d20 2274  out ".model = "t
+00000940: 6578 742d 6164 612d 3030 3122 0a74 656d  ext-ada-001".tem
+00000950: 7065 7261 7475 7265 203d 2030 2e36 0a6d  perature = 0.6.m
+00000960: 6178 5f74 6f6b 656e 7320 3d20 350a 6e20  ax_tokens = 5.n 
+00000970: 3d20 310a 0a23 2052 6567 756c 6172 2028  = 1..# Regular (
+00000980: 7379 6e63 2920 7573 6167 650a 7265 7370  sync) usage.resp
+00000990: 6f6e 7365 203d 206d 6f6e 6974 6f72 6564  onse = monitored
+000009a0: 5f63 6f6d 706c 6574 696f 6e2e 6372 6561  _completion.crea
+000009b0: 7465 280a 2020 2020 656e 6769 6e65 3d6d  te(.    engine=m
+000009c0: 6f64 656c 2c0a 2020 2020 7072 6f6d 7074  odel,.    prompt
+000009d0: 3d70 726f 6d70 742c 0a20 2020 206d 6178  =prompt,.    max
+000009e0: 5f74 6f6b 656e 733d 6d61 785f 746f 6b65  _tokens=max_toke
+000009f0: 6e73 2c0a 2020 2020 6e3d 6e2c 0a20 2020  ns,.    n=n,.   
+00000a00: 2074 656d 7065 7261 7475 7265 3d74 656d   temperature=tem
+00000a10: 7065 7261 7475 7265 2c0a 2020 2020 4d4f  perature,.    MO
+00000a20: 4e41 5f61 6464 6974 696f 6e61 6c5f 6461  NA_additional_da
+00000a30: 7461 3d7b 2263 7573 746f 6d65 725f 6964  ta={"customer_id
+00000a40: 223a 2022 4135 3331 3235 3122 7d2c 0a29  ": "A531251"},.)
+00000a50: 0a70 7269 6e74 2872 6573 706f 6e73 652e  .print(response.
+00000a60: 6368 6f69 6365 735b 305d 2e74 6578 7429  choices[0].text)
+00000a70: 0a0a 2320 4173 796e 6320 7573 6167 650a  ..# Async usage.
+00000a80: 7265 7370 6f6e 7365 203d 2061 7379 6e63  response = async
+00000a90: 696f 2e72 756e 286d 6f6e 6974 6f72 6564  io.run(monitored
+00000aa0: 5f63 6f6d 706c 6574 696f 6e2e 6163 7265  _completion.acre
+00000ab0: 6174 6528 0a20 2020 2065 6e67 696e 653d  ate(.    engine=
+00000ac0: 6d6f 6465 6c2c 0a20 2020 2070 726f 6d70  model,.    promp
+00000ad0: 743d 7072 6f6d 7074 2c0a 2020 2020 6d61  t=prompt,.    ma
+00000ae0: 785f 746f 6b65 6e73 3d6d 6178 5f74 6f6b  x_tokens=max_tok
+00000af0: 656e 732c 0a20 2020 206e 3d6e 2c0a 2020  ens,.    n=n,.  
+00000b00: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
+00000b10: 6d70 6572 6174 7572 652c 0a20 2020 204d  mperature,.    M
+00000b20: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
+00000b30: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+00000b40: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
+00000b50: 2929 0a0a 7072 696e 7428 7265 7370 6f6e  ))..print(respon
+00000b60: 7365 2e63 686f 6963 6573 5b30 5d2e 7465  se.choices[0].te
+00000b70: 7874 290a 6060 600a 2323 2053 7570 706f  xt).```.## Suppo
+00000b80: 7274 6564 204f 7065 6e41 4920 4150 4973  rted OpenAI APIs
+00000b90: 0a43 7572 7265 6e74 6c79 2074 6869 7320  .Currently this 
+00000ba0: 636c 6965 6e74 2073 7570 706f 7274 7320  client supports 
+00000bb0: 606f 7065 6e61 692e 436f 6d70 6c65 7469  `openai.Completi
+00000bc0: 6f6e 6020 616e 6420 606f 7065 6e61 692e  on` and `openai.
+00000bd0: 4368 6174 436f 6d70 6c65 7469 6f6e 602e  ChatCompletion`.
+00000be0: 204d 6f6e 6120 6361 6e20 7375 7070 6f72   Mona can suppor
+00000bf0: 7420 7072 6f63 6573 7365 7320 6261 7365  t processes base
+00000c00: 6420 6f6e 206f 7468 6572 2041 5049 7320  d on other APIs 
+00000c10: 616e 6420 616c 736f 206e 6f6e 2d4f 7065  and also non-Ope
+00000c20: 6e41 492d 6261 7365 6420 6170 7073 2e0a  nAI-based apps..
+00000c30: 4966 2079 6f75 2068 6176 6520 6120 6469  If you have a di
+00000c40: 6666 6572 7265 6e74 2075 7365 2d63 6173  fferrent use-cas
+00000c50: 652c 2077 6527 6420 6c6f 7665 2074 6f20  e, we'd love to 
+00000c60: 6865 6172 2061 626f 7574 2069 7421 2050  hear about it! P
+00000c70: 6c65 6173 6520 656d 6169 6c20 7573 2061  lease email us a
+00000c80: 7420 7375 7070 6f72 7440 6d6f 6e61 6c61  t support@monala
+00000c90: 6273 2e69 6f2e 0a0a 2323 2055 7361 6765  bs.io...## Usage
+00000ca0: 0a23 2323 2049 6e69 7469 616c 697a 6174  .### Initializat
+00000cb0: 696f 6e0a 0a54 6865 206d 6169 6e20 616e  ion..The main an
+00000cc0: 6420 6f6e 6c79 2066 756e 6374 696f 6e20  d only function 
+00000cd0: 6578 706f 7365 6420 696e 2074 6869 7320  exposed in this 
+00000ce0: 7061 636b 6167 6520 6973 2060 6d6f 6e69  package is `moni
+00000cf0: 746f 7260 2e0a 6060 6070 790a 696d 706f  tor`..```py.impo
+00000d00: 7274 206f 7065 6e61 690a 0a66 726f 6d20  rt openai..from 
+00000d10: 6d6f 6e61 5f6f 7065 6e61 6920 696d 706f  mona_openai impo
+00000d20: 7274 206d 6f6e 6974 6f72 0a0a 6f70 656e  rt monitor..open
+00000d30: 6169 2e61 7069 5f6b 6579 203d 2065 6e76  ai.api_key = env
+00000d40: 6972 6f6e 2e67 6574 2822 4f50 454e 5f41  iron.get("OPEN_A
+00000d50: 495f 4b45 5922 290a 0a6d 6f6e 6974 6f72  I_KEY")..monitor
+00000d60: 6564 5f63 6f6d 706c 6574 696f 6e20 3d20  ed_completion = 
+00000d70: 6d6f 6e69 746f 7228 0a20 2020 206f 7065  monitor(.    ope
+00000d80: 6e61 692e 436f 6d70 6c65 7469 6f6e 2c0a  nai.Completion,.
+00000d90: 2020 2020 280a 2020 2020 2020 2020 656e      (.        en
+00000da0: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
+00000db0: 4150 495f 4b45 5922 292c 0a20 2020 2020  API_KEY"),.     
+00000dc0: 2020 2065 6e76 6972 6f6e 2e67 6574 2822     environ.get("
+00000dd0: 4d4f 4e41 5f53 4543 5245 5422 292c 0a20  MONA_SECRET"),. 
+00000de0: 2020 2029 2c0a 2020 2020 2253 4f4d 455f     ),.    "SOME_
+00000df0: 4d4f 4e49 544f 5249 4e47 5f43 4f4e 5445  MONITORING_CONTE
+00000e00: 5854 5f4e 414d 4522 2c0a 2020 2020 7b22  XT_NAME",.    {"
+00000e10: 616e 616c 7973 6973 223a 207b 2270 726f  analysis": {"pro
+00000e20: 6661 6e69 7479 223a 2046 616c 7365 7d7d  fanity": False}}
+00000e30: 0a29 0a0a 2e2e 2e0a 0a6d 6f6e 6974 6f72  .).......monitor
+00000e40: 6564 5f63 6f6d 706c 6574 696f 6e2e 6372  ed_completion.cr
+00000e50: 6561 7465 282e 2e2e 290a 6060 600a 0a54  eate(...).```..T
+00000e60: 6865 2060 6d6f 6e69 746f 7260 2066 756e  he `monitor` fun
+00000e70: 6374 696f 6e20 7265 7475 726e 7320 746f  ction returns to
+00000e80: 2079 6f75 2061 2063 6c61 7373 2074 6861   you a class tha
+00000e90: 7420 7772 6170 7320 7468 6520 6f72 6967  t wraps the orig
+00000ea0: 696e 616c 206f 7065 6e61 6920 656e 6470  inal openai endp
+00000eb0: 6f69 6e74 2063 6c61 7373 2079 6f75 2070  oint class you p
+00000ec0: 726f 7669 6465 2c20 7769 7468 2061 6e20  rovide, with an 
+00000ed0: 6571 7569 7661 6c65 6e74 2041 5049 2028  equivalent API (
+00000ee0: 6265 7369 6465 7320 736f 6d65 2061 6464  besides some add
+00000ef0: 6974 696f 6e73 206c 6973 7465 6420 6265  itions listed be
+00000f00: 6c6f 7729 2e0a 596f 7520 6361 6e20 7468  low)..You can th
+00000f10: 656e 2075 7365 2074 6865 2072 6574 7572  en use the retur
+00000f20: 6e65 6420 636c 6173 7327 2022 6372 6561  ned class' "crea
+00000f30: 7465 2220 616e 6420 2261 6372 6561 7465  te" and "acreate
+00000f40: 2220 6675 6e63 7469 6f6e 7320 6a75 7374  " functions just
+00000f50: 2061 7320 796f 7520 776f 756c 6420 6265   as you would be
+00000f60: 666f 7265 2c20 6f6e 6c79 206e 6f77 2c20  fore, only now, 
+00000f70: 6265 7369 6465 7320 6765 7474 696e 6720  besides getting 
+00000f80: 7468 6520 7265 7175 6573 7465 6420 6f70  the requested op
+00000f90: 656e 4149 2066 756e 6374 696f 6e61 6c69  enAI functionali
+00000fa0: 7479 2c20 7468 6973 2063 6c69 656e 7420  ty, this client 
+00000fb0: 7769 6c6c 206c 6f67 206f 7574 2074 6f20  will log out to 
+00000fc0: 4d6f 6e61 2773 2073 6572 7665 7220 7468  Mona's server th
+00000fd0: 6520 7061 7261 6d65 7465 7273 2079 6f75  e parameters you
+00000fe0: 2075 7365 6420 2865 2e67 2e2c 2074 656d   used (e.g., tem
+00000ff0: 7065 7261 7475 7265 292c 2064 6174 6120  perature), data 
+00001000: 6162 6f75 7420 7468 6520 7265 7370 6f6e  about the respon
+00001010: 7365 2066 726f 6d20 4f70 656e 4149 2773  se from OpenAI's
+00001020: 2073 6572 7665 722c 2061 6e64 2063 7573   server, and cus
+00001030: 746f 6d20 616e 616c 7973 6573 2061 626f  tom analyses abo
+00001040: 7574 2074 6865 2063 616c 6c20 2865 2e67  ut the call (e.g
+00001050: 2e2c 2070 726f 6661 6e69 7479 2073 636f  ., profanity sco
+00001060: 7265 732c 2070 7269 7661 6379 2063 6865  res, privacy che
+00001070: 636b 7320 666f 7220 656d 6169 6c73 2f70  cks for emails/p
+00001080: 686f 6e65 206e 756d 6265 7273 2066 6f75  hone numbers fou
+00001090: 6e64 2069 6e20 7468 6520 7465 7874 732c  nd in the texts,
+000010a0: 2074 6578 7475 616c 2061 6e61 6c79 7365   textual analyse
+000010b0: 732c 2065 7463 2e2e 2e29 0a0a 5468 6520  s, etc...)..The 
+000010c0: 606d 6f6e 6974 6f72 6020 6675 6e63 7469  `monitor` functi
+000010d0: 6f6e 2072 6563 6569 7665 7320 7468 6520  on receives the 
+000010e0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
+000010f0: 6e74 733a 0a6f 7065 6e61 695f 636c 6173  nts:.openai_clas
+00001100: 733a 2041 6e20 4f70 656e 4149 2041 5049  s: An OpenAI API
+00001110: 2063 6c61 7373 2074 6f20 7772 6170 2077   class to wrap w
+00001120: 6974 6820 6d6f 6e69 746f 7269 6e67 2063  ith monitoring c
+00001130: 6170 6162 696c 7469 6573 2e0a 6d6f 6e61  apabilties..mona
+00001140: 5f63 7265 6473 3a20 4120 6469 6374 2028  _creds: A dict (
+00001150: 636f 6e74 6169 6e69 6e67 2022 6b65 7922  containing "key"
+00001160: 2061 6e64 2022 7365 6372 6574 2229 206f   and "secret") o
+00001170: 7220 7061 6972 2028 7475 706c 6529 206f  r pair (tuple) o
+00001180: 6620 4d6f 6e61 2041 5049 206b 6579 2061  f Mona API key a
+00001190: 6e64 2073 6563 7265 7420 746f 2073 6574  nd secret to set
+000011a0: 2075 7020 4d6f 6e61 2773 2063 6c69 656e   up Mona's clien
+000011b0: 7473 2066 726f 6d20 6974 7320 5344 4b2e  ts from its SDK.
+000011c0: 0a63 6f6e 7465 7874 5f63 6c61 7373 3a20  .context_class: 
+000011d0: 5468 6520 4d6f 6e61 2063 6f6e 7465 7874  The Mona context
+000011e0: 2063 6c61 7373 206e 616d 6520 746f 2075   class name to u
+000011f0: 7365 2066 6f72 206d 6f6e 6974 6f72 696e  se for monitorin
+00001200: 672e 2055 7365 2061 2063 6f6e 7374 616e  g. Use a constan
+00001210: 7420 6e61 6d65 206f 6620 796f 7572 2063  t name of your c
+00001220: 686f 6963 652e 0a73 7065 6373 3a20 4120  hoice..specs: A 
+00001230: 6469 6374 696f 6e61 7279 206f 6620 7370  dictionary of sp
+00001240: 6563 6966 6963 6174 696f 6e73 2073 7563  ecifications suc
+00001250: 6820 6173 206d 6f6e 6974 6f72 696e 6720  h as monitoring 
+00001260: 7361 6d70 6c69 6e67 2072 6174 696f 2e0a  sampling ratio..
+00001270: 0a23 2323 2320 5370 6563 730a 5468 6520  .#### Specs.The 
+00001280: 7370 6563 7320 6172 6720 616c 6c6f 7773  specs arg allows
+00001290: 2079 6f75 2074 6f20 636f 6e66 6967 7572   you to configur
+000012a0: 6520 7768 6174 2073 686f 756c 6420 6265  e what should be
+000012b0: 206d 6f6e 6974 6f72 6564 2e20 4974 2065   monitored. It e
+000012c0: 7870 6563 7473 2061 2070 7974 686f 6e20  xpects a python 
+000012d0: 6469 6374 2077 6974 6820 7468 6520 666f  dict with the fo
+000012e0: 6c6c 776f 696e 6720 706f 7373 6962 6c65  llwoing possible
+000012f0: 206b 6579 733a 0a2a 2073 616d 706c 696e   keys:.* samplin
+00001300: 675f 7261 7469 6f20 2831 293a 2041 206e  g_ratio (1): A n
+00001310: 756d 6265 7220 6265 7477 6565 6e20 3020  umber between 0 
+00001320: 616e 6420 3120 666f 7220 686f 7720 6f66  and 1 for how of
+00001330: 7465 6e20 7368 6f75 6c64 2074 6865 2063  ten should the c
+00001340: 616c 6c20 6265 206c 6f67 6765 642e 0a2a  all be logged..*
+00001350: 2061 766f 6964 5f6d 6f6e 6974 6f72 696e   avoid_monitorin
+00001360: 675f 6578 6365 7074 696f 6e73 2028 4661  g_exceptions (Fa
+00001370: 6c73 6529 3a20 5768 6574 6865 7220 6f72  lse): Whether or
+00001380: 206e 6f74 2074 6f20 6c6f 6720 6f75 7420   not to log out 
+00001390: 746f 204d 6f6e 6120 7768 656e 2074 6865  to Mona when the
+000013a0: 7265 2069 7320 616e 204f 7065 6e41 4920  re is an OpenAI 
+000013b0: 6578 6365 7074 696f 6e2e 2044 6566 6175  exception. Defau
+000013c0: 6c74 2069 7320 746f 2074 7261 636b 2065  lt is to track e
+000013d0: 7863 6570 7469 6f6e 7320 2d20 616e 6420  xceptions - and 
+000013e0: 4d6f 6e61 2077 696c 6c20 616c 6572 7420  Mona will alert 
+000013f0: 796f 7520 6f6e 2074 6869 6e67 7320 6c69  you on things li
+00001400: 6b65 2061 206a 756d 7020 696e 206e 756d  ke a jump in num
+00001410: 6265 7220 6f66 2065 7863 6570 7469 6f6e  ber of exception
+00001420: 730a 2a20 6578 706f 7274 5f70 726f 6d70  s.* export_promp
+00001430: 7420 2846 616c 7365 293a 2057 6865 7468  t (False): Wheth
+00001440: 6572 204d 6f6e 6120 7368 6f75 6c64 2065  er Mona should e
+00001450: 7870 6f72 7420 7468 6520 6163 7475 616c  xport the actual
+00001460: 2070 726f 6d70 7420 7465 7874 2e20 4265   prompt text. Be
+00001470: 2064 6566 6175 6c74 2073 6574 2074 6f20   default set to 
+00001480: 4661 6c73 6520 746f 2061 766f 6964 2070  False to avoid p
+00001490: 7269 7661 6379 2063 6f6e 6365 726e 732e  rivacy concerns.
+000014a0: 0a2a 2065 7870 6f72 745f 7265 7370 6f6e  .* export_respon
+000014b0: 7365 5f74 6578 7473 2028 4661 6c73 6529  se_texts (False)
+000014c0: 3a20 5768 6574 6865 7220 4d6f 6e61 2073  : Whether Mona s
+000014d0: 686f 756c 6420 6578 706f 7274 2074 6865  hould export the
+000014e0: 2061 6374 7561 6c20 7265 7370 6f6e 7365   actual response
+000014f0: 2074 6578 7473 2e20 4265 2064 6566 6175   texts. Be defau
+00001500: 6c74 2073 6574 2074 6f20 4661 6c73 6520  lt set to False 
+00001510: 746f 2061 766f 6964 2070 7269 7661 6379  to avoid privacy
+00001520: 2063 6f6e 6365 726e 732e 0a2a 2061 6e61   concerns..* ana
+00001530: 6c79 7369 733a 2041 2064 6963 7469 6f6e  lysis: A diction
+00001540: 6172 7920 6d61 7070 696e 6720 6561 6368  ary mapping each
+00001550: 2061 6e61 6c79 7369 7320 7479 7065 2074   analysis type t
+00001560: 6f20 6120 626f 6f6c 6561 6e20 7661 6c75  o a boolean valu
+00001570: 6520 7465 6c6c 696e 6720 7468 6520 636c  e telling the cl
+00001580: 6965 6e74 2077 6865 7468 6572 206f 7220  ient whether or 
+00001590: 6e6f 7420 746f 2072 756e 2073 6169 6420  not to run said 
+000015a0: 616e 616c 7973 6973 2061 6e64 206c 6f67  analysis and log
+000015b0: 2069 7420 746f 204d 6f6e 612e 2050 6f73   it to Mona. Pos
+000015c0: 7369 626c 6520 6f70 7469 6f6e 7320 6375  sible options cu
+000015d0: 7272 656e 746c 7920 6172 6520 2270 7269  rrently are "pri
+000015e0: 7661 6379 222c 2022 7072 6f66 616e 6974  vacy", "profanit
+000015f0: 7922 2c20 616e 6420 2274 6578 7475 616c  y", and "textual
+00001600: 222e 2042 7920 6465 6661 756c 742c 2061  ". By default, a
+00001610: 6c6c 2061 6e61 6c79 7365 7320 7461 6b65  ll analyses take
+00001620: 2070 6c61 6365 2061 6e64 2061 7265 206c   place and are l
+00001630: 6f67 6765 6420 6f75 7420 746f 204d 6f6e  ogged out to Mon
+00001640: 612e 0a0a 2323 2320 4361 7061 6269 6c69  a...### Capabili
+00001650: 7469 6573 2064 7572 696e 6720 4150 4920  ties during API 
+00001660: 6361 6c6c 730a 0a41 6674 6572 2077 7261  calls..After wra
+00001670: 7070 696e 6720 796f 7572 2065 6e64 706f  pping your endpo
+00001680: 696e 7420 7769 7468 2060 6d6f 6e69 746f  int with `monito
+00001690: 7260 2c20 796f 7520 7265 616c 6c79 2064  r`, you really d
+000016a0: 6f6e 2774 206e 6565 6420 746f 2064 6f20  on't need to do 
+000016b0: 616e 7974 6869 6e67 2065 6c73 652e 2057  anything else. W
+000016c0: 6865 6e20 7573 696e 6720 6063 7265 6174  hen using `creat
+000016d0: 6560 206f 7220 6061 6372 6561 7465 6020  e` or `acreate` 
+000016e0: 6461 7461 2077 696c 6c20 6265 2074 7261  data will be tra
+000016f0: 636b 6564 2061 6e64 206d 6f6e 6974 6f72  cked and monitor
+00001700: 696e 6720 7769 6c6c 2074 616b 6520 706c  ing will take pl
+00001710: 6163 652e 0a0a 5468 6572 6520 6172 652c  ace...There are,
+00001720: 2068 6f77 6576 6572 2c20 7365 7665 7261   however, severa
+00001730: 6c20 6361 7061 6269 6c69 7469 6573 2074  l capabilities t
+00001740: 6861 7420 6172 6520 6164 6465 6420 746f  hat are added to
+00001750: 2074 6865 7365 2066 756e 6374 696f 6e73   these functions
+00001760: 2e20 5370 6563 6966 6963 616c 6c79 2c20  . Specifically, 
+00001770: 796f 7520 6361 6e20 6164 6420 7468 6520  you can add the 
+00001780: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
+00001790: 6e74 7320 746f 2061 6e79 2063 7265 6174  nts to any creat
+000017a0: 6520 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63  e call:.* MONA_c
+000017b0: 6f6e 7465 7874 5f69 643a 2054 6865 2075  ontext_id: The u
+000017c0: 6e69 7175 6520 6964 206f 6620 7468 6520  nique id of the 
+000017d0: 636f 6e74 6578 7420 696e 2077 6869 6368  context in which
+000017e0: 2074 6865 2063 616c 6c20 6973 206d 6164   the call is mad
+000017f0: 652e 2042 7920 7573 696e 6720 7468 6973  e. By using this
+00001800: 2049 4420 796f 7520 6361 6e20 6578 706f   ID you can expo
+00001810: 7274 206d 6f72 6520 6461 7461 2074 6f20  rt more data to 
+00001820: 4d6f 6e61 2074 6f20 7468 6520 7361 6d65  Mona to the same
+00001830: 2063 6f6e 7465 7874 2066 726f 6d20 6f74   context from ot
+00001840: 6865 7220 706c 6163 6573 2e20 4966 206e  her places. If n
+00001850: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
+00001860: 2022 6964 2220 6669 656c 6420 6f66 2074   "id" field of t
+00001870: 6865 204f 7065 6e41 4920 456e 6470 6f69  he OpenAI Endpoi
+00001880: 6e74 2773 2072 6573 706f 6e73 6520 7769  nt's response wi
+00001890: 6c6c 2062 6520 7573 6564 2061 7320 7468  ll be used as th
+000018a0: 6520 4d6f 6e61 2063 6f6e 7465 7874 2049  e Mona context I
+000018b0: 4420 6175 746f 6d61 7469 6361 6c6c 792e  D automatically.
+000018c0: 0a2a 204d 4f4e 415f 6578 706f 7274 5f74  .* MONA_export_t
+000018d0: 696d 6573 7461 6d70 3a20 4361 6e20 6265  imestamp: Can be
+000018e0: 2075 7365 6420 746f 2073 696d 756c 6174   used to simulat
+000018f0: 6520 6173 2069 6620 7468 6520 6375 7272  e as if the curr
+00001900: 656e 7420 6361 6c6c 2077 6173 206d 6164  ent call was mad
+00001910: 6520 696e 2061 2064 6966 6665 7265 6e74  e in a different
+00001920: 2074 696d 652c 2061 7320 6661 7220 6173   time, as far as
+00001930: 204d 6f6e 6120 6973 2063 6f6e 6365 726e   Mona is concern
+00001940: 6564 2e0a 2a20 4d4f 4e41 5f61 6464 6974  ed..* MONA_addit
+00001950: 696f 6e61 6c5f 6461 7461 3a20 4120 4a53  ional_data: A JS
+00001960: 4f4e 2d73 6572 6961 6c69 7a61 626c 6520  ON-serializable 
+00001970: 6469 6374 2077 6974 6820 616e 7920 6f74  dict with any ot
+00001980: 6865 7220 6461 7461 2079 6f75 2077 616e  her data you wan
+00001990: 7420 746f 2061 6464 2074 6f20 7468 6520  t to add to the 
+000019a0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
+000019b0: 7874 2e20 5468 6973 2063 6f6d 6573 2069  xt. This comes i
+000019c0: 6e20 6861 6e64 7920 6966 2079 6f75 2077  n handy if you w
+000019d0: 616e 7420 746f 2061 6464 206d 6f72 6520  ant to add more 
+000019e0: 696e 666f 726d 6174 696f 6e20 746f 2074  information to t
+000019f0: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
+00001a00: 6e74 6578 2074 6861 7420 6973 6e27 7420  ntex that isn't 
+00001a10: 7061 7274 206f 6620 7468 6520 6261 7369  part of the basi
+00001a20: 6320 4f70 656e 4149 2041 5049 2063 616c  c OpenAI API cal
+00001a30: 6c20 696e 666f 726d 6174 696f 6e2e 2046  l information. F
+00001a40: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
+00001a50: 6f75 2061 7265 2075 7369 6e67 2061 2073  ou are using a s
+00001a60: 7065 6369 6669 6320 7465 6d70 6c61 7465  pecific template
+00001a70: 2049 4420 6f72 2069 6620 7468 6973 2063   ID or if this c
+00001a80: 616c 6c20 6973 2062 6569 6e67 206d 6164  all is being mad
+00001a90: 6520 666f 7220 6120 7370 6563 6966 6963  e for a specific
+00001aa0: 2063 7573 746f 6d65 7220 4944 2c20 7468   customer ID, th
+00001ab0: 6573 6520 6172 6520 6669 656c 6473 2079  ese are fields y
+00001ac0: 6f75 2063 616e 2061 6464 2074 6865 7265  ou can add there
+00001ad0: 2074 6f20 6865 6c70 2067 6574 2066 756c   to help get ful
+00001ae0: 6c20 636f 6e74 6578 7420 7768 656e 206d  l context when m
+00001af0: 6f6e 6974 6f72 696e 6720 7769 7468 204d  onitoring with M
+00001b00: 6f6e 612e 0a0a 4578 616d 706c 653a 0a60  ona...Example:.`
+00001b10: 6060 7079 0a72 6573 706f 6e73 6520 3d20  ``py.response = 
+00001b20: 6173 796e 6369 6f2e 7275 6e28 6d6f 6e69  asyncio.run(moni
+00001b30: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
+00001b40: 2e61 6372 6561 7465 280a 2020 2020 656e  .acreate(.    en
+00001b50: 6769 6e65 3d6d 6f64 656c 2c0a 2020 2020  gine=model,.    
+00001b60: 7072 6f6d 7074 3d70 726f 6d70 742c 0a20  prompt=prompt,. 
+00001b70: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
+00001b80: 785f 746f 6b65 6e73 2c0a 2020 2020 6e3d  x_tokens,.    n=
+00001b90: 6e2c 0a20 2020 2074 656d 7065 7261 7475  n,.    temperatu
+00001ba0: 7265 3d74 656d 7065 7261 7475 7265 2c0a  re=temperature,.
+00001bb0: 2020 2020 4d4f 4e41 5f61 6464 6974 696f      MONA_additio
+00001bc0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
+00001bd0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
+00001be0: 3122 7d2c 0a29 290a 7072 696e 7428 7265  1"},.)).print(re
+00001bf0: 7370 6f6e 7365 2e63 686f 6963 6573 5b30  sponse.choices[0
+00001c00: 5d2e 7465 7874 290a 6060 600a 0a23 2323  ].text).```..###
+00001c10: 2055 7369 6e67 204f 7065 6e41 4920 7769   Using OpenAI wi
+00001c20: 7468 2052 4553 5420 6361 6c6c 7320 696e  th REST calls in
+00001c30: 7374 6561 6420 6f66 204f 7065 6e41 4927  stead of OpenAI'
+00001c40: 7320 5079 7468 6f6e 2063 6c69 656e 740a  s Python client.
+00001c50: 496e 2073 6f6d 6520 6361 7365 7320 796f  In some cases yo
+00001c60: 7520 6d61 7920 6368 6f6f 7365 2074 6f20  u may choose to 
+00001c70: 7573 6520 4f70 656e 4149 2773 2041 5049  use OpenAI's API
+00001c80: 2064 6972 6563 746c 7920 7769 7468 2052   directly with R
+00001c90: 4553 5420 6361 6c6c 7320 616e 6420 6e6f  EST calls and no
+00001ca0: 7420 7573 696e 6720 4f70 656e 4149 2773  t using OpenAI's
+00001cb0: 2053 444b 2e20 466f 7220 7468 6573 6520   SDK. For these 
+00001cc0: 6361 7365 7320 7765 2061 6c6c 6f77 2061  cases we allow a
+00001cd0: 206d 6f72 6520 6469 7265 6374 2061 7070   more direct app
+00001ce0: 726f 6163 6820 666f 7220 6c6f 6767 696e  roach for loggin
+00001cf0: 6720 746f 204d 6f6e 6120 6173 2077 656c  g to Mona as wel
+00001d00: 6c2c 2062 7920 7573 696e 6720 7468 6520  l, by using the 
+00001d10: 2267 6574 5f72 6573 745f 6d6f 6e69 746f  "get_rest_monito
+00001d20: 7222 2066 756e 6374 696f 6e2e 2053 6565  r" function. See
+00001d30: 2065 7861 6d70 6c65 2062 656c 6f77 2e0a   example below..
+00001d40: 0a60 6060 7079 0a23 2044 6972 6563 7420  .```py.# Direct 
+00001d50: 5245 5354 2075 7361 6765 2c20 7769 7468  REST usage, with
+00001d60: 6f75 7420 4f70 656e 4149 2063 6c69 656e  out OpenAI clien
+00001d70: 740a 696d 706f 7274 2072 6571 7565 7374  t.import request
+00001d80: 730a 6672 6f6d 206f 7320 696d 706f 7274  s.from os import
+00001d90: 2065 6e76 6972 6f6e 0a66 726f 6d20 6d6f   environ.from mo
+00001da0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
+00001db0: 2067 6574 5f72 6573 745f 6d6f 6e69 746f   get_rest_monito
+00001dc0: 720a 0a0a 4d4f 4e41 5f41 5049 5f4b 4559  r...MONA_API_KEY
+00001dd0: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
+00001de0: 4d4f 4e41 5f41 5049 5f4b 4559 2229 0a4d  MONA_API_KEY").M
+00001df0: 4f4e 415f 5345 4352 4554 203d 2065 6e76  ONA_SECRET = env
+00001e00: 6972 6f6e 2e67 6574 2822 4d4f 4e41 5f53  iron.get("MONA_S
+00001e10: 4543 5245 5422 290a 4d4f 4e41 5f43 5245  ECRET").MONA_CRE
+00001e20: 4453 203d 207b 0a20 2020 2022 6b65 7922  DS = {.    "key"
+00001e30: 3a20 4d4f 4e41 5f41 5049 5f4b 4559 2c0a  : MONA_API_KEY,.
+00001e40: 2020 2020 2273 6563 7265 7422 3a20 4d4f      "secret": MO
+00001e50: 4e41 5f53 4543 5245 542c 0a7d 0a43 4f4e  NA_SECRET,.}.CON
+00001e60: 5445 5854 5f43 4c41 5353 5f4e 414d 4520  TEXT_CLASS_NAME 
+00001e70: 3d20 2253 4f4d 455f 4d4f 4e49 544f 5249  = "SOME_MONITORI
+00001e80: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
+00001e90: 0a0a 2320 4765 7420 4d6f 6e61 206c 6f67  ..# Get Mona log
+00001ea0: 6765 720a 6d6f 6e61 5f6c 6f67 6765 7220  ger.mona_logger 
+00001eb0: 3d20 6765 745f 7265 7374 5f6d 6f6e 6974  = get_rest_monit
+00001ec0: 6f72 280a 2020 2020 2243 6f6d 706c 6574  or(.    "Complet
+00001ed0: 696f 6e22 2c0a 2020 2020 4d4f 4e41 5f43  ion",.    MONA_C
+00001ee0: 5245 4453 2c0a 2020 2020 434f 4e54 4558  REDS,.    CONTEX
+00001ef0: 545f 434c 4153 535f 4e41 4d45 2c0a 290a  T_CLASS_NAME,.).
+00001f00: 0a23 2053 6574 2075 7020 7468 6520 4150  .# Set up the AP
+00001f10: 4920 656e 6470 6f69 6e74 2055 524c 2061  I endpoint URL a
+00001f20: 6e64 2061 7574 6865 6e74 6963 6174 696f  nd authenticatio
+00001f30: 6e20 6865 6164 6572 730a 7572 6c20 3d20  n headers.url = 
+00001f40: 2268 7474 7073 3a2f 2f61 7069 2e6f 7065  "https://api.ope
+00001f50: 6e61 692e 636f 6d2f 7631 2f63 6f6d 706c  nai.com/v1/compl
+00001f60: 6574 696f 6e73 220a 6865 6164 6572 7320  etions".headers 
+00001f70: 3d20 7b0a 2020 2020 2243 6f6e 7465 6e74  = {.    "Content
+00001f80: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
+00001f90: 7469 6f6e 2f6a 736f 6e22 2c0a 2020 2020  tion/json",.    
+00001fa0: 2241 7574 686f 7269 7a61 7469 6f6e 223a  "Authorization":
+00001fb0: 2066 2242 6561 7265 7220 7b65 6e76 6972   f"Bearer {envir
+00001fc0: 6f6e 2e67 6574 2827 4f50 454e 5f41 495f  on.get('OPEN_AI_
+00001fd0: 4b45 5927 297d 222c 0a7d 0a0a 2320 5365  KEY')}",.}..# Se
+00001fe0: 7420 7570 2074 6865 2072 6571 7565 7374  t up the request
+00001ff0: 2064 6174 610a 6461 7461 203d 207b 0a20   data.data = {. 
+00002000: 2020 2022 7072 6f6d 7074 223a 2070 726f     "prompt": pro
+00002010: 6d70 742c 0a20 2020 2022 6d61 785f 746f  mpt,.    "max_to
+00002020: 6b65 6e73 223a 206d 6178 5f74 6f6b 656e  kens": max_token
+00002030: 732c 0a20 2020 2022 7465 6d70 6572 6174  s,.    "temperat
+00002040: 7572 6522 3a20 7465 6d70 6572 6174 7572  ure": temperatur
+00002050: 652c 0a20 2020 2022 6d6f 6465 6c22 3a20  e,.    "model": 
+00002060: 6d6f 6465 6c2c 0a20 2020 2022 6e22 3a20  model,.    "n": 
+00002070: 6e2c 0a7d 0a0a 2320 5468 6520 6c6f 675f  n,.}..# The log_
+00002080: 7265 7175 6573 7420 6675 6e63 7469 6f6e  request function
+00002090: 2072 6574 7572 6e73 2074 776f 206f 7468   returns two oth
+000020a0: 6572 2066 756e 6374 696f 6e20 666f 7220  er function for 
+000020b0: 6c61 7465 7220 6c6f 6767 696e 670a 2320  later logging.# 
+000020c0: 7468 6520 7265 7370 6f6e 7365 206f 7220  the response or 
+000020d0: 7468 6520 6578 6365 7074 696f 6e2e 2057  the exception. W
+000020e0: 6865 6e20 7765 206c 6174 6572 2064 6f20  hen we later do 
+000020f0: 7468 6174 2c20 7468 6520 6c6f 6767 6572  that, the logger
+00002100: 2077 696c 6c0a 2320 6163 7475 616c 6c79   will.# actually
+00002110: 2063 616c 6375 6c61 7465 2061 6c6c 2074   calculate all t
+00002120: 6865 2072 656c 6576 616e 7420 6d65 7472  he relevant metr
+00002130: 6963 7320 616e 6420 7769 6c6c 2073 656e  ics and will sen
+00002140: 6420 7468 656d 2074 6f0a 2320 4d6f 6e61  d them to.# Mona
+00002150: 2e0a 7265 7370 6f6e 7365 5f6c 6f67 6765  ..response_logge
+00002160: 722c 2065 7863 6570 7469 6f6e 5f6c 6f67  r, exception_log
+00002170: 6765 7220 3d20 6d6f 6e61 5f6c 6f67 6765  ger = mona_logge
+00002180: 722e 6c6f 675f 7265 7175 6573 7428 0a20  r.log_request(. 
+00002190: 2020 2064 6174 612c 2061 6464 6974 696f     data, additio
+000021a0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
+000021b0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
+000021c0: 3122 7d0a 290a 0a74 7279 3a0a 2020 2020  1"}.)..try:.    
+000021d0: 2320 5365 6e64 2074 6865 2072 6571 7565  # Send the reque
+000021e0: 7374 2074 6f20 7468 6520 4150 490a 2020  st to the API.  
+000021f0: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
+00002200: 7565 7374 732e 706f 7374 2875 726c 2c20  uests.post(url, 
+00002210: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
+00002220: 206a 736f 6e3d 6461 7461 290a 0a20 2020   json=data)..   
+00002230: 2023 2043 6865 636b 2066 6f72 2048 5454   # Check for HTT
+00002240: 5020 6572 726f 7273 0a20 2020 2072 6573  P errors.    res
+00002250: 706f 6e73 652e 7261 6973 655f 666f 725f  ponse.raise_for_
+00002260: 7374 6174 7573 2829 0a0a 2020 2020 2320  status()..    # 
+00002270: 4c6f 6720 7265 7370 6f6e 7365 2074 6f20  Log response to 
+00002280: 4d6f 6e61 0a20 2020 2072 6573 706f 6e73  Mona.    respons
+00002290: 655f 6c6f 6767 6572 2872 6573 706f 6e73  e_logger(respons
+000022a0: 652e 6a73 6f6e 2829 290a 2020 2020 7072  e.json()).    pr
+000022b0: 696e 7428 7265 7370 6f6e 7365 2e6a 736f  int(response.jso
+000022c0: 6e28 295b 2263 686f 6963 6573 225d 5b30  n()["choices"][0
+000022d0: 5d5b 2274 6578 7422 5d29 0a0a 6578 6365  ]["text"])..exce
+000022e0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000022f0: 6572 723a 0a20 2020 2023 204c 6f67 2065  err:.    # Log e
+00002300: 7863 6570 7469 6f6e 2074 6f20 4d6f 6e61  xception to Mona
+00002310: 0a20 2020 2065 7863 6570 7469 6f6e 5f6c  .    exception_l
+00002320: 6f67 6765 7228 290a 6060 600a 0a23 2323  ogger().```..###
+00002330: 2053 7472 6561 6d20 7375 7070 6f72 740a   Stream support.
+00002340: 0a4f 7065 6e41 4920 616c 6c6f 7773 2072  .OpenAI allows r
+00002350: 6563 6569 7669 6e67 2072 6573 706f 6e73  eceiving respons
+00002360: 6573 2061 7320 6120 7374 7265 616d 206f  es as a stream o
+00002370: 6620 746f 6b65 6e73 2075 7369 6e67 2074  f tokens using t
+00002380: 6865 2022 7374 7265 616d 2220 7061 7261  he "stream" para
+00002390: 6d65 7465 722e 2057 6865 6e20 7468 6973  meter. When this
+000023a0: 2069 7320 646f 6e65 2c20 4d6f 6e61 2077   is done, Mona w
+000023b0: 696c 6c20 636f 6c6c 6563 7420 616c 6c20  ill collect all 
+000023c0: 7468 6520 746f 6b65 6e73 2069 6e20 6d65  the tokens in me
+000023d0: 6d6f 7279 2061 6e64 2077 696c 6c20 6372  mory and will cr
+000023e0: 6561 7465 2074 6865 2061 6e61 6c79 7369  eate the analysi
+000023f0: 7320 616e 6420 6c6f 6720 6f75 7420 7468  s and log out th
+00002400: 6520 6461 7461 2074 6865 206d 6f6d 656e  e data the momen
+00002410: 7420 7468 6520 7374 7265 616d 2069 7320  t the stream is 
+00002420: 6f76 6572 2e20 596f 7520 646f 6e27 7420  over. You don't 
+00002430: 6e65 6564 2074 6f20 646f 2061 6e79 7468  need to do anyth
+00002440: 696e 6720 746f 206d 616b 6520 7468 6973  ing to make this
+00002450: 2068 6170 7065 6e2e 0a0a 5369 6e63 6520   happen...Since 
+00002460: 666f 7220 7374 7265 616d 696e 6720 7265  for streaming re
+00002470: 7370 6f6e 7365 7320 4f70 656e 4149 2064  sponses OpenAI d
+00002480: 6f65 736e 2774 2073 7570 706c 7920 7468  oesn't supply th
+00002490: 6520 6675 6c6c 2075 7361 6765 2074 6f6b  e full usage tok
+000024a0: 656e 7320 7375 6d6d 6172 792c 204d 6f6e  ens summary, Mon
+000024b0: 6120 7573 6573 2074 6865 2074 696b 746f  a uses the tikto
+000024c0: 6b65 6e20 7061 636b 6167 6520 746f 2063  ken package to c
+000024d0: 616c 6375 6c61 7465 2074 6865 2074 6f6b  alculate the tok
+000024e0: 656e 7320 6f66 2074 6865 2070 726f 6d70  ens of the promp
+000024f0: 7420 616e 6420 636f 6d70 6c65 7469 6f6e  t and completion
+00002500: 2061 6e64 206c 6f67 2074 6865 6d20 666f   and log them fo
+00002510: 7220 6d6f 6e69 746f 7269 6e67 2e0a 0a4e  r monitoring...N
+00002520: 4f54 453a 2053 7472 6561 6d20 6973 2063  OTE: Stream is c
+00002530: 7572 7265 6e74 6c79 206f 6e6c 7920 7375  urrently only su
+00002540: 7070 6f72 7465 6420 7769 7468 2053 444b  pported with SDK
+00002550: 2075 7361 6765 2c20 616e 6420 6e6f 7420   usage, and not 
+00002560: 7769 7468 2075 7369 6e67 2052 4553 5420  with using REST 
+00002570: 6469 7265 6374 6c79 2e0a 0a23 2320 4c61  directly...## La
+00002580: 6e67 4368 6169 6e20 7375 7070 6f72 740a  ngChain support.
+00002590: 0a59 6f75 2063 616e 2075 7365 2074 6865  .You can use the
+000025a0: 2065 7870 6f72 7465 6420 606d 6f6e 6974   exported `monit
+000025b0: 6f72 5f6c 616e 6763 6861 696e 5f6c 6c6d  or_langchain_llm
+000025c0: 6020 746f 2077 7261 7020 6120 4c61 6e67  ` to wrap a Lang
+000025d0: 4368 6169 6e20 4f70 656e 4149 204c 4c4d  Chain OpenAI LLM
+000025e0: 2028 6368 6174 206f 7220 6e6f 726d 616c   (chat or normal
+000025f0: 2920 7769 7468 204d 6f6e 6127 7320 6d6f  ) with Mona's mo
+00002600: 6e69 746f 7269 6e67 2063 6170 6162 696c  nitoring capabil
+00002610: 6974 6965 733a 0a0a 6060 6070 790a 6672  ities:..```py.fr
+00002620: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
+00002630: 6d70 6f72 7420 6d6f 6e69 746f 725f 6c61  mport monitor_la
+00002640: 6e67 6368 6169 6e5f 6c6c 6d0a 0a66 726f  ngchain_llm..fro
+00002650: 6d20 6c61 6e67 6368 6169 6e2e 6c6c 6d73  m langchain.llms
+00002660: 2069 6d70 6f72 7420 4f70 656e 4149 0a0a   import OpenAI..
+00002670: 2320 5772 6170 2074 6865 204c 4c4d 206f  # Wrap the LLM o
+00002680: 626a 6563 7420 7769 7468 204d 6f6e 6120  bject with Mona 
+00002690: 6d6f 6e69 746f 7269 6e67 2e0a 6c6c 6d20  monitoring..llm 
+000026a0: 3d20 6d6f 6e69 746f 725f 6c61 6e67 6368  = monitor_langch
+000026b0: 6169 6e5f 6c6c 6d28 0a20 2020 204f 7065  ain_llm(.    Ope
+000026c0: 6e41 4928 4f50 454e 5f41 495f 4b45 5929  nAI(OPEN_AI_KEY)
+000026d0: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
+000026e0: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
+000026f0: 4153 535f 4e41 4d45 290a 6060 600a 0a53  ASS_NAME).```..S
+00002700: 6565 2066 756c 6c20 6578 616d 706c 6520  ee full example 
+00002710: 696e 2063 6f6d 706c 6574 696f 6e5f 6c61  in completion_la
+00002720: 6e67 6368 6169 6e2e 7079 2069 6e20 7468  ngchain.py in th
+00002730: 6520 6578 616d 706c 6573 2066 6f6c 6465  e examples folde
+00002740: 722e 0a0a 2323 204d 6f6e 6120 5344 4b0a  r...## Mona SDK.
+00002750: 0a54 6869 7320 7061 636b 6167 6520 7573  .This package us
+00002760: 6573 2074 6865 206d 6f6e 615f 7364 6b20  es the mona_sdk 
+00002770: 7061 636b 6167 6520 746f 2065 7870 6f72  package to expor
+00002780: 7420 7468 6520 7265 6c65 7661 6e74 2064  t the relevant d
+00002790: 6174 6120 746f 204d 6f6e 612e 2054 6865  ata to Mona. The
+000027a0: 7265 2061 7265 2073 6576 6572 616c 2065  re are several e
+000027b0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+000027c0: 626c 6573 2079 6f75 2063 616e 2075 7365  bles you can use
+000027d0: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
+000027e0: 6520 5344 4b27 7320 6265 6861 7669 6f72  e SDK's behavior
+000027f0: 2e20 466f 7220 6578 616d 706c 652c 2079  . For example, y
+00002800: 6f75 2063 616e 2073 6574 2069 7420 7570  ou can set it up
+00002810: 2074 6f20 7261 6973 6520 6578 6365 7074   to raise except
+00002820: 696f 6e73 2077 6865 6e20 6578 706f 7274  ions when export
+00002830: 696e 6720 6461 7461 2074 6f20 4d6f 6e61  ing data to Mona
+00002840: 2066 6169 6c73 2028 6974 2064 6f65 736e   fails (it doesn
+00002850: 2774 2064 6f20 7468 6174 2062 7920 6465  't do that by de
+00002860: 6661 756c 7429 2e0a 0a23 2320 4d6f 6e69  fault)...## Moni
+00002870: 746f 7269 6e67 2066 6f72 2070 726f 6661  toring for profa
+00002880: 6e69 7479 0a0a 4d6f 6e61 2075 7365 7320  nity..Mona uses 
+00002890: 7468 6520 616c 742d 7072 6f66 616e 6974  the alt-profanit
+000028a0: 792d 6368 6563 6b20 7061 6361 6b67 6520  y-check pacakge 
+000028b0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000028c0: 672f 7072 6f6a 6563 742f 616c 742d 7072  g/project/alt-pr
+000028d0: 6f66 616e 6974 792d 6368 6563 6b2f 2920  ofanity-check/) 
+000028e0: 746f 2063 7265 6174 6520 626f 7468 2062  to create both b
+000028f0: 6f6f 6c65 616e 2070 7265 6469 6374 696f  oolean predictio
+00002900: 6e73 2061 6e64 2070 726f 6261 6269 6c74  ns and probabilt
+00002910: 7920 7363 6f72 6573 2066 6f72 2074 6865  y scores for the
+00002920: 2065 7869 7374 656e 6365 206f 6620 7072   existence of pr
+00002930: 6f66 616e 6974 7920 626f 7468 2069 6e20  ofanity both in 
+00002940: 7468 6520 7072 6f6d 7074 2061 6e64 2069  the prompt and i
+00002950: 6e20 7468 6520 7265 7370 6f6e 7365 732e  n the responses.
+00002960: 2057 6520 7573 6520 7468 6520 6275 696c   We use the buil
+00002970: 7420 696e 2070 6163 6b61 6765 206d 6574  t in package met
+00002980: 686f 6473 2066 6f72 2074 6861 742e 2049  hods for that. I
+00002990: 6620 796f 7520 7761 6e74 2c20 666f 7220  f you want, for 
+000029a0: 6578 616d 706c 652c 2074 6f20 7573 6520  example, to use 
+000029b0: 6120 6469 6666 6572 656e 7420 7072 6f62  a different prob
+000029c0: 6162 696c 6974 7920 7468 7265 7368 6f6c  ability threshol
+000029d0: 6420 666f 7220 7468 6520 626f 6f6c 6561  d for the boolea
+000029e0: 6e20 7072 6564 6963 7469 6f6e 2c20 796f  n prediction, yo
+000029f0: 7520 6361 6e20 646f 2074 6861 7420 6279  u can do that by
+00002a00: 2063 6861 6e67 696e 6720 796f 7572 204d   changing your M
+00002a10: 6f6e 6120 636f 6e66 6967 206f 6e20 7468  ona config on th
+00002a20: 6520 4d6f 6e61 2064 6173 6862 6f61 7264  e Mona dashboard
+00002a30: 2e0a                                     ..
```

### Comparing `mona-openai-0.0.7/README.md` & `mona-openai-0.0.8/mona_openai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,573 +1,676 @@
-00000000: 2320 4d6f 6e61 2d4f 7065 6e41 4920 496e  # Mona-OpenAI In
-00000010: 7465 6772 6174 696f 6e20 436c 6965 6e74  tegration Client
-00000020: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000030: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
-00000040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000050: 6f6d 2f6d 6f6e 616c 6162 732f 6d6f 6e61  om/monalabs/mona
-00000060: 2d73 646b 2f62 6c6f 622f 6d61 696e 2f6d  -sdk/blob/main/m
-00000070: 6f6e 615f 6c6f 676f 2e70 6e67 3f72 6177  ona_logo.png?raw
-00000080: 3d74 7275 6522 2061 6c74 3d22 4d6f 6e61  =true" alt="Mona
-00000090: 2773 206c 6f67 6f22 2077 6964 7468 3d22  's logo" width="
-000000a0: 3138 3022 2f3e 0a3c 2f70 3e0a 0a0a 5573  180"/>.</p>...Us
-000000b0: 6520 6f6e 6520 6c69 6e65 206f 6620 636f  e one line of co
-000000c0: 6465 2074 6f20 6765 7420 696e 7374 616e  de to get instan
-000000d0: 7420 6c69 7665 206d 6f6e 6974 6f72 696e  t live monitorin
-000000e0: 6720 666f 7220 796f 7572 204f 7065 6e41  g for your OpenA
-000000f0: 4920 7573 6167 6520 696e 636c 7564 696e  I usage includin
-00000100: 673a 0a2a 2054 6f6b 656e 7320 7573 6167  g:.* Tokens usag
-00000110: 650a 2a20 4861 6c6c 7563 696e 6174 696f  e.* Hallucinatio
-00000120: 6e20 616c 6572 7473 0a2a 2050 726f 6661  n alerts.* Profa
-00000130: 6e69 7479 2061 6e64 2070 7269 7661 6379  nity and privacy
-00000140: 2061 6e61 6c79 7365 730a 2a20 4265 6861   analyses.* Beha
-00000150: 7669 6f72 616c 2064 7269 6674 7320 616e  vioral drifts an
-00000160: 6420 616e 6f6d 616c 6965 730a 2a20 4d75  d anomalies.* Mu
-00000170: 6368 206d 7563 6820 6d6f 7265 2e0a 0a23  ch much more...#
-00000180: 2320 5365 7474 696e 6720 5570 0a0a 2d20  # Setting Up..- 
-00000190: 544f 444f 3a20 4164 6420 7061 7274 2061  TODO: Add part a
-000001a0: 626f 7574 204d 6f6e 6120 7265 6769 7374  bout Mona regist
-000001b0: 7261 7469 6f6e 2077 6974 6820 6120 6c69  ration with a li
-000001c0: 6e6b 2074 6f20 7468 6520 7265 6c65 7661  nk to the releva
-000001d0: 6e74 206c 616e 6469 6e67 2070 6167 6520  nt landing page 
-000001e0: 7768 6572 6520 7468 6520 7265 6164 6572  where the reader
-000001f0: 2063 616e 2073 6967 6e20 7570 2e0a 6060   can sign up..``
-00000200: 6063 6f6e 736f 6c65 0a24 2070 6970 2069  `console.$ pip i
-00000210: 6e73 7461 6c6c 206d 6f6e 615f 6f70 656e  nstall mona_open
-00000220: 6169 0a60 6060 0a0a 2323 2051 7569 636b  ai.```..## Quick
-00000230: 2053 7461 7274 2061 6e64 2045 7861 6d70   Start and Examp
-00000240: 6c65 0a0a 4578 616d 706c 6520 626f 696c  le..Example boil
-00000250: 6572 706c 6174 6520 636f 6465 2066 6f72  erplate code for
-00000260: 2062 6f74 6820 7379 6e63 2061 6e64 2061   both sync and a
-00000270: 7379 6e63 2075 7361 6765 2069 7320 6769  sync usage is gi
-00000280: 7665 6e20 696e 2074 6865 2066 696c 6520  ven in the file 
-00000290: 2265 7861 6d70 6c65 5f75 7361 6765 2e70  "example_usage.p
-000002a0: 7922 2061 6e64 2068 6572 653a 0a60 6060  y" and here:.```
-000002b0: 7079 0a66 726f 6d20 6f73 2069 6d70 6f72  py.from os impor
-000002c0: 7420 656e 7669 726f 6e0a 696d 706f 7274  t environ.import
-000002d0: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
-000002e0: 6f70 656e 6169 0a0a 6672 6f6d 206d 6f6e  openai..from mon
-000002f0: 615f 6f70 656e 6169 2069 6d70 6f72 7420  a_openai import 
-00000300: 6d6f 6e69 746f 720a 0a6f 7065 6e61 692e  monitor..openai.
-00000310: 6170 695f 6b65 7920 3d20 656e 7669 726f  api_key = enviro
-00000320: 6e2e 6765 7428 224f 5045 4e5f 4149 5f4b  n.get("OPEN_AI_K
-00000330: 4559 2229 0a0a 4d4f 4e41 5f41 5049 5f4b  EY")..MONA_API_K
-00000340: 4559 203d 2065 6e76 6972 6f6e 2e67 6574  EY = environ.get
-00000350: 2822 4d4f 4e41 5f41 5049 5f4b 4559 2229  ("MONA_API_KEY")
-00000360: 0a4d 4f4e 415f 5345 4352 4554 203d 2065  .MONA_SECRET = e
-00000370: 6e76 6972 6f6e 2e67 6574 2822 4d4f 4e41  nviron.get("MONA
-00000380: 5f53 4543 5245 5422 290a 4d4f 4e41 5f43  _SECRET").MONA_C
-00000390: 5245 4453 203d 207b 0a20 2020 2022 6b65  REDS = {.    "ke
-000003a0: 7922 3a20 4d4f 4e41 5f41 5049 5f4b 4559  y": MONA_API_KEY
-000003b0: 2c0a 2020 2020 2273 6563 7265 7422 3a20  ,.    "secret": 
-000003c0: 4d4f 4e41 5f53 4543 5245 542c 0a7d 0a43  MONA_SECRET,.}.C
-000003d0: 4f4e 5445 5854 5f43 4c41 5353 5f4e 414d  ONTEXT_CLASS_NAM
-000003e0: 4520 3d20 2253 4f4d 455f 4d4f 4e49 544f  E = "SOME_MONITO
-000003f0: 5249 4e47 5f43 4f4e 5445 5854 5f4e 414d  RING_CONTEXT_NAM
-00000400: 4522 0a0a 0a6d 6f6e 6974 6f72 6564 5f63  E"...monitored_c
-00000410: 6f6d 706c 6574 696f 6e20 3d20 6d6f 6e69  ompletion = moni
-00000420: 746f 7228 0a20 2020 206f 7065 6e61 692e  tor(.    openai.
-00000430: 436f 6d70 6c65 7469 6f6e 2c0a 2020 2020  Completion,.    
-00000440: 4d4f 4e41 5f43 5245 4453 2c0a 2020 2020  MONA_CREDS,.    
-00000450: 434f 4e54 4558 545f 434c 4153 535f 4e41  CONTEXT_CLASS_NA
-00000460: 4d45 2c0a 290a 0a0a 7072 6f6d 7074 203d  ME,.)...prompt =
-00000470: 2022 4920 7761 6e74 2074 6f20 6765 6e65   "I want to gene
-00000480: 7261 7465 2073 6f6d 6520 7465 7874 2061  rate some text a
-00000490: 626f 7574 2022 0a6d 6f64 656c 203d 2022  bout ".model = "
-000004a0: 7465 7874 2d61 6461 2d30 3031 220a 7465  text-ada-001".te
-000004b0: 6d70 6572 6174 7572 6520 3d20 302e 360a  mperature = 0.6.
-000004c0: 6d61 785f 746f 6b65 6e73 203d 2035 0a6e  max_tokens = 5.n
-000004d0: 203d 2031 0a0a 2320 5265 6775 6c61 7220   = 1..# Regular 
-000004e0: 2873 796e 6329 2075 7361 6765 0a72 6573  (sync) usage.res
-000004f0: 706f 6e73 6520 3d20 6d6f 6e69 746f 7265  ponse = monitore
-00000500: 645f 636f 6d70 6c65 7469 6f6e 2e63 7265  d_completion.cre
-00000510: 6174 6528 0a20 2020 2065 6e67 696e 653d  ate(.    engine=
-00000520: 6d6f 6465 6c2c 0a20 2020 2070 726f 6d70  model,.    promp
-00000530: 743d 7072 6f6d 7074 2c0a 2020 2020 6d61  t=prompt,.    ma
-00000540: 785f 746f 6b65 6e73 3d6d 6178 5f74 6f6b  x_tokens=max_tok
-00000550: 656e 732c 0a20 2020 206e 3d6e 2c0a 2020  ens,.    n=n,.  
-00000560: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
-00000570: 6d70 6572 6174 7572 652c 0a20 2020 204d  mperature,.    M
-00000580: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
-00000590: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
-000005a0: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
-000005b0: 290a 7072 696e 7428 7265 7370 6f6e 7365  ).print(response
-000005c0: 2e63 686f 6963 6573 5b30 5d2e 7465 7874  .choices[0].text
-000005d0: 290a 0a23 2041 7379 6e63 2075 7361 6765  )..# Async usage
-000005e0: 0a72 6573 706f 6e73 6520 3d20 6173 796e  .response = asyn
-000005f0: 6369 6f2e 7275 6e28 6d6f 6e69 746f 7265  cio.run(monitore
-00000600: 645f 636f 6d70 6c65 7469 6f6e 2e61 6372  d_completion.acr
-00000610: 6561 7465 280a 2020 2020 656e 6769 6e65  eate(.    engine
-00000620: 3d6d 6f64 656c 2c0a 2020 2020 7072 6f6d  =model,.    prom
-00000630: 7074 3d70 726f 6d70 742c 0a20 2020 206d  pt=prompt,.    m
-00000640: 6178 5f74 6f6b 656e 733d 6d61 785f 746f  ax_tokens=max_to
-00000650: 6b65 6e73 2c0a 2020 2020 6e3d 6e2c 0a20  kens,.    n=n,. 
-00000660: 2020 2074 656d 7065 7261 7475 7265 3d74     temperature=t
-00000670: 656d 7065 7261 7475 7265 2c0a 2020 2020  emperature,.    
-00000680: 4d4f 4e41 5f61 6464 6974 696f 6e61 6c5f  MONA_additional_
-00000690: 6461 7461 3d7b 2263 7573 746f 6d65 725f  data={"customer_
-000006a0: 6964 223a 2022 4135 3331 3235 3122 7d2c  id": "A531251"},
-000006b0: 0a29 290a 0a70 7269 6e74 2872 6573 706f  .))..print(respo
-000006c0: 6e73 652e 6368 6f69 6365 735b 305d 2e74  nse.choices[0].t
-000006d0: 6578 7429 0a60 6060 0a23 2320 5375 7070  ext).```.## Supp
-000006e0: 6f72 7465 6420 4f70 656e 4149 2041 5049  orted OpenAI API
-000006f0: 730a 4375 7272 656e 746c 7920 7468 6973  s.Currently this
-00000700: 2063 6c69 656e 7420 7375 7070 6f72 7473   client supports
-00000710: 2060 6f70 656e 6169 2e43 6f6d 706c 6574   `openai.Complet
-00000720: 696f 6e60 2061 6e64 2060 6f70 656e 6169  ion` and `openai
-00000730: 2e43 6861 7443 6f6d 706c 6574 696f 6e60  .ChatCompletion`
-00000740: 2e20 4d6f 6e61 2063 616e 2073 7570 706f  . Mona can suppo
-00000750: 7274 2070 726f 6365 7373 6573 2062 6173  rt processes bas
-00000760: 6564 206f 6e20 6f74 6865 7220 4150 4973  ed on other APIs
-00000770: 2061 6e64 2061 6c73 6f20 6e6f 6e2d 4f70   and also non-Op
-00000780: 656e 4149 2d62 6173 6564 2061 7070 732e  enAI-based apps.
-00000790: 0a49 6620 796f 7520 6861 7665 2061 2064  .If you have a d
-000007a0: 6966 6665 7272 656e 7420 7573 652d 6361  ifferrent use-ca
-000007b0: 7365 2c20 7765 2764 206c 6f76 6520 746f  se, we'd love to
-000007c0: 2068 6561 7220 6162 6f75 7420 6974 2120   hear about it! 
-000007d0: 506c 6561 7365 2065 6d61 696c 2075 7320  Please email us 
-000007e0: 6174 2073 7570 706f 7274 406d 6f6e 616c  at support@monal
-000007f0: 6162 732e 696f 2e0a 0a23 2320 5573 6167  abs.io...## Usag
-00000800: 650a 2323 2320 496e 6974 6961 6c69 7a61  e.### Initializa
-00000810: 7469 6f6e 0a0a 5468 6520 6d61 696e 2061  tion..The main a
-00000820: 6e64 206f 6e6c 7920 6675 6e63 7469 6f6e  nd only function
-00000830: 2065 7870 6f73 6564 2069 6e20 7468 6973   exposed in this
-00000840: 2070 6163 6b61 6765 2069 7320 606d 6f6e   package is `mon
-00000850: 6974 6f72 602e 0a60 6060 7079 0a69 6d70  itor`..```py.imp
-00000860: 6f72 7420 6f70 656e 6169 0a0a 6672 6f6d  ort openai..from
-00000870: 206d 6f6e 615f 6f70 656e 6169 2069 6d70   mona_openai imp
-00000880: 6f72 7420 6d6f 6e69 746f 720a 0a6f 7065  ort monitor..ope
-00000890: 6e61 692e 6170 695f 6b65 7920 3d20 656e  nai.api_key = en
-000008a0: 7669 726f 6e2e 6765 7428 224f 5045 4e5f  viron.get("OPEN_
-000008b0: 4149 5f4b 4559 2229 0a0a 6d6f 6e69 746f  AI_KEY")..monito
-000008c0: 7265 645f 636f 6d70 6c65 7469 6f6e 203d  red_completion =
-000008d0: 206d 6f6e 6974 6f72 280a 2020 2020 6f70   monitor(.    op
-000008e0: 656e 6169 2e43 6f6d 706c 6574 696f 6e2c  enai.Completion,
-000008f0: 0a20 2020 2028 0a20 2020 2020 2020 2065  .    (.        e
-00000900: 6e76 6972 6f6e 2e67 6574 2822 4d4f 4e41  nviron.get("MONA
-00000910: 5f41 5049 5f4b 4559 2229 2c0a 2020 2020  _API_KEY"),.    
-00000920: 2020 2020 656e 7669 726f 6e2e 6765 7428      environ.get(
-00000930: 224d 4f4e 415f 5345 4352 4554 2229 2c0a  "MONA_SECRET"),.
-00000940: 2020 2020 292c 0a20 2020 2022 534f 4d45      ),.    "SOME
-00000950: 5f4d 4f4e 4954 4f52 494e 475f 434f 4e54  _MONITORING_CONT
-00000960: 4558 545f 4e41 4d45 222c 0a20 2020 207b  EXT_NAME",.    {
-00000970: 2261 6e61 6c79 7369 7322 3a20 7b22 7072  "analysis": {"pr
-00000980: 6f66 616e 6974 7922 3a20 4661 6c73 657d  ofanity": False}
-00000990: 7d0a 290a 0a2e 2e2e 0a0a 6d6f 6e69 746f  }.).......monito
-000009a0: 7265 645f 636f 6d70 6c65 7469 6f6e 2e63  red_completion.c
-000009b0: 7265 6174 6528 2e2e 2e29 0a60 6060 0a0a  reate(...).```..
-000009c0: 5468 6520 606d 6f6e 6974 6f72 6020 6675  The `monitor` fu
-000009d0: 6e63 7469 6f6e 2072 6574 7572 6e73 2074  nction returns t
-000009e0: 6f20 796f 7520 6120 636c 6173 7320 7468  o you a class th
-000009f0: 6174 2077 7261 7073 2074 6865 206f 7269  at wraps the ori
-00000a00: 6769 6e61 6c20 6f70 656e 6169 2065 6e64  ginal openai end
-00000a10: 706f 696e 7420 636c 6173 7320 796f 7520  point class you 
-00000a20: 7072 6f76 6964 652c 2077 6974 6820 616e  provide, with an
-00000a30: 2065 7175 6976 616c 656e 7420 4150 4920   equivalent API 
-00000a40: 2862 6573 6964 6573 2073 6f6d 6520 6164  (besides some ad
-00000a50: 6469 7469 6f6e 7320 6c69 7374 6564 2062  ditions listed b
-00000a60: 656c 6f77 292e 0a59 6f75 2063 616e 2074  elow)..You can t
-00000a70: 6865 6e20 7573 6520 7468 6520 7265 7475  hen use the retu
-00000a80: 726e 6564 2063 6c61 7373 2720 2263 7265  rned class' "cre
-00000a90: 6174 6522 2061 6e64 2022 6163 7265 6174  ate" and "acreat
-00000aa0: 6522 2066 756e 6374 696f 6e73 206a 7573  e" functions jus
-00000ab0: 7420 6173 2079 6f75 2077 6f75 6c64 2062  t as you would b
-00000ac0: 6566 6f72 652c 206f 6e6c 7920 6e6f 772c  efore, only now,
-00000ad0: 2062 6573 6964 6573 2067 6574 7469 6e67   besides getting
-00000ae0: 2074 6865 2072 6571 7565 7374 6564 206f   the requested o
-00000af0: 7065 6e41 4920 6675 6e63 7469 6f6e 616c  penAI functional
-00000b00: 6974 792c 2074 6869 7320 636c 6965 6e74  ity, this client
-00000b10: 2077 696c 6c20 6c6f 6720 6f75 7420 746f   will log out to
-00000b20: 204d 6f6e 6127 7320 7365 7276 6572 2074   Mona's server t
-00000b30: 6865 2070 6172 616d 6574 6572 7320 796f  he parameters yo
-00000b40: 7520 7573 6564 2028 652e 672e 2c20 7465  u used (e.g., te
-00000b50: 6d70 6572 6174 7572 6529 2c20 6461 7461  mperature), data
-00000b60: 2061 626f 7574 2074 6865 2072 6573 706f   about the respo
-00000b70: 6e73 6520 6672 6f6d 204f 7065 6e41 4927  nse from OpenAI'
-00000b80: 7320 7365 7276 6572 2c20 616e 6420 6375  s server, and cu
-00000b90: 7374 6f6d 2061 6e61 6c79 7365 7320 6162  stom analyses ab
-00000ba0: 6f75 7420 7468 6520 6361 6c6c 2028 652e  out the call (e.
-00000bb0: 672e 2c20 7072 6f66 616e 6974 7920 7363  g., profanity sc
-00000bc0: 6f72 6573 2c20 7072 6976 6163 7920 6368  ores, privacy ch
-00000bd0: 6563 6b73 2066 6f72 2065 6d61 696c 732f  ecks for emails/
-00000be0: 7068 6f6e 6520 6e75 6d62 6572 7320 666f  phone numbers fo
-00000bf0: 756e 6420 696e 2074 6865 2074 6578 7473  und in the texts
-00000c00: 2c20 7465 7874 7561 6c20 616e 616c 7973  , textual analys
-00000c10: 6573 2c20 6574 632e 2e2e 290a 0a54 6865  es, etc...)..The
-00000c20: 2060 6d6f 6e69 746f 7260 2066 756e 6374   `monitor` funct
-00000c30: 696f 6e20 7265 6365 6976 6573 2074 6865  ion receives the
-00000c40: 2066 6f6c 6c6f 7769 6e67 2061 7267 756d   following argum
-00000c50: 656e 7473 3a0a 6f70 656e 6169 5f63 6c61  ents:.openai_cla
-00000c60: 7373 3a20 416e 204f 7065 6e41 4920 4150  ss: An OpenAI AP
-00000c70: 4920 636c 6173 7320 746f 2077 7261 7020  I class to wrap 
-00000c80: 7769 7468 206d 6f6e 6974 6f72 696e 6720  with monitoring 
-00000c90: 6361 7061 6269 6c74 6965 732e 0a6d 6f6e  capabilties..mon
-00000ca0: 615f 6372 6564 733a 2041 2064 6963 7420  a_creds: A dict 
-00000cb0: 2863 6f6e 7461 696e 696e 6720 226b 6579  (containing "key
-00000cc0: 2220 616e 6420 2273 6563 7265 7422 2920  " and "secret") 
-00000cd0: 6f72 2070 6169 7220 2874 7570 6c65 2920  or pair (tuple) 
-00000ce0: 6f66 204d 6f6e 6120 4150 4920 6b65 7920  of Mona API key 
-00000cf0: 616e 6420 7365 6372 6574 2074 6f20 7365  and secret to se
-00000d00: 7420 7570 204d 6f6e 6127 7320 636c 6965  t up Mona's clie
-00000d10: 6e74 7320 6672 6f6d 2069 7473 2053 444b  nts from its SDK
-00000d20: 2e0a 636f 6e74 6578 745f 636c 6173 733a  ..context_class:
-00000d30: 2054 6865 204d 6f6e 6120 636f 6e74 6578   The Mona contex
-00000d40: 7420 636c 6173 7320 6e61 6d65 2074 6f20  t class name to 
-00000d50: 7573 6520 666f 7220 6d6f 6e69 746f 7269  use for monitori
-00000d60: 6e67 2e20 5573 6520 6120 636f 6e73 7461  ng. Use a consta
-00000d70: 6e74 206e 616d 6520 6f66 2079 6f75 7220  nt name of your 
-00000d80: 6368 6f69 6365 2e0a 7370 6563 733a 2041  choice..specs: A
-00000d90: 2064 6963 7469 6f6e 6172 7920 6f66 2073   dictionary of s
-00000da0: 7065 6369 6669 6361 7469 6f6e 7320 7375  pecifications su
-00000db0: 6368 2061 7320 6d6f 6e69 746f 7269 6e67  ch as monitoring
-00000dc0: 2073 616d 706c 696e 6720 7261 7469 6f2e   sampling ratio.
-00000dd0: 0a0a 2323 2323 2053 7065 6373 0a54 6865  ..#### Specs.The
-00000de0: 2073 7065 6373 2061 7267 2061 6c6c 6f77   specs arg allow
-00000df0: 7320 796f 7520 746f 2063 6f6e 6669 6775  s you to configu
-00000e00: 7265 2077 6861 7420 7368 6f75 6c64 2062  re what should b
-00000e10: 6520 6d6f 6e69 746f 7265 642e 2049 7420  e monitored. It 
-00000e20: 6578 7065 6374 7320 6120 7079 7468 6f6e  expects a python
-00000e30: 2064 6963 7420 7769 7468 2074 6865 2066   dict with the f
-00000e40: 6f6c 6c77 6f69 6e67 2070 6f73 7369 626c  ollwoing possibl
-00000e50: 6520 6b65 7973 3a0a 2a20 7361 6d70 6c69  e keys:.* sampli
-00000e60: 6e67 5f72 6174 696f 2028 3129 3a20 4120  ng_ratio (1): A 
-00000e70: 6e75 6d62 6572 2062 6574 7765 656e 2030  number between 0
-00000e80: 2061 6e64 2031 2066 6f72 2068 6f77 206f   and 1 for how o
-00000e90: 6674 656e 2073 686f 756c 6420 7468 6520  ften should the 
-00000ea0: 6361 6c6c 2062 6520 6c6f 6767 6564 2e0a  call be logged..
-00000eb0: 2a20 6176 6f69 645f 6d6f 6e69 746f 7269  * avoid_monitori
-00000ec0: 6e67 5f65 7863 6570 7469 6f6e 7320 2846  ng_exceptions (F
-00000ed0: 616c 7365 293a 2057 6865 7468 6572 206f  alse): Whether o
-00000ee0: 7220 6e6f 7420 746f 206c 6f67 206f 7574  r not to log out
-00000ef0: 2074 6f20 4d6f 6e61 2077 6865 6e20 7468   to Mona when th
-00000f00: 6572 6520 6973 2061 6e20 4f70 656e 4149  ere is an OpenAI
-00000f10: 2065 7863 6570 7469 6f6e 2e20 4465 6661   exception. Defa
-00000f20: 756c 7420 6973 2074 6f20 7472 6163 6b20  ult is to track 
-00000f30: 6578 6365 7074 696f 6e73 202d 2061 6e64  exceptions - and
-00000f40: 204d 6f6e 6120 7769 6c6c 2061 6c65 7274   Mona will alert
-00000f50: 2079 6f75 206f 6e20 7468 696e 6773 206c   you on things l
-00000f60: 696b 6520 6120 6a75 6d70 2069 6e20 6e75  ike a jump in nu
-00000f70: 6d62 6572 206f 6620 6578 6365 7074 696f  mber of exceptio
-00000f80: 6e73 0a2a 2065 7870 6f72 745f 7072 6f6d  ns.* export_prom
-00000f90: 7074 2028 4661 6c73 6529 3a20 5768 6574  pt (False): Whet
-00000fa0: 6865 7220 4d6f 6e61 2073 686f 756c 6420  her Mona should 
-00000fb0: 6578 706f 7274 2074 6865 2061 6374 7561  export the actua
-00000fc0: 6c20 7072 6f6d 7074 2074 6578 742e 2042  l prompt text. B
-00000fd0: 6520 6465 6661 756c 7420 7365 7420 746f  e default set to
-00000fe0: 2046 616c 7365 2074 6f20 6176 6f69 6420   False to avoid 
-00000ff0: 7072 6976 6163 7920 636f 6e63 6572 6e73  privacy concerns
-00001000: 2e0a 2a20 6578 706f 7274 5f72 6573 706f  ..* export_respo
-00001010: 6e73 655f 7465 7874 7320 2846 616c 7365  nse_texts (False
-00001020: 293a 2057 6865 7468 6572 204d 6f6e 6120  ): Whether Mona 
-00001030: 7368 6f75 6c64 2065 7870 6f72 7420 7468  should export th
-00001040: 6520 6163 7475 616c 2072 6573 706f 6e73  e actual respons
-00001050: 6520 7465 7874 732e 2042 6520 6465 6661  e texts. Be defa
-00001060: 756c 7420 7365 7420 746f 2046 616c 7365  ult set to False
-00001070: 2074 6f20 6176 6f69 6420 7072 6976 6163   to avoid privac
-00001080: 7920 636f 6e63 6572 6e73 2e0a 2a20 616e  y concerns..* an
-00001090: 616c 7973 6973 3a20 4120 6469 6374 696f  alysis: A dictio
-000010a0: 6e61 7279 206d 6170 7069 6e67 2065 6163  nary mapping eac
-000010b0: 6820 616e 616c 7973 6973 2074 7970 6520  h analysis type 
-000010c0: 746f 2061 2062 6f6f 6c65 616e 2076 616c  to a boolean val
-000010d0: 7565 2074 656c 6c69 6e67 2074 6865 2063  ue telling the c
-000010e0: 6c69 656e 7420 7768 6574 6865 7220 6f72  lient whether or
-000010f0: 206e 6f74 2074 6f20 7275 6e20 7361 6964   not to run said
-00001100: 2061 6e61 6c79 7369 7320 616e 6420 6c6f   analysis and lo
-00001110: 6720 6974 2074 6f20 4d6f 6e61 2e20 506f  g it to Mona. Po
-00001120: 7373 6962 6c65 206f 7074 696f 6e73 2063  ssible options c
-00001130: 7572 7265 6e74 6c79 2061 7265 2022 7072  urrently are "pr
-00001140: 6976 6163 7922 2c20 2270 726f 6661 6e69  ivacy", "profani
-00001150: 7479 222c 2061 6e64 2022 7465 7874 7561  ty", and "textua
-00001160: 6c22 2e20 4279 2064 6566 6175 6c74 2c20  l". By default, 
-00001170: 616c 6c20 616e 616c 7973 6573 2074 616b  all analyses tak
-00001180: 6520 706c 6163 6520 616e 6420 6172 6520  e place and are 
-00001190: 6c6f 6767 6564 206f 7574 2074 6f20 4d6f  logged out to Mo
-000011a0: 6e61 2e0a 0a23 2323 2043 6170 6162 696c  na...### Capabil
-000011b0: 6974 6965 7320 6475 7269 6e67 2041 5049  ities during API
-000011c0: 2063 616c 6c73 0a0a 4166 7465 7220 7772   calls..After wr
-000011d0: 6170 7069 6e67 2079 6f75 7220 656e 6470  apping your endp
-000011e0: 6f69 6e74 2077 6974 6820 606d 6f6e 6974  oint with `monit
-000011f0: 6f72 602c 2079 6f75 2072 6561 6c6c 7920  or`, you really 
-00001200: 646f 6e27 7420 6e65 6564 2074 6f20 646f  don't need to do
-00001210: 2061 6e79 7468 696e 6720 656c 7365 2e20   anything else. 
-00001220: 5768 656e 2075 7369 6e67 2060 6372 6561  When using `crea
-00001230: 7465 6020 6f72 2060 6163 7265 6174 6560  te` or `acreate`
-00001240: 2064 6174 6120 7769 6c6c 2062 6520 7472   data will be tr
-00001250: 6163 6b65 6420 616e 6420 6d6f 6e69 746f  acked and monito
-00001260: 7269 6e67 2077 696c 6c20 7461 6b65 2070  ring will take p
-00001270: 6c61 6365 2e0a 0a54 6865 7265 2061 7265  lace...There are
-00001280: 2c20 686f 7765 7665 722c 2073 6576 6572  , however, sever
-00001290: 616c 2063 6170 6162 696c 6974 6965 7320  al capabilities 
-000012a0: 7468 6174 2061 7265 2061 6464 6564 2074  that are added t
-000012b0: 6f20 7468 6573 6520 6675 6e63 7469 6f6e  o these function
-000012c0: 732e 2053 7065 6369 6669 6361 6c6c 792c  s. Specifically,
-000012d0: 2079 6f75 2063 616e 2061 6464 2074 6865   you can add the
-000012e0: 2066 6f6c 6c6f 7769 6e67 2061 7267 756d   following argum
-000012f0: 656e 7473 2074 6f20 616e 7920 6372 6561  ents to any crea
-00001300: 7465 2063 616c 6c3a 0a2a 204d 4f4e 415f  te call:.* MONA_
-00001310: 636f 6e74 6578 745f 6964 3a20 5468 6520  context_id: The 
-00001320: 756e 6971 7565 2069 6420 6f66 2074 6865  unique id of the
-00001330: 2063 6f6e 7465 7874 2069 6e20 7768 6963   context in whic
-00001340: 6820 7468 6520 6361 6c6c 2069 7320 6d61  h the call is ma
-00001350: 6465 2e20 4279 2075 7369 6e67 2074 6869  de. By using thi
-00001360: 7320 4944 2079 6f75 2063 616e 2065 7870  s ID you can exp
-00001370: 6f72 7420 6d6f 7265 2064 6174 6120 746f  ort more data to
-00001380: 204d 6f6e 6120 746f 2074 6865 2073 616d   Mona to the sam
-00001390: 6520 636f 6e74 6578 7420 6672 6f6d 206f  e context from o
-000013a0: 7468 6572 2070 6c61 6365 732e 2049 6620  ther places. If 
-000013b0: 6e6f 7420 7375 7070 6c69 6564 2c20 7468  not supplied, th
-000013c0: 6520 2269 6422 2066 6965 6c64 206f 6620  e "id" field of 
-000013d0: 7468 6520 4f70 656e 4149 2045 6e64 706f  the OpenAI Endpo
-000013e0: 696e 7427 7320 7265 7370 6f6e 7365 2077  int's response w
-000013f0: 696c 6c20 6265 2075 7365 6420 6173 2074  ill be used as t
-00001400: 6865 204d 6f6e 6120 636f 6e74 6578 7420  he Mona context 
-00001410: 4944 2061 7574 6f6d 6174 6963 616c 6c79  ID automatically
-00001420: 2e0a 2a20 4d4f 4e41 5f65 7870 6f72 745f  ..* MONA_export_
-00001430: 7469 6d65 7374 616d 703a 2043 616e 2062  timestamp: Can b
-00001440: 6520 7573 6564 2074 6f20 7369 6d75 6c61  e used to simula
-00001450: 7465 2061 7320 6966 2074 6865 2063 7572  te as if the cur
-00001460: 7265 6e74 2063 616c 6c20 7761 7320 6d61  rent call was ma
-00001470: 6465 2069 6e20 6120 6469 6666 6572 656e  de in a differen
-00001480: 7420 7469 6d65 2c20 6173 2066 6172 2061  t time, as far a
-00001490: 7320 4d6f 6e61 2069 7320 636f 6e63 6572  s Mona is concer
-000014a0: 6e65 642e 0a2a 204d 4f4e 415f 6164 6469  ned..* MONA_addi
-000014b0: 7469 6f6e 616c 5f64 6174 613a 2041 204a  tional_data: A J
-000014c0: 534f 4e2d 7365 7269 616c 697a 6162 6c65  SON-serializable
-000014d0: 2064 6963 7420 7769 7468 2061 6e79 206f   dict with any o
-000014e0: 7468 6572 2064 6174 6120 796f 7520 7761  ther data you wa
-000014f0: 6e74 2074 6f20 6164 6420 746f 2074 6865  nt to add to the
-00001500: 206d 6f6e 6974 6f72 696e 6720 636f 6e74   monitoring cont
-00001510: 6578 742e 2054 6869 7320 636f 6d65 7320  ext. This comes 
-00001520: 696e 2068 616e 6479 2069 6620 796f 7520  in handy if you 
-00001530: 7761 6e74 2074 6f20 6164 6420 6d6f 7265  want to add more
-00001540: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
-00001550: 7468 6520 6d6f 6e69 746f 7269 6e67 2063  the monitoring c
-00001560: 6f6e 7465 7820 7468 6174 2069 736e 2774  ontex that isn't
-00001570: 2070 6172 7420 6f66 2074 6865 2062 6173   part of the bas
-00001580: 6963 204f 7065 6e41 4920 4150 4920 6361  ic OpenAI API ca
-00001590: 6c6c 2069 6e66 6f72 6d61 7469 6f6e 2e20  ll information. 
-000015a0: 466f 7220 6578 616d 706c 652c 2069 6620  For example, if 
-000015b0: 796f 7520 6172 6520 7573 696e 6720 6120  you are using a 
-000015c0: 7370 6563 6966 6963 2074 656d 706c 6174  specific templat
-000015d0: 6520 4944 206f 7220 6966 2074 6869 7320  e ID or if this 
-000015e0: 6361 6c6c 2069 7320 6265 696e 6720 6d61  call is being ma
-000015f0: 6465 2066 6f72 2061 2073 7065 6369 6669  de for a specifi
-00001600: 6320 6375 7374 6f6d 6572 2049 442c 2074  c customer ID, t
-00001610: 6865 7365 2061 7265 2066 6965 6c64 7320  hese are fields 
-00001620: 796f 7520 6361 6e20 6164 6420 7468 6572  you can add ther
-00001630: 6520 746f 2068 656c 7020 6765 7420 6675  e to help get fu
-00001640: 6c6c 2063 6f6e 7465 7874 2077 6865 6e20  ll context when 
-00001650: 6d6f 6e69 746f 7269 6e67 2077 6974 6820  monitoring with 
-00001660: 4d6f 6e61 2e0a 0a45 7861 6d70 6c65 3a0a  Mona...Example:.
-00001670: 6060 6070 790a 7265 7370 6f6e 7365 203d  ```py.response =
-00001680: 2061 7379 6e63 696f 2e72 756e 286d 6f6e   asyncio.run(mon
-00001690: 6974 6f72 6564 5f63 6f6d 706c 6574 696f  itored_completio
-000016a0: 6e2e 6163 7265 6174 6528 0a20 2020 2065  n.acreate(.    e
-000016b0: 6e67 696e 653d 6d6f 6465 6c2c 0a20 2020  ngine=model,.   
-000016c0: 2070 726f 6d70 743d 7072 6f6d 7074 2c0a   prompt=prompt,.
-000016d0: 2020 2020 6d61 785f 746f 6b65 6e73 3d6d      max_tokens=m
-000016e0: 6178 5f74 6f6b 656e 732c 0a20 2020 206e  ax_tokens,.    n
-000016f0: 3d6e 2c0a 2020 2020 7465 6d70 6572 6174  =n,.    temperat
-00001700: 7572 653d 7465 6d70 6572 6174 7572 652c  ure=temperature,
-00001710: 0a20 2020 204d 4f4e 415f 6164 6469 7469  .    MONA_additi
-00001720: 6f6e 616c 5f64 6174 613d 7b22 6375 7374  onal_data={"cust
-00001730: 6f6d 6572 5f69 6422 3a20 2241 3533 3132  omer_id": "A5312
-00001740: 3531 227d 2c0a 2929 0a70 7269 6e74 2872  51"},.)).print(r
-00001750: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
-00001760: 305d 2e74 6578 7429 0a60 6060 0a0a 2323  0].text).```..##
-00001770: 2320 5573 696e 6720 4f70 656e 4149 2077  # Using OpenAI w
-00001780: 6974 6820 5245 5354 2063 616c 6c73 2069  ith REST calls i
-00001790: 6e73 7465 6164 206f 6620 4f70 656e 4149  nstead of OpenAI
-000017a0: 2773 2050 7974 686f 6e20 636c 6965 6e74  's Python client
-000017b0: 0a49 6e20 736f 6d65 2063 6173 6573 2079  .In some cases y
-000017c0: 6f75 206d 6179 2063 686f 6f73 6520 746f  ou may choose to
-000017d0: 2075 7365 204f 7065 6e41 4927 7320 4150   use OpenAI's AP
-000017e0: 4920 6469 7265 6374 6c79 2077 6974 6820  I directly with 
-000017f0: 5245 5354 2063 616c 6c73 2061 6e64 206e  REST calls and n
-00001800: 6f74 2075 7369 6e67 204f 7065 6e41 4927  ot using OpenAI'
-00001810: 7320 5344 4b2e 2046 6f72 2074 6865 7365  s SDK. For these
-00001820: 2063 6173 6573 2077 6520 616c 6c6f 7720   cases we allow 
-00001830: 6120 6d6f 7265 2064 6972 6563 7420 6170  a more direct ap
-00001840: 7072 6f61 6368 2066 6f72 206c 6f67 6769  proach for loggi
-00001850: 6e67 2074 6f20 4d6f 6e61 2061 7320 7765  ng to Mona as we
-00001860: 6c6c 2c20 6279 2075 7369 6e67 2074 6865  ll, by using the
-00001870: 2022 6765 745f 7265 7374 5f6d 6f6e 6974   "get_rest_monit
-00001880: 6f72 2220 6675 6e63 7469 6f6e 2e20 5365  or" function. Se
-00001890: 6520 6578 616d 706c 6520 6265 6c6f 772e  e example below.
-000018a0: 0a0a 6060 6070 790a 2320 4469 7265 6374  ..```py.# Direct
-000018b0: 2052 4553 5420 7573 6167 652c 2077 6974   REST usage, wit
-000018c0: 686f 7574 204f 7065 6e41 4920 636c 6965  hout OpenAI clie
-000018d0: 6e74 0a69 6d70 6f72 7420 7265 7175 6573  nt.import reques
-000018e0: 7473 0a66 726f 6d20 6f73 2069 6d70 6f72  ts.from os impor
-000018f0: 7420 656e 7669 726f 6e0a 6672 6f6d 206d  t environ.from m
-00001900: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
-00001910: 7420 6765 745f 7265 7374 5f6d 6f6e 6974  t get_rest_monit
-00001920: 6f72 0a0a 0a4d 4f4e 415f 4150 495f 4b45  or...MONA_API_KE
-00001930: 5920 3d20 656e 7669 726f 6e2e 6765 7428  Y = environ.get(
-00001940: 224d 4f4e 415f 4150 495f 4b45 5922 290a  "MONA_API_KEY").
-00001950: 4d4f 4e41 5f53 4543 5245 5420 3d20 656e  MONA_SECRET = en
-00001960: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
-00001970: 5345 4352 4554 2229 0a4d 4f4e 415f 4352  SECRET").MONA_CR
-00001980: 4544 5320 3d20 7b0a 2020 2020 226b 6579  EDS = {.    "key
-00001990: 223a 204d 4f4e 415f 4150 495f 4b45 592c  ": MONA_API_KEY,
-000019a0: 0a20 2020 2022 7365 6372 6574 223a 204d  .    "secret": M
-000019b0: 4f4e 415f 5345 4352 4554 2c0a 7d0a 434f  ONA_SECRET,.}.CO
-000019c0: 4e54 4558 545f 434c 4153 535f 4e41 4d45  NTEXT_CLASS_NAME
-000019d0: 203d 2022 534f 4d45 5f4d 4f4e 4954 4f52   = "SOME_MONITOR
-000019e0: 494e 475f 434f 4e54 4558 545f 4e41 4d45  ING_CONTEXT_NAME
-000019f0: 220a 0a23 2047 6574 204d 6f6e 6120 6c6f  "..# Get Mona lo
-00001a00: 6767 6572 0a6d 6f6e 615f 6c6f 6767 6572  gger.mona_logger
-00001a10: 203d 2067 6574 5f72 6573 745f 6d6f 6e69   = get_rest_moni
-00001a20: 746f 7228 0a20 2020 2022 436f 6d70 6c65  tor(.    "Comple
-00001a30: 7469 6f6e 222c 0a20 2020 204d 4f4e 415f  tion",.    MONA_
-00001a40: 4352 4544 532c 0a20 2020 2043 4f4e 5445  CREDS,.    CONTE
-00001a50: 5854 5f43 4c41 5353 5f4e 414d 452c 0a29  XT_CLASS_NAME,.)
-00001a60: 0a0a 2320 5365 7420 7570 2074 6865 2041  ..# Set up the A
-00001a70: 5049 2065 6e64 706f 696e 7420 5552 4c20  PI endpoint URL 
-00001a80: 616e 6420 6175 7468 656e 7469 6361 7469  and authenticati
-00001a90: 6f6e 2068 6561 6465 7273 0a75 726c 203d  on headers.url =
-00001aa0: 2022 6874 7470 733a 2f2f 6170 692e 6f70   "https://api.op
-00001ab0: 656e 6169 2e63 6f6d 2f76 312f 636f 6d70  enai.com/v1/comp
-00001ac0: 6c65 7469 6f6e 7322 0a68 6561 6465 7273  letions".headers
-00001ad0: 203d 207b 0a20 2020 2022 436f 6e74 656e   = {.    "Conten
-00001ae0: 742d 5479 7065 223a 2022 6170 706c 6963  t-Type": "applic
-00001af0: 6174 696f 6e2f 6a73 6f6e 222c 0a20 2020  ation/json",.   
-00001b00: 2022 4175 7468 6f72 697a 6174 696f 6e22   "Authorization"
-00001b10: 3a20 6622 4265 6172 6572 207b 656e 7669  : f"Bearer {envi
-00001b20: 726f 6e2e 6765 7428 274f 5045 4e5f 4149  ron.get('OPEN_AI
-00001b30: 5f4b 4559 2729 7d22 2c0a 7d0a 0a23 2053  _KEY')}",.}..# S
-00001b40: 6574 2075 7020 7468 6520 7265 7175 6573  et up the reques
-00001b50: 7420 6461 7461 0a64 6174 6120 3d20 7b0a  t data.data = {.
-00001b60: 2020 2020 2270 726f 6d70 7422 3a20 7072      "prompt": pr
-00001b70: 6f6d 7074 2c0a 2020 2020 226d 6178 5f74  ompt,.    "max_t
-00001b80: 6f6b 656e 7322 3a20 6d61 785f 746f 6b65  okens": max_toke
-00001b90: 6e73 2c0a 2020 2020 2274 656d 7065 7261  ns,.    "tempera
-00001ba0: 7475 7265 223a 2074 656d 7065 7261 7475  ture": temperatu
-00001bb0: 7265 2c0a 2020 2020 226d 6f64 656c 223a  re,.    "model":
-00001bc0: 206d 6f64 656c 2c0a 2020 2020 226e 223a   model,.    "n":
-00001bd0: 206e 2c0a 7d0a 0a23 2054 6865 206c 6f67   n,.}..# The log
-00001be0: 5f72 6571 7565 7374 2066 756e 6374 696f  _request functio
-00001bf0: 6e20 7265 7475 726e 7320 7477 6f20 6f74  n returns two ot
-00001c00: 6865 7220 6675 6e63 7469 6f6e 2066 6f72  her function for
-00001c10: 206c 6174 6572 206c 6f67 6769 6e67 0a23   later logging.#
-00001c20: 2074 6865 2072 6573 706f 6e73 6520 6f72   the response or
-00001c30: 2074 6865 2065 7863 6570 7469 6f6e 2e20   the exception. 
-00001c40: 5768 656e 2077 6520 6c61 7465 7220 646f  When we later do
-00001c50: 2074 6861 742c 2074 6865 206c 6f67 6765   that, the logge
-00001c60: 7220 7769 6c6c 0a23 2061 6374 7561 6c6c  r will.# actuall
-00001c70: 7920 6361 6c63 756c 6174 6520 616c 6c20  y calculate all 
-00001c80: 7468 6520 7265 6c65 7661 6e74 206d 6574  the relevant met
-00001c90: 7269 6373 2061 6e64 2077 696c 6c20 7365  rics and will se
-00001ca0: 6e64 2074 6865 6d20 746f 0a23 204d 6f6e  nd them to.# Mon
-00001cb0: 612e 0a72 6573 706f 6e73 655f 6c6f 6767  a..response_logg
-00001cc0: 6572 2c20 6578 6365 7074 696f 6e5f 6c6f  er, exception_lo
-00001cd0: 6767 6572 203d 206d 6f6e 615f 6c6f 6767  gger = mona_logg
-00001ce0: 6572 2e6c 6f67 5f72 6571 7565 7374 280a  er.log_request(.
-00001cf0: 2020 2020 6461 7461 2c20 6164 6469 7469      data, additi
-00001d00: 6f6e 616c 5f64 6174 613d 7b22 6375 7374  onal_data={"cust
-00001d10: 6f6d 6572 5f69 6422 3a20 2241 3533 3132  omer_id": "A5312
-00001d20: 3531 227d 0a29 0a0a 7472 793a 0a20 2020  51"}.)..try:.   
-00001d30: 2023 2053 656e 6420 7468 6520 7265 7175   # Send the requ
-00001d40: 6573 7420 746f 2074 6865 2041 5049 0a20  est to the API. 
-00001d50: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-00001d60: 7175 6573 7473 2e70 6f73 7428 7572 6c2c  quests.post(url,
-00001d70: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
-00001d80: 2c20 6a73 6f6e 3d64 6174 6129 0a0a 2020  , json=data)..  
-00001d90: 2020 2320 4368 6563 6b20 666f 7220 4854    # Check for HT
-00001da0: 5450 2065 7272 6f72 730a 2020 2020 7265  TP errors.    re
-00001db0: 7370 6f6e 7365 2e72 6169 7365 5f66 6f72  sponse.raise_for
-00001dc0: 5f73 7461 7475 7328 290a 0a20 2020 2023  _status()..    #
-00001dd0: 204c 6f67 2072 6573 706f 6e73 6520 746f   Log response to
-00001de0: 204d 6f6e 610a 2020 2020 7265 7370 6f6e   Mona.    respon
-00001df0: 7365 5f6c 6f67 6765 7228 7265 7370 6f6e  se_logger(respon
-00001e00: 7365 2e6a 736f 6e28 2929 0a20 2020 2070  se.json()).    p
-00001e10: 7269 6e74 2872 6573 706f 6e73 652e 6a73  rint(response.js
-00001e20: 6f6e 2829 5b22 6368 6f69 6365 7322 5d5b  on()["choices"][
-00001e30: 305d 5b22 7465 7874 225d 290a 0a65 7863  0]["text"])..exc
-00001e40: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00001e50: 2065 7272 3a0a 2020 2020 2320 4c6f 6720   err:.    # Log 
-00001e60: 6578 6365 7074 696f 6e20 746f 204d 6f6e  exception to Mon
-00001e70: 610a 2020 2020 6578 6365 7074 696f 6e5f  a.    exception_
-00001e80: 6c6f 6767 6572 2829 0a60 6060 0a0a 2323  logger().```..##
-00001e90: 2320 5374 7265 616d 2073 7570 706f 7274  # Stream support
-00001ea0: 0a0a 4f70 656e 4149 2061 6c6c 6f77 7320  ..OpenAI allows 
-00001eb0: 7265 6365 6976 696e 6720 7265 7370 6f6e  receiving respon
-00001ec0: 7365 7320 6173 2061 2073 7472 6561 6d20  ses as a stream 
-00001ed0: 6f66 2074 6f6b 656e 7320 7573 696e 6720  of tokens using 
-00001ee0: 7468 6520 2273 7472 6561 6d22 2070 6172  the "stream" par
-00001ef0: 616d 6574 6572 2e20 5768 656e 2074 6869  ameter. When thi
-00001f00: 7320 6973 2064 6f6e 652c 204d 6f6e 6120  s is done, Mona 
-00001f10: 7769 6c6c 2063 6f6c 6c65 6374 2061 6c6c  will collect all
-00001f20: 2074 6865 2074 6f6b 656e 7320 696e 206d   the tokens in m
-00001f30: 656d 6f72 7920 616e 6420 7769 6c6c 2063  emory and will c
-00001f40: 7265 6174 6520 7468 6520 616e 616c 7973  reate the analys
-00001f50: 6973 2061 6e64 206c 6f67 206f 7574 2074  is and log out t
-00001f60: 6865 2064 6174 6120 7468 6520 6d6f 6d65  he data the mome
-00001f70: 6e74 2074 6865 2073 7472 6561 6d20 6973  nt the stream is
-00001f80: 206f 7665 722e 2059 6f75 2064 6f6e 2774   over. You don't
-00001f90: 206e 6565 6420 746f 2064 6f20 616e 7974   need to do anyt
-00001fa0: 6869 6e67 2074 6f20 6d61 6b65 2074 6869  hing to make thi
-00001fb0: 7320 6861 7070 656e 2e0a 0a53 696e 6365  s happen...Since
-00001fc0: 2066 6f72 2073 7472 6561 6d69 6e67 2072   for streaming r
-00001fd0: 6573 706f 6e73 6573 204f 7065 6e41 4920  esponses OpenAI 
-00001fe0: 646f 6573 6e27 7420 7375 7070 6c79 2074  doesn't supply t
-00001ff0: 6865 2066 756c 6c20 7573 6167 6520 746f  he full usage to
-00002000: 6b65 6e73 2073 756d 6d61 7279 2c20 4d6f  kens summary, Mo
-00002010: 6e61 2075 7365 7320 7468 6520 7469 6b74  na uses the tikt
-00002020: 6f6b 656e 2070 6163 6b61 6765 2074 6f20  oken package to 
-00002030: 6361 6c63 756c 6174 6520 7468 6520 746f  calculate the to
-00002040: 6b65 6e73 206f 6620 7468 6520 7072 6f6d  kens of the prom
-00002050: 7074 2061 6e64 2063 6f6d 706c 6574 696f  pt and completio
-00002060: 6e20 616e 6420 6c6f 6720 7468 656d 2066  n and log them f
-00002070: 6f72 206d 6f6e 6974 6f72 696e 672e 0a0a  or monitoring...
-00002080: 4e4f 5445 3a20 5374 7265 616d 2069 7320  NOTE: Stream is 
-00002090: 6375 7272 656e 746c 7920 6f6e 6c79 2073  currently only s
-000020a0: 7570 706f 7274 6564 2077 6974 6820 5344  upported with SD
-000020b0: 4b20 7573 6167 652c 2061 6e64 206e 6f74  K usage, and not
-000020c0: 2077 6974 6820 7573 696e 6720 5245 5354   with using REST
-000020d0: 2064 6972 6563 746c 792e 0a0a 0a23 2320   directly....## 
-000020e0: 4d6f 6e61 2053 444b 0a0a 5468 6973 2070  Mona SDK..This p
-000020f0: 6163 6b61 6765 2075 7365 7320 7468 6520  ackage uses the 
-00002100: 6d6f 6e61 5f73 646b 2070 6163 6b61 6765  mona_sdk package
-00002110: 2074 6f20 6578 706f 7274 2074 6865 2072   to export the r
-00002120: 656c 6576 616e 7420 6461 7461 2074 6f20  elevant data to 
-00002130: 4d6f 6e61 2e20 5468 6572 6520 6172 6520  Mona. There are 
-00002140: 7365 7665 7261 6c20 656e 7669 726f 6e6d  several environm
-00002150: 656e 7420 7661 7269 6162 6c65 7320 796f  ent variables yo
-00002160: 7520 6361 6e20 7573 6520 746f 2063 6f6e  u can use to con
-00002170: 6669 6775 7265 2074 6865 2053 444b 2773  figure the SDK's
-00002180: 2062 6568 6176 696f 722e 2046 6f72 2065   behavior. For e
-00002190: 7861 6d70 6c65 2c20 796f 7520 6361 6e20  xample, you can 
-000021a0: 7365 7420 6974 2075 7020 746f 2072 6169  set it up to rai
-000021b0: 7365 2065 7863 6570 7469 6f6e 7320 7768  se exceptions wh
-000021c0: 656e 2065 7870 6f72 7469 6e67 2064 6174  en exporting dat
-000021d0: 6120 746f 204d 6f6e 6120 6661 696c 7320  a to Mona fails 
-000021e0: 2869 7420 646f 6573 6e27 7420 646f 2074  (it doesn't do t
-000021f0: 6861 7420 6279 2064 6566 6175 6c74 292e  hat by default).
-00002200: 0a0a 2323 204d 6f6e 6974 6f72 696e 6720  ..## Monitoring 
-00002210: 666f 7220 7072 6f66 616e 6974 790a 0a4d  for profanity..M
-00002220: 6f6e 6120 7573 6573 2074 6865 2061 6c74  ona uses the alt
-00002230: 2d70 726f 6661 6e69 7479 2d63 6865 636b  -profanity-check
-00002240: 2070 6163 616b 6765 2028 6874 7470 733a   pacakge (https:
-00002250: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00002260: 6374 2f61 6c74 2d70 726f 6661 6e69 7479  ct/alt-profanity
-00002270: 2d63 6865 636b 2f29 2074 6f20 6372 6561  -check/) to crea
-00002280: 7465 2062 6f74 6820 626f 6f6c 6561 6e20  te both boolean 
-00002290: 7072 6564 6963 7469 6f6e 7320 616e 6420  predictions and 
-000022a0: 7072 6f62 6162 696c 7479 2073 636f 7265  probabilty score
-000022b0: 7320 666f 7220 7468 6520 6578 6973 7465  s for the existe
-000022c0: 6e63 6520 6f66 2070 726f 6661 6e69 7479  nce of profanity
-000022d0: 2062 6f74 6820 696e 2074 6865 2070 726f   both in the pro
-000022e0: 6d70 7420 616e 6420 696e 2074 6865 2072  mpt and in the r
-000022f0: 6573 706f 6e73 6573 2e20 5765 2075 7365  esponses. We use
-00002300: 2074 6865 2062 7569 6c74 2069 6e20 7061   the built in pa
-00002310: 636b 6167 6520 6d65 7468 6f64 7320 666f  ckage methods fo
-00002320: 7220 7468 6174 2e20 4966 2079 6f75 2077  r that. If you w
-00002330: 616e 742c 2066 6f72 2065 7861 6d70 6c65  ant, for example
-00002340: 2c20 746f 2075 7365 2061 2064 6966 6665  , to use a diffe
-00002350: 7265 6e74 2070 726f 6261 6269 6c69 7479  rent probability
-00002360: 2074 6872 6573 686f 6c64 2066 6f72 2074   threshold for t
-00002370: 6865 2062 6f6f 6c65 616e 2070 7265 6469  he boolean predi
-00002380: 6374 696f 6e2c 2079 6f75 2063 616e 2064  ction, you can d
-00002390: 6f20 7468 6174 2062 7920 6368 616e 6769  o that by changi
-000023a0: 6e67 2079 6f75 7220 4d6f 6e61 2063 6f6e  ng your Mona con
-000023b0: 6669 6720 6f6e 2074 6865 204d 6f6e 6120  fig on the Mona 
-000023c0: 6461 7368 626f 6172 642e                 dashboard.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e61  : 2.1.Name: mona
+00000020: 2d6f 7065 6e61 690a 5665 7273 696f 6e3a  -openai.Version:
+00000030: 2030 2e30 2e38 0a53 756d 6d61 7279 3a20   0.0.8.Summary: 
+00000040: 496e 7465 6772 6174 696f 6e20 636c 6965  Integration clie
+00000050: 6e74 2066 6f72 206d 6f6e 6974 6f72 696e  nt for monitorin
+00000060: 6720 4f70 656e 4149 2075 7361 6765 2077  g OpenAI usage w
+00000070: 6974 6820 4d6f 6e61 0a41 7574 686f 722d  ith Mona.Author-
+00000080: 656d 6169 6c3a 2049 7461 6920 4261 7220  email: Itai Bar 
+00000090: 5369 6e61 6920 3c69 7461 6940 6d6f 6e61  Sinai <itai@mona
+000000a0: 6c61 6273 2e69 6f3e 0a50 726f 6a65 6374  labs.io>.Project
+000000b0: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
+000000c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000d0: 6f6d 2f6d 6f6e 616c 6162 732f 6d6f 6e61  om/monalabs/mona
+000000e0: 2d6f 7065 6e61 690a 5072 6f6a 6563 742d  -openai.Project-
+000000f0: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
+00000100: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000110: 2e63 6f6d 2f6d 6f6e 616c 6162 732f 6d6f  .com/monalabs/mo
+00000120: 6e61 2d6f 7065 6e61 692f 6973 7375 6573  na-openai/issues
+00000130: 0a4b 6579 776f 7264 733a 204f 7065 6e41  .Keywords: OpenA
+00000140: 492c 4c4c 4d73 2c47 5054 2c4d 6f6e 612c  I,LLMs,GPT,Mona,
+00000150: 4d6f 6e69 746f 7269 6e67 2c41 490a 436c  Monitoring,AI.Cl
+00000160: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000170: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000180: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+00000190: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+000001a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001b0: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
+000001c0: 7761 7265 204c 6963 656e 7365 0a43 6c61  ware License.Cla
+000001d0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
+000001e0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+000001f0: 496e 6465 7065 6e64 656e 740a 5265 7175  Independent.Requ
+00000200: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
+00000210: 2e39 0a44 6573 6372 6970 7469 6f6e 2d43  .9.Description-C
+00000220: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000230: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+00000240: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000250: 0a0a 2320 4d6f 6e61 2d4f 7065 6e41 4920  ..# Mona-OpenAI 
+00000260: 496e 7465 6772 6174 696f 6e20 436c 6965  Integration Clie
+00000270: 6e74 0a3c 7020 616c 6967 6e3d 2263 656e  nt.<p align="cen
+00000280: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
+00000290: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000002a0: 2e63 6f6d 2f6d 6f6e 616c 6162 732f 6d6f  .com/monalabs/mo
+000002b0: 6e61 2d73 646b 2f62 6c6f 622f 6d61 696e  na-sdk/blob/main
+000002c0: 2f6d 6f6e 615f 6c6f 676f 2e70 6e67 3f72  /mona_logo.png?r
+000002d0: 6177 3d74 7275 6522 2061 6c74 3d22 4d6f  aw=true" alt="Mo
+000002e0: 6e61 2773 206c 6f67 6f22 2077 6964 7468  na's logo" width
+000002f0: 3d22 3138 3022 2f3e 0a3c 2f70 3e0a 0a3c  ="180"/>.</p>..<
+00000300: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000310: 3e3c 6120 7461 7267 6574 3d22 5f62 6c61  ><a target="_bla
+00000320: 6e6b 2220 6872 6566 3d22 6874 7470 733a  nk" href="https:
+00000330: 2f2f 6d6f 6e61 6c61 6273 2e77 6973 7469  //monalabs.wisti
+00000340: 612e 636f 6d2f 6d65 6469 6173 2f6c 3678  a.com/medias/l6x
+00000350: 6d64 6a33 6364 363f 7776 6964 656f 3d6c  mdj3cd6?wvideo=l
+00000360: 3678 6d64 6a33 6364 3622 3e3c 696d 6720  6xmdj3cd6"><img 
+00000370: 7372 633d 2268 7474 7073 3a2f 2f65 6d62  src="https://emb
+00000380: 6564 2d73 736c 2e77 6973 7469 612e 636f  ed-ssl.wistia.co
+00000390: 6d2f 6465 6c69 7665 7269 6573 2f63 3135  m/deliveries/c15
+000003a0: 6262 3631 3661 3338 3966 6137 6437 3532  bb616a389fa7d752
+000003b0: 3936 3863 6362 3361 6632 6162 342e 6a70  968ccb3af2ab4.jp
+000003c0: 673f 7769 7374 6961 2d6c 3678 6d64 6a33  g?wistia-l6xmdj3
+000003d0: 6364 362d 312d 6c36 786d 646a 3363 6436  cd6-1-l6xmdj3cd6
+000003e0: 2d76 6964 656f 2d74 6875 6d62 6e61 696c  -video-thumbnail
+000003f0: 3d31 2661 6d70 3b69 6d61 6765 5f70 6c61  =1&amp;image_pla
+00000400: 795f 6275 7474 6f6e 5f73 697a 653d 3278  y_button_size=2x
+00000410: 2661 6d70 3b69 6d61 6765 5f63 726f 705f  &amp;image_crop_
+00000420: 7265 7369 7a65 643d 3936 3078 3534 3026  resized=960x540&
+00000430: 616d 703b 696d 6167 655f 706c 6179 5f62  amp;image_play_b
+00000440: 7574 746f 6e3d 3126 616d 703b 696d 6167  utton=1&amp;imag
+00000450: 655f 706c 6179 5f62 7574 746f 6e5f 636f  e_play_button_co
+00000460: 6c6f 723d 3636 6337 6431 6530 2220 7769  lor=66c7d1e0" wi
+00000470: 6474 683d 2234 3030 2220 6865 6967 6874  dth="400" height
+00000480: 3d22 3232 3522 2073 7479 6c65 3d22 7769  ="225" style="wi
+00000490: 6474 683a 2034 3030 7078 3b20 6865 6967  dth: 400px; heig
+000004a0: 6874 3a20 3232 3570 783b 223e 3c2f 613e  ht: 225px;"></a>
+000004b0: 3c2f 703e 3c70 2061 6c69 676e 3d22 6365  </p><p align="ce
+000004c0: 6e74 6572 223e 3c61 2068 7265 663d 2268  nter"><a href="h
+000004d0: 7474 7073 3a2f 2f6d 6f6e 616c 6162 732e  ttps://monalabs.
+000004e0: 7769 7374 6961 2e63 6f6d 2f6d 6564 6961  wistia.com/media
+000004f0: 732f 6c36 786d 646a 3363 6436 3f77 7669  s/l6xmdj3cd6?wvi
+00000500: 6465 6f3d 6c36 786d 646a 3363 6436 223e  deo=l6xmdj3cd6">
+00000510: 4f70 656e 4149 2047 5054 2049 6e74 6567  OpenAI GPT Integ
+00000520: 7261 7469 6f6e 2054 7574 6f72 6961 6c3c  ration Tutorial<
+00000530: 2f61 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e  /a></p>...Use on
+00000540: 6520 6c69 6e65 206f 6620 636f 6465 2074  e line of code t
+00000550: 6f20 6765 7420 696e 7374 616e 7420 6c69  o get instant li
+00000560: 7665 206d 6f6e 6974 6f72 696e 6720 666f  ve monitoring fo
+00000570: 7220 796f 7572 204f 7065 6e41 4920 7573  r your OpenAI us
+00000580: 6167 6520 696e 636c 7564 696e 673a 0a2a  age including:.*
+00000590: 2054 6f6b 656e 7320 7573 6167 650a 2a20   Tokens usage.* 
+000005a0: 4861 6c6c 7563 696e 6174 696f 6e20 616c  Hallucination al
+000005b0: 6572 7473 0a2a 2050 726f 6661 6e69 7479  erts.* Profanity
+000005c0: 2061 6e64 2070 7269 7661 6379 2061 6e61   and privacy ana
+000005d0: 6c79 7365 730a 2a20 4265 6861 7669 6f72  lyses.* Behavior
+000005e0: 616c 2064 7269 6674 7320 616e 6420 616e  al drifts and an
+000005f0: 6f6d 616c 6965 730a 2a20 4c61 6e67 4368  omalies.* LangCh
+00000600: 6169 6e20 7375 7070 6f72 740a 2a20 4d75  ain support.* Mu
+00000610: 6368 206d 7563 6820 6d6f 7265 0a0a 2323  ch much more..##
+00000620: 2053 6574 7469 6e67 2055 700a 0a2d 2054   Setting Up..- T
+00000630: 4f44 4f3a 2041 6464 2070 6172 7420 6162  ODO: Add part ab
+00000640: 6f75 7420 4d6f 6e61 2072 6567 6973 7472  out Mona registr
+00000650: 6174 696f 6e20 7769 7468 2061 206c 696e  ation with a lin
+00000660: 6b20 746f 2074 6865 2072 656c 6576 616e  k to the relevan
+00000670: 7420 6c61 6e64 696e 6720 7061 6765 2077  t landing page w
+00000680: 6865 7265 2074 6865 2072 6561 6465 7220  here the reader 
+00000690: 6361 6e20 7369 676e 2075 702e 0a60 6060  can sign up..```
+000006a0: 636f 6e73 6f6c 650a 2420 7069 7020 696e  console.$ pip in
+000006b0: 7374 616c 6c20 6d6f 6e61 5f6f 7065 6e61  stall mona_opena
+000006c0: 690a 6060 600a 0a23 2320 5175 6963 6b20  i.```..## Quick 
+000006d0: 5374 6172 7420 616e 6420 4578 616d 706c  Start and Exampl
+000006e0: 650a 0a45 7861 6d70 6c65 2062 6f69 6c65  e..Example boile
+000006f0: 7270 6c61 7465 2063 6f64 6520 666f 7220  rplate code for 
+00000700: 626f 7468 2073 796e 6320 616e 6420 6173  both sync and as
+00000710: 796e 6320 7573 6167 6520 6973 2067 6976  ync usage is giv
+00000720: 656e 2069 6e20 7468 6520 6669 6c65 2022  en in the file "
+00000730: 6578 616d 706c 655f 7573 6167 652e 7079  example_usage.py
+00000740: 2220 616e 6420 6865 7265 3a0a 6060 6070  " and here:.```p
+00000750: 790a 6672 6f6d 206f 7320 696d 706f 7274  y.from os import
+00000760: 2065 6e76 6972 6f6e 0a69 6d70 6f72 7420   environ.import 
+00000770: 6173 796e 6369 6f0a 696d 706f 7274 206f  asyncio.import o
+00000780: 7065 6e61 690a 0a66 726f 6d20 6d6f 6e61  penai..from mona
+00000790: 5f6f 7065 6e61 6920 696d 706f 7274 206d  _openai import m
+000007a0: 6f6e 6974 6f72 0a0a 6f70 656e 6169 2e61  onitor..openai.a
+000007b0: 7069 5f6b 6579 203d 2065 6e76 6972 6f6e  pi_key = environ
+000007c0: 2e67 6574 2822 4f50 454e 5f41 495f 4b45  .get("OPEN_AI_KE
+000007d0: 5922 290a 0a4d 4f4e 415f 4150 495f 4b45  Y")..MONA_API_KE
+000007e0: 5920 3d20 656e 7669 726f 6e2e 6765 7428  Y = environ.get(
+000007f0: 224d 4f4e 415f 4150 495f 4b45 5922 290a  "MONA_API_KEY").
+00000800: 4d4f 4e41 5f53 4543 5245 5420 3d20 656e  MONA_SECRET = en
+00000810: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
+00000820: 5345 4352 4554 2229 0a4d 4f4e 415f 4352  SECRET").MONA_CR
+00000830: 4544 5320 3d20 7b0a 2020 2020 226b 6579  EDS = {.    "key
+00000840: 223a 204d 4f4e 415f 4150 495f 4b45 592c  ": MONA_API_KEY,
+00000850: 0a20 2020 2022 7365 6372 6574 223a 204d  .    "secret": M
+00000860: 4f4e 415f 5345 4352 4554 2c0a 7d0a 434f  ONA_SECRET,.}.CO
+00000870: 4e54 4558 545f 434c 4153 535f 4e41 4d45  NTEXT_CLASS_NAME
+00000880: 203d 2022 534f 4d45 5f4d 4f4e 4954 4f52   = "SOME_MONITOR
+00000890: 494e 475f 434f 4e54 4558 545f 4e41 4d45  ING_CONTEXT_NAME
+000008a0: 220a 0a0a 6d6f 6e69 746f 7265 645f 636f  "...monitored_co
+000008b0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
+000008c0: 6f72 280a 2020 2020 6f70 656e 6169 2e43  or(.    openai.C
+000008d0: 6f6d 706c 6574 696f 6e2c 0a20 2020 204d  ompletion,.    M
+000008e0: 4f4e 415f 4352 4544 532c 0a20 2020 2043  ONA_CREDS,.    C
+000008f0: 4f4e 5445 5854 5f43 4c41 5353 5f4e 414d  ONTEXT_CLASS_NAM
+00000900: 452c 0a29 0a0a 0a70 726f 6d70 7420 3d20  E,.)...prompt = 
+00000910: 2249 2077 616e 7420 746f 2067 656e 6572  "I want to gener
+00000920: 6174 6520 736f 6d65 2074 6578 7420 6162  ate some text ab
+00000930: 6f75 7420 220a 6d6f 6465 6c20 3d20 2274  out ".model = "t
+00000940: 6578 742d 6164 612d 3030 3122 0a74 656d  ext-ada-001".tem
+00000950: 7065 7261 7475 7265 203d 2030 2e36 0a6d  perature = 0.6.m
+00000960: 6178 5f74 6f6b 656e 7320 3d20 350a 6e20  ax_tokens = 5.n 
+00000970: 3d20 310a 0a23 2052 6567 756c 6172 2028  = 1..# Regular (
+00000980: 7379 6e63 2920 7573 6167 650a 7265 7370  sync) usage.resp
+00000990: 6f6e 7365 203d 206d 6f6e 6974 6f72 6564  onse = monitored
+000009a0: 5f63 6f6d 706c 6574 696f 6e2e 6372 6561  _completion.crea
+000009b0: 7465 280a 2020 2020 656e 6769 6e65 3d6d  te(.    engine=m
+000009c0: 6f64 656c 2c0a 2020 2020 7072 6f6d 7074  odel,.    prompt
+000009d0: 3d70 726f 6d70 742c 0a20 2020 206d 6178  =prompt,.    max
+000009e0: 5f74 6f6b 656e 733d 6d61 785f 746f 6b65  _tokens=max_toke
+000009f0: 6e73 2c0a 2020 2020 6e3d 6e2c 0a20 2020  ns,.    n=n,.   
+00000a00: 2074 656d 7065 7261 7475 7265 3d74 656d   temperature=tem
+00000a10: 7065 7261 7475 7265 2c0a 2020 2020 4d4f  perature,.    MO
+00000a20: 4e41 5f61 6464 6974 696f 6e61 6c5f 6461  NA_additional_da
+00000a30: 7461 3d7b 2263 7573 746f 6d65 725f 6964  ta={"customer_id
+00000a40: 223a 2022 4135 3331 3235 3122 7d2c 0a29  ": "A531251"},.)
+00000a50: 0a70 7269 6e74 2872 6573 706f 6e73 652e  .print(response.
+00000a60: 6368 6f69 6365 735b 305d 2e74 6578 7429  choices[0].text)
+00000a70: 0a0a 2320 4173 796e 6320 7573 6167 650a  ..# Async usage.
+00000a80: 7265 7370 6f6e 7365 203d 2061 7379 6e63  response = async
+00000a90: 696f 2e72 756e 286d 6f6e 6974 6f72 6564  io.run(monitored
+00000aa0: 5f63 6f6d 706c 6574 696f 6e2e 6163 7265  _completion.acre
+00000ab0: 6174 6528 0a20 2020 2065 6e67 696e 653d  ate(.    engine=
+00000ac0: 6d6f 6465 6c2c 0a20 2020 2070 726f 6d70  model,.    promp
+00000ad0: 743d 7072 6f6d 7074 2c0a 2020 2020 6d61  t=prompt,.    ma
+00000ae0: 785f 746f 6b65 6e73 3d6d 6178 5f74 6f6b  x_tokens=max_tok
+00000af0: 656e 732c 0a20 2020 206e 3d6e 2c0a 2020  ens,.    n=n,.  
+00000b00: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
+00000b10: 6d70 6572 6174 7572 652c 0a20 2020 204d  mperature,.    M
+00000b20: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
+00000b30: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+00000b40: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
+00000b50: 2929 0a0a 7072 696e 7428 7265 7370 6f6e  ))..print(respon
+00000b60: 7365 2e63 686f 6963 6573 5b30 5d2e 7465  se.choices[0].te
+00000b70: 7874 290a 6060 600a 2323 2053 7570 706f  xt).```.## Suppo
+00000b80: 7274 6564 204f 7065 6e41 4920 4150 4973  rted OpenAI APIs
+00000b90: 0a43 7572 7265 6e74 6c79 2074 6869 7320  .Currently this 
+00000ba0: 636c 6965 6e74 2073 7570 706f 7274 7320  client supports 
+00000bb0: 606f 7065 6e61 692e 436f 6d70 6c65 7469  `openai.Completi
+00000bc0: 6f6e 6020 616e 6420 606f 7065 6e61 692e  on` and `openai.
+00000bd0: 4368 6174 436f 6d70 6c65 7469 6f6e 602e  ChatCompletion`.
+00000be0: 204d 6f6e 6120 6361 6e20 7375 7070 6f72   Mona can suppor
+00000bf0: 7420 7072 6f63 6573 7365 7320 6261 7365  t processes base
+00000c00: 6420 6f6e 206f 7468 6572 2041 5049 7320  d on other APIs 
+00000c10: 616e 6420 616c 736f 206e 6f6e 2d4f 7065  and also non-Ope
+00000c20: 6e41 492d 6261 7365 6420 6170 7073 2e0a  nAI-based apps..
+00000c30: 4966 2079 6f75 2068 6176 6520 6120 6469  If you have a di
+00000c40: 6666 6572 7265 6e74 2075 7365 2d63 6173  fferrent use-cas
+00000c50: 652c 2077 6527 6420 6c6f 7665 2074 6f20  e, we'd love to 
+00000c60: 6865 6172 2061 626f 7574 2069 7421 2050  hear about it! P
+00000c70: 6c65 6173 6520 656d 6169 6c20 7573 2061  lease email us a
+00000c80: 7420 7375 7070 6f72 7440 6d6f 6e61 6c61  t support@monala
+00000c90: 6273 2e69 6f2e 0a0a 2323 2055 7361 6765  bs.io...## Usage
+00000ca0: 0a23 2323 2049 6e69 7469 616c 697a 6174  .### Initializat
+00000cb0: 696f 6e0a 0a54 6865 206d 6169 6e20 616e  ion..The main an
+00000cc0: 6420 6f6e 6c79 2066 756e 6374 696f 6e20  d only function 
+00000cd0: 6578 706f 7365 6420 696e 2074 6869 7320  exposed in this 
+00000ce0: 7061 636b 6167 6520 6973 2060 6d6f 6e69  package is `moni
+00000cf0: 746f 7260 2e0a 6060 6070 790a 696d 706f  tor`..```py.impo
+00000d00: 7274 206f 7065 6e61 690a 0a66 726f 6d20  rt openai..from 
+00000d10: 6d6f 6e61 5f6f 7065 6e61 6920 696d 706f  mona_openai impo
+00000d20: 7274 206d 6f6e 6974 6f72 0a0a 6f70 656e  rt monitor..open
+00000d30: 6169 2e61 7069 5f6b 6579 203d 2065 6e76  ai.api_key = env
+00000d40: 6972 6f6e 2e67 6574 2822 4f50 454e 5f41  iron.get("OPEN_A
+00000d50: 495f 4b45 5922 290a 0a6d 6f6e 6974 6f72  I_KEY")..monitor
+00000d60: 6564 5f63 6f6d 706c 6574 696f 6e20 3d20  ed_completion = 
+00000d70: 6d6f 6e69 746f 7228 0a20 2020 206f 7065  monitor(.    ope
+00000d80: 6e61 692e 436f 6d70 6c65 7469 6f6e 2c0a  nai.Completion,.
+00000d90: 2020 2020 280a 2020 2020 2020 2020 656e      (.        en
+00000da0: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
+00000db0: 4150 495f 4b45 5922 292c 0a20 2020 2020  API_KEY"),.     
+00000dc0: 2020 2065 6e76 6972 6f6e 2e67 6574 2822     environ.get("
+00000dd0: 4d4f 4e41 5f53 4543 5245 5422 292c 0a20  MONA_SECRET"),. 
+00000de0: 2020 2029 2c0a 2020 2020 2253 4f4d 455f     ),.    "SOME_
+00000df0: 4d4f 4e49 544f 5249 4e47 5f43 4f4e 5445  MONITORING_CONTE
+00000e00: 5854 5f4e 414d 4522 2c0a 2020 2020 7b22  XT_NAME",.    {"
+00000e10: 616e 616c 7973 6973 223a 207b 2270 726f  analysis": {"pro
+00000e20: 6661 6e69 7479 223a 2046 616c 7365 7d7d  fanity": False}}
+00000e30: 0a29 0a0a 2e2e 2e0a 0a6d 6f6e 6974 6f72  .).......monitor
+00000e40: 6564 5f63 6f6d 706c 6574 696f 6e2e 6372  ed_completion.cr
+00000e50: 6561 7465 282e 2e2e 290a 6060 600a 0a54  eate(...).```..T
+00000e60: 6865 2060 6d6f 6e69 746f 7260 2066 756e  he `monitor` fun
+00000e70: 6374 696f 6e20 7265 7475 726e 7320 746f  ction returns to
+00000e80: 2079 6f75 2061 2063 6c61 7373 2074 6861   you a class tha
+00000e90: 7420 7772 6170 7320 7468 6520 6f72 6967  t wraps the orig
+00000ea0: 696e 616c 206f 7065 6e61 6920 656e 6470  inal openai endp
+00000eb0: 6f69 6e74 2063 6c61 7373 2079 6f75 2070  oint class you p
+00000ec0: 726f 7669 6465 2c20 7769 7468 2061 6e20  rovide, with an 
+00000ed0: 6571 7569 7661 6c65 6e74 2041 5049 2028  equivalent API (
+00000ee0: 6265 7369 6465 7320 736f 6d65 2061 6464  besides some add
+00000ef0: 6974 696f 6e73 206c 6973 7465 6420 6265  itions listed be
+00000f00: 6c6f 7729 2e0a 596f 7520 6361 6e20 7468  low)..You can th
+00000f10: 656e 2075 7365 2074 6865 2072 6574 7572  en use the retur
+00000f20: 6e65 6420 636c 6173 7327 2022 6372 6561  ned class' "crea
+00000f30: 7465 2220 616e 6420 2261 6372 6561 7465  te" and "acreate
+00000f40: 2220 6675 6e63 7469 6f6e 7320 6a75 7374  " functions just
+00000f50: 2061 7320 796f 7520 776f 756c 6420 6265   as you would be
+00000f60: 666f 7265 2c20 6f6e 6c79 206e 6f77 2c20  fore, only now, 
+00000f70: 6265 7369 6465 7320 6765 7474 696e 6720  besides getting 
+00000f80: 7468 6520 7265 7175 6573 7465 6420 6f70  the requested op
+00000f90: 656e 4149 2066 756e 6374 696f 6e61 6c69  enAI functionali
+00000fa0: 7479 2c20 7468 6973 2063 6c69 656e 7420  ty, this client 
+00000fb0: 7769 6c6c 206c 6f67 206f 7574 2074 6f20  will log out to 
+00000fc0: 4d6f 6e61 2773 2073 6572 7665 7220 7468  Mona's server th
+00000fd0: 6520 7061 7261 6d65 7465 7273 2079 6f75  e parameters you
+00000fe0: 2075 7365 6420 2865 2e67 2e2c 2074 656d   used (e.g., tem
+00000ff0: 7065 7261 7475 7265 292c 2064 6174 6120  perature), data 
+00001000: 6162 6f75 7420 7468 6520 7265 7370 6f6e  about the respon
+00001010: 7365 2066 726f 6d20 4f70 656e 4149 2773  se from OpenAI's
+00001020: 2073 6572 7665 722c 2061 6e64 2063 7573   server, and cus
+00001030: 746f 6d20 616e 616c 7973 6573 2061 626f  tom analyses abo
+00001040: 7574 2074 6865 2063 616c 6c20 2865 2e67  ut the call (e.g
+00001050: 2e2c 2070 726f 6661 6e69 7479 2073 636f  ., profanity sco
+00001060: 7265 732c 2070 7269 7661 6379 2063 6865  res, privacy che
+00001070: 636b 7320 666f 7220 656d 6169 6c73 2f70  cks for emails/p
+00001080: 686f 6e65 206e 756d 6265 7273 2066 6f75  hone numbers fou
+00001090: 6e64 2069 6e20 7468 6520 7465 7874 732c  nd in the texts,
+000010a0: 2074 6578 7475 616c 2061 6e61 6c79 7365   textual analyse
+000010b0: 732c 2065 7463 2e2e 2e29 0a0a 5468 6520  s, etc...)..The 
+000010c0: 606d 6f6e 6974 6f72 6020 6675 6e63 7469  `monitor` functi
+000010d0: 6f6e 2072 6563 6569 7665 7320 7468 6520  on receives the 
+000010e0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
+000010f0: 6e74 733a 0a6f 7065 6e61 695f 636c 6173  nts:.openai_clas
+00001100: 733a 2041 6e20 4f70 656e 4149 2041 5049  s: An OpenAI API
+00001110: 2063 6c61 7373 2074 6f20 7772 6170 2077   class to wrap w
+00001120: 6974 6820 6d6f 6e69 746f 7269 6e67 2063  ith monitoring c
+00001130: 6170 6162 696c 7469 6573 2e0a 6d6f 6e61  apabilties..mona
+00001140: 5f63 7265 6473 3a20 4120 6469 6374 2028  _creds: A dict (
+00001150: 636f 6e74 6169 6e69 6e67 2022 6b65 7922  containing "key"
+00001160: 2061 6e64 2022 7365 6372 6574 2229 206f   and "secret") o
+00001170: 7220 7061 6972 2028 7475 706c 6529 206f  r pair (tuple) o
+00001180: 6620 4d6f 6e61 2041 5049 206b 6579 2061  f Mona API key a
+00001190: 6e64 2073 6563 7265 7420 746f 2073 6574  nd secret to set
+000011a0: 2075 7020 4d6f 6e61 2773 2063 6c69 656e   up Mona's clien
+000011b0: 7473 2066 726f 6d20 6974 7320 5344 4b2e  ts from its SDK.
+000011c0: 0a63 6f6e 7465 7874 5f63 6c61 7373 3a20  .context_class: 
+000011d0: 5468 6520 4d6f 6e61 2063 6f6e 7465 7874  The Mona context
+000011e0: 2063 6c61 7373 206e 616d 6520 746f 2075   class name to u
+000011f0: 7365 2066 6f72 206d 6f6e 6974 6f72 696e  se for monitorin
+00001200: 672e 2055 7365 2061 2063 6f6e 7374 616e  g. Use a constan
+00001210: 7420 6e61 6d65 206f 6620 796f 7572 2063  t name of your c
+00001220: 686f 6963 652e 0a73 7065 6373 3a20 4120  hoice..specs: A 
+00001230: 6469 6374 696f 6e61 7279 206f 6620 7370  dictionary of sp
+00001240: 6563 6966 6963 6174 696f 6e73 2073 7563  ecifications suc
+00001250: 6820 6173 206d 6f6e 6974 6f72 696e 6720  h as monitoring 
+00001260: 7361 6d70 6c69 6e67 2072 6174 696f 2e0a  sampling ratio..
+00001270: 0a23 2323 2320 5370 6563 730a 5468 6520  .#### Specs.The 
+00001280: 7370 6563 7320 6172 6720 616c 6c6f 7773  specs arg allows
+00001290: 2079 6f75 2074 6f20 636f 6e66 6967 7572   you to configur
+000012a0: 6520 7768 6174 2073 686f 756c 6420 6265  e what should be
+000012b0: 206d 6f6e 6974 6f72 6564 2e20 4974 2065   monitored. It e
+000012c0: 7870 6563 7473 2061 2070 7974 686f 6e20  xpects a python 
+000012d0: 6469 6374 2077 6974 6820 7468 6520 666f  dict with the fo
+000012e0: 6c6c 776f 696e 6720 706f 7373 6962 6c65  llwoing possible
+000012f0: 206b 6579 733a 0a2a 2073 616d 706c 696e   keys:.* samplin
+00001300: 675f 7261 7469 6f20 2831 293a 2041 206e  g_ratio (1): A n
+00001310: 756d 6265 7220 6265 7477 6565 6e20 3020  umber between 0 
+00001320: 616e 6420 3120 666f 7220 686f 7720 6f66  and 1 for how of
+00001330: 7465 6e20 7368 6f75 6c64 2074 6865 2063  ten should the c
+00001340: 616c 6c20 6265 206c 6f67 6765 642e 0a2a  all be logged..*
+00001350: 2061 766f 6964 5f6d 6f6e 6974 6f72 696e   avoid_monitorin
+00001360: 675f 6578 6365 7074 696f 6e73 2028 4661  g_exceptions (Fa
+00001370: 6c73 6529 3a20 5768 6574 6865 7220 6f72  lse): Whether or
+00001380: 206e 6f74 2074 6f20 6c6f 6720 6f75 7420   not to log out 
+00001390: 746f 204d 6f6e 6120 7768 656e 2074 6865  to Mona when the
+000013a0: 7265 2069 7320 616e 204f 7065 6e41 4920  re is an OpenAI 
+000013b0: 6578 6365 7074 696f 6e2e 2044 6566 6175  exception. Defau
+000013c0: 6c74 2069 7320 746f 2074 7261 636b 2065  lt is to track e
+000013d0: 7863 6570 7469 6f6e 7320 2d20 616e 6420  xceptions - and 
+000013e0: 4d6f 6e61 2077 696c 6c20 616c 6572 7420  Mona will alert 
+000013f0: 796f 7520 6f6e 2074 6869 6e67 7320 6c69  you on things li
+00001400: 6b65 2061 206a 756d 7020 696e 206e 756d  ke a jump in num
+00001410: 6265 7220 6f66 2065 7863 6570 7469 6f6e  ber of exception
+00001420: 730a 2a20 6578 706f 7274 5f70 726f 6d70  s.* export_promp
+00001430: 7420 2846 616c 7365 293a 2057 6865 7468  t (False): Wheth
+00001440: 6572 204d 6f6e 6120 7368 6f75 6c64 2065  er Mona should e
+00001450: 7870 6f72 7420 7468 6520 6163 7475 616c  xport the actual
+00001460: 2070 726f 6d70 7420 7465 7874 2e20 4265   prompt text. Be
+00001470: 2064 6566 6175 6c74 2073 6574 2074 6f20   default set to 
+00001480: 4661 6c73 6520 746f 2061 766f 6964 2070  False to avoid p
+00001490: 7269 7661 6379 2063 6f6e 6365 726e 732e  rivacy concerns.
+000014a0: 0a2a 2065 7870 6f72 745f 7265 7370 6f6e  .* export_respon
+000014b0: 7365 5f74 6578 7473 2028 4661 6c73 6529  se_texts (False)
+000014c0: 3a20 5768 6574 6865 7220 4d6f 6e61 2073  : Whether Mona s
+000014d0: 686f 756c 6420 6578 706f 7274 2074 6865  hould export the
+000014e0: 2061 6374 7561 6c20 7265 7370 6f6e 7365   actual response
+000014f0: 2074 6578 7473 2e20 4265 2064 6566 6175   texts. Be defau
+00001500: 6c74 2073 6574 2074 6f20 4661 6c73 6520  lt set to False 
+00001510: 746f 2061 766f 6964 2070 7269 7661 6379  to avoid privacy
+00001520: 2063 6f6e 6365 726e 732e 0a2a 2061 6e61   concerns..* ana
+00001530: 6c79 7369 733a 2041 2064 6963 7469 6f6e  lysis: A diction
+00001540: 6172 7920 6d61 7070 696e 6720 6561 6368  ary mapping each
+00001550: 2061 6e61 6c79 7369 7320 7479 7065 2074   analysis type t
+00001560: 6f20 6120 626f 6f6c 6561 6e20 7661 6c75  o a boolean valu
+00001570: 6520 7465 6c6c 696e 6720 7468 6520 636c  e telling the cl
+00001580: 6965 6e74 2077 6865 7468 6572 206f 7220  ient whether or 
+00001590: 6e6f 7420 746f 2072 756e 2073 6169 6420  not to run said 
+000015a0: 616e 616c 7973 6973 2061 6e64 206c 6f67  analysis and log
+000015b0: 2069 7420 746f 204d 6f6e 612e 2050 6f73   it to Mona. Pos
+000015c0: 7369 626c 6520 6f70 7469 6f6e 7320 6375  sible options cu
+000015d0: 7272 656e 746c 7920 6172 6520 2270 7269  rrently are "pri
+000015e0: 7661 6379 222c 2022 7072 6f66 616e 6974  vacy", "profanit
+000015f0: 7922 2c20 616e 6420 2274 6578 7475 616c  y", and "textual
+00001600: 222e 2042 7920 6465 6661 756c 742c 2061  ". By default, a
+00001610: 6c6c 2061 6e61 6c79 7365 7320 7461 6b65  ll analyses take
+00001620: 2070 6c61 6365 2061 6e64 2061 7265 206c   place and are l
+00001630: 6f67 6765 6420 6f75 7420 746f 204d 6f6e  ogged out to Mon
+00001640: 612e 0a0a 2323 2320 4361 7061 6269 6c69  a...### Capabili
+00001650: 7469 6573 2064 7572 696e 6720 4150 4920  ties during API 
+00001660: 6361 6c6c 730a 0a41 6674 6572 2077 7261  calls..After wra
+00001670: 7070 696e 6720 796f 7572 2065 6e64 706f  pping your endpo
+00001680: 696e 7420 7769 7468 2060 6d6f 6e69 746f  int with `monito
+00001690: 7260 2c20 796f 7520 7265 616c 6c79 2064  r`, you really d
+000016a0: 6f6e 2774 206e 6565 6420 746f 2064 6f20  on't need to do 
+000016b0: 616e 7974 6869 6e67 2065 6c73 652e 2057  anything else. W
+000016c0: 6865 6e20 7573 696e 6720 6063 7265 6174  hen using `creat
+000016d0: 6560 206f 7220 6061 6372 6561 7465 6020  e` or `acreate` 
+000016e0: 6461 7461 2077 696c 6c20 6265 2074 7261  data will be tra
+000016f0: 636b 6564 2061 6e64 206d 6f6e 6974 6f72  cked and monitor
+00001700: 696e 6720 7769 6c6c 2074 616b 6520 706c  ing will take pl
+00001710: 6163 652e 0a0a 5468 6572 6520 6172 652c  ace...There are,
+00001720: 2068 6f77 6576 6572 2c20 7365 7665 7261   however, severa
+00001730: 6c20 6361 7061 6269 6c69 7469 6573 2074  l capabilities t
+00001740: 6861 7420 6172 6520 6164 6465 6420 746f  hat are added to
+00001750: 2074 6865 7365 2066 756e 6374 696f 6e73   these functions
+00001760: 2e20 5370 6563 6966 6963 616c 6c79 2c20  . Specifically, 
+00001770: 796f 7520 6361 6e20 6164 6420 7468 6520  you can add the 
+00001780: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
+00001790: 6e74 7320 746f 2061 6e79 2063 7265 6174  nts to any creat
+000017a0: 6520 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63  e call:.* MONA_c
+000017b0: 6f6e 7465 7874 5f69 643a 2054 6865 2075  ontext_id: The u
+000017c0: 6e69 7175 6520 6964 206f 6620 7468 6520  nique id of the 
+000017d0: 636f 6e74 6578 7420 696e 2077 6869 6368  context in which
+000017e0: 2074 6865 2063 616c 6c20 6973 206d 6164   the call is mad
+000017f0: 652e 2042 7920 7573 696e 6720 7468 6973  e. By using this
+00001800: 2049 4420 796f 7520 6361 6e20 6578 706f   ID you can expo
+00001810: 7274 206d 6f72 6520 6461 7461 2074 6f20  rt more data to 
+00001820: 4d6f 6e61 2074 6f20 7468 6520 7361 6d65  Mona to the same
+00001830: 2063 6f6e 7465 7874 2066 726f 6d20 6f74   context from ot
+00001840: 6865 7220 706c 6163 6573 2e20 4966 206e  her places. If n
+00001850: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
+00001860: 2022 6964 2220 6669 656c 6420 6f66 2074   "id" field of t
+00001870: 6865 204f 7065 6e41 4920 456e 6470 6f69  he OpenAI Endpoi
+00001880: 6e74 2773 2072 6573 706f 6e73 6520 7769  nt's response wi
+00001890: 6c6c 2062 6520 7573 6564 2061 7320 7468  ll be used as th
+000018a0: 6520 4d6f 6e61 2063 6f6e 7465 7874 2049  e Mona context I
+000018b0: 4420 6175 746f 6d61 7469 6361 6c6c 792e  D automatically.
+000018c0: 0a2a 204d 4f4e 415f 6578 706f 7274 5f74  .* MONA_export_t
+000018d0: 696d 6573 7461 6d70 3a20 4361 6e20 6265  imestamp: Can be
+000018e0: 2075 7365 6420 746f 2073 696d 756c 6174   used to simulat
+000018f0: 6520 6173 2069 6620 7468 6520 6375 7272  e as if the curr
+00001900: 656e 7420 6361 6c6c 2077 6173 206d 6164  ent call was mad
+00001910: 6520 696e 2061 2064 6966 6665 7265 6e74  e in a different
+00001920: 2074 696d 652c 2061 7320 6661 7220 6173   time, as far as
+00001930: 204d 6f6e 6120 6973 2063 6f6e 6365 726e   Mona is concern
+00001940: 6564 2e0a 2a20 4d4f 4e41 5f61 6464 6974  ed..* MONA_addit
+00001950: 696f 6e61 6c5f 6461 7461 3a20 4120 4a53  ional_data: A JS
+00001960: 4f4e 2d73 6572 6961 6c69 7a61 626c 6520  ON-serializable 
+00001970: 6469 6374 2077 6974 6820 616e 7920 6f74  dict with any ot
+00001980: 6865 7220 6461 7461 2079 6f75 2077 616e  her data you wan
+00001990: 7420 746f 2061 6464 2074 6f20 7468 6520  t to add to the 
+000019a0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
+000019b0: 7874 2e20 5468 6973 2063 6f6d 6573 2069  xt. This comes i
+000019c0: 6e20 6861 6e64 7920 6966 2079 6f75 2077  n handy if you w
+000019d0: 616e 7420 746f 2061 6464 206d 6f72 6520  ant to add more 
+000019e0: 696e 666f 726d 6174 696f 6e20 746f 2074  information to t
+000019f0: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
+00001a00: 6e74 6578 2074 6861 7420 6973 6e27 7420  ntex that isn't 
+00001a10: 7061 7274 206f 6620 7468 6520 6261 7369  part of the basi
+00001a20: 6320 4f70 656e 4149 2041 5049 2063 616c  c OpenAI API cal
+00001a30: 6c20 696e 666f 726d 6174 696f 6e2e 2046  l information. F
+00001a40: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
+00001a50: 6f75 2061 7265 2075 7369 6e67 2061 2073  ou are using a s
+00001a60: 7065 6369 6669 6320 7465 6d70 6c61 7465  pecific template
+00001a70: 2049 4420 6f72 2069 6620 7468 6973 2063   ID or if this c
+00001a80: 616c 6c20 6973 2062 6569 6e67 206d 6164  all is being mad
+00001a90: 6520 666f 7220 6120 7370 6563 6966 6963  e for a specific
+00001aa0: 2063 7573 746f 6d65 7220 4944 2c20 7468   customer ID, th
+00001ab0: 6573 6520 6172 6520 6669 656c 6473 2079  ese are fields y
+00001ac0: 6f75 2063 616e 2061 6464 2074 6865 7265  ou can add there
+00001ad0: 2074 6f20 6865 6c70 2067 6574 2066 756c   to help get ful
+00001ae0: 6c20 636f 6e74 6578 7420 7768 656e 206d  l context when m
+00001af0: 6f6e 6974 6f72 696e 6720 7769 7468 204d  onitoring with M
+00001b00: 6f6e 612e 0a0a 4578 616d 706c 653a 0a60  ona...Example:.`
+00001b10: 6060 7079 0a72 6573 706f 6e73 6520 3d20  ``py.response = 
+00001b20: 6173 796e 6369 6f2e 7275 6e28 6d6f 6e69  asyncio.run(moni
+00001b30: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
+00001b40: 2e61 6372 6561 7465 280a 2020 2020 656e  .acreate(.    en
+00001b50: 6769 6e65 3d6d 6f64 656c 2c0a 2020 2020  gine=model,.    
+00001b60: 7072 6f6d 7074 3d70 726f 6d70 742c 0a20  prompt=prompt,. 
+00001b70: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
+00001b80: 785f 746f 6b65 6e73 2c0a 2020 2020 6e3d  x_tokens,.    n=
+00001b90: 6e2c 0a20 2020 2074 656d 7065 7261 7475  n,.    temperatu
+00001ba0: 7265 3d74 656d 7065 7261 7475 7265 2c0a  re=temperature,.
+00001bb0: 2020 2020 4d4f 4e41 5f61 6464 6974 696f      MONA_additio
+00001bc0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
+00001bd0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
+00001be0: 3122 7d2c 0a29 290a 7072 696e 7428 7265  1"},.)).print(re
+00001bf0: 7370 6f6e 7365 2e63 686f 6963 6573 5b30  sponse.choices[0
+00001c00: 5d2e 7465 7874 290a 6060 600a 0a23 2323  ].text).```..###
+00001c10: 2055 7369 6e67 204f 7065 6e41 4920 7769   Using OpenAI wi
+00001c20: 7468 2052 4553 5420 6361 6c6c 7320 696e  th REST calls in
+00001c30: 7374 6561 6420 6f66 204f 7065 6e41 4927  stead of OpenAI'
+00001c40: 7320 5079 7468 6f6e 2063 6c69 656e 740a  s Python client.
+00001c50: 496e 2073 6f6d 6520 6361 7365 7320 796f  In some cases yo
+00001c60: 7520 6d61 7920 6368 6f6f 7365 2074 6f20  u may choose to 
+00001c70: 7573 6520 4f70 656e 4149 2773 2041 5049  use OpenAI's API
+00001c80: 2064 6972 6563 746c 7920 7769 7468 2052   directly with R
+00001c90: 4553 5420 6361 6c6c 7320 616e 6420 6e6f  EST calls and no
+00001ca0: 7420 7573 696e 6720 4f70 656e 4149 2773  t using OpenAI's
+00001cb0: 2053 444b 2e20 466f 7220 7468 6573 6520   SDK. For these 
+00001cc0: 6361 7365 7320 7765 2061 6c6c 6f77 2061  cases we allow a
+00001cd0: 206d 6f72 6520 6469 7265 6374 2061 7070   more direct app
+00001ce0: 726f 6163 6820 666f 7220 6c6f 6767 696e  roach for loggin
+00001cf0: 6720 746f 204d 6f6e 6120 6173 2077 656c  g to Mona as wel
+00001d00: 6c2c 2062 7920 7573 696e 6720 7468 6520  l, by using the 
+00001d10: 2267 6574 5f72 6573 745f 6d6f 6e69 746f  "get_rest_monito
+00001d20: 7222 2066 756e 6374 696f 6e2e 2053 6565  r" function. See
+00001d30: 2065 7861 6d70 6c65 2062 656c 6f77 2e0a   example below..
+00001d40: 0a60 6060 7079 0a23 2044 6972 6563 7420  .```py.# Direct 
+00001d50: 5245 5354 2075 7361 6765 2c20 7769 7468  REST usage, with
+00001d60: 6f75 7420 4f70 656e 4149 2063 6c69 656e  out OpenAI clien
+00001d70: 740a 696d 706f 7274 2072 6571 7565 7374  t.import request
+00001d80: 730a 6672 6f6d 206f 7320 696d 706f 7274  s.from os import
+00001d90: 2065 6e76 6972 6f6e 0a66 726f 6d20 6d6f   environ.from mo
+00001da0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
+00001db0: 2067 6574 5f72 6573 745f 6d6f 6e69 746f   get_rest_monito
+00001dc0: 720a 0a0a 4d4f 4e41 5f41 5049 5f4b 4559  r...MONA_API_KEY
+00001dd0: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
+00001de0: 4d4f 4e41 5f41 5049 5f4b 4559 2229 0a4d  MONA_API_KEY").M
+00001df0: 4f4e 415f 5345 4352 4554 203d 2065 6e76  ONA_SECRET = env
+00001e00: 6972 6f6e 2e67 6574 2822 4d4f 4e41 5f53  iron.get("MONA_S
+00001e10: 4543 5245 5422 290a 4d4f 4e41 5f43 5245  ECRET").MONA_CRE
+00001e20: 4453 203d 207b 0a20 2020 2022 6b65 7922  DS = {.    "key"
+00001e30: 3a20 4d4f 4e41 5f41 5049 5f4b 4559 2c0a  : MONA_API_KEY,.
+00001e40: 2020 2020 2273 6563 7265 7422 3a20 4d4f      "secret": MO
+00001e50: 4e41 5f53 4543 5245 542c 0a7d 0a43 4f4e  NA_SECRET,.}.CON
+00001e60: 5445 5854 5f43 4c41 5353 5f4e 414d 4520  TEXT_CLASS_NAME 
+00001e70: 3d20 2253 4f4d 455f 4d4f 4e49 544f 5249  = "SOME_MONITORI
+00001e80: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
+00001e90: 0a0a 2320 4765 7420 4d6f 6e61 206c 6f67  ..# Get Mona log
+00001ea0: 6765 720a 6d6f 6e61 5f6c 6f67 6765 7220  ger.mona_logger 
+00001eb0: 3d20 6765 745f 7265 7374 5f6d 6f6e 6974  = get_rest_monit
+00001ec0: 6f72 280a 2020 2020 2243 6f6d 706c 6574  or(.    "Complet
+00001ed0: 696f 6e22 2c0a 2020 2020 4d4f 4e41 5f43  ion",.    MONA_C
+00001ee0: 5245 4453 2c0a 2020 2020 434f 4e54 4558  REDS,.    CONTEX
+00001ef0: 545f 434c 4153 535f 4e41 4d45 2c0a 290a  T_CLASS_NAME,.).
+00001f00: 0a23 2053 6574 2075 7020 7468 6520 4150  .# Set up the AP
+00001f10: 4920 656e 6470 6f69 6e74 2055 524c 2061  I endpoint URL a
+00001f20: 6e64 2061 7574 6865 6e74 6963 6174 696f  nd authenticatio
+00001f30: 6e20 6865 6164 6572 730a 7572 6c20 3d20  n headers.url = 
+00001f40: 2268 7474 7073 3a2f 2f61 7069 2e6f 7065  "https://api.ope
+00001f50: 6e61 692e 636f 6d2f 7631 2f63 6f6d 706c  nai.com/v1/compl
+00001f60: 6574 696f 6e73 220a 6865 6164 6572 7320  etions".headers 
+00001f70: 3d20 7b0a 2020 2020 2243 6f6e 7465 6e74  = {.    "Content
+00001f80: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
+00001f90: 7469 6f6e 2f6a 736f 6e22 2c0a 2020 2020  tion/json",.    
+00001fa0: 2241 7574 686f 7269 7a61 7469 6f6e 223a  "Authorization":
+00001fb0: 2066 2242 6561 7265 7220 7b65 6e76 6972   f"Bearer {envir
+00001fc0: 6f6e 2e67 6574 2827 4f50 454e 5f41 495f  on.get('OPEN_AI_
+00001fd0: 4b45 5927 297d 222c 0a7d 0a0a 2320 5365  KEY')}",.}..# Se
+00001fe0: 7420 7570 2074 6865 2072 6571 7565 7374  t up the request
+00001ff0: 2064 6174 610a 6461 7461 203d 207b 0a20   data.data = {. 
+00002000: 2020 2022 7072 6f6d 7074 223a 2070 726f     "prompt": pro
+00002010: 6d70 742c 0a20 2020 2022 6d61 785f 746f  mpt,.    "max_to
+00002020: 6b65 6e73 223a 206d 6178 5f74 6f6b 656e  kens": max_token
+00002030: 732c 0a20 2020 2022 7465 6d70 6572 6174  s,.    "temperat
+00002040: 7572 6522 3a20 7465 6d70 6572 6174 7572  ure": temperatur
+00002050: 652c 0a20 2020 2022 6d6f 6465 6c22 3a20  e,.    "model": 
+00002060: 6d6f 6465 6c2c 0a20 2020 2022 6e22 3a20  model,.    "n": 
+00002070: 6e2c 0a7d 0a0a 2320 5468 6520 6c6f 675f  n,.}..# The log_
+00002080: 7265 7175 6573 7420 6675 6e63 7469 6f6e  request function
+00002090: 2072 6574 7572 6e73 2074 776f 206f 7468   returns two oth
+000020a0: 6572 2066 756e 6374 696f 6e20 666f 7220  er function for 
+000020b0: 6c61 7465 7220 6c6f 6767 696e 670a 2320  later logging.# 
+000020c0: 7468 6520 7265 7370 6f6e 7365 206f 7220  the response or 
+000020d0: 7468 6520 6578 6365 7074 696f 6e2e 2057  the exception. W
+000020e0: 6865 6e20 7765 206c 6174 6572 2064 6f20  hen we later do 
+000020f0: 7468 6174 2c20 7468 6520 6c6f 6767 6572  that, the logger
+00002100: 2077 696c 6c0a 2320 6163 7475 616c 6c79   will.# actually
+00002110: 2063 616c 6375 6c61 7465 2061 6c6c 2074   calculate all t
+00002120: 6865 2072 656c 6576 616e 7420 6d65 7472  he relevant metr
+00002130: 6963 7320 616e 6420 7769 6c6c 2073 656e  ics and will sen
+00002140: 6420 7468 656d 2074 6f0a 2320 4d6f 6e61  d them to.# Mona
+00002150: 2e0a 7265 7370 6f6e 7365 5f6c 6f67 6765  ..response_logge
+00002160: 722c 2065 7863 6570 7469 6f6e 5f6c 6f67  r, exception_log
+00002170: 6765 7220 3d20 6d6f 6e61 5f6c 6f67 6765  ger = mona_logge
+00002180: 722e 6c6f 675f 7265 7175 6573 7428 0a20  r.log_request(. 
+00002190: 2020 2064 6174 612c 2061 6464 6974 696f     data, additio
+000021a0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
+000021b0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
+000021c0: 3122 7d0a 290a 0a74 7279 3a0a 2020 2020  1"}.)..try:.    
+000021d0: 2320 5365 6e64 2074 6865 2072 6571 7565  # Send the reque
+000021e0: 7374 2074 6f20 7468 6520 4150 490a 2020  st to the API.  
+000021f0: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
+00002200: 7565 7374 732e 706f 7374 2875 726c 2c20  uests.post(url, 
+00002210: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
+00002220: 206a 736f 6e3d 6461 7461 290a 0a20 2020   json=data)..   
+00002230: 2023 2043 6865 636b 2066 6f72 2048 5454   # Check for HTT
+00002240: 5020 6572 726f 7273 0a20 2020 2072 6573  P errors.    res
+00002250: 706f 6e73 652e 7261 6973 655f 666f 725f  ponse.raise_for_
+00002260: 7374 6174 7573 2829 0a0a 2020 2020 2320  status()..    # 
+00002270: 4c6f 6720 7265 7370 6f6e 7365 2074 6f20  Log response to 
+00002280: 4d6f 6e61 0a20 2020 2072 6573 706f 6e73  Mona.    respons
+00002290: 655f 6c6f 6767 6572 2872 6573 706f 6e73  e_logger(respons
+000022a0: 652e 6a73 6f6e 2829 290a 2020 2020 7072  e.json()).    pr
+000022b0: 696e 7428 7265 7370 6f6e 7365 2e6a 736f  int(response.jso
+000022c0: 6e28 295b 2263 686f 6963 6573 225d 5b30  n()["choices"][0
+000022d0: 5d5b 2274 6578 7422 5d29 0a0a 6578 6365  ]["text"])..exce
+000022e0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000022f0: 6572 723a 0a20 2020 2023 204c 6f67 2065  err:.    # Log e
+00002300: 7863 6570 7469 6f6e 2074 6f20 4d6f 6e61  xception to Mona
+00002310: 0a20 2020 2065 7863 6570 7469 6f6e 5f6c  .    exception_l
+00002320: 6f67 6765 7228 290a 6060 600a 0a23 2323  ogger().```..###
+00002330: 2053 7472 6561 6d20 7375 7070 6f72 740a   Stream support.
+00002340: 0a4f 7065 6e41 4920 616c 6c6f 7773 2072  .OpenAI allows r
+00002350: 6563 6569 7669 6e67 2072 6573 706f 6e73  eceiving respons
+00002360: 6573 2061 7320 6120 7374 7265 616d 206f  es as a stream o
+00002370: 6620 746f 6b65 6e73 2075 7369 6e67 2074  f tokens using t
+00002380: 6865 2022 7374 7265 616d 2220 7061 7261  he "stream" para
+00002390: 6d65 7465 722e 2057 6865 6e20 7468 6973  meter. When this
+000023a0: 2069 7320 646f 6e65 2c20 4d6f 6e61 2077   is done, Mona w
+000023b0: 696c 6c20 636f 6c6c 6563 7420 616c 6c20  ill collect all 
+000023c0: 7468 6520 746f 6b65 6e73 2069 6e20 6d65  the tokens in me
+000023d0: 6d6f 7279 2061 6e64 2077 696c 6c20 6372  mory and will cr
+000023e0: 6561 7465 2074 6865 2061 6e61 6c79 7369  eate the analysi
+000023f0: 7320 616e 6420 6c6f 6720 6f75 7420 7468  s and log out th
+00002400: 6520 6461 7461 2074 6865 206d 6f6d 656e  e data the momen
+00002410: 7420 7468 6520 7374 7265 616d 2069 7320  t the stream is 
+00002420: 6f76 6572 2e20 596f 7520 646f 6e27 7420  over. You don't 
+00002430: 6e65 6564 2074 6f20 646f 2061 6e79 7468  need to do anyth
+00002440: 696e 6720 746f 206d 616b 6520 7468 6973  ing to make this
+00002450: 2068 6170 7065 6e2e 0a0a 5369 6e63 6520   happen...Since 
+00002460: 666f 7220 7374 7265 616d 696e 6720 7265  for streaming re
+00002470: 7370 6f6e 7365 7320 4f70 656e 4149 2064  sponses OpenAI d
+00002480: 6f65 736e 2774 2073 7570 706c 7920 7468  oesn't supply th
+00002490: 6520 6675 6c6c 2075 7361 6765 2074 6f6b  e full usage tok
+000024a0: 656e 7320 7375 6d6d 6172 792c 204d 6f6e  ens summary, Mon
+000024b0: 6120 7573 6573 2074 6865 2074 696b 746f  a uses the tikto
+000024c0: 6b65 6e20 7061 636b 6167 6520 746f 2063  ken package to c
+000024d0: 616c 6375 6c61 7465 2074 6865 2074 6f6b  alculate the tok
+000024e0: 656e 7320 6f66 2074 6865 2070 726f 6d70  ens of the promp
+000024f0: 7420 616e 6420 636f 6d70 6c65 7469 6f6e  t and completion
+00002500: 2061 6e64 206c 6f67 2074 6865 6d20 666f   and log them fo
+00002510: 7220 6d6f 6e69 746f 7269 6e67 2e0a 0a4e  r monitoring...N
+00002520: 4f54 453a 2053 7472 6561 6d20 6973 2063  OTE: Stream is c
+00002530: 7572 7265 6e74 6c79 206f 6e6c 7920 7375  urrently only su
+00002540: 7070 6f72 7465 6420 7769 7468 2053 444b  pported with SDK
+00002550: 2075 7361 6765 2c20 616e 6420 6e6f 7420   usage, and not 
+00002560: 7769 7468 2075 7369 6e67 2052 4553 5420  with using REST 
+00002570: 6469 7265 6374 6c79 2e0a 0a23 2320 4c61  directly...## La
+00002580: 6e67 4368 6169 6e20 7375 7070 6f72 740a  ngChain support.
+00002590: 0a59 6f75 2063 616e 2075 7365 2074 6865  .You can use the
+000025a0: 2065 7870 6f72 7465 6420 606d 6f6e 6974   exported `monit
+000025b0: 6f72 5f6c 616e 6763 6861 696e 5f6c 6c6d  or_langchain_llm
+000025c0: 6020 746f 2077 7261 7020 6120 4c61 6e67  ` to wrap a Lang
+000025d0: 4368 6169 6e20 4f70 656e 4149 204c 4c4d  Chain OpenAI LLM
+000025e0: 2028 6368 6174 206f 7220 6e6f 726d 616c   (chat or normal
+000025f0: 2920 7769 7468 204d 6f6e 6127 7320 6d6f  ) with Mona's mo
+00002600: 6e69 746f 7269 6e67 2063 6170 6162 696c  nitoring capabil
+00002610: 6974 6965 733a 0a0a 6060 6070 790a 6672  ities:..```py.fr
+00002620: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
+00002630: 6d70 6f72 7420 6d6f 6e69 746f 725f 6c61  mport monitor_la
+00002640: 6e67 6368 6169 6e5f 6c6c 6d0a 0a66 726f  ngchain_llm..fro
+00002650: 6d20 6c61 6e67 6368 6169 6e2e 6c6c 6d73  m langchain.llms
+00002660: 2069 6d70 6f72 7420 4f70 656e 4149 0a0a   import OpenAI..
+00002670: 2320 5772 6170 2074 6865 204c 4c4d 206f  # Wrap the LLM o
+00002680: 626a 6563 7420 7769 7468 204d 6f6e 6120  bject with Mona 
+00002690: 6d6f 6e69 746f 7269 6e67 2e0a 6c6c 6d20  monitoring..llm 
+000026a0: 3d20 6d6f 6e69 746f 725f 6c61 6e67 6368  = monitor_langch
+000026b0: 6169 6e5f 6c6c 6d28 0a20 2020 204f 7065  ain_llm(.    Ope
+000026c0: 6e41 4928 4f50 454e 5f41 495f 4b45 5929  nAI(OPEN_AI_KEY)
+000026d0: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
+000026e0: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
+000026f0: 4153 535f 4e41 4d45 290a 6060 600a 0a53  ASS_NAME).```..S
+00002700: 6565 2066 756c 6c20 6578 616d 706c 6520  ee full example 
+00002710: 696e 2063 6f6d 706c 6574 696f 6e5f 6c61  in completion_la
+00002720: 6e67 6368 6169 6e2e 7079 2069 6e20 7468  ngchain.py in th
+00002730: 6520 6578 616d 706c 6573 2066 6f6c 6465  e examples folde
+00002740: 722e 0a0a 2323 204d 6f6e 6120 5344 4b0a  r...## Mona SDK.
+00002750: 0a54 6869 7320 7061 636b 6167 6520 7573  .This package us
+00002760: 6573 2074 6865 206d 6f6e 615f 7364 6b20  es the mona_sdk 
+00002770: 7061 636b 6167 6520 746f 2065 7870 6f72  package to expor
+00002780: 7420 7468 6520 7265 6c65 7661 6e74 2064  t the relevant d
+00002790: 6174 6120 746f 204d 6f6e 612e 2054 6865  ata to Mona. The
+000027a0: 7265 2061 7265 2073 6576 6572 616c 2065  re are several e
+000027b0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+000027c0: 626c 6573 2079 6f75 2063 616e 2075 7365  bles you can use
+000027d0: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
+000027e0: 6520 5344 4b27 7320 6265 6861 7669 6f72  e SDK's behavior
+000027f0: 2e20 466f 7220 6578 616d 706c 652c 2079  . For example, y
+00002800: 6f75 2063 616e 2073 6574 2069 7420 7570  ou can set it up
+00002810: 2074 6f20 7261 6973 6520 6578 6365 7074   to raise except
+00002820: 696f 6e73 2077 6865 6e20 6578 706f 7274  ions when export
+00002830: 696e 6720 6461 7461 2074 6f20 4d6f 6e61  ing data to Mona
+00002840: 2066 6169 6c73 2028 6974 2064 6f65 736e   fails (it doesn
+00002850: 2774 2064 6f20 7468 6174 2062 7920 6465  't do that by de
+00002860: 6661 756c 7429 2e0a 0a23 2320 4d6f 6e69  fault)...## Moni
+00002870: 746f 7269 6e67 2066 6f72 2070 726f 6661  toring for profa
+00002880: 6e69 7479 0a0a 4d6f 6e61 2075 7365 7320  nity..Mona uses 
+00002890: 7468 6520 616c 742d 7072 6f66 616e 6974  the alt-profanit
+000028a0: 792d 6368 6563 6b20 7061 6361 6b67 6520  y-check pacakge 
+000028b0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000028c0: 672f 7072 6f6a 6563 742f 616c 742d 7072  g/project/alt-pr
+000028d0: 6f66 616e 6974 792d 6368 6563 6b2f 2920  ofanity-check/) 
+000028e0: 746f 2063 7265 6174 6520 626f 7468 2062  to create both b
+000028f0: 6f6f 6c65 616e 2070 7265 6469 6374 696f  oolean predictio
+00002900: 6e73 2061 6e64 2070 726f 6261 6269 6c74  ns and probabilt
+00002910: 7920 7363 6f72 6573 2066 6f72 2074 6865  y scores for the
+00002920: 2065 7869 7374 656e 6365 206f 6620 7072   existence of pr
+00002930: 6f66 616e 6974 7920 626f 7468 2069 6e20  ofanity both in 
+00002940: 7468 6520 7072 6f6d 7074 2061 6e64 2069  the prompt and i
+00002950: 6e20 7468 6520 7265 7370 6f6e 7365 732e  n the responses.
+00002960: 2057 6520 7573 6520 7468 6520 6275 696c   We use the buil
+00002970: 7420 696e 2070 6163 6b61 6765 206d 6574  t in package met
+00002980: 686f 6473 2066 6f72 2074 6861 742e 2049  hods for that. I
+00002990: 6620 796f 7520 7761 6e74 2c20 666f 7220  f you want, for 
+000029a0: 6578 616d 706c 652c 2074 6f20 7573 6520  example, to use 
+000029b0: 6120 6469 6666 6572 656e 7420 7072 6f62  a different prob
+000029c0: 6162 696c 6974 7920 7468 7265 7368 6f6c  ability threshol
+000029d0: 6420 666f 7220 7468 6520 626f 6f6c 6561  d for the boolea
+000029e0: 6e20 7072 6564 6963 7469 6f6e 2c20 796f  n prediction, yo
+000029f0: 7520 6361 6e20 646f 2074 6861 7420 6279  u can do that by
+00002a00: 2063 6861 6e67 696e 6720 796f 7572 204d   changing your M
+00002a10: 6f6e 6120 636f 6e66 6967 206f 6e20 7468  ona config on th
+00002a20: 6520 4d6f 6e61 2064 6173 6862 6f61 7264  e Mona dashboard
+00002a30: 2e0a                                     ..
```

### Comparing `mona-openai-0.0.7/mona_openai/analysis/privacy.py` & `mona-openai-0.0.8/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/analysis/textual.py` & `mona-openai-0.0.8/mona_openai/analysis/textual.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,17 +106,18 @@
         """
         return len(self._prepositions)
 
     def get_preposition_ratio(self):
         """
         Returns the ratio of prepositions in the text.
         """
+        word_count = self.get_word_count()
         return (
-            self.get_preposition_count() / self.get_word_count()
-            if len(self._text)
+            self.get_preposition_count() / word_count
+            if word_count
             else 0
         )
 
     def get_words_not_in_others_count(
         self, others: Iterable["TextualAnalyzer"]
     ):
         """
```

### Comparing `mona-openai-0.0.7/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.0.8/mona_openai/endpoints/chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
                 )
             ),
             "answer_words_not_in_prompt_ratio": tuple(
                 analyzer.get_words_not_in_others_count(
                     messages_textual_analyzers
                 )
                 / analyzer.get_word_count()
+                if analyzer.get_word_count() > 0
+                else 0.0
                 for analyzer in answers_textual_analyzers
             ),
         }
 
         if last_user_message_analyzer is not None:
             ret.update(
                 {
```

### Comparing `mona-openai-0.0.7/mona_openai/endpoints/completion.py` & `mona-openai-0.0.8/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.0.8/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.0.8/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/mona_client.py` & `mona-openai-0.0.8/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/mona_openai.py` & `mona-openai-0.0.8/mona_openai/mona_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 import logging
 from copy import deepcopy
 from types import MappingProxyType
 
 from mona_sdk import MonaSingleMessage
 
+from .exceptions import InvalidLagnchainLLMException
 from .endpoints.wrapping_getter import get_endpoint_wrapping
 from .mona_client import get_mona_clients
 from .util.func_util import add_conditional_sampling
 from .util.async_util import (
     run_in_an_event_loop,
     call_non_blocking_sync_or_async,
 )
@@ -498,7 +499,24 @@
             Returns the two Mona client this class works with to allow
             exporting more data or communicating directly with Mona's
             API.
             """
             return client, async_client
 
     return RestClient
+
+
+def monitor_langchain_llm(
+    llm,
+    mona_creds,
+    context_class,
+    specs=EMPTY_DICT,
+    mona_clients_getter=get_mona_clients,
+):
+    if not hasattr(llm, "client"):
+        raise InvalidLagnchainLLMException(
+            "LLM has no client attribute - must be an OpenAI LLM"
+        )
+    llm.client = monitor(
+        llm.client, mona_creds, context_class, specs, mona_clients_getter
+    )
+    return llm
```

### Comparing `mona-openai-0.0.7/mona_openai/util/async_util.py` & `mona-openai-0.0.8/mona_openai/util/async_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/util/func_util.py` & `mona-openai-0.0.8/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/util/oop_util.py` & `mona-openai-0.0.8/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/util/stream_util.py` & `mona-openai-0.0.8/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/util/tokens_util.py` & `mona-openai-0.0.8/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai/util/validation_util.py` & `mona-openai-0.0.8/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,610 +1,638 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e61  : 2.1.Name: mona
-00000020: 2d6f 7065 6e61 690a 5665 7273 696f 6e3a  -openai.Version:
-00000030: 2030 2e30 2e37 0a53 756d 6d61 7279 3a20   0.0.7.Summary: 
-00000040: 496e 7465 6772 6174 696f 6e20 636c 6965  Integration clie
-00000050: 6e74 2066 6f72 206d 6f6e 6974 6f72 696e  nt for monitorin
-00000060: 6720 4f70 656e 4149 2075 7361 6765 2077  g OpenAI usage w
-00000070: 6974 6820 4d6f 6e61 0a41 7574 686f 722d  ith Mona.Author-
-00000080: 656d 6169 6c3a 2049 7461 6920 4261 7220  email: Itai Bar 
-00000090: 5369 6e61 6920 3c69 7461 6940 6d6f 6e61  Sinai <itai@mona
-000000a0: 6c61 6273 2e69 6f3e 0a50 726f 6a65 6374  labs.io>.Project
-000000b0: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
-000000c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000d0: 6f6d 2f6d 6f6e 616c 6162 732f 6d6f 6e61  om/monalabs/mona
-000000e0: 2d6f 7065 6e61 690a 5072 6f6a 6563 742d  -openai.Project-
-000000f0: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
-00000100: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000110: 2e63 6f6d 2f6d 6f6e 616c 6162 732f 6d6f  .com/monalabs/mo
-00000120: 6e61 2d6f 7065 6e61 692f 6973 7375 6573  na-openai/issues
-00000130: 0a4b 6579 776f 7264 733a 204f 7065 6e41  .Keywords: OpenA
-00000140: 492c 4c4c 4d73 2c47 5054 2c4d 6f6e 612c  I,LLMs,GPT,Mona,
-00000150: 4d6f 6e69 746f 7269 6e67 2c41 490a 436c  Monitoring,AI.Cl
-00000160: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000170: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000180: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-00000190: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000001a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001b0: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
-000001c0: 7761 7265 204c 6963 656e 7365 0a43 6c61  ware License.Cla
-000001d0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-000001e0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000001f0: 496e 6465 7065 6e64 656e 740a 5265 7175  Independent.Requ
-00000200: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-00000210: 2e39 0a44 6573 6372 6970 7469 6f6e 2d43  .9.Description-C
-00000220: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000230: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-00000240: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000250: 0a0a 2320 4d6f 6e61 2d4f 7065 6e41 4920  ..# Mona-OpenAI 
-00000260: 496e 7465 6772 6174 696f 6e20 436c 6965  Integration Clie
-00000270: 6e74 0a3c 7020 616c 6967 6e3d 2263 656e  nt.<p align="cen
-00000280: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-00000290: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-000002a0: 2e63 6f6d 2f6d 6f6e 616c 6162 732f 6d6f  .com/monalabs/mo
-000002b0: 6e61 2d73 646b 2f62 6c6f 622f 6d61 696e  na-sdk/blob/main
-000002c0: 2f6d 6f6e 615f 6c6f 676f 2e70 6e67 3f72  /mona_logo.png?r
-000002d0: 6177 3d74 7275 6522 2061 6c74 3d22 4d6f  aw=true" alt="Mo
-000002e0: 6e61 2773 206c 6f67 6f22 2077 6964 7468  na's logo" width
-000002f0: 3d22 3138 3022 2f3e 0a3c 2f70 3e0a 0a0a  ="180"/>.</p>...
-00000300: 5573 6520 6f6e 6520 6c69 6e65 206f 6620  Use one line of 
-00000310: 636f 6465 2074 6f20 6765 7420 696e 7374  code to get inst
-00000320: 616e 7420 6c69 7665 206d 6f6e 6974 6f72  ant live monitor
-00000330: 696e 6720 666f 7220 796f 7572 204f 7065  ing for your Ope
-00000340: 6e41 4920 7573 6167 6520 696e 636c 7564  nAI usage includ
-00000350: 696e 673a 0a2a 2054 6f6b 656e 7320 7573  ing:.* Tokens us
-00000360: 6167 650a 2a20 4861 6c6c 7563 696e 6174  age.* Hallucinat
-00000370: 696f 6e20 616c 6572 7473 0a2a 2050 726f  ion alerts.* Pro
-00000380: 6661 6e69 7479 2061 6e64 2070 7269 7661  fanity and priva
-00000390: 6379 2061 6e61 6c79 7365 730a 2a20 4265  cy analyses.* Be
-000003a0: 6861 7669 6f72 616c 2064 7269 6674 7320  havioral drifts 
-000003b0: 616e 6420 616e 6f6d 616c 6965 730a 2a20  and anomalies.* 
-000003c0: 4d75 6368 206d 7563 6820 6d6f 7265 2e0a  Much much more..
-000003d0: 0a23 2320 5365 7474 696e 6720 5570 0a0a  .## Setting Up..
-000003e0: 2d20 544f 444f 3a20 4164 6420 7061 7274  - TODO: Add part
-000003f0: 2061 626f 7574 204d 6f6e 6120 7265 6769   about Mona regi
-00000400: 7374 7261 7469 6f6e 2077 6974 6820 6120  stration with a 
-00000410: 6c69 6e6b 2074 6f20 7468 6520 7265 6c65  link to the rele
-00000420: 7661 6e74 206c 616e 6469 6e67 2070 6167  vant landing pag
-00000430: 6520 7768 6572 6520 7468 6520 7265 6164  e where the read
-00000440: 6572 2063 616e 2073 6967 6e20 7570 2e0a  er can sign up..
-00000450: 6060 6063 6f6e 736f 6c65 0a24 2070 6970  ```console.$ pip
-00000460: 2069 6e73 7461 6c6c 206d 6f6e 615f 6f70   install mona_op
-00000470: 656e 6169 0a60 6060 0a0a 2323 2051 7569  enai.```..## Qui
-00000480: 636b 2053 7461 7274 2061 6e64 2045 7861  ck Start and Exa
-00000490: 6d70 6c65 0a0a 4578 616d 706c 6520 626f  mple..Example bo
-000004a0: 696c 6572 706c 6174 6520 636f 6465 2066  ilerplate code f
-000004b0: 6f72 2062 6f74 6820 7379 6e63 2061 6e64  or both sync and
-000004c0: 2061 7379 6e63 2075 7361 6765 2069 7320   async usage is 
-000004d0: 6769 7665 6e20 696e 2074 6865 2066 696c  given in the fil
-000004e0: 6520 2265 7861 6d70 6c65 5f75 7361 6765  e "example_usage
-000004f0: 2e70 7922 2061 6e64 2068 6572 653a 0a60  .py" and here:.`
-00000500: 6060 7079 0a66 726f 6d20 6f73 2069 6d70  ``py.from os imp
-00000510: 6f72 7420 656e 7669 726f 6e0a 696d 706f  ort environ.impo
-00000520: 7274 2061 7379 6e63 696f 0a69 6d70 6f72  rt asyncio.impor
-00000530: 7420 6f70 656e 6169 0a0a 6672 6f6d 206d  t openai..from m
-00000540: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
-00000550: 7420 6d6f 6e69 746f 720a 0a6f 7065 6e61  t monitor..opena
-00000560: 692e 6170 695f 6b65 7920 3d20 656e 7669  i.api_key = envi
-00000570: 726f 6e2e 6765 7428 224f 5045 4e5f 4149  ron.get("OPEN_AI
-00000580: 5f4b 4559 2229 0a0a 4d4f 4e41 5f41 5049  _KEY")..MONA_API
-00000590: 5f4b 4559 203d 2065 6e76 6972 6f6e 2e67  _KEY = environ.g
-000005a0: 6574 2822 4d4f 4e41 5f41 5049 5f4b 4559  et("MONA_API_KEY
-000005b0: 2229 0a4d 4f4e 415f 5345 4352 4554 203d  ").MONA_SECRET =
-000005c0: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
-000005d0: 4e41 5f53 4543 5245 5422 290a 4d4f 4e41  NA_SECRET").MONA
-000005e0: 5f43 5245 4453 203d 207b 0a20 2020 2022  _CREDS = {.    "
-000005f0: 6b65 7922 3a20 4d4f 4e41 5f41 5049 5f4b  key": MONA_API_K
-00000600: 4559 2c0a 2020 2020 2273 6563 7265 7422  EY,.    "secret"
-00000610: 3a20 4d4f 4e41 5f53 4543 5245 542c 0a7d  : MONA_SECRET,.}
-00000620: 0a43 4f4e 5445 5854 5f43 4c41 5353 5f4e  .CONTEXT_CLASS_N
-00000630: 414d 4520 3d20 2253 4f4d 455f 4d4f 4e49  AME = "SOME_MONI
-00000640: 544f 5249 4e47 5f43 4f4e 5445 5854 5f4e  TORING_CONTEXT_N
-00000650: 414d 4522 0a0a 0a6d 6f6e 6974 6f72 6564  AME"...monitored
-00000660: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
-00000670: 6e69 746f 7228 0a20 2020 206f 7065 6e61  nitor(.    opena
-00000680: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
-00000690: 2020 4d4f 4e41 5f43 5245 4453 2c0a 2020    MONA_CREDS,.  
-000006a0: 2020 434f 4e54 4558 545f 434c 4153 535f    CONTEXT_CLASS_
-000006b0: 4e41 4d45 2c0a 290a 0a0a 7072 6f6d 7074  NAME,.)...prompt
-000006c0: 203d 2022 4920 7761 6e74 2074 6f20 6765   = "I want to ge
-000006d0: 6e65 7261 7465 2073 6f6d 6520 7465 7874  nerate some text
-000006e0: 2061 626f 7574 2022 0a6d 6f64 656c 203d   about ".model =
-000006f0: 2022 7465 7874 2d61 6461 2d30 3031 220a   "text-ada-001".
-00000700: 7465 6d70 6572 6174 7572 6520 3d20 302e  temperature = 0.
-00000710: 360a 6d61 785f 746f 6b65 6e73 203d 2035  6.max_tokens = 5
-00000720: 0a6e 203d 2031 0a0a 2320 5265 6775 6c61  .n = 1..# Regula
-00000730: 7220 2873 796e 6329 2075 7361 6765 0a72  r (sync) usage.r
-00000740: 6573 706f 6e73 6520 3d20 6d6f 6e69 746f  esponse = monito
-00000750: 7265 645f 636f 6d70 6c65 7469 6f6e 2e63  red_completion.c
-00000760: 7265 6174 6528 0a20 2020 2065 6e67 696e  reate(.    engin
-00000770: 653d 6d6f 6465 6c2c 0a20 2020 2070 726f  e=model,.    pro
-00000780: 6d70 743d 7072 6f6d 7074 2c0a 2020 2020  mpt=prompt,.    
-00000790: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
-000007a0: 6f6b 656e 732c 0a20 2020 206e 3d6e 2c0a  okens,.    n=n,.
-000007b0: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
-000007c0: 7465 6d70 6572 6174 7572 652c 0a20 2020  temperature,.   
-000007d0: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
-000007e0: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
-000007f0: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
-00000800: 2c0a 290a 7072 696e 7428 7265 7370 6f6e  ,.).print(respon
-00000810: 7365 2e63 686f 6963 6573 5b30 5d2e 7465  se.choices[0].te
-00000820: 7874 290a 0a23 2041 7379 6e63 2075 7361  xt)..# Async usa
-00000830: 6765 0a72 6573 706f 6e73 6520 3d20 6173  ge.response = as
-00000840: 796e 6369 6f2e 7275 6e28 6d6f 6e69 746f  yncio.run(monito
-00000850: 7265 645f 636f 6d70 6c65 7469 6f6e 2e61  red_completion.a
-00000860: 6372 6561 7465 280a 2020 2020 656e 6769  create(.    engi
-00000870: 6e65 3d6d 6f64 656c 2c0a 2020 2020 7072  ne=model,.    pr
-00000880: 6f6d 7074 3d70 726f 6d70 742c 0a20 2020  ompt=prompt,.   
-00000890: 206d 6178 5f74 6f6b 656e 733d 6d61 785f   max_tokens=max_
-000008a0: 746f 6b65 6e73 2c0a 2020 2020 6e3d 6e2c  tokens,.    n=n,
-000008b0: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
-000008c0: 3d74 656d 7065 7261 7475 7265 2c0a 2020  =temperature,.  
-000008d0: 2020 4d4f 4e41 5f61 6464 6974 696f 6e61    MONA_additiona
-000008e0: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
-000008f0: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
-00000900: 7d2c 0a29 290a 0a70 7269 6e74 2872 6573  },.))..print(res
-00000910: 706f 6e73 652e 6368 6f69 6365 735b 305d  ponse.choices[0]
-00000920: 2e74 6578 7429 0a60 6060 0a23 2320 5375  .text).```.## Su
-00000930: 7070 6f72 7465 6420 4f70 656e 4149 2041  pported OpenAI A
-00000940: 5049 730a 4375 7272 656e 746c 7920 7468  PIs.Currently th
-00000950: 6973 2063 6c69 656e 7420 7375 7070 6f72  is client suppor
-00000960: 7473 2060 6f70 656e 6169 2e43 6f6d 706c  ts `openai.Compl
-00000970: 6574 696f 6e60 2061 6e64 2060 6f70 656e  etion` and `open
-00000980: 6169 2e43 6861 7443 6f6d 706c 6574 696f  ai.ChatCompletio
-00000990: 6e60 2e20 4d6f 6e61 2063 616e 2073 7570  n`. Mona can sup
-000009a0: 706f 7274 2070 726f 6365 7373 6573 2062  port processes b
-000009b0: 6173 6564 206f 6e20 6f74 6865 7220 4150  ased on other AP
-000009c0: 4973 2061 6e64 2061 6c73 6f20 6e6f 6e2d  Is and also non-
-000009d0: 4f70 656e 4149 2d62 6173 6564 2061 7070  OpenAI-based app
-000009e0: 732e 0a49 6620 796f 7520 6861 7665 2061  s..If you have a
-000009f0: 2064 6966 6665 7272 656e 7420 7573 652d   differrent use-
-00000a00: 6361 7365 2c20 7765 2764 206c 6f76 6520  case, we'd love 
-00000a10: 746f 2068 6561 7220 6162 6f75 7420 6974  to hear about it
-00000a20: 2120 506c 6561 7365 2065 6d61 696c 2075  ! Please email u
-00000a30: 7320 6174 2073 7570 706f 7274 406d 6f6e  s at support@mon
-00000a40: 616c 6162 732e 696f 2e0a 0a23 2320 5573  alabs.io...## Us
-00000a50: 6167 650a 2323 2320 496e 6974 6961 6c69  age.### Initiali
-00000a60: 7a61 7469 6f6e 0a0a 5468 6520 6d61 696e  zation..The main
-00000a70: 2061 6e64 206f 6e6c 7920 6675 6e63 7469   and only functi
-00000a80: 6f6e 2065 7870 6f73 6564 2069 6e20 7468  on exposed in th
-00000a90: 6973 2070 6163 6b61 6765 2069 7320 606d  is package is `m
-00000aa0: 6f6e 6974 6f72 602e 0a60 6060 7079 0a69  onitor`..```py.i
-00000ab0: 6d70 6f72 7420 6f70 656e 6169 0a0a 6672  mport openai..fr
-00000ac0: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
-00000ad0: 6d70 6f72 7420 6d6f 6e69 746f 720a 0a6f  mport monitor..o
-00000ae0: 7065 6e61 692e 6170 695f 6b65 7920 3d20  penai.api_key = 
-00000af0: 656e 7669 726f 6e2e 6765 7428 224f 5045  environ.get("OPE
-00000b00: 4e5f 4149 5f4b 4559 2229 0a0a 6d6f 6e69  N_AI_KEY")..moni
-00000b10: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00000b20: 203d 206d 6f6e 6974 6f72 280a 2020 2020   = monitor(.    
-00000b30: 6f70 656e 6169 2e43 6f6d 706c 6574 696f  openai.Completio
-00000b40: 6e2c 0a20 2020 2028 0a20 2020 2020 2020  n,.    (.       
-00000b50: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
-00000b60: 4e41 5f41 5049 5f4b 4559 2229 2c0a 2020  NA_API_KEY"),.  
-00000b70: 2020 2020 2020 656e 7669 726f 6e2e 6765        environ.ge
-00000b80: 7428 224d 4f4e 415f 5345 4352 4554 2229  t("MONA_SECRET")
-00000b90: 2c0a 2020 2020 292c 0a20 2020 2022 534f  ,.    ),.    "SO
-00000ba0: 4d45 5f4d 4f4e 4954 4f52 494e 475f 434f  ME_MONITORING_CO
-00000bb0: 4e54 4558 545f 4e41 4d45 222c 0a20 2020  NTEXT_NAME",.   
-00000bc0: 207b 2261 6e61 6c79 7369 7322 3a20 7b22   {"analysis": {"
-00000bd0: 7072 6f66 616e 6974 7922 3a20 4661 6c73  profanity": Fals
-00000be0: 657d 7d0a 290a 0a2e 2e2e 0a0a 6d6f 6e69  e}}.).......moni
-00000bf0: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00000c00: 2e63 7265 6174 6528 2e2e 2e29 0a60 6060  .create(...).```
-00000c10: 0a0a 5468 6520 606d 6f6e 6974 6f72 6020  ..The `monitor` 
-00000c20: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-00000c30: 2074 6f20 796f 7520 6120 636c 6173 7320   to you a class 
-00000c40: 7468 6174 2077 7261 7073 2074 6865 206f  that wraps the o
-00000c50: 7269 6769 6e61 6c20 6f70 656e 6169 2065  riginal openai e
-00000c60: 6e64 706f 696e 7420 636c 6173 7320 796f  ndpoint class yo
-00000c70: 7520 7072 6f76 6964 652c 2077 6974 6820  u provide, with 
-00000c80: 616e 2065 7175 6976 616c 656e 7420 4150  an equivalent AP
-00000c90: 4920 2862 6573 6964 6573 2073 6f6d 6520  I (besides some 
-00000ca0: 6164 6469 7469 6f6e 7320 6c69 7374 6564  additions listed
-00000cb0: 2062 656c 6f77 292e 0a59 6f75 2063 616e   below)..You can
-00000cc0: 2074 6865 6e20 7573 6520 7468 6520 7265   then use the re
-00000cd0: 7475 726e 6564 2063 6c61 7373 2720 2263  turned class' "c
-00000ce0: 7265 6174 6522 2061 6e64 2022 6163 7265  reate" and "acre
-00000cf0: 6174 6522 2066 756e 6374 696f 6e73 206a  ate" functions j
-00000d00: 7573 7420 6173 2079 6f75 2077 6f75 6c64  ust as you would
-00000d10: 2062 6566 6f72 652c 206f 6e6c 7920 6e6f   before, only no
-00000d20: 772c 2062 6573 6964 6573 2067 6574 7469  w, besides getti
-00000d30: 6e67 2074 6865 2072 6571 7565 7374 6564  ng the requested
-00000d40: 206f 7065 6e41 4920 6675 6e63 7469 6f6e   openAI function
-00000d50: 616c 6974 792c 2074 6869 7320 636c 6965  ality, this clie
-00000d60: 6e74 2077 696c 6c20 6c6f 6720 6f75 7420  nt will log out 
-00000d70: 746f 204d 6f6e 6127 7320 7365 7276 6572  to Mona's server
-00000d80: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-00000d90: 796f 7520 7573 6564 2028 652e 672e 2c20  you used (e.g., 
-00000da0: 7465 6d70 6572 6174 7572 6529 2c20 6461  temperature), da
-00000db0: 7461 2061 626f 7574 2074 6865 2072 6573  ta about the res
-00000dc0: 706f 6e73 6520 6672 6f6d 204f 7065 6e41  ponse from OpenA
-00000dd0: 4927 7320 7365 7276 6572 2c20 616e 6420  I's server, and 
-00000de0: 6375 7374 6f6d 2061 6e61 6c79 7365 7320  custom analyses 
-00000df0: 6162 6f75 7420 7468 6520 6361 6c6c 2028  about the call (
-00000e00: 652e 672e 2c20 7072 6f66 616e 6974 7920  e.g., profanity 
-00000e10: 7363 6f72 6573 2c20 7072 6976 6163 7920  scores, privacy 
-00000e20: 6368 6563 6b73 2066 6f72 2065 6d61 696c  checks for email
-00000e30: 732f 7068 6f6e 6520 6e75 6d62 6572 7320  s/phone numbers 
-00000e40: 666f 756e 6420 696e 2074 6865 2074 6578  found in the tex
-00000e50: 7473 2c20 7465 7874 7561 6c20 616e 616c  ts, textual anal
-00000e60: 7973 6573 2c20 6574 632e 2e2e 290a 0a54  yses, etc...)..T
-00000e70: 6865 2060 6d6f 6e69 746f 7260 2066 756e  he `monitor` fun
-00000e80: 6374 696f 6e20 7265 6365 6976 6573 2074  ction receives t
-00000e90: 6865 2066 6f6c 6c6f 7769 6e67 2061 7267  he following arg
-00000ea0: 756d 656e 7473 3a0a 6f70 656e 6169 5f63  uments:.openai_c
-00000eb0: 6c61 7373 3a20 416e 204f 7065 6e41 4920  lass: An OpenAI 
-00000ec0: 4150 4920 636c 6173 7320 746f 2077 7261  API class to wra
-00000ed0: 7020 7769 7468 206d 6f6e 6974 6f72 696e  p with monitorin
-00000ee0: 6720 6361 7061 6269 6c74 6965 732e 0a6d  g capabilties..m
-00000ef0: 6f6e 615f 6372 6564 733a 2041 2064 6963  ona_creds: A dic
-00000f00: 7420 2863 6f6e 7461 696e 696e 6720 226b  t (containing "k
-00000f10: 6579 2220 616e 6420 2273 6563 7265 7422  ey" and "secret"
-00000f20: 2920 6f72 2070 6169 7220 2874 7570 6c65  ) or pair (tuple
-00000f30: 2920 6f66 204d 6f6e 6120 4150 4920 6b65  ) of Mona API ke
-00000f40: 7920 616e 6420 7365 6372 6574 2074 6f20  y and secret to 
-00000f50: 7365 7420 7570 204d 6f6e 6127 7320 636c  set up Mona's cl
-00000f60: 6965 6e74 7320 6672 6f6d 2069 7473 2053  ients from its S
-00000f70: 444b 2e0a 636f 6e74 6578 745f 636c 6173  DK..context_clas
-00000f80: 733a 2054 6865 204d 6f6e 6120 636f 6e74  s: The Mona cont
-00000f90: 6578 7420 636c 6173 7320 6e61 6d65 2074  ext class name t
-00000fa0: 6f20 7573 6520 666f 7220 6d6f 6e69 746f  o use for monito
-00000fb0: 7269 6e67 2e20 5573 6520 6120 636f 6e73  ring. Use a cons
-00000fc0: 7461 6e74 206e 616d 6520 6f66 2079 6f75  tant name of you
-00000fd0: 7220 6368 6f69 6365 2e0a 7370 6563 733a  r choice..specs:
-00000fe0: 2041 2064 6963 7469 6f6e 6172 7920 6f66   A dictionary of
-00000ff0: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
-00001000: 7375 6368 2061 7320 6d6f 6e69 746f 7269  such as monitori
-00001010: 6e67 2073 616d 706c 696e 6720 7261 7469  ng sampling rati
-00001020: 6f2e 0a0a 2323 2323 2053 7065 6373 0a54  o...#### Specs.T
-00001030: 6865 2073 7065 6373 2061 7267 2061 6c6c  he specs arg all
-00001040: 6f77 7320 796f 7520 746f 2063 6f6e 6669  ows you to confi
-00001050: 6775 7265 2077 6861 7420 7368 6f75 6c64  gure what should
-00001060: 2062 6520 6d6f 6e69 746f 7265 642e 2049   be monitored. I
-00001070: 7420 6578 7065 6374 7320 6120 7079 7468  t expects a pyth
-00001080: 6f6e 2064 6963 7420 7769 7468 2074 6865  on dict with the
-00001090: 2066 6f6c 6c77 6f69 6e67 2070 6f73 7369   follwoing possi
-000010a0: 626c 6520 6b65 7973 3a0a 2a20 7361 6d70  ble keys:.* samp
-000010b0: 6c69 6e67 5f72 6174 696f 2028 3129 3a20  ling_ratio (1): 
-000010c0: 4120 6e75 6d62 6572 2062 6574 7765 656e  A number between
-000010d0: 2030 2061 6e64 2031 2066 6f72 2068 6f77   0 and 1 for how
-000010e0: 206f 6674 656e 2073 686f 756c 6420 7468   often should th
-000010f0: 6520 6361 6c6c 2062 6520 6c6f 6767 6564  e call be logged
-00001100: 2e0a 2a20 6176 6f69 645f 6d6f 6e69 746f  ..* avoid_monito
-00001110: 7269 6e67 5f65 7863 6570 7469 6f6e 7320  ring_exceptions 
-00001120: 2846 616c 7365 293a 2057 6865 7468 6572  (False): Whether
-00001130: 206f 7220 6e6f 7420 746f 206c 6f67 206f   or not to log o
-00001140: 7574 2074 6f20 4d6f 6e61 2077 6865 6e20  ut to Mona when 
-00001150: 7468 6572 6520 6973 2061 6e20 4f70 656e  there is an Open
-00001160: 4149 2065 7863 6570 7469 6f6e 2e20 4465  AI exception. De
-00001170: 6661 756c 7420 6973 2074 6f20 7472 6163  fault is to trac
-00001180: 6b20 6578 6365 7074 696f 6e73 202d 2061  k exceptions - a
-00001190: 6e64 204d 6f6e 6120 7769 6c6c 2061 6c65  nd Mona will ale
-000011a0: 7274 2079 6f75 206f 6e20 7468 696e 6773  rt you on things
-000011b0: 206c 696b 6520 6120 6a75 6d70 2069 6e20   like a jump in 
-000011c0: 6e75 6d62 6572 206f 6620 6578 6365 7074  number of except
-000011d0: 696f 6e73 0a2a 2065 7870 6f72 745f 7072  ions.* export_pr
-000011e0: 6f6d 7074 2028 4661 6c73 6529 3a20 5768  ompt (False): Wh
-000011f0: 6574 6865 7220 4d6f 6e61 2073 686f 756c  ether Mona shoul
-00001200: 6420 6578 706f 7274 2074 6865 2061 6374  d export the act
-00001210: 7561 6c20 7072 6f6d 7074 2074 6578 742e  ual prompt text.
-00001220: 2042 6520 6465 6661 756c 7420 7365 7420   Be default set 
-00001230: 746f 2046 616c 7365 2074 6f20 6176 6f69  to False to avoi
-00001240: 6420 7072 6976 6163 7920 636f 6e63 6572  d privacy concer
-00001250: 6e73 2e0a 2a20 6578 706f 7274 5f72 6573  ns..* export_res
-00001260: 706f 6e73 655f 7465 7874 7320 2846 616c  ponse_texts (Fal
-00001270: 7365 293a 2057 6865 7468 6572 204d 6f6e  se): Whether Mon
-00001280: 6120 7368 6f75 6c64 2065 7870 6f72 7420  a should export 
-00001290: 7468 6520 6163 7475 616c 2072 6573 706f  the actual respo
-000012a0: 6e73 6520 7465 7874 732e 2042 6520 6465  nse texts. Be de
-000012b0: 6661 756c 7420 7365 7420 746f 2046 616c  fault set to Fal
-000012c0: 7365 2074 6f20 6176 6f69 6420 7072 6976  se to avoid priv
-000012d0: 6163 7920 636f 6e63 6572 6e73 2e0a 2a20  acy concerns..* 
-000012e0: 616e 616c 7973 6973 3a20 4120 6469 6374  analysis: A dict
-000012f0: 696f 6e61 7279 206d 6170 7069 6e67 2065  ionary mapping e
-00001300: 6163 6820 616e 616c 7973 6973 2074 7970  ach analysis typ
-00001310: 6520 746f 2061 2062 6f6f 6c65 616e 2076  e to a boolean v
-00001320: 616c 7565 2074 656c 6c69 6e67 2074 6865  alue telling the
-00001330: 2063 6c69 656e 7420 7768 6574 6865 7220   client whether 
-00001340: 6f72 206e 6f74 2074 6f20 7275 6e20 7361  or not to run sa
-00001350: 6964 2061 6e61 6c79 7369 7320 616e 6420  id analysis and 
-00001360: 6c6f 6720 6974 2074 6f20 4d6f 6e61 2e20  log it to Mona. 
-00001370: 506f 7373 6962 6c65 206f 7074 696f 6e73  Possible options
-00001380: 2063 7572 7265 6e74 6c79 2061 7265 2022   currently are "
-00001390: 7072 6976 6163 7922 2c20 2270 726f 6661  privacy", "profa
-000013a0: 6e69 7479 222c 2061 6e64 2022 7465 7874  nity", and "text
-000013b0: 7561 6c22 2e20 4279 2064 6566 6175 6c74  ual". By default
-000013c0: 2c20 616c 6c20 616e 616c 7973 6573 2074  , all analyses t
-000013d0: 616b 6520 706c 6163 6520 616e 6420 6172  ake place and ar
-000013e0: 6520 6c6f 6767 6564 206f 7574 2074 6f20  e logged out to 
-000013f0: 4d6f 6e61 2e0a 0a23 2323 2043 6170 6162  Mona...### Capab
-00001400: 696c 6974 6965 7320 6475 7269 6e67 2041  ilities during A
-00001410: 5049 2063 616c 6c73 0a0a 4166 7465 7220  PI calls..After 
-00001420: 7772 6170 7069 6e67 2079 6f75 7220 656e  wrapping your en
-00001430: 6470 6f69 6e74 2077 6974 6820 606d 6f6e  dpoint with `mon
-00001440: 6974 6f72 602c 2079 6f75 2072 6561 6c6c  itor`, you reall
-00001450: 7920 646f 6e27 7420 6e65 6564 2074 6f20  y don't need to 
-00001460: 646f 2061 6e79 7468 696e 6720 656c 7365  do anything else
-00001470: 2e20 5768 656e 2075 7369 6e67 2060 6372  . When using `cr
-00001480: 6561 7465 6020 6f72 2060 6163 7265 6174  eate` or `acreat
-00001490: 6560 2064 6174 6120 7769 6c6c 2062 6520  e` data will be 
-000014a0: 7472 6163 6b65 6420 616e 6420 6d6f 6e69  tracked and moni
-000014b0: 746f 7269 6e67 2077 696c 6c20 7461 6b65  toring will take
-000014c0: 2070 6c61 6365 2e0a 0a54 6865 7265 2061   place...There a
-000014d0: 7265 2c20 686f 7765 7665 722c 2073 6576  re, however, sev
-000014e0: 6572 616c 2063 6170 6162 696c 6974 6965  eral capabilitie
-000014f0: 7320 7468 6174 2061 7265 2061 6464 6564  s that are added
-00001500: 2074 6f20 7468 6573 6520 6675 6e63 7469   to these functi
-00001510: 6f6e 732e 2053 7065 6369 6669 6361 6c6c  ons. Specificall
-00001520: 792c 2079 6f75 2063 616e 2061 6464 2074  y, you can add t
-00001530: 6865 2066 6f6c 6c6f 7769 6e67 2061 7267  he following arg
-00001540: 756d 656e 7473 2074 6f20 616e 7920 6372  uments to any cr
-00001550: 6561 7465 2063 616c 6c3a 0a2a 204d 4f4e  eate call:.* MON
-00001560: 415f 636f 6e74 6578 745f 6964 3a20 5468  A_context_id: Th
-00001570: 6520 756e 6971 7565 2069 6420 6f66 2074  e unique id of t
-00001580: 6865 2063 6f6e 7465 7874 2069 6e20 7768  he context in wh
-00001590: 6963 6820 7468 6520 6361 6c6c 2069 7320  ich the call is 
-000015a0: 6d61 6465 2e20 4279 2075 7369 6e67 2074  made. By using t
-000015b0: 6869 7320 4944 2079 6f75 2063 616e 2065  his ID you can e
-000015c0: 7870 6f72 7420 6d6f 7265 2064 6174 6120  xport more data 
-000015d0: 746f 204d 6f6e 6120 746f 2074 6865 2073  to Mona to the s
-000015e0: 616d 6520 636f 6e74 6578 7420 6672 6f6d  ame context from
-000015f0: 206f 7468 6572 2070 6c61 6365 732e 2049   other places. I
-00001600: 6620 6e6f 7420 7375 7070 6c69 6564 2c20  f not supplied, 
-00001610: 7468 6520 2269 6422 2066 6965 6c64 206f  the "id" field o
-00001620: 6620 7468 6520 4f70 656e 4149 2045 6e64  f the OpenAI End
-00001630: 706f 696e 7427 7320 7265 7370 6f6e 7365  point's response
-00001640: 2077 696c 6c20 6265 2075 7365 6420 6173   will be used as
-00001650: 2074 6865 204d 6f6e 6120 636f 6e74 6578   the Mona contex
-00001660: 7420 4944 2061 7574 6f6d 6174 6963 616c  t ID automatical
-00001670: 6c79 2e0a 2a20 4d4f 4e41 5f65 7870 6f72  ly..* MONA_expor
-00001680: 745f 7469 6d65 7374 616d 703a 2043 616e  t_timestamp: Can
-00001690: 2062 6520 7573 6564 2074 6f20 7369 6d75   be used to simu
-000016a0: 6c61 7465 2061 7320 6966 2074 6865 2063  late as if the c
-000016b0: 7572 7265 6e74 2063 616c 6c20 7761 7320  urrent call was 
-000016c0: 6d61 6465 2069 6e20 6120 6469 6666 6572  made in a differ
-000016d0: 656e 7420 7469 6d65 2c20 6173 2066 6172  ent time, as far
-000016e0: 2061 7320 4d6f 6e61 2069 7320 636f 6e63   as Mona is conc
-000016f0: 6572 6e65 642e 0a2a 204d 4f4e 415f 6164  erned..* MONA_ad
-00001700: 6469 7469 6f6e 616c 5f64 6174 613a 2041  ditional_data: A
-00001710: 204a 534f 4e2d 7365 7269 616c 697a 6162   JSON-serializab
-00001720: 6c65 2064 6963 7420 7769 7468 2061 6e79  le dict with any
-00001730: 206f 7468 6572 2064 6174 6120 796f 7520   other data you 
-00001740: 7761 6e74 2074 6f20 6164 6420 746f 2074  want to add to t
-00001750: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
-00001760: 6e74 6578 742e 2054 6869 7320 636f 6d65  ntext. This come
-00001770: 7320 696e 2068 616e 6479 2069 6620 796f  s in handy if yo
-00001780: 7520 7761 6e74 2074 6f20 6164 6420 6d6f  u want to add mo
-00001790: 7265 2069 6e66 6f72 6d61 7469 6f6e 2074  re information t
-000017a0: 6f20 7468 6520 6d6f 6e69 746f 7269 6e67  o the monitoring
-000017b0: 2063 6f6e 7465 7820 7468 6174 2069 736e   contex that isn
-000017c0: 2774 2070 6172 7420 6f66 2074 6865 2062  't part of the b
-000017d0: 6173 6963 204f 7065 6e41 4920 4150 4920  asic OpenAI API 
-000017e0: 6361 6c6c 2069 6e66 6f72 6d61 7469 6f6e  call information
-000017f0: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
-00001800: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-00001810: 6120 7370 6563 6966 6963 2074 656d 706c  a specific templ
-00001820: 6174 6520 4944 206f 7220 6966 2074 6869  ate ID or if thi
-00001830: 7320 6361 6c6c 2069 7320 6265 696e 6720  s call is being 
-00001840: 6d61 6465 2066 6f72 2061 2073 7065 6369  made for a speci
-00001850: 6669 6320 6375 7374 6f6d 6572 2049 442c  fic customer ID,
-00001860: 2074 6865 7365 2061 7265 2066 6965 6c64   these are field
-00001870: 7320 796f 7520 6361 6e20 6164 6420 7468  s you can add th
-00001880: 6572 6520 746f 2068 656c 7020 6765 7420  ere to help get 
-00001890: 6675 6c6c 2063 6f6e 7465 7874 2077 6865  full context whe
-000018a0: 6e20 6d6f 6e69 746f 7269 6e67 2077 6974  n monitoring wit
-000018b0: 6820 4d6f 6e61 2e0a 0a45 7861 6d70 6c65  h Mona...Example
-000018c0: 3a0a 6060 6070 790a 7265 7370 6f6e 7365  :.```py.response
-000018d0: 203d 2061 7379 6e63 696f 2e72 756e 286d   = asyncio.run(m
-000018e0: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
-000018f0: 696f 6e2e 6163 7265 6174 6528 0a20 2020  ion.acreate(.   
-00001900: 2065 6e67 696e 653d 6d6f 6465 6c2c 0a20   engine=model,. 
-00001910: 2020 2070 726f 6d70 743d 7072 6f6d 7074     prompt=prompt
-00001920: 2c0a 2020 2020 6d61 785f 746f 6b65 6e73  ,.    max_tokens
-00001930: 3d6d 6178 5f74 6f6b 656e 732c 0a20 2020  =max_tokens,.   
-00001940: 206e 3d6e 2c0a 2020 2020 7465 6d70 6572   n=n,.    temper
-00001950: 6174 7572 653d 7465 6d70 6572 6174 7572  ature=temperatur
-00001960: 652c 0a20 2020 204d 4f4e 415f 6164 6469  e,.    MONA_addi
-00001970: 7469 6f6e 616c 5f64 6174 613d 7b22 6375  tional_data={"cu
-00001980: 7374 6f6d 6572 5f69 6422 3a20 2241 3533  stomer_id": "A53
-00001990: 3132 3531 227d 2c0a 2929 0a70 7269 6e74  1251"},.)).print
-000019a0: 2872 6573 706f 6e73 652e 6368 6f69 6365  (response.choice
-000019b0: 735b 305d 2e74 6578 7429 0a60 6060 0a0a  s[0].text).```..
-000019c0: 2323 2320 5573 696e 6720 4f70 656e 4149  ### Using OpenAI
-000019d0: 2077 6974 6820 5245 5354 2063 616c 6c73   with REST calls
-000019e0: 2069 6e73 7465 6164 206f 6620 4f70 656e   instead of Open
-000019f0: 4149 2773 2050 7974 686f 6e20 636c 6965  AI's Python clie
-00001a00: 6e74 0a49 6e20 736f 6d65 2063 6173 6573  nt.In some cases
-00001a10: 2079 6f75 206d 6179 2063 686f 6f73 6520   you may choose 
-00001a20: 746f 2075 7365 204f 7065 6e41 4927 7320  to use OpenAI's 
-00001a30: 4150 4920 6469 7265 6374 6c79 2077 6974  API directly wit
-00001a40: 6820 5245 5354 2063 616c 6c73 2061 6e64  h REST calls and
-00001a50: 206e 6f74 2075 7369 6e67 204f 7065 6e41   not using OpenA
-00001a60: 4927 7320 5344 4b2e 2046 6f72 2074 6865  I's SDK. For the
-00001a70: 7365 2063 6173 6573 2077 6520 616c 6c6f  se cases we allo
-00001a80: 7720 6120 6d6f 7265 2064 6972 6563 7420  w a more direct 
-00001a90: 6170 7072 6f61 6368 2066 6f72 206c 6f67  approach for log
-00001aa0: 6769 6e67 2074 6f20 4d6f 6e61 2061 7320  ging to Mona as 
-00001ab0: 7765 6c6c 2c20 6279 2075 7369 6e67 2074  well, by using t
-00001ac0: 6865 2022 6765 745f 7265 7374 5f6d 6f6e  he "get_rest_mon
-00001ad0: 6974 6f72 2220 6675 6e63 7469 6f6e 2e20  itor" function. 
-00001ae0: 5365 6520 6578 616d 706c 6520 6265 6c6f  See example belo
-00001af0: 772e 0a0a 6060 6070 790a 2320 4469 7265  w...```py.# Dire
-00001b00: 6374 2052 4553 5420 7573 6167 652c 2077  ct REST usage, w
-00001b10: 6974 686f 7574 204f 7065 6e41 4920 636c  ithout OpenAI cl
-00001b20: 6965 6e74 0a69 6d70 6f72 7420 7265 7175  ient.import requ
-00001b30: 6573 7473 0a66 726f 6d20 6f73 2069 6d70  ests.from os imp
-00001b40: 6f72 7420 656e 7669 726f 6e0a 6672 6f6d  ort environ.from
-00001b50: 206d 6f6e 615f 6f70 656e 6169 2069 6d70   mona_openai imp
-00001b60: 6f72 7420 6765 745f 7265 7374 5f6d 6f6e  ort get_rest_mon
-00001b70: 6974 6f72 0a0a 0a4d 4f4e 415f 4150 495f  itor...MONA_API_
-00001b80: 4b45 5920 3d20 656e 7669 726f 6e2e 6765  KEY = environ.ge
-00001b90: 7428 224d 4f4e 415f 4150 495f 4b45 5922  t("MONA_API_KEY"
-00001ba0: 290a 4d4f 4e41 5f53 4543 5245 5420 3d20  ).MONA_SECRET = 
-00001bb0: 656e 7669 726f 6e2e 6765 7428 224d 4f4e  environ.get("MON
-00001bc0: 415f 5345 4352 4554 2229 0a4d 4f4e 415f  A_SECRET").MONA_
-00001bd0: 4352 4544 5320 3d20 7b0a 2020 2020 226b  CREDS = {.    "k
-00001be0: 6579 223a 204d 4f4e 415f 4150 495f 4b45  ey": MONA_API_KE
-00001bf0: 592c 0a20 2020 2022 7365 6372 6574 223a  Y,.    "secret":
-00001c00: 204d 4f4e 415f 5345 4352 4554 2c0a 7d0a   MONA_SECRET,.}.
-00001c10: 434f 4e54 4558 545f 434c 4153 535f 4e41  CONTEXT_CLASS_NA
-00001c20: 4d45 203d 2022 534f 4d45 5f4d 4f4e 4954  ME = "SOME_MONIT
-00001c30: 4f52 494e 475f 434f 4e54 4558 545f 4e41  ORING_CONTEXT_NA
-00001c40: 4d45 220a 0a23 2047 6574 204d 6f6e 6120  ME"..# Get Mona 
-00001c50: 6c6f 6767 6572 0a6d 6f6e 615f 6c6f 6767  logger.mona_logg
-00001c60: 6572 203d 2067 6574 5f72 6573 745f 6d6f  er = get_rest_mo
-00001c70: 6e69 746f 7228 0a20 2020 2022 436f 6d70  nitor(.    "Comp
-00001c80: 6c65 7469 6f6e 222c 0a20 2020 204d 4f4e  letion",.    MON
-00001c90: 415f 4352 4544 532c 0a20 2020 2043 4f4e  A_CREDS,.    CON
-00001ca0: 5445 5854 5f43 4c41 5353 5f4e 414d 452c  TEXT_CLASS_NAME,
-00001cb0: 0a29 0a0a 2320 5365 7420 7570 2074 6865  .)..# Set up the
-00001cc0: 2041 5049 2065 6e64 706f 696e 7420 5552   API endpoint UR
-00001cd0: 4c20 616e 6420 6175 7468 656e 7469 6361  L and authentica
-00001ce0: 7469 6f6e 2068 6561 6465 7273 0a75 726c  tion headers.url
-00001cf0: 203d 2022 6874 7470 733a 2f2f 6170 692e   = "https://api.
-00001d00: 6f70 656e 6169 2e63 6f6d 2f76 312f 636f  openai.com/v1/co
-00001d10: 6d70 6c65 7469 6f6e 7322 0a68 6561 6465  mpletions".heade
-00001d20: 7273 203d 207b 0a20 2020 2022 436f 6e74  rs = {.    "Cont
-00001d30: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-00001d40: 6963 6174 696f 6e2f 6a73 6f6e 222c 0a20  ication/json",. 
-00001d50: 2020 2022 4175 7468 6f72 697a 6174 696f     "Authorizatio
-00001d60: 6e22 3a20 6622 4265 6172 6572 207b 656e  n": f"Bearer {en
-00001d70: 7669 726f 6e2e 6765 7428 274f 5045 4e5f  viron.get('OPEN_
-00001d80: 4149 5f4b 4559 2729 7d22 2c0a 7d0a 0a23  AI_KEY')}",.}..#
-00001d90: 2053 6574 2075 7020 7468 6520 7265 7175   Set up the requ
-00001da0: 6573 7420 6461 7461 0a64 6174 6120 3d20  est data.data = 
-00001db0: 7b0a 2020 2020 2270 726f 6d70 7422 3a20  {.    "prompt": 
-00001dc0: 7072 6f6d 7074 2c0a 2020 2020 226d 6178  prompt,.    "max
-00001dd0: 5f74 6f6b 656e 7322 3a20 6d61 785f 746f  _tokens": max_to
-00001de0: 6b65 6e73 2c0a 2020 2020 2274 656d 7065  kens,.    "tempe
-00001df0: 7261 7475 7265 223a 2074 656d 7065 7261  rature": tempera
-00001e00: 7475 7265 2c0a 2020 2020 226d 6f64 656c  ture,.    "model
-00001e10: 223a 206d 6f64 656c 2c0a 2020 2020 226e  ": model,.    "n
-00001e20: 223a 206e 2c0a 7d0a 0a23 2054 6865 206c  ": n,.}..# The l
-00001e30: 6f67 5f72 6571 7565 7374 2066 756e 6374  og_request funct
-00001e40: 696f 6e20 7265 7475 726e 7320 7477 6f20  ion returns two 
-00001e50: 6f74 6865 7220 6675 6e63 7469 6f6e 2066  other function f
-00001e60: 6f72 206c 6174 6572 206c 6f67 6769 6e67  or later logging
-00001e70: 0a23 2074 6865 2072 6573 706f 6e73 6520  .# the response 
-00001e80: 6f72 2074 6865 2065 7863 6570 7469 6f6e  or the exception
-00001e90: 2e20 5768 656e 2077 6520 6c61 7465 7220  . When we later 
-00001ea0: 646f 2074 6861 742c 2074 6865 206c 6f67  do that, the log
-00001eb0: 6765 7220 7769 6c6c 0a23 2061 6374 7561  ger will.# actua
-00001ec0: 6c6c 7920 6361 6c63 756c 6174 6520 616c  lly calculate al
-00001ed0: 6c20 7468 6520 7265 6c65 7661 6e74 206d  l the relevant m
-00001ee0: 6574 7269 6373 2061 6e64 2077 696c 6c20  etrics and will 
-00001ef0: 7365 6e64 2074 6865 6d20 746f 0a23 204d  send them to.# M
-00001f00: 6f6e 612e 0a72 6573 706f 6e73 655f 6c6f  ona..response_lo
-00001f10: 6767 6572 2c20 6578 6365 7074 696f 6e5f  gger, exception_
-00001f20: 6c6f 6767 6572 203d 206d 6f6e 615f 6c6f  logger = mona_lo
-00001f30: 6767 6572 2e6c 6f67 5f72 6571 7565 7374  gger.log_request
-00001f40: 280a 2020 2020 6461 7461 2c20 6164 6469  (.    data, addi
-00001f50: 7469 6f6e 616c 5f64 6174 613d 7b22 6375  tional_data={"cu
-00001f60: 7374 6f6d 6572 5f69 6422 3a20 2241 3533  stomer_id": "A53
-00001f70: 3132 3531 227d 0a29 0a0a 7472 793a 0a20  1251"}.)..try:. 
-00001f80: 2020 2023 2053 656e 6420 7468 6520 7265     # Send the re
-00001f90: 7175 6573 7420 746f 2074 6865 2041 5049  quest to the API
-00001fa0: 0a20 2020 2072 6573 706f 6e73 6520 3d20  .    response = 
-00001fb0: 7265 7175 6573 7473 2e70 6f73 7428 7572  requests.post(ur
-00001fc0: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
-00001fd0: 7273 2c20 6a73 6f6e 3d64 6174 6129 0a0a  rs, json=data)..
-00001fe0: 2020 2020 2320 4368 6563 6b20 666f 7220      # Check for 
-00001ff0: 4854 5450 2065 7272 6f72 730a 2020 2020  HTTP errors.    
-00002000: 7265 7370 6f6e 7365 2e72 6169 7365 5f66  response.raise_f
-00002010: 6f72 5f73 7461 7475 7328 290a 0a20 2020  or_status()..   
-00002020: 2023 204c 6f67 2072 6573 706f 6e73 6520   # Log response 
-00002030: 746f 204d 6f6e 610a 2020 2020 7265 7370  to Mona.    resp
-00002040: 6f6e 7365 5f6c 6f67 6765 7228 7265 7370  onse_logger(resp
-00002050: 6f6e 7365 2e6a 736f 6e28 2929 0a20 2020  onse.json()).   
-00002060: 2070 7269 6e74 2872 6573 706f 6e73 652e   print(response.
-00002070: 6a73 6f6e 2829 5b22 6368 6f69 6365 7322  json()["choices"
-00002080: 5d5b 305d 5b22 7465 7874 225d 290a 0a65  ][0]["text"])..e
-00002090: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-000020a0: 6173 2065 7272 3a0a 2020 2020 2320 4c6f  as err:.    # Lo
-000020b0: 6720 6578 6365 7074 696f 6e20 746f 204d  g exception to M
-000020c0: 6f6e 610a 2020 2020 6578 6365 7074 696f  ona.    exceptio
-000020d0: 6e5f 6c6f 6767 6572 2829 0a60 6060 0a0a  n_logger().```..
-000020e0: 2323 2320 5374 7265 616d 2073 7570 706f  ### Stream suppo
-000020f0: 7274 0a0a 4f70 656e 4149 2061 6c6c 6f77  rt..OpenAI allow
-00002100: 7320 7265 6365 6976 696e 6720 7265 7370  s receiving resp
-00002110: 6f6e 7365 7320 6173 2061 2073 7472 6561  onses as a strea
-00002120: 6d20 6f66 2074 6f6b 656e 7320 7573 696e  m of tokens usin
-00002130: 6720 7468 6520 2273 7472 6561 6d22 2070  g the "stream" p
-00002140: 6172 616d 6574 6572 2e20 5768 656e 2074  arameter. When t
-00002150: 6869 7320 6973 2064 6f6e 652c 204d 6f6e  his is done, Mon
-00002160: 6120 7769 6c6c 2063 6f6c 6c65 6374 2061  a will collect a
-00002170: 6c6c 2074 6865 2074 6f6b 656e 7320 696e  ll the tokens in
-00002180: 206d 656d 6f72 7920 616e 6420 7769 6c6c   memory and will
-00002190: 2063 7265 6174 6520 7468 6520 616e 616c   create the anal
-000021a0: 7973 6973 2061 6e64 206c 6f67 206f 7574  ysis and log out
-000021b0: 2074 6865 2064 6174 6120 7468 6520 6d6f   the data the mo
-000021c0: 6d65 6e74 2074 6865 2073 7472 6561 6d20  ment the stream 
-000021d0: 6973 206f 7665 722e 2059 6f75 2064 6f6e  is over. You don
-000021e0: 2774 206e 6565 6420 746f 2064 6f20 616e  't need to do an
-000021f0: 7974 6869 6e67 2074 6f20 6d61 6b65 2074  ything to make t
-00002200: 6869 7320 6861 7070 656e 2e0a 0a53 696e  his happen...Sin
-00002210: 6365 2066 6f72 2073 7472 6561 6d69 6e67  ce for streaming
-00002220: 2072 6573 706f 6e73 6573 204f 7065 6e41   responses OpenA
-00002230: 4920 646f 6573 6e27 7420 7375 7070 6c79  I doesn't supply
-00002240: 2074 6865 2066 756c 6c20 7573 6167 6520   the full usage 
-00002250: 746f 6b65 6e73 2073 756d 6d61 7279 2c20  tokens summary, 
-00002260: 4d6f 6e61 2075 7365 7320 7468 6520 7469  Mona uses the ti
-00002270: 6b74 6f6b 656e 2070 6163 6b61 6765 2074  ktoken package t
-00002280: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00002290: 746f 6b65 6e73 206f 6620 7468 6520 7072  tokens of the pr
-000022a0: 6f6d 7074 2061 6e64 2063 6f6d 706c 6574  ompt and complet
-000022b0: 696f 6e20 616e 6420 6c6f 6720 7468 656d  ion and log them
-000022c0: 2066 6f72 206d 6f6e 6974 6f72 696e 672e   for monitoring.
-000022d0: 0a0a 4e4f 5445 3a20 5374 7265 616d 2069  ..NOTE: Stream i
-000022e0: 7320 6375 7272 656e 746c 7920 6f6e 6c79  s currently only
-000022f0: 2073 7570 706f 7274 6564 2077 6974 6820   supported with 
-00002300: 5344 4b20 7573 6167 652c 2061 6e64 206e  SDK usage, and n
-00002310: 6f74 2077 6974 6820 7573 696e 6720 5245  ot with using RE
-00002320: 5354 2064 6972 6563 746c 792e 0a0a 0a23  ST directly....#
-00002330: 2320 4d6f 6e61 2053 444b 0a0a 5468 6973  # Mona SDK..This
-00002340: 2070 6163 6b61 6765 2075 7365 7320 7468   package uses th
-00002350: 6520 6d6f 6e61 5f73 646b 2070 6163 6b61  e mona_sdk packa
-00002360: 6765 2074 6f20 6578 706f 7274 2074 6865  ge to export the
-00002370: 2072 656c 6576 616e 7420 6461 7461 2074   relevant data t
-00002380: 6f20 4d6f 6e61 2e20 5468 6572 6520 6172  o Mona. There ar
-00002390: 6520 7365 7665 7261 6c20 656e 7669 726f  e several enviro
-000023a0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-000023b0: 796f 7520 6361 6e20 7573 6520 746f 2063  you can use to c
-000023c0: 6f6e 6669 6775 7265 2074 6865 2053 444b  onfigure the SDK
-000023d0: 2773 2062 6568 6176 696f 722e 2046 6f72  's behavior. For
-000023e0: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
-000023f0: 6e20 7365 7420 6974 2075 7020 746f 2072  n set it up to r
-00002400: 6169 7365 2065 7863 6570 7469 6f6e 7320  aise exceptions 
-00002410: 7768 656e 2065 7870 6f72 7469 6e67 2064  when exporting d
-00002420: 6174 6120 746f 204d 6f6e 6120 6661 696c  ata to Mona fail
-00002430: 7320 2869 7420 646f 6573 6e27 7420 646f  s (it doesn't do
-00002440: 2074 6861 7420 6279 2064 6566 6175 6c74   that by default
-00002450: 292e 0a0a 2323 204d 6f6e 6974 6f72 696e  )...## Monitorin
-00002460: 6720 666f 7220 7072 6f66 616e 6974 790a  g for profanity.
-00002470: 0a4d 6f6e 6120 7573 6573 2074 6865 2061  .Mona uses the a
-00002480: 6c74 2d70 726f 6661 6e69 7479 2d63 6865  lt-profanity-che
-00002490: 636b 2070 6163 616b 6765 2028 6874 7470  ck pacakge (http
-000024a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000024b0: 6a65 6374 2f61 6c74 2d70 726f 6661 6e69  ject/alt-profani
-000024c0: 7479 2d63 6865 636b 2f29 2074 6f20 6372  ty-check/) to cr
-000024d0: 6561 7465 2062 6f74 6820 626f 6f6c 6561  eate both boolea
-000024e0: 6e20 7072 6564 6963 7469 6f6e 7320 616e  n predictions an
-000024f0: 6420 7072 6f62 6162 696c 7479 2073 636f  d probabilty sco
-00002500: 7265 7320 666f 7220 7468 6520 6578 6973  res for the exis
-00002510: 7465 6e63 6520 6f66 2070 726f 6661 6e69  tence of profani
-00002520: 7479 2062 6f74 6820 696e 2074 6865 2070  ty both in the p
-00002530: 726f 6d70 7420 616e 6420 696e 2074 6865  rompt and in the
-00002540: 2072 6573 706f 6e73 6573 2e20 5765 2075   responses. We u
-00002550: 7365 2074 6865 2062 7569 6c74 2069 6e20  se the built in 
-00002560: 7061 636b 6167 6520 6d65 7468 6f64 7320  package methods 
-00002570: 666f 7220 7468 6174 2e20 4966 2079 6f75  for that. If you
-00002580: 2077 616e 742c 2066 6f72 2065 7861 6d70   want, for examp
-00002590: 6c65 2c20 746f 2075 7365 2061 2064 6966  le, to use a dif
-000025a0: 6665 7265 6e74 2070 726f 6261 6269 6c69  ferent probabili
-000025b0: 7479 2074 6872 6573 686f 6c64 2066 6f72  ty threshold for
-000025c0: 2074 6865 2062 6f6f 6c65 616e 2070 7265   the boolean pre
-000025d0: 6469 6374 696f 6e2c 2079 6f75 2063 616e  diction, you can
-000025e0: 2064 6f20 7468 6174 2062 7920 6368 616e   do that by chan
-000025f0: 6769 6e67 2079 6f75 7220 4d6f 6e61 2063  ging your Mona c
-00002600: 6f6e 6669 6720 6f6e 2074 6865 204d 6f6e  onfig on the Mon
-00002610: 6120 6461 7368 626f 6172 642e 0a         a dashboard..
+00000000: 2320 4d6f 6e61 2d4f 7065 6e41 4920 496e  # Mona-OpenAI In
+00000010: 7465 6772 6174 696f 6e20 436c 6965 6e74  tegration Client
+00000020: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000030: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
+00000040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000050: 6f6d 2f6d 6f6e 616c 6162 732f 6d6f 6e61  om/monalabs/mona
+00000060: 2d73 646b 2f62 6c6f 622f 6d61 696e 2f6d  -sdk/blob/main/m
+00000070: 6f6e 615f 6c6f 676f 2e70 6e67 3f72 6177  ona_logo.png?raw
+00000080: 3d74 7275 6522 2061 6c74 3d22 4d6f 6e61  =true" alt="Mona
+00000090: 2773 206c 6f67 6f22 2077 6964 7468 3d22  's logo" width="
+000000a0: 3138 3022 2f3e 0a3c 2f70 3e0a 0a3c 7020  180"/>.</p>..<p 
+000000b0: 616c 6967 6e3d 2263 656e 7465 7222 3e3c  align="center"><
+000000c0: 6120 7461 7267 6574 3d22 5f62 6c61 6e6b  a target="_blank
+000000d0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+000000e0: 6d6f 6e61 6c61 6273 2e77 6973 7469 612e  monalabs.wistia.
+000000f0: 636f 6d2f 6d65 6469 6173 2f6c 3678 6d64  com/medias/l6xmd
+00000100: 6a33 6364 363f 7776 6964 656f 3d6c 3678  j3cd6?wvideo=l6x
+00000110: 6d64 6a33 6364 3622 3e3c 696d 6720 7372  mdj3cd6"><img sr
+00000120: 633d 2268 7474 7073 3a2f 2f65 6d62 6564  c="https://embed
+00000130: 2d73 736c 2e77 6973 7469 612e 636f 6d2f  -ssl.wistia.com/
+00000140: 6465 6c69 7665 7269 6573 2f63 3135 6262  deliveries/c15bb
+00000150: 3631 3661 3338 3966 6137 6437 3532 3936  616a389fa7d75296
+00000160: 3863 6362 3361 6632 6162 342e 6a70 673f  8ccb3af2ab4.jpg?
+00000170: 7769 7374 6961 2d6c 3678 6d64 6a33 6364  wistia-l6xmdj3cd
+00000180: 362d 312d 6c36 786d 646a 3363 6436 2d76  6-1-l6xmdj3cd6-v
+00000190: 6964 656f 2d74 6875 6d62 6e61 696c 3d31  ideo-thumbnail=1
+000001a0: 2661 6d70 3b69 6d61 6765 5f70 6c61 795f  &amp;image_play_
+000001b0: 6275 7474 6f6e 5f73 697a 653d 3278 2661  button_size=2x&a
+000001c0: 6d70 3b69 6d61 6765 5f63 726f 705f 7265  mp;image_crop_re
+000001d0: 7369 7a65 643d 3936 3078 3534 3026 616d  sized=960x540&am
+000001e0: 703b 696d 6167 655f 706c 6179 5f62 7574  p;image_play_but
+000001f0: 746f 6e3d 3126 616d 703b 696d 6167 655f  ton=1&amp;image_
+00000200: 706c 6179 5f62 7574 746f 6e5f 636f 6c6f  play_button_colo
+00000210: 723d 3636 6337 6431 6530 2220 7769 6474  r=66c7d1e0" widt
+00000220: 683d 2234 3030 2220 6865 6967 6874 3d22  h="400" height="
+00000230: 3232 3522 2073 7479 6c65 3d22 7769 6474  225" style="widt
+00000240: 683a 2034 3030 7078 3b20 6865 6967 6874  h: 400px; height
+00000250: 3a20 3232 3570 783b 223e 3c2f 613e 3c2f  : 225px;"></a></
+00000260: 703e 3c70 2061 6c69 676e 3d22 6365 6e74  p><p align="cent
+00000270: 6572 223e 3c61 2068 7265 663d 2268 7474  er"><a href="htt
+00000280: 7073 3a2f 2f6d 6f6e 616c 6162 732e 7769  ps://monalabs.wi
+00000290: 7374 6961 2e63 6f6d 2f6d 6564 6961 732f  stia.com/medias/
+000002a0: 6c36 786d 646a 3363 6436 3f77 7669 6465  l6xmdj3cd6?wvide
+000002b0: 6f3d 6c36 786d 646a 3363 6436 223e 4f70  o=l6xmdj3cd6">Op
+000002c0: 656e 4149 2047 5054 2049 6e74 6567 7261  enAI GPT Integra
+000002d0: 7469 6f6e 2054 7574 6f72 6961 6c3c 2f61  tion Tutorial</a
+000002e0: 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e 6520  ></p>...Use one 
+000002f0: 6c69 6e65 206f 6620 636f 6465 2074 6f20  line of code to 
+00000300: 6765 7420 696e 7374 616e 7420 6c69 7665  get instant live
+00000310: 206d 6f6e 6974 6f72 696e 6720 666f 7220   monitoring for 
+00000320: 796f 7572 204f 7065 6e41 4920 7573 6167  your OpenAI usag
+00000330: 6520 696e 636c 7564 696e 673a 0a2a 2054  e including:.* T
+00000340: 6f6b 656e 7320 7573 6167 650a 2a20 4861  okens usage.* Ha
+00000350: 6c6c 7563 696e 6174 696f 6e20 616c 6572  llucination aler
+00000360: 7473 0a2a 2050 726f 6661 6e69 7479 2061  ts.* Profanity a
+00000370: 6e64 2070 7269 7661 6379 2061 6e61 6c79  nd privacy analy
+00000380: 7365 730a 2a20 4265 6861 7669 6f72 616c  ses.* Behavioral
+00000390: 2064 7269 6674 7320 616e 6420 616e 6f6d   drifts and anom
+000003a0: 616c 6965 730a 2a20 4c61 6e67 4368 6169  alies.* LangChai
+000003b0: 6e20 7375 7070 6f72 740a 2a20 4d75 6368  n support.* Much
+000003c0: 206d 7563 6820 6d6f 7265 0a0a 2323 2053   much more..## S
+000003d0: 6574 7469 6e67 2055 700a 0a2d 2054 4f44  etting Up..- TOD
+000003e0: 4f3a 2041 6464 2070 6172 7420 6162 6f75  O: Add part abou
+000003f0: 7420 4d6f 6e61 2072 6567 6973 7472 6174  t Mona registrat
+00000400: 696f 6e20 7769 7468 2061 206c 696e 6b20  ion with a link 
+00000410: 746f 2074 6865 2072 656c 6576 616e 7420  to the relevant 
+00000420: 6c61 6e64 696e 6720 7061 6765 2077 6865  landing page whe
+00000430: 7265 2074 6865 2072 6561 6465 7220 6361  re the reader ca
+00000440: 6e20 7369 676e 2075 702e 0a60 6060 636f  n sign up..```co
+00000450: 6e73 6f6c 650a 2420 7069 7020 696e 7374  nsole.$ pip inst
+00000460: 616c 6c20 6d6f 6e61 5f6f 7065 6e61 690a  all mona_openai.
+00000470: 6060 600a 0a23 2320 5175 6963 6b20 5374  ```..## Quick St
+00000480: 6172 7420 616e 6420 4578 616d 706c 650a  art and Example.
+00000490: 0a45 7861 6d70 6c65 2062 6f69 6c65 7270  .Example boilerp
+000004a0: 6c61 7465 2063 6f64 6520 666f 7220 626f  late code for bo
+000004b0: 7468 2073 796e 6320 616e 6420 6173 796e  th sync and asyn
+000004c0: 6320 7573 6167 6520 6973 2067 6976 656e  c usage is given
+000004d0: 2069 6e20 7468 6520 6669 6c65 2022 6578   in the file "ex
+000004e0: 616d 706c 655f 7573 6167 652e 7079 2220  ample_usage.py" 
+000004f0: 616e 6420 6865 7265 3a0a 6060 6070 790a  and here:.```py.
+00000500: 6672 6f6d 206f 7320 696d 706f 7274 2065  from os import e
+00000510: 6e76 6972 6f6e 0a69 6d70 6f72 7420 6173  nviron.import as
+00000520: 796e 6369 6f0a 696d 706f 7274 206f 7065  yncio.import ope
+00000530: 6e61 690a 0a66 726f 6d20 6d6f 6e61 5f6f  nai..from mona_o
+00000540: 7065 6e61 6920 696d 706f 7274 206d 6f6e  penai import mon
+00000550: 6974 6f72 0a0a 6f70 656e 6169 2e61 7069  itor..openai.api
+00000560: 5f6b 6579 203d 2065 6e76 6972 6f6e 2e67  _key = environ.g
+00000570: 6574 2822 4f50 454e 5f41 495f 4b45 5922  et("OPEN_AI_KEY"
+00000580: 290a 0a4d 4f4e 415f 4150 495f 4b45 5920  )..MONA_API_KEY 
+00000590: 3d20 656e 7669 726f 6e2e 6765 7428 224d  = environ.get("M
+000005a0: 4f4e 415f 4150 495f 4b45 5922 290a 4d4f  ONA_API_KEY").MO
+000005b0: 4e41 5f53 4543 5245 5420 3d20 656e 7669  NA_SECRET = envi
+000005c0: 726f 6e2e 6765 7428 224d 4f4e 415f 5345  ron.get("MONA_SE
+000005d0: 4352 4554 2229 0a4d 4f4e 415f 4352 4544  CRET").MONA_CRED
+000005e0: 5320 3d20 7b0a 2020 2020 226b 6579 223a  S = {.    "key":
+000005f0: 204d 4f4e 415f 4150 495f 4b45 592c 0a20   MONA_API_KEY,. 
+00000600: 2020 2022 7365 6372 6574 223a 204d 4f4e     "secret": MON
+00000610: 415f 5345 4352 4554 2c0a 7d0a 434f 4e54  A_SECRET,.}.CONT
+00000620: 4558 545f 434c 4153 535f 4e41 4d45 203d  EXT_CLASS_NAME =
+00000630: 2022 534f 4d45 5f4d 4f4e 4954 4f52 494e   "SOME_MONITORIN
+00000640: 475f 434f 4e54 4558 545f 4e41 4d45 220a  G_CONTEXT_NAME".
+00000650: 0a0a 6d6f 6e69 746f 7265 645f 636f 6d70  ..monitored_comp
+00000660: 6c65 7469 6f6e 203d 206d 6f6e 6974 6f72  letion = monitor
+00000670: 280a 2020 2020 6f70 656e 6169 2e43 6f6d  (.    openai.Com
+00000680: 706c 6574 696f 6e2c 0a20 2020 204d 4f4e  pletion,.    MON
+00000690: 415f 4352 4544 532c 0a20 2020 2043 4f4e  A_CREDS,.    CON
+000006a0: 5445 5854 5f43 4c41 5353 5f4e 414d 452c  TEXT_CLASS_NAME,
+000006b0: 0a29 0a0a 0a70 726f 6d70 7420 3d20 2249  .)...prompt = "I
+000006c0: 2077 616e 7420 746f 2067 656e 6572 6174   want to generat
+000006d0: 6520 736f 6d65 2074 6578 7420 6162 6f75  e some text abou
+000006e0: 7420 220a 6d6f 6465 6c20 3d20 2274 6578  t ".model = "tex
+000006f0: 742d 6164 612d 3030 3122 0a74 656d 7065  t-ada-001".tempe
+00000700: 7261 7475 7265 203d 2030 2e36 0a6d 6178  rature = 0.6.max
+00000710: 5f74 6f6b 656e 7320 3d20 350a 6e20 3d20  _tokens = 5.n = 
+00000720: 310a 0a23 2052 6567 756c 6172 2028 7379  1..# Regular (sy
+00000730: 6e63 2920 7573 6167 650a 7265 7370 6f6e  nc) usage.respon
+00000740: 7365 203d 206d 6f6e 6974 6f72 6564 5f63  se = monitored_c
+00000750: 6f6d 706c 6574 696f 6e2e 6372 6561 7465  ompletion.create
+00000760: 280a 2020 2020 656e 6769 6e65 3d6d 6f64  (.    engine=mod
+00000770: 656c 2c0a 2020 2020 7072 6f6d 7074 3d70  el,.    prompt=p
+00000780: 726f 6d70 742c 0a20 2020 206d 6178 5f74  rompt,.    max_t
+00000790: 6f6b 656e 733d 6d61 785f 746f 6b65 6e73  okens=max_tokens
+000007a0: 2c0a 2020 2020 6e3d 6e2c 0a20 2020 2074  ,.    n=n,.    t
+000007b0: 656d 7065 7261 7475 7265 3d74 656d 7065  emperature=tempe
+000007c0: 7261 7475 7265 2c0a 2020 2020 4d4f 4e41  rature,.    MONA
+000007d0: 5f61 6464 6974 696f 6e61 6c5f 6461 7461  _additional_data
+000007e0: 3d7b 2263 7573 746f 6d65 725f 6964 223a  ={"customer_id":
+000007f0: 2022 4135 3331 3235 3122 7d2c 0a29 0a70   "A531251"},.).p
+00000800: 7269 6e74 2872 6573 706f 6e73 652e 6368  rint(response.ch
+00000810: 6f69 6365 735b 305d 2e74 6578 7429 0a0a  oices[0].text)..
+00000820: 2320 4173 796e 6320 7573 6167 650a 7265  # Async usage.re
+00000830: 7370 6f6e 7365 203d 2061 7379 6e63 696f  sponse = asyncio
+00000840: 2e72 756e 286d 6f6e 6974 6f72 6564 5f63  .run(monitored_c
+00000850: 6f6d 706c 6574 696f 6e2e 6163 7265 6174  ompletion.acreat
+00000860: 6528 0a20 2020 2065 6e67 696e 653d 6d6f  e(.    engine=mo
+00000870: 6465 6c2c 0a20 2020 2070 726f 6d70 743d  del,.    prompt=
+00000880: 7072 6f6d 7074 2c0a 2020 2020 6d61 785f  prompt,.    max_
+00000890: 746f 6b65 6e73 3d6d 6178 5f74 6f6b 656e  tokens=max_token
+000008a0: 732c 0a20 2020 206e 3d6e 2c0a 2020 2020  s,.    n=n,.    
+000008b0: 7465 6d70 6572 6174 7572 653d 7465 6d70  temperature=temp
+000008c0: 6572 6174 7572 652c 0a20 2020 204d 4f4e  erature,.    MON
+000008d0: 415f 6164 6469 7469 6f6e 616c 5f64 6174  A_additional_dat
+000008e0: 613d 7b22 6375 7374 6f6d 6572 5f69 6422  a={"customer_id"
+000008f0: 3a20 2241 3533 3132 3531 227d 2c0a 2929  : "A531251"},.))
+00000900: 0a0a 7072 696e 7428 7265 7370 6f6e 7365  ..print(response
+00000910: 2e63 686f 6963 6573 5b30 5d2e 7465 7874  .choices[0].text
+00000920: 290a 6060 600a 2323 2053 7570 706f 7274  ).```.## Support
+00000930: 6564 204f 7065 6e41 4920 4150 4973 0a43  ed OpenAI APIs.C
+00000940: 7572 7265 6e74 6c79 2074 6869 7320 636c  urrently this cl
+00000950: 6965 6e74 2073 7570 706f 7274 7320 606f  ient supports `o
+00000960: 7065 6e61 692e 436f 6d70 6c65 7469 6f6e  penai.Completion
+00000970: 6020 616e 6420 606f 7065 6e61 692e 4368  ` and `openai.Ch
+00000980: 6174 436f 6d70 6c65 7469 6f6e 602e 204d  atCompletion`. M
+00000990: 6f6e 6120 6361 6e20 7375 7070 6f72 7420  ona can support 
+000009a0: 7072 6f63 6573 7365 7320 6261 7365 6420  processes based 
+000009b0: 6f6e 206f 7468 6572 2041 5049 7320 616e  on other APIs an
+000009c0: 6420 616c 736f 206e 6f6e 2d4f 7065 6e41  d also non-OpenA
+000009d0: 492d 6261 7365 6420 6170 7073 2e0a 4966  I-based apps..If
+000009e0: 2079 6f75 2068 6176 6520 6120 6469 6666   you have a diff
+000009f0: 6572 7265 6e74 2075 7365 2d63 6173 652c  errent use-case,
+00000a00: 2077 6527 6420 6c6f 7665 2074 6f20 6865   we'd love to he
+00000a10: 6172 2061 626f 7574 2069 7421 2050 6c65  ar about it! Ple
+00000a20: 6173 6520 656d 6169 6c20 7573 2061 7420  ase email us at 
+00000a30: 7375 7070 6f72 7440 6d6f 6e61 6c61 6273  support@monalabs
+00000a40: 2e69 6f2e 0a0a 2323 2055 7361 6765 0a23  .io...## Usage.#
+00000a50: 2323 2049 6e69 7469 616c 697a 6174 696f  ## Initializatio
+00000a60: 6e0a 0a54 6865 206d 6169 6e20 616e 6420  n..The main and 
+00000a70: 6f6e 6c79 2066 756e 6374 696f 6e20 6578  only function ex
+00000a80: 706f 7365 6420 696e 2074 6869 7320 7061  posed in this pa
+00000a90: 636b 6167 6520 6973 2060 6d6f 6e69 746f  ckage is `monito
+00000aa0: 7260 2e0a 6060 6070 790a 696d 706f 7274  r`..```py.import
+00000ab0: 206f 7065 6e61 690a 0a66 726f 6d20 6d6f   openai..from mo
+00000ac0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
+00000ad0: 206d 6f6e 6974 6f72 0a0a 6f70 656e 6169   monitor..openai
+00000ae0: 2e61 7069 5f6b 6579 203d 2065 6e76 6972  .api_key = envir
+00000af0: 6f6e 2e67 6574 2822 4f50 454e 5f41 495f  on.get("OPEN_AI_
+00000b00: 4b45 5922 290a 0a6d 6f6e 6974 6f72 6564  KEY")..monitored
+00000b10: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
+00000b20: 6e69 746f 7228 0a20 2020 206f 7065 6e61  nitor(.    opena
+00000b30: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
+00000b40: 2020 280a 2020 2020 2020 2020 656e 7669    (.        envi
+00000b50: 726f 6e2e 6765 7428 224d 4f4e 415f 4150  ron.get("MONA_AP
+00000b60: 495f 4b45 5922 292c 0a20 2020 2020 2020  I_KEY"),.       
+00000b70: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
+00000b80: 4e41 5f53 4543 5245 5422 292c 0a20 2020  NA_SECRET"),.   
+00000b90: 2029 2c0a 2020 2020 2253 4f4d 455f 4d4f   ),.    "SOME_MO
+00000ba0: 4e49 544f 5249 4e47 5f43 4f4e 5445 5854  NITORING_CONTEXT
+00000bb0: 5f4e 414d 4522 2c0a 2020 2020 7b22 616e  _NAME",.    {"an
+00000bc0: 616c 7973 6973 223a 207b 2270 726f 6661  alysis": {"profa
+00000bd0: 6e69 7479 223a 2046 616c 7365 7d7d 0a29  nity": False}}.)
+00000be0: 0a0a 2e2e 2e0a 0a6d 6f6e 6974 6f72 6564  .......monitored
+00000bf0: 5f63 6f6d 706c 6574 696f 6e2e 6372 6561  _completion.crea
+00000c00: 7465 282e 2e2e 290a 6060 600a 0a54 6865  te(...).```..The
+00000c10: 2060 6d6f 6e69 746f 7260 2066 756e 6374   `monitor` funct
+00000c20: 696f 6e20 7265 7475 726e 7320 746f 2079  ion returns to y
+00000c30: 6f75 2061 2063 6c61 7373 2074 6861 7420  ou a class that 
+00000c40: 7772 6170 7320 7468 6520 6f72 6967 696e  wraps the origin
+00000c50: 616c 206f 7065 6e61 6920 656e 6470 6f69  al openai endpoi
+00000c60: 6e74 2063 6c61 7373 2079 6f75 2070 726f  nt class you pro
+00000c70: 7669 6465 2c20 7769 7468 2061 6e20 6571  vide, with an eq
+00000c80: 7569 7661 6c65 6e74 2041 5049 2028 6265  uivalent API (be
+00000c90: 7369 6465 7320 736f 6d65 2061 6464 6974  sides some addit
+00000ca0: 696f 6e73 206c 6973 7465 6420 6265 6c6f  ions listed belo
+00000cb0: 7729 2e0a 596f 7520 6361 6e20 7468 656e  w)..You can then
+00000cc0: 2075 7365 2074 6865 2072 6574 7572 6e65   use the returne
+00000cd0: 6420 636c 6173 7327 2022 6372 6561 7465  d class' "create
+00000ce0: 2220 616e 6420 2261 6372 6561 7465 2220  " and "acreate" 
+00000cf0: 6675 6e63 7469 6f6e 7320 6a75 7374 2061  functions just a
+00000d00: 7320 796f 7520 776f 756c 6420 6265 666f  s you would befo
+00000d10: 7265 2c20 6f6e 6c79 206e 6f77 2c20 6265  re, only now, be
+00000d20: 7369 6465 7320 6765 7474 696e 6720 7468  sides getting th
+00000d30: 6520 7265 7175 6573 7465 6420 6f70 656e  e requested open
+00000d40: 4149 2066 756e 6374 696f 6e61 6c69 7479  AI functionality
+00000d50: 2c20 7468 6973 2063 6c69 656e 7420 7769  , this client wi
+00000d60: 6c6c 206c 6f67 206f 7574 2074 6f20 4d6f  ll log out to Mo
+00000d70: 6e61 2773 2073 6572 7665 7220 7468 6520  na's server the 
+00000d80: 7061 7261 6d65 7465 7273 2079 6f75 2075  parameters you u
+00000d90: 7365 6420 2865 2e67 2e2c 2074 656d 7065  sed (e.g., tempe
+00000da0: 7261 7475 7265 292c 2064 6174 6120 6162  rature), data ab
+00000db0: 6f75 7420 7468 6520 7265 7370 6f6e 7365  out the response
+00000dc0: 2066 726f 6d20 4f70 656e 4149 2773 2073   from OpenAI's s
+00000dd0: 6572 7665 722c 2061 6e64 2063 7573 746f  erver, and custo
+00000de0: 6d20 616e 616c 7973 6573 2061 626f 7574  m analyses about
+00000df0: 2074 6865 2063 616c 6c20 2865 2e67 2e2c   the call (e.g.,
+00000e00: 2070 726f 6661 6e69 7479 2073 636f 7265   profanity score
+00000e10: 732c 2070 7269 7661 6379 2063 6865 636b  s, privacy check
+00000e20: 7320 666f 7220 656d 6169 6c73 2f70 686f  s for emails/pho
+00000e30: 6e65 206e 756d 6265 7273 2066 6f75 6e64  ne numbers found
+00000e40: 2069 6e20 7468 6520 7465 7874 732c 2074   in the texts, t
+00000e50: 6578 7475 616c 2061 6e61 6c79 7365 732c  extual analyses,
+00000e60: 2065 7463 2e2e 2e29 0a0a 5468 6520 606d   etc...)..The `m
+00000e70: 6f6e 6974 6f72 6020 6675 6e63 7469 6f6e  onitor` function
+00000e80: 2072 6563 6569 7665 7320 7468 6520 666f   receives the fo
+00000e90: 6c6c 6f77 696e 6720 6172 6775 6d65 6e74  llowing argument
+00000ea0: 733a 0a6f 7065 6e61 695f 636c 6173 733a  s:.openai_class:
+00000eb0: 2041 6e20 4f70 656e 4149 2041 5049 2063   An OpenAI API c
+00000ec0: 6c61 7373 2074 6f20 7772 6170 2077 6974  lass to wrap wit
+00000ed0: 6820 6d6f 6e69 746f 7269 6e67 2063 6170  h monitoring cap
+00000ee0: 6162 696c 7469 6573 2e0a 6d6f 6e61 5f63  abilties..mona_c
+00000ef0: 7265 6473 3a20 4120 6469 6374 2028 636f  reds: A dict (co
+00000f00: 6e74 6169 6e69 6e67 2022 6b65 7922 2061  ntaining "key" a
+00000f10: 6e64 2022 7365 6372 6574 2229 206f 7220  nd "secret") or 
+00000f20: 7061 6972 2028 7475 706c 6529 206f 6620  pair (tuple) of 
+00000f30: 4d6f 6e61 2041 5049 206b 6579 2061 6e64  Mona API key and
+00000f40: 2073 6563 7265 7420 746f 2073 6574 2075   secret to set u
+00000f50: 7020 4d6f 6e61 2773 2063 6c69 656e 7473  p Mona's clients
+00000f60: 2066 726f 6d20 6974 7320 5344 4b2e 0a63   from its SDK..c
+00000f70: 6f6e 7465 7874 5f63 6c61 7373 3a20 5468  ontext_class: Th
+00000f80: 6520 4d6f 6e61 2063 6f6e 7465 7874 2063  e Mona context c
+00000f90: 6c61 7373 206e 616d 6520 746f 2075 7365  lass name to use
+00000fa0: 2066 6f72 206d 6f6e 6974 6f72 696e 672e   for monitoring.
+00000fb0: 2055 7365 2061 2063 6f6e 7374 616e 7420   Use a constant 
+00000fc0: 6e61 6d65 206f 6620 796f 7572 2063 686f  name of your cho
+00000fd0: 6963 652e 0a73 7065 6373 3a20 4120 6469  ice..specs: A di
+00000fe0: 6374 696f 6e61 7279 206f 6620 7370 6563  ctionary of spec
+00000ff0: 6966 6963 6174 696f 6e73 2073 7563 6820  ifications such 
+00001000: 6173 206d 6f6e 6974 6f72 696e 6720 7361  as monitoring sa
+00001010: 6d70 6c69 6e67 2072 6174 696f 2e0a 0a23  mpling ratio...#
+00001020: 2323 2320 5370 6563 730a 5468 6520 7370  ### Specs.The sp
+00001030: 6563 7320 6172 6720 616c 6c6f 7773 2079  ecs arg allows y
+00001040: 6f75 2074 6f20 636f 6e66 6967 7572 6520  ou to configure 
+00001050: 7768 6174 2073 686f 756c 6420 6265 206d  what should be m
+00001060: 6f6e 6974 6f72 6564 2e20 4974 2065 7870  onitored. It exp
+00001070: 6563 7473 2061 2070 7974 686f 6e20 6469  ects a python di
+00001080: 6374 2077 6974 6820 7468 6520 666f 6c6c  ct with the foll
+00001090: 776f 696e 6720 706f 7373 6962 6c65 206b  woing possible k
+000010a0: 6579 733a 0a2a 2073 616d 706c 696e 675f  eys:.* sampling_
+000010b0: 7261 7469 6f20 2831 293a 2041 206e 756d  ratio (1): A num
+000010c0: 6265 7220 6265 7477 6565 6e20 3020 616e  ber between 0 an
+000010d0: 6420 3120 666f 7220 686f 7720 6f66 7465  d 1 for how ofte
+000010e0: 6e20 7368 6f75 6c64 2074 6865 2063 616c  n should the cal
+000010f0: 6c20 6265 206c 6f67 6765 642e 0a2a 2061  l be logged..* a
+00001100: 766f 6964 5f6d 6f6e 6974 6f72 696e 675f  void_monitoring_
+00001110: 6578 6365 7074 696f 6e73 2028 4661 6c73  exceptions (Fals
+00001120: 6529 3a20 5768 6574 6865 7220 6f72 206e  e): Whether or n
+00001130: 6f74 2074 6f20 6c6f 6720 6f75 7420 746f  ot to log out to
+00001140: 204d 6f6e 6120 7768 656e 2074 6865 7265   Mona when there
+00001150: 2069 7320 616e 204f 7065 6e41 4920 6578   is an OpenAI ex
+00001160: 6365 7074 696f 6e2e 2044 6566 6175 6c74  ception. Default
+00001170: 2069 7320 746f 2074 7261 636b 2065 7863   is to track exc
+00001180: 6570 7469 6f6e 7320 2d20 616e 6420 4d6f  eptions - and Mo
+00001190: 6e61 2077 696c 6c20 616c 6572 7420 796f  na will alert yo
+000011a0: 7520 6f6e 2074 6869 6e67 7320 6c69 6b65  u on things like
+000011b0: 2061 206a 756d 7020 696e 206e 756d 6265   a jump in numbe
+000011c0: 7220 6f66 2065 7863 6570 7469 6f6e 730a  r of exceptions.
+000011d0: 2a20 6578 706f 7274 5f70 726f 6d70 7420  * export_prompt 
+000011e0: 2846 616c 7365 293a 2057 6865 7468 6572  (False): Whether
+000011f0: 204d 6f6e 6120 7368 6f75 6c64 2065 7870   Mona should exp
+00001200: 6f72 7420 7468 6520 6163 7475 616c 2070  ort the actual p
+00001210: 726f 6d70 7420 7465 7874 2e20 4265 2064  rompt text. Be d
+00001220: 6566 6175 6c74 2073 6574 2074 6f20 4661  efault set to Fa
+00001230: 6c73 6520 746f 2061 766f 6964 2070 7269  lse to avoid pri
+00001240: 7661 6379 2063 6f6e 6365 726e 732e 0a2a  vacy concerns..*
+00001250: 2065 7870 6f72 745f 7265 7370 6f6e 7365   export_response
+00001260: 5f74 6578 7473 2028 4661 6c73 6529 3a20  _texts (False): 
+00001270: 5768 6574 6865 7220 4d6f 6e61 2073 686f  Whether Mona sho
+00001280: 756c 6420 6578 706f 7274 2074 6865 2061  uld export the a
+00001290: 6374 7561 6c20 7265 7370 6f6e 7365 2074  ctual response t
+000012a0: 6578 7473 2e20 4265 2064 6566 6175 6c74  exts. Be default
+000012b0: 2073 6574 2074 6f20 4661 6c73 6520 746f   set to False to
+000012c0: 2061 766f 6964 2070 7269 7661 6379 2063   avoid privacy c
+000012d0: 6f6e 6365 726e 732e 0a2a 2061 6e61 6c79  oncerns..* analy
+000012e0: 7369 733a 2041 2064 6963 7469 6f6e 6172  sis: A dictionar
+000012f0: 7920 6d61 7070 696e 6720 6561 6368 2061  y mapping each a
+00001300: 6e61 6c79 7369 7320 7479 7065 2074 6f20  nalysis type to 
+00001310: 6120 626f 6f6c 6561 6e20 7661 6c75 6520  a boolean value 
+00001320: 7465 6c6c 696e 6720 7468 6520 636c 6965  telling the clie
+00001330: 6e74 2077 6865 7468 6572 206f 7220 6e6f  nt whether or no
+00001340: 7420 746f 2072 756e 2073 6169 6420 616e  t to run said an
+00001350: 616c 7973 6973 2061 6e64 206c 6f67 2069  alysis and log i
+00001360: 7420 746f 204d 6f6e 612e 2050 6f73 7369  t to Mona. Possi
+00001370: 626c 6520 6f70 7469 6f6e 7320 6375 7272  ble options curr
+00001380: 656e 746c 7920 6172 6520 2270 7269 7661  ently are "priva
+00001390: 6379 222c 2022 7072 6f66 616e 6974 7922  cy", "profanity"
+000013a0: 2c20 616e 6420 2274 6578 7475 616c 222e  , and "textual".
+000013b0: 2042 7920 6465 6661 756c 742c 2061 6c6c   By default, all
+000013c0: 2061 6e61 6c79 7365 7320 7461 6b65 2070   analyses take p
+000013d0: 6c61 6365 2061 6e64 2061 7265 206c 6f67  lace and are log
+000013e0: 6765 6420 6f75 7420 746f 204d 6f6e 612e  ged out to Mona.
+000013f0: 0a0a 2323 2320 4361 7061 6269 6c69 7469  ..### Capabiliti
+00001400: 6573 2064 7572 696e 6720 4150 4920 6361  es during API ca
+00001410: 6c6c 730a 0a41 6674 6572 2077 7261 7070  lls..After wrapp
+00001420: 696e 6720 796f 7572 2065 6e64 706f 696e  ing your endpoin
+00001430: 7420 7769 7468 2060 6d6f 6e69 746f 7260  t with `monitor`
+00001440: 2c20 796f 7520 7265 616c 6c79 2064 6f6e  , you really don
+00001450: 2774 206e 6565 6420 746f 2064 6f20 616e  't need to do an
+00001460: 7974 6869 6e67 2065 6c73 652e 2057 6865  ything else. Whe
+00001470: 6e20 7573 696e 6720 6063 7265 6174 6560  n using `create`
+00001480: 206f 7220 6061 6372 6561 7465 6020 6461   or `acreate` da
+00001490: 7461 2077 696c 6c20 6265 2074 7261 636b  ta will be track
+000014a0: 6564 2061 6e64 206d 6f6e 6974 6f72 696e  ed and monitorin
+000014b0: 6720 7769 6c6c 2074 616b 6520 706c 6163  g will take plac
+000014c0: 652e 0a0a 5468 6572 6520 6172 652c 2068  e...There are, h
+000014d0: 6f77 6576 6572 2c20 7365 7665 7261 6c20  owever, several 
+000014e0: 6361 7061 6269 6c69 7469 6573 2074 6861  capabilities tha
+000014f0: 7420 6172 6520 6164 6465 6420 746f 2074  t are added to t
+00001500: 6865 7365 2066 756e 6374 696f 6e73 2e20  hese functions. 
+00001510: 5370 6563 6966 6963 616c 6c79 2c20 796f  Specifically, yo
+00001520: 7520 6361 6e20 6164 6420 7468 6520 666f  u can add the fo
+00001530: 6c6c 6f77 696e 6720 6172 6775 6d65 6e74  llowing argument
+00001540: 7320 746f 2061 6e79 2063 7265 6174 6520  s to any create 
+00001550: 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63 6f6e  call:.* MONA_con
+00001560: 7465 7874 5f69 643a 2054 6865 2075 6e69  text_id: The uni
+00001570: 7175 6520 6964 206f 6620 7468 6520 636f  que id of the co
+00001580: 6e74 6578 7420 696e 2077 6869 6368 2074  ntext in which t
+00001590: 6865 2063 616c 6c20 6973 206d 6164 652e  he call is made.
+000015a0: 2042 7920 7573 696e 6720 7468 6973 2049   By using this I
+000015b0: 4420 796f 7520 6361 6e20 6578 706f 7274  D you can export
+000015c0: 206d 6f72 6520 6461 7461 2074 6f20 4d6f   more data to Mo
+000015d0: 6e61 2074 6f20 7468 6520 7361 6d65 2063  na to the same c
+000015e0: 6f6e 7465 7874 2066 726f 6d20 6f74 6865  ontext from othe
+000015f0: 7220 706c 6163 6573 2e20 4966 206e 6f74  r places. If not
+00001600: 2073 7570 706c 6965 642c 2074 6865 2022   supplied, the "
+00001610: 6964 2220 6669 656c 6420 6f66 2074 6865  id" field of the
+00001620: 204f 7065 6e41 4920 456e 6470 6f69 6e74   OpenAI Endpoint
+00001630: 2773 2072 6573 706f 6e73 6520 7769 6c6c  's response will
+00001640: 2062 6520 7573 6564 2061 7320 7468 6520   be used as the 
+00001650: 4d6f 6e61 2063 6f6e 7465 7874 2049 4420  Mona context ID 
+00001660: 6175 746f 6d61 7469 6361 6c6c 792e 0a2a  automatically..*
+00001670: 204d 4f4e 415f 6578 706f 7274 5f74 696d   MONA_export_tim
+00001680: 6573 7461 6d70 3a20 4361 6e20 6265 2075  estamp: Can be u
+00001690: 7365 6420 746f 2073 696d 756c 6174 6520  sed to simulate 
+000016a0: 6173 2069 6620 7468 6520 6375 7272 656e  as if the curren
+000016b0: 7420 6361 6c6c 2077 6173 206d 6164 6520  t call was made 
+000016c0: 696e 2061 2064 6966 6665 7265 6e74 2074  in a different t
+000016d0: 696d 652c 2061 7320 6661 7220 6173 204d  ime, as far as M
+000016e0: 6f6e 6120 6973 2063 6f6e 6365 726e 6564  ona is concerned
+000016f0: 2e0a 2a20 4d4f 4e41 5f61 6464 6974 696f  ..* MONA_additio
+00001700: 6e61 6c5f 6461 7461 3a20 4120 4a53 4f4e  nal_data: A JSON
+00001710: 2d73 6572 6961 6c69 7a61 626c 6520 6469  -serializable di
+00001720: 6374 2077 6974 6820 616e 7920 6f74 6865  ct with any othe
+00001730: 7220 6461 7461 2079 6f75 2077 616e 7420  r data you want 
+00001740: 746f 2061 6464 2074 6f20 7468 6520 6d6f  to add to the mo
+00001750: 6e69 746f 7269 6e67 2063 6f6e 7465 7874  nitoring context
+00001760: 2e20 5468 6973 2063 6f6d 6573 2069 6e20  . This comes in 
+00001770: 6861 6e64 7920 6966 2079 6f75 2077 616e  handy if you wan
+00001780: 7420 746f 2061 6464 206d 6f72 6520 696e  t to add more in
+00001790: 666f 726d 6174 696f 6e20 746f 2074 6865  formation to the
+000017a0: 206d 6f6e 6974 6f72 696e 6720 636f 6e74   monitoring cont
+000017b0: 6578 2074 6861 7420 6973 6e27 7420 7061  ex that isn't pa
+000017c0: 7274 206f 6620 7468 6520 6261 7369 6320  rt of the basic 
+000017d0: 4f70 656e 4149 2041 5049 2063 616c 6c20  OpenAI API call 
+000017e0: 696e 666f 726d 6174 696f 6e2e 2046 6f72  information. For
+000017f0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
+00001800: 2061 7265 2075 7369 6e67 2061 2073 7065   are using a spe
+00001810: 6369 6669 6320 7465 6d70 6c61 7465 2049  cific template I
+00001820: 4420 6f72 2069 6620 7468 6973 2063 616c  D or if this cal
+00001830: 6c20 6973 2062 6569 6e67 206d 6164 6520  l is being made 
+00001840: 666f 7220 6120 7370 6563 6966 6963 2063  for a specific c
+00001850: 7573 746f 6d65 7220 4944 2c20 7468 6573  ustomer ID, thes
+00001860: 6520 6172 6520 6669 656c 6473 2079 6f75  e are fields you
+00001870: 2063 616e 2061 6464 2074 6865 7265 2074   can add there t
+00001880: 6f20 6865 6c70 2067 6574 2066 756c 6c20  o help get full 
+00001890: 636f 6e74 6578 7420 7768 656e 206d 6f6e  context when mon
+000018a0: 6974 6f72 696e 6720 7769 7468 204d 6f6e  itoring with Mon
+000018b0: 612e 0a0a 4578 616d 706c 653a 0a60 6060  a...Example:.```
+000018c0: 7079 0a72 6573 706f 6e73 6520 3d20 6173  py.response = as
+000018d0: 796e 6369 6f2e 7275 6e28 6d6f 6e69 746f  yncio.run(monito
+000018e0: 7265 645f 636f 6d70 6c65 7469 6f6e 2e61  red_completion.a
+000018f0: 6372 6561 7465 280a 2020 2020 656e 6769  create(.    engi
+00001900: 6e65 3d6d 6f64 656c 2c0a 2020 2020 7072  ne=model,.    pr
+00001910: 6f6d 7074 3d70 726f 6d70 742c 0a20 2020  ompt=prompt,.   
+00001920: 206d 6178 5f74 6f6b 656e 733d 6d61 785f   max_tokens=max_
+00001930: 746f 6b65 6e73 2c0a 2020 2020 6e3d 6e2c  tokens,.    n=n,
+00001940: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
+00001950: 3d74 656d 7065 7261 7475 7265 2c0a 2020  =temperature,.  
+00001960: 2020 4d4f 4e41 5f61 6464 6974 696f 6e61    MONA_additiona
+00001970: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
+00001980: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
+00001990: 7d2c 0a29 290a 7072 696e 7428 7265 7370  },.)).print(resp
+000019a0: 6f6e 7365 2e63 686f 6963 6573 5b30 5d2e  onse.choices[0].
+000019b0: 7465 7874 290a 6060 600a 0a23 2323 2055  text).```..### U
+000019c0: 7369 6e67 204f 7065 6e41 4920 7769 7468  sing OpenAI with
+000019d0: 2052 4553 5420 6361 6c6c 7320 696e 7374   REST calls inst
+000019e0: 6561 6420 6f66 204f 7065 6e41 4927 7320  ead of OpenAI's 
+000019f0: 5079 7468 6f6e 2063 6c69 656e 740a 496e  Python client.In
+00001a00: 2073 6f6d 6520 6361 7365 7320 796f 7520   some cases you 
+00001a10: 6d61 7920 6368 6f6f 7365 2074 6f20 7573  may choose to us
+00001a20: 6520 4f70 656e 4149 2773 2041 5049 2064  e OpenAI's API d
+00001a30: 6972 6563 746c 7920 7769 7468 2052 4553  irectly with RES
+00001a40: 5420 6361 6c6c 7320 616e 6420 6e6f 7420  T calls and not 
+00001a50: 7573 696e 6720 4f70 656e 4149 2773 2053  using OpenAI's S
+00001a60: 444b 2e20 466f 7220 7468 6573 6520 6361  DK. For these ca
+00001a70: 7365 7320 7765 2061 6c6c 6f77 2061 206d  ses we allow a m
+00001a80: 6f72 6520 6469 7265 6374 2061 7070 726f  ore direct appro
+00001a90: 6163 6820 666f 7220 6c6f 6767 696e 6720  ach for logging 
+00001aa0: 746f 204d 6f6e 6120 6173 2077 656c 6c2c  to Mona as well,
+00001ab0: 2062 7920 7573 696e 6720 7468 6520 2267   by using the "g
+00001ac0: 6574 5f72 6573 745f 6d6f 6e69 746f 7222  et_rest_monitor"
+00001ad0: 2066 756e 6374 696f 6e2e 2053 6565 2065   function. See e
+00001ae0: 7861 6d70 6c65 2062 656c 6f77 2e0a 0a60  xample below...`
+00001af0: 6060 7079 0a23 2044 6972 6563 7420 5245  ``py.# Direct RE
+00001b00: 5354 2075 7361 6765 2c20 7769 7468 6f75  ST usage, withou
+00001b10: 7420 4f70 656e 4149 2063 6c69 656e 740a  t OpenAI client.
+00001b20: 696d 706f 7274 2072 6571 7565 7374 730a  import requests.
+00001b30: 6672 6f6d 206f 7320 696d 706f 7274 2065  from os import e
+00001b40: 6e76 6972 6f6e 0a66 726f 6d20 6d6f 6e61  nviron.from mona
+00001b50: 5f6f 7065 6e61 6920 696d 706f 7274 2067  _openai import g
+00001b60: 6574 5f72 6573 745f 6d6f 6e69 746f 720a  et_rest_monitor.
+00001b70: 0a0a 4d4f 4e41 5f41 5049 5f4b 4559 203d  ..MONA_API_KEY =
+00001b80: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
+00001b90: 4e41 5f41 5049 5f4b 4559 2229 0a4d 4f4e  NA_API_KEY").MON
+00001ba0: 415f 5345 4352 4554 203d 2065 6e76 6972  A_SECRET = envir
+00001bb0: 6f6e 2e67 6574 2822 4d4f 4e41 5f53 4543  on.get("MONA_SEC
+00001bc0: 5245 5422 290a 4d4f 4e41 5f43 5245 4453  RET").MONA_CREDS
+00001bd0: 203d 207b 0a20 2020 2022 6b65 7922 3a20   = {.    "key": 
+00001be0: 4d4f 4e41 5f41 5049 5f4b 4559 2c0a 2020  MONA_API_KEY,.  
+00001bf0: 2020 2273 6563 7265 7422 3a20 4d4f 4e41    "secret": MONA
+00001c00: 5f53 4543 5245 542c 0a7d 0a43 4f4e 5445  _SECRET,.}.CONTE
+00001c10: 5854 5f43 4c41 5353 5f4e 414d 4520 3d20  XT_CLASS_NAME = 
+00001c20: 2253 4f4d 455f 4d4f 4e49 544f 5249 4e47  "SOME_MONITORING
+00001c30: 5f43 4f4e 5445 5854 5f4e 414d 4522 0a0a  _CONTEXT_NAME"..
+00001c40: 2320 4765 7420 4d6f 6e61 206c 6f67 6765  # Get Mona logge
+00001c50: 720a 6d6f 6e61 5f6c 6f67 6765 7220 3d20  r.mona_logger = 
+00001c60: 6765 745f 7265 7374 5f6d 6f6e 6974 6f72  get_rest_monitor
+00001c70: 280a 2020 2020 2243 6f6d 706c 6574 696f  (.    "Completio
+00001c80: 6e22 2c0a 2020 2020 4d4f 4e41 5f43 5245  n",.    MONA_CRE
+00001c90: 4453 2c0a 2020 2020 434f 4e54 4558 545f  DS,.    CONTEXT_
+00001ca0: 434c 4153 535f 4e41 4d45 2c0a 290a 0a23  CLASS_NAME,.)..#
+00001cb0: 2053 6574 2075 7020 7468 6520 4150 4920   Set up the API 
+00001cc0: 656e 6470 6f69 6e74 2055 524c 2061 6e64  endpoint URL and
+00001cd0: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+00001ce0: 6865 6164 6572 730a 7572 6c20 3d20 2268  headers.url = "h
+00001cf0: 7474 7073 3a2f 2f61 7069 2e6f 7065 6e61  ttps://api.opena
+00001d00: 692e 636f 6d2f 7631 2f63 6f6d 706c 6574  i.com/v1/complet
+00001d10: 696f 6e73 220a 6865 6164 6572 7320 3d20  ions".headers = 
+00001d20: 7b0a 2020 2020 2243 6f6e 7465 6e74 2d54  {.    "Content-T
+00001d30: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
+00001d40: 6f6e 2f6a 736f 6e22 2c0a 2020 2020 2241  on/json",.    "A
+00001d50: 7574 686f 7269 7a61 7469 6f6e 223a 2066  uthorization": f
+00001d60: 2242 6561 7265 7220 7b65 6e76 6972 6f6e  "Bearer {environ
+00001d70: 2e67 6574 2827 4f50 454e 5f41 495f 4b45  .get('OPEN_AI_KE
+00001d80: 5927 297d 222c 0a7d 0a0a 2320 5365 7420  Y')}",.}..# Set 
+00001d90: 7570 2074 6865 2072 6571 7565 7374 2064  up the request d
+00001da0: 6174 610a 6461 7461 203d 207b 0a20 2020  ata.data = {.   
+00001db0: 2022 7072 6f6d 7074 223a 2070 726f 6d70   "prompt": promp
+00001dc0: 742c 0a20 2020 2022 6d61 785f 746f 6b65  t,.    "max_toke
+00001dd0: 6e73 223a 206d 6178 5f74 6f6b 656e 732c  ns": max_tokens,
+00001de0: 0a20 2020 2022 7465 6d70 6572 6174 7572  .    "temperatur
+00001df0: 6522 3a20 7465 6d70 6572 6174 7572 652c  e": temperature,
+00001e00: 0a20 2020 2022 6d6f 6465 6c22 3a20 6d6f  .    "model": mo
+00001e10: 6465 6c2c 0a20 2020 2022 6e22 3a20 6e2c  del,.    "n": n,
+00001e20: 0a7d 0a0a 2320 5468 6520 6c6f 675f 7265  .}..# The log_re
+00001e30: 7175 6573 7420 6675 6e63 7469 6f6e 2072  quest function r
+00001e40: 6574 7572 6e73 2074 776f 206f 7468 6572  eturns two other
+00001e50: 2066 756e 6374 696f 6e20 666f 7220 6c61   function for la
+00001e60: 7465 7220 6c6f 6767 696e 670a 2320 7468  ter logging.# th
+00001e70: 6520 7265 7370 6f6e 7365 206f 7220 7468  e response or th
+00001e80: 6520 6578 6365 7074 696f 6e2e 2057 6865  e exception. Whe
+00001e90: 6e20 7765 206c 6174 6572 2064 6f20 7468  n we later do th
+00001ea0: 6174 2c20 7468 6520 6c6f 6767 6572 2077  at, the logger w
+00001eb0: 696c 6c0a 2320 6163 7475 616c 6c79 2063  ill.# actually c
+00001ec0: 616c 6375 6c61 7465 2061 6c6c 2074 6865  alculate all the
+00001ed0: 2072 656c 6576 616e 7420 6d65 7472 6963   relevant metric
+00001ee0: 7320 616e 6420 7769 6c6c 2073 656e 6420  s and will send 
+00001ef0: 7468 656d 2074 6f0a 2320 4d6f 6e61 2e0a  them to.# Mona..
+00001f00: 7265 7370 6f6e 7365 5f6c 6f67 6765 722c  response_logger,
+00001f10: 2065 7863 6570 7469 6f6e 5f6c 6f67 6765   exception_logge
+00001f20: 7220 3d20 6d6f 6e61 5f6c 6f67 6765 722e  r = mona_logger.
+00001f30: 6c6f 675f 7265 7175 6573 7428 0a20 2020  log_request(.   
+00001f40: 2064 6174 612c 2061 6464 6974 696f 6e61   data, additiona
+00001f50: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
+00001f60: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
+00001f70: 7d0a 290a 0a74 7279 3a0a 2020 2020 2320  }.)..try:.    # 
+00001f80: 5365 6e64 2074 6865 2072 6571 7565 7374  Send the request
+00001f90: 2074 6f20 7468 6520 4150 490a 2020 2020   to the API.    
+00001fa0: 7265 7370 6f6e 7365 203d 2072 6571 7565  response = reque
+00001fb0: 7374 732e 706f 7374 2875 726c 2c20 6865  sts.post(url, he
+00001fc0: 6164 6572 733d 6865 6164 6572 732c 206a  aders=headers, j
+00001fd0: 736f 6e3d 6461 7461 290a 0a20 2020 2023  son=data)..    #
+00001fe0: 2043 6865 636b 2066 6f72 2048 5454 5020   Check for HTTP 
+00001ff0: 6572 726f 7273 0a20 2020 2072 6573 706f  errors.    respo
+00002000: 6e73 652e 7261 6973 655f 666f 725f 7374  nse.raise_for_st
+00002010: 6174 7573 2829 0a0a 2020 2020 2320 4c6f  atus()..    # Lo
+00002020: 6720 7265 7370 6f6e 7365 2074 6f20 4d6f  g response to Mo
+00002030: 6e61 0a20 2020 2072 6573 706f 6e73 655f  na.    response_
+00002040: 6c6f 6767 6572 2872 6573 706f 6e73 652e  logger(response.
+00002050: 6a73 6f6e 2829 290a 2020 2020 7072 696e  json()).    prin
+00002060: 7428 7265 7370 6f6e 7365 2e6a 736f 6e28  t(response.json(
+00002070: 295b 2263 686f 6963 6573 225d 5b30 5d5b  )["choices"][0][
+00002080: 2274 6578 7422 5d29 0a0a 6578 6365 7074  "text"])..except
+00002090: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
+000020a0: 723a 0a20 2020 2023 204c 6f67 2065 7863  r:.    # Log exc
+000020b0: 6570 7469 6f6e 2074 6f20 4d6f 6e61 0a20  eption to Mona. 
+000020c0: 2020 2065 7863 6570 7469 6f6e 5f6c 6f67     exception_log
+000020d0: 6765 7228 290a 6060 600a 0a23 2323 2053  ger().```..### S
+000020e0: 7472 6561 6d20 7375 7070 6f72 740a 0a4f  tream support..O
+000020f0: 7065 6e41 4920 616c 6c6f 7773 2072 6563  penAI allows rec
+00002100: 6569 7669 6e67 2072 6573 706f 6e73 6573  eiving responses
+00002110: 2061 7320 6120 7374 7265 616d 206f 6620   as a stream of 
+00002120: 746f 6b65 6e73 2075 7369 6e67 2074 6865  tokens using the
+00002130: 2022 7374 7265 616d 2220 7061 7261 6d65   "stream" parame
+00002140: 7465 722e 2057 6865 6e20 7468 6973 2069  ter. When this i
+00002150: 7320 646f 6e65 2c20 4d6f 6e61 2077 696c  s done, Mona wil
+00002160: 6c20 636f 6c6c 6563 7420 616c 6c20 7468  l collect all th
+00002170: 6520 746f 6b65 6e73 2069 6e20 6d65 6d6f  e tokens in memo
+00002180: 7279 2061 6e64 2077 696c 6c20 6372 6561  ry and will crea
+00002190: 7465 2074 6865 2061 6e61 6c79 7369 7320  te the analysis 
+000021a0: 616e 6420 6c6f 6720 6f75 7420 7468 6520  and log out the 
+000021b0: 6461 7461 2074 6865 206d 6f6d 656e 7420  data the moment 
+000021c0: 7468 6520 7374 7265 616d 2069 7320 6f76  the stream is ov
+000021d0: 6572 2e20 596f 7520 646f 6e27 7420 6e65  er. You don't ne
+000021e0: 6564 2074 6f20 646f 2061 6e79 7468 696e  ed to do anythin
+000021f0: 6720 746f 206d 616b 6520 7468 6973 2068  g to make this h
+00002200: 6170 7065 6e2e 0a0a 5369 6e63 6520 666f  appen...Since fo
+00002210: 7220 7374 7265 616d 696e 6720 7265 7370  r streaming resp
+00002220: 6f6e 7365 7320 4f70 656e 4149 2064 6f65  onses OpenAI doe
+00002230: 736e 2774 2073 7570 706c 7920 7468 6520  sn't supply the 
+00002240: 6675 6c6c 2075 7361 6765 2074 6f6b 656e  full usage token
+00002250: 7320 7375 6d6d 6172 792c 204d 6f6e 6120  s summary, Mona 
+00002260: 7573 6573 2074 6865 2074 696b 746f 6b65  uses the tiktoke
+00002270: 6e20 7061 636b 6167 6520 746f 2063 616c  n package to cal
+00002280: 6375 6c61 7465 2074 6865 2074 6f6b 656e  culate the token
+00002290: 7320 6f66 2074 6865 2070 726f 6d70 7420  s of the prompt 
+000022a0: 616e 6420 636f 6d70 6c65 7469 6f6e 2061  and completion a
+000022b0: 6e64 206c 6f67 2074 6865 6d20 666f 7220  nd log them for 
+000022c0: 6d6f 6e69 746f 7269 6e67 2e0a 0a4e 4f54  monitoring...NOT
+000022d0: 453a 2053 7472 6561 6d20 6973 2063 7572  E: Stream is cur
+000022e0: 7265 6e74 6c79 206f 6e6c 7920 7375 7070  rently only supp
+000022f0: 6f72 7465 6420 7769 7468 2053 444b 2075  orted with SDK u
+00002300: 7361 6765 2c20 616e 6420 6e6f 7420 7769  sage, and not wi
+00002310: 7468 2075 7369 6e67 2052 4553 5420 6469  th using REST di
+00002320: 7265 6374 6c79 2e0a 0a23 2320 4c61 6e67  rectly...## Lang
+00002330: 4368 6169 6e20 7375 7070 6f72 740a 0a59  Chain support..Y
+00002340: 6f75 2063 616e 2075 7365 2074 6865 2065  ou can use the e
+00002350: 7870 6f72 7465 6420 606d 6f6e 6974 6f72  xported `monitor
+00002360: 5f6c 616e 6763 6861 696e 5f6c 6c6d 6020  _langchain_llm` 
+00002370: 746f 2077 7261 7020 6120 4c61 6e67 4368  to wrap a LangCh
+00002380: 6169 6e20 4f70 656e 4149 204c 4c4d 2028  ain OpenAI LLM (
+00002390: 6368 6174 206f 7220 6e6f 726d 616c 2920  chat or normal) 
+000023a0: 7769 7468 204d 6f6e 6127 7320 6d6f 6e69  with Mona's moni
+000023b0: 746f 7269 6e67 2063 6170 6162 696c 6974  toring capabilit
+000023c0: 6965 733a 0a0a 6060 6070 790a 6672 6f6d  ies:..```py.from
+000023d0: 206d 6f6e 615f 6f70 656e 6169 2069 6d70   mona_openai imp
+000023e0: 6f72 7420 6d6f 6e69 746f 725f 6c61 6e67  ort monitor_lang
+000023f0: 6368 6169 6e5f 6c6c 6d0a 0a66 726f 6d20  chain_llm..from 
+00002400: 6c61 6e67 6368 6169 6e2e 6c6c 6d73 2069  langchain.llms i
+00002410: 6d70 6f72 7420 4f70 656e 4149 0a0a 2320  mport OpenAI..# 
+00002420: 5772 6170 2074 6865 204c 4c4d 206f 626a  Wrap the LLM obj
+00002430: 6563 7420 7769 7468 204d 6f6e 6120 6d6f  ect with Mona mo
+00002440: 6e69 746f 7269 6e67 2e0a 6c6c 6d20 3d20  nitoring..llm = 
+00002450: 6d6f 6e69 746f 725f 6c61 6e67 6368 6169  monitor_langchai
+00002460: 6e5f 6c6c 6d28 0a20 2020 204f 7065 6e41  n_llm(.    OpenA
+00002470: 4928 4f50 454e 5f41 495f 4b45 5929 2c0a  I(OPEN_AI_KEY),.
+00002480: 2020 2020 4d4f 4e41 5f43 5245 4453 2c0a      MONA_CREDS,.
+00002490: 2020 2020 434f 4e54 4558 545f 434c 4153      CONTEXT_CLAS
+000024a0: 535f 4e41 4d45 290a 6060 600a 0a53 6565  S_NAME).```..See
+000024b0: 2066 756c 6c20 6578 616d 706c 6520 696e   full example in
+000024c0: 2063 6f6d 706c 6574 696f 6e5f 6c61 6e67   completion_lang
+000024d0: 6368 6169 6e2e 7079 2069 6e20 7468 6520  chain.py in the 
+000024e0: 6578 616d 706c 6573 2066 6f6c 6465 722e  examples folder.
+000024f0: 0a0a 2323 204d 6f6e 6120 5344 4b0a 0a54  ..## Mona SDK..T
+00002500: 6869 7320 7061 636b 6167 6520 7573 6573  his package uses
+00002510: 2074 6865 206d 6f6e 615f 7364 6b20 7061   the mona_sdk pa
+00002520: 636b 6167 6520 746f 2065 7870 6f72 7420  ckage to export 
+00002530: 7468 6520 7265 6c65 7661 6e74 2064 6174  the relevant dat
+00002540: 6120 746f 204d 6f6e 612e 2054 6865 7265  a to Mona. There
+00002550: 2061 7265 2073 6576 6572 616c 2065 6e76   are several env
+00002560: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00002570: 6573 2079 6f75 2063 616e 2075 7365 2074  es you can use t
+00002580: 6f20 636f 6e66 6967 7572 6520 7468 6520  o configure the 
+00002590: 5344 4b27 7320 6265 6861 7669 6f72 2e20  SDK's behavior. 
+000025a0: 466f 7220 6578 616d 706c 652c 2079 6f75  For example, you
+000025b0: 2063 616e 2073 6574 2069 7420 7570 2074   can set it up t
+000025c0: 6f20 7261 6973 6520 6578 6365 7074 696f  o raise exceptio
+000025d0: 6e73 2077 6865 6e20 6578 706f 7274 696e  ns when exportin
+000025e0: 6720 6461 7461 2074 6f20 4d6f 6e61 2066  g data to Mona f
+000025f0: 6169 6c73 2028 6974 2064 6f65 736e 2774  ails (it doesn't
+00002600: 2064 6f20 7468 6174 2062 7920 6465 6661   do that by defa
+00002610: 756c 7429 2e0a 0a23 2320 4d6f 6e69 746f  ult)...## Monito
+00002620: 7269 6e67 2066 6f72 2070 726f 6661 6e69  ring for profani
+00002630: 7479 0a0a 4d6f 6e61 2075 7365 7320 7468  ty..Mona uses th
+00002640: 6520 616c 742d 7072 6f66 616e 6974 792d  e alt-profanity-
+00002650: 6368 6563 6b20 7061 6361 6b67 6520 2868  check pacakge (h
+00002660: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00002670: 7072 6f6a 6563 742f 616c 742d 7072 6f66  project/alt-prof
+00002680: 616e 6974 792d 6368 6563 6b2f 2920 746f  anity-check/) to
+00002690: 2063 7265 6174 6520 626f 7468 2062 6f6f   create both boo
+000026a0: 6c65 616e 2070 7265 6469 6374 696f 6e73  lean predictions
+000026b0: 2061 6e64 2070 726f 6261 6269 6c74 7920   and probabilty 
+000026c0: 7363 6f72 6573 2066 6f72 2074 6865 2065  scores for the e
+000026d0: 7869 7374 656e 6365 206f 6620 7072 6f66  xistence of prof
+000026e0: 616e 6974 7920 626f 7468 2069 6e20 7468  anity both in th
+000026f0: 6520 7072 6f6d 7074 2061 6e64 2069 6e20  e prompt and in 
+00002700: 7468 6520 7265 7370 6f6e 7365 732e 2057  the responses. W
+00002710: 6520 7573 6520 7468 6520 6275 696c 7420  e use the built 
+00002720: 696e 2070 6163 6b61 6765 206d 6574 686f  in package metho
+00002730: 6473 2066 6f72 2074 6861 742e 2049 6620  ds for that. If 
+00002740: 796f 7520 7761 6e74 2c20 666f 7220 6578  you want, for ex
+00002750: 616d 706c 652c 2074 6f20 7573 6520 6120  ample, to use a 
+00002760: 6469 6666 6572 656e 7420 7072 6f62 6162  different probab
+00002770: 696c 6974 7920 7468 7265 7368 6f6c 6420  ility threshold 
+00002780: 666f 7220 7468 6520 626f 6f6c 6561 6e20  for the boolean 
+00002790: 7072 6564 6963 7469 6f6e 2c20 796f 7520  prediction, you 
+000027a0: 6361 6e20 646f 2074 6861 7420 6279 2063  can do that by c
+000027b0: 6861 6e67 696e 6720 796f 7572 204d 6f6e  hanging your Mon
+000027c0: 6120 636f 6e66 6967 206f 6e20 7468 6520  a config on the 
+000027d0: 4d6f 6e61 2064 6173 6862 6f61 7264 2e0a  Mona dashboard..
```

### Comparing `mona-openai-0.0.7/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.8/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/pyproject.toml` & `mona-openai-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mona-openai-0.0.7/tests/test_chat_completion.py` & `mona-openai-0.0.8/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/tests/test_completion.py` & `mona-openai-0.0.8/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/tests/test_privacy_analyzer.py` & `mona-openai-0.0.8/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.7/tests/test_textual_analyzer.py` & `mona-openai-0.0.8/tests/test_textual_analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 
 def test_get_preposition_ratio():
     text = "bla balskdf of nblaskd from there"
     assert TextualAnalyzer(text).get_preposition_ratio() == 2 / 6
 
 
+def test_get_preposition_ratio_no_words():
+    text = "  "
+    assert TextualAnalyzer(text).get_preposition_ratio() == 0
+
+
 def test_new_words():
     assert (
         TextualAnalyzer("this is a word").get_words_not_in_others_count(
             (
                 TextualAnalyzer("has this word"),
                 TextualAnalyzer("no bla bla is"),
             )
```

