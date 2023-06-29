# Comparing `tmp/aos_prov-4.2.0b2-py3-none-any.whl.zip` & `tmp/aos_prov-4.2.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 78751 bytes, number of entries: 64
+Zip file size: 78759 bytes, number of entries: 64
 -rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/__init__.py
 -rw-rw-rw-  2.0 fat     3156 b- defN 23-Jun-21 10:54 aos_prov/actions.py
 -rw-rw-rw-  2.0 fat     7927 b- defN 23-Jun-21 10:54 aos_prov/main.py
 -rw-rw-rw-  2.0 fat       93 b- defN 22-Oct-13 13:59 aos_prov/commands/__init__.py
 -rw-rw-rw-  2.0 fat     6021 b- defN 23-May-30 08:28 aos_prov/commands/command_provision.py
 -rw-rw-rw-  2.0 fat     5021 b- defN 23-Jan-19 15:42 aos_prov/commands/command_vm.py
 -rw-rw-rw-  2.0 fat     2406 b- defN 22-Dec-15 18:20 aos_prov/commands/command_vm_libvirt.py
@@ -44,23 +44,23 @@
 -rw-rw-rw-  2.0 fat     9804 b- defN 23-May-30 08:28 aos_prov/communication/unit/v4/unit_communication_v4.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/__init__.py
 -rw-rw-rw-  2.0 fat    18732 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
 -rw-rw-rw-  2.0 fat    34140 b- defN 22-Dec-02 13:22 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 -rw-rw-rw-  2.0 fat     2750 b- defN 22-Feb-07 18:56 aos_prov/files/1rootCA.crt
 -rw-rw-rw-  2.0 fat     2767 b- defN 22-Oct-13 13:59 aos_prov/files/vm.xml
 -rw-rw-rw-  2.0 fat      771 b- defN 22-Oct-13 13:59 aos_prov/utils/__init__.py
--rw-rw-rw-  2.0 fat     1703 b- defN 23-Mar-13 12:54 aos_prov/utils/common.py
+-rw-rw-rw-  2.0 fat     1685 b- defN 23-Jun-29 09:26 aos_prov/utils/common.py
 -rw-rw-rw-  2.0 fat     2667 b- defN 23-May-30 08:28 aos_prov/utils/config.py
 -rw-rw-rw-  2.0 fat      504 b- defN 23-May-30 08:28 aos_prov/utils/errors.py
 -rw-rw-rw-  2.0 fat     1229 b- defN 22-Dec-02 13:22 aos_prov/utils/unit_certificate.py
 -rw-rw-rw-  2.0 fat     7659 b- defN 23-Mar-13 10:35 aos_prov/utils/user_credentials.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-13 13:59 test/utils/__init__.py
 -rw-rw-rw-  2.0 fat      665 b- defN 22-Dec-02 13:22 test/utils/test_config.py
 -rw-rw-rw-  2.0 fat      656 b- defN 22-Dec-02 13:22 test/utils/test_unit_certificate.py
 -rw-rw-rw-  2.0 fat      456 b- defN 22-Oct-13 13:59 test/utils/test_user_credentials.py
--rw-rw-rw-  2.0 fat     2575 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     6399 b- defN 23-Jun-21 10:57 aos_prov-4.2.0b2.dist-info/RECORD
-64 files, 394372 bytes uncompressed, 68179 bytes compressed:  82.7%
+-rw-rw-rw-  2.0 fat     2575 b- defN 23-Jun-29 09:27 aos_prov-4.2.0b3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 09:27 aos_prov-4.2.0b3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-29 09:27 aos_prov-4.2.0b3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-29 09:27 aos_prov-4.2.0b3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     6399 b- defN 23-Jun-29 09:27 aos_prov-4.2.0b3.dist-info/RECORD
+64 files, 394354 bytes uncompressed, 68187 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -171,23 +171,23 @@
 
 Filename: test/utils/test_unit_certificate.py
 Comment: 
 
 Filename: test/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.2.0b2.dist-info/METADATA
