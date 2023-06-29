# Comparing `tmp/cns-1.0.37-py3-none-any.whl.zip` & `tmp/cns-1.0.38-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 484962 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat   177152 b- defN 23-Jun-29 09:00 cns/DataX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat   153088 b- defN 23-Jun-29 09:00 cns/DataX.cp39-win_amd64.pyd
+Zip file size: 485201 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-29 09:38 cns/DataX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-29 09:38 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-23 11:03 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      417 b- defN 23-Jun-26 05:16 cns/__init__.py
 -rw-rw-rw-  2.0 fat   101888 b- defN 23-Jun-26 14:00 cns/cmdX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    87040 b- defN 23-Jun-26 14:00 cns/cmdX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-29 09:07 cns-1.0.37.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2001 b- defN 23-Jun-29 09:07 cns-1.0.37.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-29 09:07 cns-1.0.37.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-29 09:07 cns-1.0.37.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1399 b- defN 23-Jun-29 09:07 cns-1.0.37.dist-info/RECORD
-17 files, 1096999 bytes uncompressed, 482694 bytes compressed:  56.0%
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2001 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1399 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/RECORD
+17 files, 1098535 bytes uncompressed, 482933 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: cns/cmdX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/cmdX.cp39-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.0.37.dist-info/LICENSE
+Filename: cns-1.0.38.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.37.dist-info/METADATA
+Filename: cns-1.0.38.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.37.dist-info/WHEEL
+Filename: cns-1.0.38.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.37.dist-info/top_level.txt
+Filename: cns-1.0.38.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.37.dist-info/RECORD
+Filename: cns-1.0.38.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cns-1.0.37.dist-info/METADATA` & `cns-1.0.38.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.37
+Version: 1.0.38
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: Rambo
 Author-email: 6566666@qq.com
 License: Copyright (C) 2023 CNS. All Rights Reserved. See LICENSE for license.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.37.dist-info/RECORD` & `cns-1.0.38.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-cns/DataX.cp36-win_amd64.pyd,sha256=cjvC_A7xONAmEptWGG9vjgXWU4f1o8srD2BPZ4GRMVw,177152
-cns/DataX.cp39-win_amd64.pyd,sha256=VeTI7bM7SPGpmuPmVYitGoy6EMxv_GtJ_eRN-G8a3ek,153088
+cns/DataX.cp36-win_amd64.pyd,sha256=tfeVxdEgqCDZd_uS9CEBbH3vk_cZLtcee_hB_ZeNE0o,178176
+cns/DataX.cp39-win_amd64.pyd,sha256=uuL22X4jAKstGC5Utsvdt7_ccDC7GjFAO7zZ3NRKcz4,153600
 cns/DateTimeX.cp36-win32.pyd,sha256=X6jjFZbOMmTTqnw0r3SfmiTRG9RFEpRdfVyU6AiFvCk,82944
 cns/DateTimeX.cp36-win_amd64.pyd,sha256=w-g6QPTK_U3il2bFu7PcucBGixhSX2Gm4M54ItAYMTk,99840
 cns/DateTimeX.cp39-win_amd64.pyd,sha256=bp9N6_ettlJ1odtrHJ3qU_yTBAsvULggzIyfz-eJuEk,88576
 cns/SQLstrX.cp36-win_amd64.pyd,sha256=3NLRKJa7q2Dl1sKlzVBbScgYjcgoSgMOClS2BuxDIzI,84992
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
 cns/TextX.cp36-win_amd64.pyd,sha256=cbQwr_FGkhhWoyyq3i43Tj11YSa-8r_3ZSN5JpXTcWk,77312
 cns/TextX.cp39-win_amd64.pyd,sha256=tJkutc00Vya2KBtXFWGcCm0wOSt9vvAm_7cZBsB1DgE,65536
 cns/__init__.py,sha256=t6RixBCw_0B4wUVAo2KTIOea-6tMeUneUQs6hXOS2ao,417
 cns/cmdX.cp36-win_amd64.pyd,sha256=-saULFU8EL3nYz7hBAYhKrg81qdSsLYVepV3QmHaz4g,101888
 cns/cmdX.cp39-win_amd64.pyd,sha256=jangzLwhz4_0gTB2rTdKsogUe01conQguA3LJKLgGNE,87040
-cns-1.0.37.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.37.dist-info/METADATA,sha256=v1hnX0wXwD3TXTSXFRVcwAawsj429xsJnb4vepu6wj8,2001
-cns-1.0.37.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.37.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.37.dist-info/RECORD,,
+cns-1.0.38.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.38.dist-info/METADATA,sha256=e0jaElhwS1jdMAHZbrfhQ1Z8uQxiJmNv7KzT9X8pnq0,2001
+cns-1.0.38.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.38.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.38.dist-info/RECORD,,
```

