# Comparing `tmp/esp-coredump-1.5.1.tar.gz` & `tmp/esp-coredump-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-coredump-1.5.1.tar", last modified: Mon May 22 10:43:22 2023, max compression
+gzip compressed data, was "dist/esp-coredump-1.5.2.tar", last modified: Thu Jun 29 17:21:03 2023, max compression
```

## Comparing `esp-coredump-1.5.1.tar` & `esp-coredump-1.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/cli_ext.py
--rwxrwxrwx   0 root         (0) root         (0)    21962 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/coredump.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/corefile/
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/_parse_soc_header.py
--rw-rw-rw-   0 root         (0) root         (0)    12070 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     5300 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)    28157 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/riscv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c3.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32c6.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32h2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32s2.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/soc_headers/esp32s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11177 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/corefile/xtensa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/espcoredump.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/scripts/run_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/esp_coredump/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/esp_coredump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:43:22.000000 esp-coredump-1.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4334 2023-05-22 10:42:57.000000 esp-coredump-1.5.1/tests/test_espcoredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/cli_ext.py
+-rwxrwxrwx   0 root         (0) root         (0)    22322 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/coredump.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/corefile/
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/_parse_soc_header.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5339 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)    28537 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/riscv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c3.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32c6.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32h2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32s2.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/soc_headers/esp32s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11177 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/corefile/xtensa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/espcoredump.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/scripts/run_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/esp_coredump/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/esp_coredump.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:21:03.000000 esp-coredump-1.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2023-06-29 17:20:29.000000 esp-coredump-1.5.2/tests/test_espcoredump.py
```

### Comparing `esp-coredump-1.5.1/LICENSE` & `esp-coredump-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/PKG-INFO` & `esp-coredump-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.1
+Version: 1.5.2
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.1/README.md` & `esp-coredump-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/__init__.py` & `esp-coredump-1.5.2/esp_coredump/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 from .coredump import CoreDump
 
 __all__ = [
     'CoreDump',
 ]
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
```

### Comparing `esp-coredump-1.5.1/esp_coredump/cli_ext.py` & `esp-coredump-1.5.2/esp_coredump/cli_ext.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/coredump.py` & `esp-coredump-1.5.2/esp_coredump/coredump.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 MORE_INFO_MSG = 'Read more: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html'
 GDB_NOT_FOUND_ERROR = (
     f'GDB executable not found. Please install GDB or set up ESP-IDF to complete the action. '
     f'{MORE_INFO_MSG}'
 )
 IDF_SETUP_ERROR = f'Please set up ESP-IDF to complete the action. {MORE_INFO_MSG}'
 
+RETRY_ATTEMPTS = 3
+
 
 if os.name == 'nt':
     CLOSE_FDS = False
 else:
     CLOSE_FDS = True
 
 
@@ -63,14 +65,15 @@
                  port: str = os.environ.get('ESPTOOL_PORT', ESPLoader.DEFAULT_PORT),
                  gdb_timeout_sec: int = DEFAULT_GDB_TIMEOUT_SEC,
                  core: Optional[str] = None,
                  chip_rev: Optional[int] = None,
                  gdb: Optional[str] = None,
                  extra_gdbinit_file: Optional[str] = None,
                  off: Optional[int] = None,
+                 parttable_off: Optional[int] = None,
                  prog: Optional[str] = None,
                  print_mem: Optional[str] = None,
                  rom_elf: Optional[str] = None,
                  save_core: Optional[str] = None,
                  ):
         if prog is None:
             raise ValueError("Path to program\'s ELF binary is not provided")
@@ -79,15 +82,16 @@
         self.chip = chip
         self.core = core
         self.chip_rev = chip_rev
         self.core_format = core_format
         self.gdb = gdb
         self.gdb_timeout_sec = gdb_timeout_sec
         self.extra_gdbinit_file = extra_gdbinit_file