+Filename: aos_prov-4.2.0b3.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.2.0b2.dist-info/WHEEL
+Filename: aos_prov-4.2.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.2.0b2.dist-info/entry_points.txt
+Filename: aos_prov-4.2.0b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.2.0b2.dist-info/top_level.txt
+Filename: aos_prov-4.2.0b3.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.2.0b2.dist-info/RECORD
+Filename: aos_prov-4.2.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/utils/common.py

```diff
@@ -1,54 +1,55 @@
-#
-#  Copyright (c) 2018-2023 Renesas Inc.
-#  Copyright (c) 2018-2023 EPAM Systems Inc.
-#
-
-import random
-import string
-from pathlib import Path
-
-from rich.console import Console
-
-CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
-DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
-AOS_DISKS_PATH = DOWNLOADS_PATH
-NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
-NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
-
-DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/R4.0.5.tar.gz?' \
-                          '0b4212dd0fd3cf5e29e44f35e2b3fafa474156bf99a8b9399de3b40bb0586a' \
-                          '0822e3a9396e05a96aed7f8e79650aeabdd0abe0d1876b2a621c37e28ebc' \
-
-console = Console()
-error_console = Console(stderr=True, style='red')
-allow_print = True
-
-def print_message(formatted_text, end="\n", ljust: int = 0):
-    if allow_print:
-        if ljust > 0:
-            formatted_text = formatted_text.ljust(ljust)
-        console.print(formatted_text, end=end)
-
-def print_left(formatted_text, ljust=60):
-    print_message(formatted_text, end='', ljust = ljust)
-
-def print_done():
-    print_message('[green]DONE')
-
-def print_success(message):
-    print_message(f'[green]{str(message)}')
-
-def print_error(message):
-    if allow_print:
-        error_console.print(message)
-
-def generate_random_password() -> str:
-    """
-    Generate random password from letters and digits.
-
-    Returns:
-        str: Random string password
-    """
-    dictionary = string.ascii_letters + string.digits
-    password_length = random.randint(10, 15)
-    return ''.join(random.choice(dictionary) for _ in range(password_length))
+#
+#  Copyright (c) 2018-2023 Renesas Inc.
+#  Copyright (c) 2018-2023 EPAM Systems Inc.
+#
+
+import random
+import string
+from pathlib import Path
+
+from rich.console import Console
+
+CONTENT_ENCRYPTION_ALGORITHM = 'aes256_cbc'
+DOWNLOADS_PATH = Path.home() / '.aos' / 'downloads'
+AOS_DISKS_PATH = DOWNLOADS_PATH
+NODE0_IMAGE_FILENAME = 'aos-vm-node0-genericx86-64.wic.vmdk'
+NODE1_IMAGE_FILENAME = 'aos-vm-node1-genericx86-64.wic.vmdk'
+
+DISK_IMAGE_DOWNLOAD_URL = 'https://aos-prod-cdn-endpoint.azureedge.net/vm/prerelease_R4.0.6.tar.gz?' \
+                          '0b4220cd64a5d136a30b1b7aad5d565f6aadac8a81f8f052580aa7416764f4a73a9e5f7e59b' \
+                          'a66f0cc16b4bd7b6f44f50958dbad8b6496cac0c37839a7911f0d191ad7f090a5f8eb74' \
+
+
+console = Console()
+error_console = Console(stderr=True, style='red')
+allow_print = True
+
+def print_message(formatted_text, end="\n", ljust: int = 0):
+    if allow_print:
+        if ljust > 0:
+            formatted_text = formatted_text.ljust(ljust)
+        console.print(formatted_text, end=end)
+
+def print_left(formatted_text, ljust=60):
+    print_message(formatted_text, end='', ljust = ljust)
+
+def print_done():
+    print_message('[green]DONE')
+
+def print_success(message):
+    print_message(f'[green]{str(message)}')
+
+def print_error(message):
+    if allow_print:
+        error_console.print(message)
+
+def generate_random_password() -> str:
+    """
+    Generate random password from letters and digits.
+
+    Returns:
+        str: Random string password
+    """
+    dictionary = string.ascii_letters + string.digits
+    password_length = random.randint(10, 15)
+    return ''.join(random.choice(dictionary) for _ in range(password_length))
```

## Comparing `aos_prov-4.2.0b2.dist-info/METADATA` & `aos_prov-4.2.0b3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.2.0b2
+Version: 4.2.0b3
 Summary: AosEdge Unit provisioning tool
 Home-page: UNKNOWN
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
```

## Comparing `aos_prov-4.2.0b2.dist-info/RECORD` & `aos_prov-4.2.0b3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=H1pfCM_tawiz1ft3IHbLOrZTgZbFglXTx19XpshmylY,9804
 aos_prov/communication/unit/v4/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=P0Xx1TV4ymcLyLhyHLUU9OR1hZqn0jPIVp32ZyFGh84,18732
 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=1C3DLG1-k5tUWKd7jzjWa3MHykb9gpKiseta3d_UlEI,34140
 aos_prov/files/1rootCA.crt,sha256=X3mH5kWiKpchVXfrW0HAhI94103mLhjftx2dR4KyWbw,2750
 aos_prov/files/vm.xml,sha256=67Z-mGXFGmiekJCfV1vzluEZWKKKeQXfcAmFn4DwKf8,2767
 aos_prov/utils/__init__.py,sha256=EfRSGsK_O0hF3vTrYEs5StBNfhuDk-RDquRYIm1aGBc,771
-aos_prov/utils/common.py,sha256=IJgC21J0XxeErfZWtH5l_lsHPgg3fjYQmxkOTNzg3R8,1703
+aos_prov/utils/common.py,sha256=bDgg6LMa88Evjf7vqVHlqnVNza9tFQvXz1rLSpK0jxQ,1685
 aos_prov/utils/config.py,sha256=A-LTNGcmTNmkyTKTRA_W7XLo3Qx5q345FRSp4cHPjbE,2667
 aos_prov/utils/errors.py,sha256=T5Mbl-OixiUeBS3U2j0s11tu1nx0XDjrTsYyuDpxr7o,504
 aos_prov/utils/unit_certificate.py,sha256=aKi3tYOCe-0gFpfiv5_9QxlX5z9mOMK2gQbAz7oIFh4,1229
 aos_prov/utils/user_credentials.py,sha256=EF9GTLsb6zBKccXPJC3RyKbo7GFN6JClWG3NCcMV_ew,7659
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/test_config.py,sha256=JuofpwzS7FGqWcfRHOaGSlrvqVYu9rS55K-yE5JhrNs,665
 test/utils/test_unit_certificate.py,sha256=ayJbD0Qrj1FICnDRjVPBpH0zMqLEMjqzR3ZNTxSAzHU,656
 test/utils/test_user_credentials.py,sha256=_g-oGXprFMiqRD9ZklnTiqxWsvsXtW0As5oJpWOqQW0,456
-aos_prov-4.2.0b2.dist-info/METADATA,sha256=-IFNR4-GQY_wmPKUU_CRZ9UOEViC-HRr2jTqgXq4sDs,2575
-aos_prov-4.2.0b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_prov-4.2.0b2.dist-info/entry_points.txt,sha256=pSYEWtSRNsmqfdoCn0tQJAqVxSOeLGpaSi6UPJv_kfA,49
-aos_prov-4.2.0b2.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
-aos_prov-4.2.0b2.dist-info/RECORD,,
+aos_prov-4.2.0b3.dist-info/METADATA,sha256=6P596A5xn9vipJmnr_UvLZgITW-tQVDGHPHiT5BaxA4,2575
+aos_prov-4.2.0b3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_prov-4.2.0b3.dist-info/entry_points.txt,sha256=pSYEWtSRNsmqfdoCn0tQJAqVxSOeLGpaSi6UPJv_kfA,49
+aos_prov-4.2.0b3.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
+aos_prov-4.2.0b3.dist-info/RECORD,,
```