-        self.off = off
+        self.coredump_off = off
+        self.parttable_off = parttable_off
         self.prog = prog
         self.port = port
         self.print_mem = print_mem
         self.rom_elf = rom_elf
         self.save_core = save_core
 
     @staticmethod
@@ -126,15 +130,15 @@
         }
 
         if not self.core:
             # Core file not specified, try to read core dump from flash.
             if not IDF_PATH:
                 print(IDF_SETUP_ERROR)
                 sys.exit(1)
-            loader = ESPCoreDumpFlashLoader(self.off, self.chip, port=self.port, baud=self.baud)
+            loader = ESPCoreDumpFlashLoader(self.coredump_off, port=self.port, baud=self.baud, part_table_offset=self.parttable_off)
         elif self.core_format != 'elf':
             # Core file specified, but not yet in ELF format. Convert it from raw or base64 into ELF.
             loader = ESPCoreDumpFileLoader(self.core, self.core_format == 'b64')
         else:
             # Core file is already in the ELF format
             core_dump_info_map['core_elf_path'] = self.core
             chip_rev = self.extract_chip_rev_from_elf()
@@ -300,15 +304,20 @@
             task_name = self.gdb_esp.get_freertos_task_name(marker)
             print("\nCrashed task handle: 0x%x, name: '%s', GDB name: 'process %d'"
                   % (marker, task_name, marker))  # type: ignore
 
     def print_threads_info(self, task_info):  # type: (Optional[list[Container]]) -> None
         print(self.gdb_esp.run_cmd('info threads'))
         # THREADS STACKS
-        threads, _ = self.gdb_esp.get_thread_info()
+        for attempt in range(1, RETRY_ATTEMPTS + 1):
+            threads, _ = self.gdb_esp.get_thread_info(attempt * DEFAULT_GDB_TIMEOUT_SEC)
+            if threads:
+                break
+
+            print('Retrying reading threads information...')
 
         if not threads:
             print('\nThe threads information for the current task could not be retrieved. '
                   'Please try running this command again with --gdb-timeout-sec option to increase '
                   f'the default value of internal delay for gdb responses (Default: {DEFAULT_GDB_TIMEOUT_SEC})')
             return
```

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/__init__.py` & `esp-coredump-1.5.2/esp_coredump/corefile/__init__.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/_parse_soc_header.py` & `esp-coredump-1.5.2/esp_coredump/corefile/_parse_soc_header.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/elf.py` & `esp-coredump-1.5.2/esp_coredump/corefile/elf.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/gdb.py` & `esp-coredump-1.5.2/esp_coredump/corefile/gdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,17 +94,17 @@
                                                                done_message='done', done_type='result')
         return ''.join([x['payload'] for x in filtered_responses]) \
             .replace('\\n', '\n') \
             .replace('\\t', '\t') \
             .rstrip('\n') \
             .replace('\\"', '"')
 
-    def get_thread_info(self):
+    def get_thread_info(self, response_delay_sec=DEFAULT_GDB_TIMEOUT_SEC):
         """ Get information about all threads known to GDB, and the current thread ID """
-        result = self._gdbmi_run_cmd_get_one_response('-thread-info', 'done', 'result', response_delay_sec=DEFAULT_GDB_TIMEOUT_SEC)['payload']
+        result = self._gdbmi_run_cmd_get_one_response('-thread-info', 'done', 'result', response_delay_sec=response_delay_sec)['payload']
         if not result:
             return None, None
 
         current_thread_id = result['current-thread-id']
         threads = result['threads']
         return threads, current_thread_id
```

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/loader.py` & `esp-coredump-1.5.2/esp_coredump/corefile/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -481,19 +481,21 @@
         core_elf.e_type = ElfFile.ET_CORE
         core_elf.dump(self.core_elf_file)  # type: ignore
 
 
 class ESPCoreDumpFlashLoader(EspCoreDumpLoader):
     ESP_COREDUMP_PART_TABLE_OFF = 0x8000
 
-    def __init__(self, offset, target=None, port=None, baud=None):
-        # type: (Optional[int], Optional[str], Optional[str], Optional[int]) -> None
+    def __init__(self, offset, target=None, port=None, baud=None, part_table_offset=0x8000):
+        # type: (Optional[int], Optional[str], Optional[str], Optional[int], Optional[int]) -> None
+        # TODO in next major release drop offset argument and use just parttool to find offset of coredump partition
         super(ESPCoreDumpFlashLoader, self).__init__()
         self.port = port
         self.baud = baud
+        self.part_table_offset = part_table_offset
 
         self._get_core_src(offset, target)
         self.target = self._load_core_src()
 
     def _get_core_src(self, off, target=None):  # type: (Optional[int], Optional[str]) -> None
         """
         Loads core dump from flash using parttool or esptool (if offset is set)
@@ -556,35 +558,38 @@
     def _invoke_parttool(self):  # type: () -> None
         """
         Loads core dump from flash using parttool
         """
         tool_args = [sys.executable, PARTTOOL_PY]
         if self.port:
             tool_args.extend(['--port', self.port])
+        if self.baud:
+            tool_args.extend(['--baud', str(self.baud)])
+        if self.part_table_offset:
+            tool_args.extend(['--partition-table-offset', str(self.part_table_offset)])
         tool_args.extend(['read_partition', '--partition-type', 'data', '--partition-subtype', 'coredump', '--output'])
 
         self.core_src_file = self._create_temp_file()
         try:
             tool_args.append(self.core_src_file)  # type: ignore
             # read core dump partition
             et_out = subprocess.check_output(tool_args, stderr=subprocess.STDOUT)
             if et_out:
                 logging.info(et_out.decode('utf-8'))
         except subprocess.CalledProcessError as e:
             raise ESPCoreDumpLoaderError(f'parttool script execution failed with error {e.returncode}, '
                                          f"failed command was: '{' '.join(e.cmd)}'",
                                          extra_output=e.output.decode('utf-8', 'ignore'))
 
-    def _get_core_dump_partition_info(self, part_off=None):  # type: (Optional[int]) -> Tuple[int, int]
+    def _get_core_dump_partition_info(self):  # type: () -> Tuple[int, int]
         """
         Get core dump partition info using parttool
         """
         logging.info('Retrieving core dump partition offset and size...')
-        if not part_off:
-            part_off = self.ESP_COREDUMP_PART_TABLE_OFF
+        part_off = self.part_table_offset or self.ESP_COREDUMP_PART_TABLE_OFF
         try:
             tool_args = [sys.executable, PARTTOOL_PY, '-q', '--partition-table-offset', str(part_off)]
             if self.port:
                 tool_args.extend(['--port', self.port])
             invoke_args = tool_args + ['get_partition_info', '--partition-type', 'data',
                                        '--partition-subtype', 'coredump',
                                        '--info', 'offset', 'size']
```

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/riscv.py` & `esp-coredump-1.5.2/esp_coredump/corefile/riscv.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/corefile/xtensa.py` & `esp-coredump-1.5.2/esp_coredump/corefile/xtensa.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/scripts/espcoredump.py` & `esp-coredump-1.5.2/esp_coredump/scripts/espcoredump.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump/scripts/run_tests.py` & `esp-coredump-1.5.2/esp_coredump/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/esp_coredump.egg-info/PKG-INFO` & `esp-coredump-1.5.2/esp_coredump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-coredump
-Version: 1.5.1
+Version: 1.5.2
 Summary: Generate core dumps on unrecoverable software errors
 Home-page: https://github.com/espressif/esp-idf
 Author: Espressif Systems
 Author-email: aleksei.apaseev@espressif.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `esp-coredump-1.5.1/esp_coredump.egg-info/SOURCES.txt` & `esp-coredump-1.5.2/esp_coredump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/setup.py` & `esp-coredump-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `esp-coredump-1.5.1/tests/test_espcoredump.py` & `esp-coredump-1.5.2/tests/test_espcoredump.py`

 * *Files identical despite different names*

