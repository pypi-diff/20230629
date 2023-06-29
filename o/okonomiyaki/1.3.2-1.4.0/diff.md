# Comparing `tmp/okonomiyaki-1.3.2.tar.gz` & `tmp/okonomiyaki-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/okonomiyaki-1.3.2.tar", last modified: Thu Jul  1 17:20:31 2021, max compression
+gzip compressed data, was "okonomiyaki-1.4.0.tar", last modified: Thu Jun 29 17:47:38 2023, max compression
```

## Comparing `okonomiyaki-1.3.2.tar` & `okonomiyaki-1.4.0.tar`

### file list

```diff
@@ -1,214 +1,232 @@
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/_cli/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/_cli/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/_cli/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2580 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/_cli/tests/test_cli.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2799 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/_cli/__init__.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      516 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    95689 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/pkg_info_data.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16630 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/platform_tag.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    39610 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/python_tag.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    41741 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/common.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    40260 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__egg_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16343 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__package_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2612 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__wheel_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    17802 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_egg_file_format.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8181 2021-06-29 13:10:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_legacy.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5968 2021-06-29 13:10:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_setuptools_file_format.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      387 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    34031 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_egg_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16305 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_package_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      235 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_wheel_common.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1853 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/_wheel_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7773 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/egg.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4075 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/legacy.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5877 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/file_formats/setuptools_egg.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3784 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/common.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3385 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test__arch.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1506 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_abi.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    20277 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_epd_platform.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1766 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_pep425.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6072 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_platform.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7676 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_platform_filters.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4878 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_python_implementation.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      430 2021-03-05 12:28:34.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2691 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/_arch.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4383 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/_pep425_impl.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5157 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/_platform.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3851 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/abi.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    15964 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/epd_platform.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3202 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/legacy.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1363 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/pep425.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4342 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/platform_filters.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2945 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/platforms/python_implementation.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/broken_legacy_eggs/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2645 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/broken_legacy_eggs/mccabe-0.2.1-2.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4766 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/Cython-0.19.1-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1562 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2175 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/PySide-1.0.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5316 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/PySide-1.1.0-3.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1209 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/_osx64app-1.0-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5870 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/enstaller-4.5.0-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    10027 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/ets-4.3.0-3.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4570 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/medialog.boardfile-1.6.1-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1717 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/numexpr-2.2.2-3.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2386 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pip-6.0.8-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3905 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pip-7.0.3-py3.4.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3825 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pymongo-2.8-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4908 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pymongo_description.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      974 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pymultinest-0.1-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7571 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/setuptools-16.0-py3.4.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4591 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/setuptools-40.8.0-py2.7.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    23400 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/supervisor-3.0-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4811 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-4.6.0.dev235-py2.7-macosx-10.10-intel.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5508 2021-06-29 13:10:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-linux-x86_64.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5510 2021-06-29 13:10:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-macosx-10.14-x86_64.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5528 2021-06-29 13:10:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-win-amd64.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1198 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/xz-5.2.0-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/repositories/__init__.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4152 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4125 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    14409 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime_metadata.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       85 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      207 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/common.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6777 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7503 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_info.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8801 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_metadata.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4688 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_schemas.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      803 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1581 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1386 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/numpy-1.9.2-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      755 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1525 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1331 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/numpy-1.9.2-1.egg
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      755 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1524 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1328 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/numpy-1.9.2-1.egg
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      807 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1576 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1380 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/numpy-1.9.2-1.egg
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      806 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1580 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1384 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/numpy-1.9.2-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      807 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1575 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1380 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/numpy-1.9.2-1.egg
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      799 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1577 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1382 2021-06-28 13:23:41.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/numpy-1.9.2-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      744 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/MKL-10.3-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1516 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/nose-1.3.4-1.egg
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1321 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/numpy-1.9.2-1.egg
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/wheels/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3184 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/wheels/okonomiyaki-0.17.0.dev799-py2-none-any.whl
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7545 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      568 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime.invalid
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh6_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191419 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227252 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86_64-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh6_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191411 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227249 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86_64-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      599 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      588 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime.invalid
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh6_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191415 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227250 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86_64-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh6_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191415 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227250 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86_64-msvc2008.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh6_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191603 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86-msvc2015.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227438 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86_64-msvc2015.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-osx_x86_64-darwin.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-rh7_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   203403 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86-msvc2019.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   230294 2021-05-27 11:38:25.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86_64-msvc2019.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      518 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/julia-0.3.11+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      525 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/julia-0.3.11+1-win_x86_64-mingw.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      555 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/pypy-2.6.0+1-rh5_x86_64-gnu.runtime
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      508 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/test_data/r-3.0.0+1-rh5_x86_64-gnu.runtime
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2279 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_eggs.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1107 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_main.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5806 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_misc.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1595 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_test_data.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1656 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6745 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/utils/misc.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2092 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/py3compat.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1199 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/utils/testing.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/versions/
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4567 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_enpkg_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1784 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_metadata_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     9149 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_pep386_workaround.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6309 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_pep440.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2129 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_runtime_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8596 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_semver.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      425 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2910 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/versions/enpkg.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2001 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/versions/metadata_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    12090 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/pep386.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3159 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/pep386_workaround.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5677 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/versions/pep440.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2037 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/versions/runtime_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6308 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/okonomiyaki/versions/semver.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      304 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/__init__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       63 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/__main__.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      301 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki/_version.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2911 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/okonomiyaki/errors.py
-drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2679 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/PKG-INFO
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     9339 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/SOURCES.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        1 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/dependency_links.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      126 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/requires.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       12 2021-07-01 17:20:30.000000 okonomiyaki-1.3.2/okonomiyaki.egg-info/top_level.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1616 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/LICENSE.txt
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       63 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/MANIFEST.in
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1815 2021-03-05 11:23:18.000000 okonomiyaki-1.3.2/README.rst
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5222 2021-07-01 17:20:11.000000 okonomiyaki-1.3.2/setup.py
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2679 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/PKG-INFO
--rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       38 2021-07-01 17:20:31.000000 okonomiyaki-1.3.2/setup.cfg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    10032 2023-06-29 17:47:16.000000 okonomiyaki-1.4.0/CHANGELOG
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1616 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/LICENSE.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      136 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/MANIFEST.in
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    12456 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/PKG-INFO
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1815 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/README.rst
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      304 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       63 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/__main__.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/_cli/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2799 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/_cli/__init__.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/_cli/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/_cli/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2580 2023-06-23 13:43:26.000000 okonomiyaki-1.4.0/okonomiyaki/_cli/tests/test_cli.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      302 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki/_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2911 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/errors.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/file_formats/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      387 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/__init__.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      516 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    95704 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/pkg_info_data.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16630 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/platform_tag.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    39610 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/python_tag.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    33683 2023-06-29 14:35:26.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_egg_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16305 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_package_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      235 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_wheel_common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1853 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/_wheel_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7773 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/egg.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4075 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/legacy.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5877 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/setuptools_egg.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    41741 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    40055 2023-06-29 14:35:26.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__egg_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16343 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__package_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2612 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__wheel_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    17802 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_egg_file_format.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8181 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_legacy.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5968 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_setuptools_file_format.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/platforms/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      448 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2765 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/_arch.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3769 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/_pep425_impl.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6415 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/_platform.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3917 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/abi.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    16031 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/epd_platform.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3202 2023-06-28 22:45:50.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/legacy.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1363 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/pep425.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4342 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/platform_filters.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3021 2023-06-29 12:19:37.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/python_implementation.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4549 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3369 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test__arch.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1770 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_abi.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    20522 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_epd_platform.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2466 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_pep425.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     9922 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_platform.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7676 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_platform_filters.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4083 2023-06-29 12:19:37.000000 okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_python_implementation.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/repositories/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/__init__.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.410348 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/__init__.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.420348 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5498 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/Cython-0.19.1-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1250 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1761 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/PySide-1.0.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5108 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/PySide-1.1.0-3.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1209 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/_osx64app-1.0-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.420348 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/broken_legacy_eggs/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2645 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/broken_legacy_eggs/mccabe-0.2.1-2.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5870 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/enstaller-4.5.0-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    10225 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/ets-4.3.0-3.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4208 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/medialog.boardfile-1.6.1-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1406 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/numexpr-2.2.2-3.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1971 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pip-6.0.8-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3905 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pip-7.0.3-py3.4.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3515 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pymongo-2.8-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4908 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pymongo_description.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      766 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pymultinest-0.1-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7571 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/setuptools-16.0-py3.4.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4591 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/setuptools-40.8.0-py2.7.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    23400 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/supervisor-3.0-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4811 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-4.6.0.dev235-py2.7-macosx-10.10-intel.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5508 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-linux-x86_64.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5510 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-macosx-10.14-x86_64.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5528 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-win-amd64.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      938 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/xz-5.2.0-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.420348 okonomiyaki-1.4.0/okonomiyaki/runtimes/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       85 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      207 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/common.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6777 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     7503 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8801 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_metadata.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4688 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_schemas.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.420348 okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4152 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4125 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime_info.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    12529 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime_metadata.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.420348 okonomiyaki-1.4.0/okonomiyaki/utils/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1656 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6745 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/misc.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2092 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/py3compat.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     9173 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      568 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime.invalid
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh6_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191419 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227252 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86_64-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh6_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1778 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191411 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227249 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86_64-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      599 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      588 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime.invalid
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1582 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.11.2+2-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2106 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.11.2+2-rh8_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   231276 2023-06-28 21:05:10.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.11.2+2-win_x86_64-msvc2022.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh6_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191415 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227250 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86_64-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh6_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191415 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227250 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86_64-msvc2008.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2093 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh6_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   191603 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86-msvc2015.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   227438 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86_64-msvc2015.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2095 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-osx_x86_64-darwin.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2094 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-rh7_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   203403 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86-msvc2019.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)   230294 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86_64-msvc2019.runtime
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      755 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/MKL-10.3-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      812 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1582 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1387 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      803 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1581 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1386 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/numpy-1.9.2-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1525 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1331 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      755 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1524 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1328 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      807 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1576 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1380 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      807 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/MKL-10.3-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      806 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1580 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1384 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/numpy-1.9.2-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1575 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1380 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      917 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1581 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1385 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      744 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/MKL-10.3-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      809 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1576 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1382 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/numpy-1.9.2-1.egg
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      799 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/MKL-10.3-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1577 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1382 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/numpy-1.9.2-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1516 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/nose-1.3.4-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1321 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/numpy-1.9.2-1.egg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      518 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/julia-0.3.11+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      525 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/julia-0.3.11+1-win_x86_64-mingw.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      555 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/pypy-2.6.0+1-rh5_x86_64-gnu.runtime
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      508 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/r-3.0.0+1-rh5_x86_64-gnu.runtime
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/wheels/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3184 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/test_data/wheels/okonomiyaki-0.17.0.dev799-py2-none-any.whl
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1199 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/testing.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/utils/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3298 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_eggs.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1107 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_main.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5806 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_misc.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1353 2023-06-29 16:56:36.000000 okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_runtimes.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/versions/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      425 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2910 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/enpkg.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2001 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/metadata_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    12129 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/pep386.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     3159 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/pep386_workaround.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     5686 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/pep440.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2142 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/runtime_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6308 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/semver.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/okonomiyaki/versions/tests/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        0 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/__init__.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     4567 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_enpkg_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     1784 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_metadata_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     9149 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_pep386_workaround.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     6547 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_pep440.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2368 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_runtime_version.py
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     8596 2023-06-23 12:03:49.000000 okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_semver.py
+drwxrwxr-x   0 itziakos  (1000) itziakos  (1000)        0 2023-06-29 17:47:38.400348 okonomiyaki-1.4.0/okonomiyaki.egg-info/
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    12456 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/PKG-INFO
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)    10204 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/SOURCES.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        1 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/dependency_links.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)        1 2023-06-28 21:05:32.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/not-zip-safe
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)      231 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/requires.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)       12 2023-06-29 17:47:38.000000 okonomiyaki-1.4.0/okonomiyaki.egg-info/top_level.txt
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2074 2023-06-29 17:47:38.430348 okonomiyaki-1.4.0/setup.cfg
+-rw-rw-r--   0 itziakos  (1000) itziakos  (1000)     2997 2023-06-29 17:27:48.000000 okonomiyaki-1.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/_cli/tests/test_cli.py` & `okonomiyaki-1.4.0/okonomiyaki/_cli/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/_cli/__init__.py` & `okonomiyaki-1.4.0/okonomiyaki/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/__init__.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/__init__.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/pkg_info_data.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/pkg_info_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding=utf-8
+# flake8: noqa
 import os.path
 
 
 B3_1_4_1 = u"""\
 Metadata-Version: 1.0
 Name: b3
 Version: 1.4.1
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/platform_tag.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/platform_tag.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_blacklist/python_tag.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_blacklist/python_tag.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/common.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/common.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__egg_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__egg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from okonomiyaki.errors import (
     InvalidEggName, InvalidMetadataField, MissingMetadata, UnsupportedMetadata,
     InvalidRequirementStringHyphen)
 from okonomiyaki.utils import tempdir
 from okonomiyaki.utils.test_data import (
     MKL_10_3_RH5_X86_64, NOSE_1_3_4_RH6_X86_64, NOSE_1_3_4_RH5_X86_64)
 from okonomiyaki.platforms import EPDPlatform, PlatformABI
-from okonomiyaki.platforms.legacy import LegacyEPDPlatform
 from okonomiyaki.versions import EnpkgVersion, MetadataVersion
 
 from .._egg_info import (
     Requirement, EggMetadata, LegacySpecDepend, parse_rawspec,
     split_egg_name)
 
 from .common import (
@@ -191,18 +190,14 @@
 """
         depend = LegacySpecDepend.from_string(r_depend)
 
         # Then
         self.assertEqual(depend.arch, "x86")
         self.assertEqual(depend.platform, "win32")
         self.assertIsNone(depend.osdist)
-        self.assertEqual(
-            depend._epd_legacy_platform,
-            LegacyEPDPlatform.from_epd_platform_string("win-32")
-        )
         self.assertEqual(depend.platform_abi, "msvc2008")
 
     def test_format_1_3(self):
         r_depend = """\
 metadata_version = "1.3"
 name= "numpy_debug"
 version = "1.9.2"
@@ -325,26 +320,26 @@
         with mock.patch(
             "okonomiyaki.file_formats._egg_info.compute_sha256",
             return_value=sha256sum
         ):
             spec_depend = LegacySpecDepend.from_egg(egg)
 
         # Then
-        self.assertEqual(str(spec_depend._epd_legacy_platform), "win-32")
+        self.assertEqual(spec_depend._epd_platform.pep425_tag, "win32")
 
         # When
         with mock.patch(
             "okonomiyaki.file_formats._egg_info.compute_sha256",
             return_value=sha256sum
         ):
             with zipfile2.ZipFile(egg) as zp:
                 spec_depend = LegacySpecDepend.from_egg(zp)
 
         # Then
-        self.assertEqual(str(spec_depend._epd_legacy_platform), "win-32")
+        self.assertEqual(spec_depend._epd_platform.pep425_tag, "win32")
 
     def test_missing_spec_depend(self):
         # When/Then
         with tempdir() as d:
             path = os.path.join(d, 'egg-5.1-1.egg')
             with zipfile2.ZipFile(path, "w") as zp:
                 zp.writestr("dummy", b"")
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__package_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__package_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test__wheel_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test__wheel_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_egg_file_format.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_egg_file_format.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_legacy.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/tests/test_setuptools_file_format.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/tests/test_setuptools_file_format.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_egg_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_egg_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from attr import attr, attributes
 from attr.validators import instance_of, optional
 
 from okonomiyaki.errors import (
     InvalidRequirementString, InvalidRequirementStringHyphen,
     InvalidEggName, InvalidMetadataField,
     MissingMetadata, UnsupportedMetadata)
-from okonomiyaki.platforms.legacy import LegacyEPDPlatform
 from okonomiyaki.platforms import (
     EPDPlatform, PlatformABI, PythonABI, PythonImplementation)
 from okonomiyaki.utils import (
     compute_sha256, decode_if_needed, encode_if_needed, parse_assignments)
 from okonomiyaki.utils.py3compat import StringIO, string_types
 from okonomiyaki.versions import EnpkgVersion, MetadataVersion
 from .legacy import (
@@ -417,49 +416,37 @@
     """
 
     packages = attr(validator=instance_of(list))
     """
     List of dependencies for this egg
     """
 
-    _epd_legacy_platform = attr(
-        validator=optional(instance_of(LegacyEPDPlatform))
-    )
-
+    _epd_platform = attr(validator=optional(instance_of(EPDPlatform)))
     _metadata_version = attr(validator=instance_of(MetadataVersion))
 
     @classmethod
     def _from_data(cls, data, epd_platform):
         args = data.copy()
         args[_TAG_METADATA_VERSION] = M(
-            args.get(_TAG_METADATA_VERSION, _METADATA_DEFAULT_VERSION_STRING)
-        )
-
-        if epd_platform is None:
-            _epd_legacy_platform = None
-        else:
-            _epd_legacy_platform = LegacyEPDPlatform(epd_platform)
-        args["_epd_legacy_platform"] = _epd_legacy_platform
-
+            args.get(_TAG_METADATA_VERSION, _METADATA_DEFAULT_VERSION_STRING))
         args[_TAG_PACKAGES] = [
             Requirement.from_spec_string(s)
-            for s in args.get(_TAG_PACKAGES, [])
-        ]
+            for s in args.get(_TAG_PACKAGES, [])]
 
         return cls(
             args["name"],
             args["version"],
             args["build"],
             args["python"],
             args["python_tag"],
             args["abi_tag"],
             args["platform_tag"],
             args["platform_abi"],
             args["packages"],
-            args["_epd_legacy_platform"],
+            epd_platform,
             args["metadata_version"],
         )
 
     @classmethod
     def from_egg(cls, path_or_file):
         sha256 = None
         if isinstance(path_or_file, string_types):
@@ -506,42 +493,57 @@
         return cls._from_data(data, epd_platform)
 
     @property
     def arch(self):
         """
         Egg architecture.
         """
-        if self._epd_legacy_platform is None:
+        epd_platform = self._epd_platform
+        if epd_platform is None:
             return None
         else:
-            return self._epd_legacy_platform.arch._legacy_name
+            return epd_platform.arch._legacy_name
 
     @property
     def egg_name(self):
         """
         Full egg name (including .egg extension).
         """
         return egg_name(self.name, self.version, self.build)
 
     @property
     def osdist(self):
-        if self._epd_legacy_platform is None:
+        epd_platform = self._epd_platform
+        if epd_platform is None:
             return None
-        else:
-            return self._epd_legacy_platform.osdist
+        name = epd_platform.platform_name
+        if name in ('osx', 'win'):
+            return None
+        elif name == 'sol':
+            return 'Solaris 10'
+        elif name.startswith('rh'):
+            return 'RedHat_{}'.format(name[2:])
 
     @property
     def platform(self):
         """
         The legacy platform name (sys.platform).
         """
-        if self._epd_legacy_platform is None:
+        epd_platform = self._epd_platform
+        if epd_platform is None:
             return None
-        else:
-            return self._epd_legacy_platform.platform
+        name = epd_platform.platform_name
+        if name == 'osx':
+            return 'darwin'
+        elif name == 'win':
+            return 'win32'
+        elif name == 'sol':
+            return 'sunos5'
+        elif name.startswith('rh'):
+            return 'linux2'
 
     @property
     def metadata_version(self):
         return self._metadata_version
 
     @metadata_version.setter
     def metadata_version(self, value):
@@ -636,16 +638,15 @@
 
     python_tag = EGG_PYTHON_TAG_BLACK_LIST.get(sha256)
     if python_tag:
         data[_TAG_PYTHON_PEP425_TAG] = python_tag
     else:
         if metadata_version < M("1.2"):
             data[_TAG_PYTHON_PEP425_TAG] = _guess_python_tag(
-                raw_data[_TAG_PYTHON]
-            )
+                raw_data[_TAG_PYTHON])
         else:
             data[_TAG_PYTHON_PEP425_TAG] = raw_data[_TAG_PYTHON_PEP425_TAG]
 
     if metadata_version < M("1.3"):
         python_tag = data[_TAG_PYTHON_PEP425_TAG]
         data[_TAG_ABI_PEP425_TAG] = _guess_abi_tag(epd_platform, python_tag)
         data[_TAG_PLATFORM_PEP425_TAG] = _guess_platform_tag(epd_platform)
@@ -781,34 +782,24 @@
 
         return cls._from_spec_depend(spec_depend, pkg_info_string, summary)
 
     @classmethod
     def _from_spec_depend(cls, spec_depend, pkg_info, summary,
                           metadata_version=None):
         raw_name = spec_depend.name
-
-        version = EnpkgVersion.from_upstream_and_build(spec_depend.version,
-                                                       spec_depend.build)
-
+        version = EnpkgVersion.from_upstream_and_build(
+            spec_depend.version, spec_depend.build)
         python_tag = spec_depend.python_tag
         abi_tag = spec_depend.abi_tag
         platform_abi = spec_depend.platform_abi
-
-        if spec_depend._epd_legacy_platform is None:
-            platform = None
-        else:
-            platform = spec_depend._epd_legacy_platform._epd_platform
-
+        epd_platform = spec_depend._epd_platform
         dependencies = Dependencies(
-            tuple(dep for dep in spec_depend.packages)
-        )
-
+            tuple(dep for dep in spec_depend.packages))
         metadata_version = metadata_version or spec_depend.metadata_version
-
-        return cls(raw_name, version, platform, python_tag, abi_tag,
+        return cls(raw_name, version, epd_platform, python_tag, abi_tag,
                    platform_abi, dependencies, pkg_info, summary,
                    metadata_version)
 
     @classmethod
     def from_egg_metadata(cls, egg_metadata, **kw):
         """ Utility ctor to create a new EggMetadata instance from an existing
         one, potentially updating some metadata.
@@ -957,15 +948,14 @@
         """ The package name."""
         return self._raw_name.lower().replace("-", "_")
 
     @property
     def pkg_info(self):
         if isinstance(self._pkg_info, six.string_types):
             self._pkg_info = PackageInfo.from_string(self._pkg_info)
-
         return self._pkg_info
 
     @property
     def platform_abi_tag(self):
         if self.platform_abi is None:
             return None
         else:
@@ -1017,34 +1007,27 @@
     @property
     def _spec_depend(self):
         if not self.is_strictly_supported:
             msg = "Cannot write back metadata with unsupported version {0!r}"
             raise UnsupportedMetadata(
                 self.metadata_version, msg.format(str(self.metadata_version))
             )
-
-        if self.platform is None:
-            epd_platform = None
-        else:
-            legacy_epd_platform = LegacyEPDPlatform(self.platform)
-            epd_platform = legacy_epd_platform._epd_platform
-
         args = {
             "name": self._raw_name,
             "version": self.upstream_version,
             "build": self.build,
             "python": self._python,
             "python_tag": self.python_tag,
             "abi_tag": self.abi_tag,
             "platform_tag": self.platform_tag,
             "platform_abi": self.platform_abi_tag,
             "packages": [six.text_type(p) for p in self.runtime_dependencies],
             "metadata_version": six.text_type(self.metadata_version),
         }
-        return LegacySpecDepend._from_data(args, epd_platform)
+        return LegacySpecDepend._from_data(args, self.platform)
 
     # Public methods
     def dump(self, path):
         """ Write the metadata to the given path as a metadata egg.
 
         A metadata egg is a zipfile using the same structured as an egg, except
         that it only contains metadata.
@@ -1052,19 +1035,17 @@
         Parameters
         ----------
         path : str
             The path to write the zipped metadata into.
         """
         with zipfile2.ZipFile(path, "w", zipfile2.ZIP_DEFLATED) as zp:
             zp.writestr(
-                _SPEC_DEPEND_LOCATION, self.spec_depend_string.encode()
-            )
+                _SPEC_DEPEND_LOCATION, self.spec_depend_string.encode())
             zp.writestr(
-                _SPEC_SUMMARY_LOCATION, self.summary.encode()
-            )
+                _SPEC_SUMMARY_LOCATION, self.summary.encode())
             if self.pkg_info:
                 self.pkg_info._dump_as_zip(zp)
 
     def to_json_dict(self):
         if self.platform is None:
             epd_platform = None
         else:
@@ -1076,27 +1057,23 @@
             _JSON_VERSION: six.text_type(self.version),
             _JSON_EPD_PLATFORM: epd_platform,
             _JSON_PYTHON_TAG: self.python_tag,
             _JSON_ABI_TAG: self.abi_tag,
             _JSON_PLATFORM_TAG: self.platform_tag,
             _JSON_PLATFORM_ABI_TAG: self.platform_abi_tag,
             _JSON_RUNTIME_DEPENDENCIES: [
-                six.text_type(p) for p in self.runtime_dependencies
-            ],
-            _JSON_SUMMARY: self.summary,
-        }
+                six.text_type(p) for p in self.runtime_dependencies],
+            _JSON_SUMMARY: self.summary}
 
     # Protocol implementations
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return (
                 self.spec_depend_string == other.spec_depend_string
                 and self.summary == other.summary
-                and self.pkg_info == other.pkg_info
-            )
+                and self.pkg_info == other.pkg_info)
         else:
             raise TypeError(
-                "Only equality between EggMetadata instances is supported"
-            )
+                "Only equality between EggMetadata instances is supported")
 
     def __ne__(self, other):
         return not self == other
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_package_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_package_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/_wheel_info.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/_wheel_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/egg.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/egg.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/legacy.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/legacy.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/file_formats/setuptools_egg.py` & `okonomiyaki-1.4.0/okonomiyaki/file_formats/setuptools_egg.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/common.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,117 +4,117 @@
 
 from okonomiyaki.utils.testing import MultiPatcher, Patcher
 
 
 # OS mocking
 # XXX: We need to patch platform.uname as well, as that function is cached, and
 # the result depend on sys.platform value.
-uname_result = collections.namedtuple("uname_result",
-                                      "system node release version machine "
-                                      "processor")
+uname_result = collections.namedtuple(
+    "uname_result",
+    "system node release version machine "
+    "processor")
 
 
 def _mock_uname(*args):
     if sys.version_info[0] == 2:
         return args
     else:
         return uname_result(*args)
 
 
 mock_darwin = MultiPatcher([
     mock.patch("sys.platform", "darwin"),
+    # These value are there to mask the running system values
     mock.patch("platform.uname",
                lambda: _mock_uname("Darwin", "localhost", "11.4.2",
                                    "Darwin Kernel Version 11.4.2 bla bla",
                                    "x86_64", "i386")),
 ])
 
 mock_linux = MultiPatcher([
     mock.patch("sys.platform", "linux2"),
+    # These value are there to mask the running system values
     mock.patch("platform.uname",
                lambda: _mock_uname("Linux", "localhost", "2.6.19-308.el5",
                                    "#1 SMP Tue Feb 21 20:06:06 EST 2012",
                                    "x86_64", "x86_64"))
 ])
 mock_solaris = MultiPatcher([
     mock.patch("sys.platform", "sunos5"),
+    # These value are there to mask the running system values
     mock.patch("platform.uname",
                lambda: _mock_uname("Solaris", "localhost", "fake",
                                    "fake", "x86_64", "x86_64")),
 ])
 mock_windows = MultiPatcher([
     mock.patch("sys.platform", "win32"),
+    # These value are there to mask the running system values
     mock.patch("platform.uname",
                lambda: _mock_uname('Windows', 'localhost', '7', '6.1.7601',
                                    'x86',
                                    ('x86 Family 6 Model 4 5 Stepping 7, '
                                     'GenuineIntel')))
 ])
 
 
-if sys.version_info < (3, 8):
-    def _mock_linux_distribution(info):
-        return Patcher(mock.patch("platform.linux_distribution", lambda: info))
-else:
-    def _mock_linux_distribution(info):
-        return Patcher(mock.patch("distro.linux_distribution", lambda: info))
+def _mock_linux_distribution(info):
+    return MultiPatcher([
+        mock_linux,
+        mock.patch("distro.linux_distribution", lambda: info[:3]),
+        mock.patch("distro.name", lambda: info[0]),
+        mock.patch("distro.version", lambda: info[1]),
+        mock.patch("distro.like", lambda: info[3])])
+
+
+mock_centos_3_5 = _mock_linux_distribution(("CentOS", "3.5", "Final", "rhel fedora"))
+mock_centos_5_8 = _mock_linux_distribution(("CentOS", "5.8", "Final", "rhel fedora"))
+mock_centos_6_3 = _mock_linux_distribution(("CentOS", "6.3", "Final", "rhel fedora"))
+mock_centos_7_0 = _mock_linux_distribution(("CentOS", "7.0", "Final", "rhel fedora"))
+mock_centos_7_6 = _mock_linux_distribution(("CentOS Linux", "7.6.1810", "Core", "rhel fedora"))
+mock_mydistro_2_8 = _mock_linux_distribution(("MyDistro", "2.8", "Final", "rhel fedora"))
+mock_rocky_8_8 = _mock_linux_distribution(("Rocky Linux", "8.8", "Green Obsidian", "rhel fedora"))
+mock_ubuntu_raring = _mock_linux_distribution(("Ubuntu", "13.04", "raring", "debian"))
 
-mock_centos_3_5 = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("CentOS", "3.5", "Final"))
-])
-
-mock_centos_5_8 = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("CentOS", "5.8", "Final"))
-])
-
-mock_centos_6_3 = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("CentOS", "6.3", "Final"))
-])
-
-mock_centos_7_0 = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("CentOS", "7.0", "Final"))
-])
-
-mock_centos_7_6 = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("CentOS Linux", "7.6.1810", "Core"))
+mock_windows_7 = MultiPatcher([
+    mock.patch("sys.platform", "win32"),
+    mock.patch("platform.win32_ver",
+               lambda: ("7", "6.1.7601", "SP1", "Multiprocessor Free"))
 ])
 
-mock_ubuntu_raring = MultiPatcher([
-    mock_linux,
-    _mock_linux_distribution(("Ubuntu", "13.04", "raring")),
+mock_windows_10 = MultiPatcher([
+    mock.patch("sys.platform", "win32"),
+    mock.patch("platform.win32_ver",
+               lambda: ('10', '10.0.19041', 'SP0', 'Multiprocessor Free'))
 ])
 
-mock_windows_7 = MultiPatcher([
+mock_windows_11 = MultiPatcher([
     mock.patch("sys.platform", "win32"),
     mock.patch("platform.win32_ver",
-               lambda: ("7", "6.1.7601", "SP1", "Multiprocessor Free"))
+               lambda: ('10', '10.0.22621', 'SP0', 'Multiprocessor Free'))
 ])
 
 mock_osx_10_7 = MultiPatcher([
     mock.patch("sys.platform", "darwin"),
     mock.patch("platform.mac_ver", lambda: ("10.7.5", ("", "", ""), "x86_64")),
 ])
 
+mock_osx_12_6 = MultiPatcher([
+    mock.patch("sys.platform", "darwin"),
+    mock.patch("platform.mac_ver", lambda: ("12.6.5", ("", "", ""), "x86_64")),
+])
+
 
 # Architecture mocking
 def mock_machine(machine):
     return Patcher(mock.patch("platform.machine", lambda: machine))
 
 
 mock_machine_x86 = Patcher(mock_machine("x86"))
 mock_architecture_32bit = Patcher(mock.patch("sys.maxsize", 2**32 - 1))
-
 mock_machine_x86_64 = Patcher(mock_machine("x86_64"))
 mock_architecture_64bit = Patcher(mock.patch("sys.maxsize", 2**64 - 1))
-
 mock_x86 = MultiPatcher([mock_machine_x86, mock_architecture_32bit])
 mock_x86_64 = MultiPatcher([mock_machine_x86_64, mock_architecture_64bit])
-# A 32 bits python process on a 64 bits OS
-mock_x86_on_x86_64 = MultiPatcher([mock_machine_x86_64,
-                                   mock_architecture_32bit])
-
 mock_machine_armv71 = Patcher(mock_machine("armv71"))
+# A 32 bits python process on a 64 bits OS
+mock_x86_on_x86_64 = MultiPatcher(
+    [mock_machine_x86_64, mock_architecture_32bit])
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test__arch.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test__arch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from okonomiyaki.errors import OkonomiyakiError
 from .._arch import Arch
 
-from .common import (mock_machine_armv71, mock_x86, mock_x86_64,
-                     mock_x86_on_x86_64)
+from .common import (
+    mock_machine_armv71, mock_x86, mock_x86_64, mock_x86_on_x86_64)
 
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_abi.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_abi.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,13 +36,20 @@
         abi = default_abi(*arguments)
 
         # then
         self.assertEqual(abi, EXAMPLE_RUNTIMES[arguments])
 
     @given(
         sampled_from([
-            ("win_x86", "cpython", "3.9.0+1"),
+            ("win_x86", "cpython", "3.12.0+1"),
             ("win_x86", "pypy", "4.1.0+1"),
             ("rh5_x86_64", "r", "3.0.0+1")]))
     def test_non_supported(self, arguments):
-        with self.assertRaises(OkonomiyakiError):
+        with self.assertRaises(OkonomiyakiError) as context:
             default_abi(*arguments)
+
+        message = str(context.exception)
+        self.assertNotIn('RuntimeVersion', message)
+        if arguments[1] == 'r':
+            self.assertIn('Unsupported implementation', message)
+        else:
+            self.assertIn('Platform', message)
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_epd_platform.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_epd_platform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-import mock
 import sys
 
 import six
 from hypothesis import given
 from hypothesis.strategies import sampled_from
 
 from okonomiyaki.errors import OkonomiyakiError
 from okonomiyaki.versions import RuntimeVersion
 
 from .. import EPDPlatform
 from ..epd_platform import (
-    _guess_epd_platform, EPD_PLATFORM_SHORT_NAMES, X86, X86_64, applies)
+    EPD_PLATFORM_SHORT_NAMES, X86, X86_64, applies)
 from ..legacy import _SUBDIR
 from .._platform import OSKind, FamilyKind, NameKind
-from .._arch import Arch
 
 from .common import (
     mock_architecture_32bit, mock_architecture_64bit, mock_centos_5_8,
     mock_centos_6_3, mock_darwin, mock_machine_x86, mock_machine_x86_64,
-    mock_solaris, mock_ubuntu_raring, mock_windows, mock_x86, mock_x86_64,
-    mock_centos_7_6
-)
+    mock_solaris, mock_ubuntu_raring, mock_x86, mock_x86_64,
+    mock_centos_7_6, mock_windows_10, mock_windows_11, mock_windows_7)
 
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
 
 
 class TestEPDPlatform(unittest.TestCase):
+
     def setUp(self):
-        self.platform_strings = tuple(
+        items = [
             platform + "-{0}".format(arch)
             for arch in ("x86", "x86_64")
-            for platform in ("osx", "win", "rh5")
-        )
+            for platform in ("osx", "win", "rh5")]
+        items = [
+            platform + "-x86_64"
+            for platform in ("rh6", "rh7", "rh8")]
+        self.platform_strings = tuple(items)
 
     def test_short_names_consistency(self):
         legacy_entries = tuple(sorted([entry[0] for entry in _SUBDIR]))
-
         self.assertEqual(EPD_PLATFORM_SHORT_NAMES, legacy_entries)
 
-    def test_epd_platform_from_string(self):
-        """Ensure every epd short platform is understood by EPDPlatform."""
+    def test_epd_platform_from_legacy_short_string(self):
         for epd_platform_string in EPD_PLATFORM_SHORT_NAMES:
-            EPDPlatform.from_string(epd_platform_string)
+            _, bits = epd_platform_string.split('-')
+            epd_platform = EPDPlatform.from_string(epd_platform_string)
+            self.assertEqual(epd_platform.short, epd_platform_string)
+            self.assertEqual(epd_platform.arch_bits, bits)
 
     def test_pep425_is_unicode(self):
         # When/Then
         for platform_string in self.platform_strings:
             platform = EPDPlatform.from_string(platform_string)
             self.assertIsInstance(platform.pep425_tag, six.text_type)
 
-    def test_platform_name(self):
+    def test_platform_name_is_unicode(self):
         # When/Then
         for platform_string in self.platform_strings:
             platform = EPDPlatform.from_string(platform_string)
             self.assertIsInstance(platform.platform_name, six.text_type)
 
     def test_str_is_unicode(self):
         # When/Then
@@ -65,86 +67,41 @@
             self.assertIsInstance(six.text_type(platform), six.text_type)
 
     def test_over_complete_strings(self):
         # When/Then
         with self.assertRaises(OkonomiyakiError):
             EPDPlatform.from_string("win_x86-64")
 
-    def test_epd_platform_from_string_new_names_underscore(self):
-        # Given
-        archs = ("i386", "x86", "i686")
-
-        # When
-        epd_platforms = tuple(
-            EPDPlatform.from_string("rh5_" + arch)
-            for arch in archs
-        )
-
-        # Then
-        for epd_platform in epd_platforms:
-            self.assertEqual(epd_platform.arch_bits, "32")
-
-        # Given
-        archs = ("amd64", "x86_64", "AMD64")
-
-        # When
-        epd_platforms = tuple(
-            EPDPlatform.from_string("rh5_" + arch)
-            for arch in archs
-        )
-
-        # Then
-        for epd_platform in epd_platforms:
-            self.assertEqual(epd_platform.arch_bits, "64")
-
-        # Given
-        s = "win_x86_64"
-
-        # When
-        epd_platform = EPDPlatform.from_string(s)
-
-        # Then
-        self.assertEqual(epd_platform, EPDPlatform.from_string("win-64"))
-
-        # Given
-        s = "osx_x86_64"
-
-        # When
-        epd_platform = EPDPlatform.from_string(s)
-
-        # Then
-        self.assertEqual(epd_platform, EPDPlatform.from_string("osx-64"))
-
     def test_epd_platform_from_string_new_names(self):
         """Ensure every epd short platform is understood by EPDPlatform."""
         # Given
         archs = ("i386", "x86", "i686")
 
         # When
         epd_platforms = tuple(
             EPDPlatform.from_string("rh5-" + arch)
-            for arch in archs
-        )
+            for arch in archs)
 
         # Then
         for epd_platform in epd_platforms:
             self.assertEqual(epd_platform.arch_bits, "32")
+            self.assertEqual(epd_platform.platform_name, "rh5")
 
         # Given
         archs = ("amd64", "x86_64", "AMD64")
 
         # When
         epd_platforms = tuple(
-            EPDPlatform.from_string("rh5-" + arch)
-            for arch in archs
-        )
+            EPDPlatform.from_string("win-" + arch)
+            for arch in archs)
 
         # Then
         for epd_platform in epd_platforms:
             self.assertEqual(epd_platform.arch_bits, "64")
+            self.assertEqual(epd_platform.platform_name, "win")
 
     def test_epd_platform_from_string_with_runtime_version(self):
         # given
         version = RuntimeVersion.from_string('3.6.5+6')
 
         # when/then
         epd_platform = EPDPlatform.from_string('osx-64', version)
@@ -152,113 +109,192 @@
         epd_platform = EPDPlatform.from_string('win-64', version)
         self.assertEqual(epd_platform.platform.release, '')
 
         # given
         version = RuntimeVersion.from_string('3.8.8+2')
 
         # when/then
-        epd_platform = EPDPlatform.from_string('osx-64', version)
+        epd_platform = EPDPlatform.from_string('osx-x86_64', version)
         self.assertEqual(epd_platform.platform.release, '10.14')
-        epd_platform = EPDPlatform.from_string('win-64', version)
+        epd_platform = EPDPlatform.from_string('win-x86_64', version)
+        self.assertEqual(epd_platform.platform.release, '10')
+
+        # given
+        version = RuntimeVersion.from_string('3.11.2+5')
+
+        # when/then
+        epd_platform = EPDPlatform.from_string('osx-x86_64', version)
+        self.assertEqual(epd_platform.platform.release, '12.0')
+        epd_platform = EPDPlatform.from_string('win-x86_64', version)
         self.assertEqual(epd_platform.platform.release, '10')
 
     @mock_darwin
     @mock_machine_x86_64
-    def test_from_running_python(self):
+    def test_from_running_python_darwin(self):
         # When
         with mock_architecture_32bit:
-            platform = EPDPlatform.from_running_python()
+            epd_platform = EPDPlatform.from_running_python()
 
         # Then
-        self.assertEqual(platform.short, "osx-32")
+        self.assertEqual(str(epd_platform), "osx_x86")
 
         # When
         with mock_architecture_64bit:
-            platform = EPDPlatform.from_running_python()
+            epd_platform = EPDPlatform.from_running_python()
 
         # Then
-        self.assertEqual(platform.short, "osx-64")
-
-    @mock_darwin
-    @mock_machine_x86_64
-    def test_from_running_system(self):
-        # When
-        with mock_architecture_32bit:
-            platform = EPDPlatform.from_running_system()
+        self.assertEqual(str(epd_platform), "osx_x86_64")
 
-        # Then
-        self.assertEqual(platform.short, "osx-64")
+    @mock_windows_7
+    def test_from_running_system_windows_7(self):
+        with mock_machine_x86:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # When
-        with mock_architecture_64bit:
-            platform = EPDPlatform.from_running_system()
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # Then
-        self.assertEqual(platform.short, "osx-64")
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system('AMD64')
 
-    def test_epd_platform_from_string_new_arch(self):
-        def old_to_new_name(epd_platform_string):
-            left, right = epd_platform_string.split("-")
-            return "{0}-{1}".format(left, {"32": X86, "64": X86_64}[right])
+        with mock_machine_x86_64:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86_64")
 
-        # Given
-        name_to_platform = {}
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # When
-        for old_name in EPD_PLATFORM_SHORT_NAMES:
-            new_name = old_to_new_name(old_name)
-            name_to_platform[old_name] = EPDPlatform.from_string(new_name)
+    @mock_windows_10
+    def test_from_running_system_windows_10(self):
+        with mock_machine_x86:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # Then
-        for old_name in name_to_platform:
-            self.assertEqual(name_to_platform[old_name].short, old_name)
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
-    def test_guessed_epd_platform(self):
-        with mock_centos_5_8:
-            epd_platform = EPDPlatform.from_running_system("x86")
-            self.assertEqual(epd_platform.short, "rh5-32")
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system('AMD64')
 
-            epd_platform = EPDPlatform.from_running_system("amd64")
-            self.assertEqual(epd_platform.short, "rh5-64")
+        with mock_machine_x86_64:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86_64")
 
-        with mock_centos_7_6:
-            epd_platform = EPDPlatform.from_running_system("amd64")
-            self.assertEqual(epd_platform.short, "rh7-64")
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
-    def test_str(self):
-        # Given
-        epd_platform = EPDPlatform.from_string("rh5-64")
+    @mock_windows_11
+    def test_from_running_system_windows_11(self):
+        with mock_machine_x86:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # When/Then
-        self.assertEqual(str(epd_platform), "rh5_x86_64")
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
-        # Given
-        epd_platform = EPDPlatform.from_string("osx-32")
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system('AMD64')
 
-        # When/Then
-        self.assertEqual(str(epd_platform), "osx_x86")
-        self.assertEqual(six.text_type(epd_platform), u"osx_x86")
-        self.assertIsInstance(six.text_type(epd_platform), six.text_type)
+        with mock_machine_x86_64:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "win_x86_64")
 
-        # Given
-        s = "osx_x86"
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "win_x86")
 
+    @mock_darwin
+    def test_from_running_system_darwin(self):
+        with mock_machine_x86:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "osx_x86")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system("x86")
+            self.assertEqual(str(epd_platform), "osx_x86")
+            # When/Then
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system("amd64")
         # When
-        epd_platform = EPDPlatform.from_string(s)
+        with mock_machine_x86_64:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "osx_x86_64")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86_64')
+            self.assertEqual(str(epd_platform), "osx_x86_64")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "osx_x86")
 
-        # Then
-        self.assertEqual(str(epd_platform), s)
+    @mock_centos_5_8
+    def test_from_running_system_centos_5(self):
+        with mock_machine_x86:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh5_x86")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh5_x86")
+            # When/Then
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system('x86_64')
+
+        with mock_machine_x86_64:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh5_x86_64")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh5_x86")
+
+    @mock_centos_6_3
+    def test_from_running_system_centos_6(self):
+        with mock_machine_x86:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh6_x86")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh6_x86")
+            # When/Then
+            with self.assertRaises(OkonomiyakiError):
+                EPDPlatform.from_running_system('x86_64')
+
+        with mock_machine_x86_64:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh6_x86_64")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh6_x86")
+
+    @mock_centos_7_6
+    def test_from_running_system_centos_7(self):
+        with mock_machine_x86:
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh7_x86")
+            # When/Then
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh7_x86")
+
+        with mock_machine_x86_64:
+            epd_platform = EPDPlatform.from_running_system()
+            self.assertEqual(str(epd_platform), "rh7_x86_64")
+            epd_platform = EPDPlatform.from_running_system('x86')
+            self.assertEqual(str(epd_platform), "rh7_x86")
 
     @given(sampled_from((
         ("rh5_x86", None, "linux_i686"),
         ("rh5_x86_64", None, "linux_x86_64"),
         ("osx_x86", None, "macosx_10_6_i386"),
         ("osx_x86", '3.8.9+1', "macosx_10_14_i386"),
         ("osx_x86_64", None, "macosx_10_6_x86_64"),
         ("osx_x86_64", '3.8.9+1', "macosx_10_14_x86_64"),
+        ("osx_x86_64", '3.11.2+1', "macosx_12_0_x86_64"),
         ("win_x86", None, "win32"),
         ("win_x86_64", None, "win_amd64"),
         ("win_x86_64", '3.9.1', "win_amd64"))))
     def test_pep425_tag(self, arguments):
         # Given
         platform_tag, version, expected = arguments
         if version is not None:
@@ -282,14 +318,15 @@
         ('darwin', None, 'amd64', 'osx_10_9_x86_64', 'cp36', 'darwin'),
         ('darwin', None, 'amd64', 'osx_10_14_x86_64', 'cp38', 'darwin'),
         ('win32', None, 'x86', 'win32', 'cp27', 'msvc2008'),
         ('win32', None, 'amd64', 'win_amd64', 'cp27', 'msvc2008'),
         ('win32', None, 'x86', 'win32', 'cp36', 'msvc2015'),
         ('win32', None, 'amd64', 'win_amd64', 'cp36', 'msvc2015'),
         ('win32', None, 'x86', 'win32', 'cp38', 'msvc2019'),
+        ('win32', None, 'amd64', 'win32', 'cp311', 'msvc2022'),
         ('win32', None, 'amd64', 'win_amd64', 'cp38', 'msvc2019'),
     )))
     def test_from_spec_depend_data(self, arguments):
         # when
         epd_platform = EPDPlatform._from_spec_depend_data(*arguments)
         platform, osdist, arch_name, platform_tag, python_version, platform_abi = arguments
 
@@ -378,17 +415,33 @@
             self.assertTrue(applies("rh5-32", "current"))
             self.assertFalse(applies("!rh5-32", "current"))
 
         with mock_x86_64:
             self.assertTrue(applies("rh5-64", "current"))
             self.assertFalse(applies("!rh5-64", "current"))
 
-    @mock_windows
+    @mock_windows_7
+    @mock_x86
+    def test_current_windows_7(self):
+        for platform in ("rh5", "rh", "osx-32"):
+            self.assertFalse(applies(platform, "current"))
+        for platform in ("win", "win-32"):
+            self.assertTrue(applies(platform, "current"))
+
+    @mock_windows_10
+    @mock_x86
+    def test_current_windows_10(self):
+        for platform in ("rh5", "rh", "osx-32"):
+            self.assertFalse(applies(platform, "current"))
+        for platform in ("win", "win-32"):
+            self.assertTrue(applies(platform, "current"))
+
+    @mock_windows_11
     @mock_x86
-    def test_current_windows(self):
+    def test_current_windows_11(self):
         for platform in ("rh5", "rh", "osx-32"):
             self.assertFalse(applies(platform, "current"))
         for platform in ("win", "win-32"):
             self.assertTrue(applies(platform, "current"))
 
     @mock_centos_5_8
     @mock_x86
@@ -397,156 +450,55 @@
         self.assertTrue(applies("rh5-64", "rh5"))
         self.assertFalse(applies("win-64", "rh5"))
         self.assertFalse(applies("rh6-64", "rh5"))
         self.assertTrue(applies("rh5-32", "rh"))
         self.assertTrue(applies("rh6-32", "rh"))
         self.assertFalse(applies("win-32", "rh"))
 
-
-class TestGuessEPDPlatform(unittest.TestCase):
-    @mock_windows
-    def test_guess_win32_platform(self):
-        epd_platform = _guess_epd_platform(Arch.from_name("x86"))
-        self.assertEqual(epd_platform.short, "win-32")
-
-        epd_platform = _guess_epd_platform(Arch.from_name("amd64"))
-        self.assertEqual(epd_platform.short, "win-64")
-
-    @mock_darwin
-    def test_guess_darwin_platform(self):
-        # When
-        with mock_machine_x86:
-            epd_platform = _guess_epd_platform(Arch.from_name("x86"))
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-32")
-
-        # When
-        with mock_machine_x86:
-            epd_platform = _guess_epd_platform(Arch.from_name("amd64"))
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-64")
-
-        # When
-        with mock_machine_x86:
-            with mock_architecture_32bit:
-                epd_platform = _guess_epd_platform()
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-32")
-
-        # When
-        with mock_machine_x86:
-            with mock_architecture_64bit:
-                epd_platform = _guess_epd_platform()
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-64")
-
-        # When
-        with mock_machine_x86_64:
-            with mock_architecture_64bit:
-                epd_platform = _guess_epd_platform()
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-64")
-
-        # When
-        with mock_machine_x86_64:
-            with mock_architecture_32bit:
-                epd_platform = _guess_epd_platform()
-
-        # Then
-        self.assertEqual(epd_platform.short, "osx-32")
-
-    def test_guess_linux2_platform(self):
-        with mock_centos_5_8:
-            epd_platform = _guess_epd_platform(Arch.from_name("x86"))
-            self.assertEqual(epd_platform.short, "rh5-32")
-
-            epd_platform = _guess_epd_platform(Arch.from_name("amd64"))
-            self.assertEqual(epd_platform.short, "rh5-64")
-
-            with mock.patch("platform.machine", lambda: "x86"):
-                with mock_architecture_32bit:
-                    epd_platform = _guess_epd_platform()
-                    self.assertEqual(epd_platform.short, "rh5-32")
-
-            with mock.patch("platform.machine", lambda: "i386"):
-                with mock_architecture_32bit:
-                    epd_platform = _guess_epd_platform()
-                    self.assertEqual(epd_platform.short, "rh5-32")
-
-            with mock.patch("platform.machine", lambda: "i686"):
-                with mock_architecture_32bit:
-                    epd_platform = _guess_epd_platform()
-                    self.assertEqual(epd_platform.short, "rh5-32")
-
-            with mock.patch("platform.machine", lambda: "x86_64"):
-                with mock_architecture_32bit:
-                    epd_platform = _guess_epd_platform()
-                    self.assertEqual(epd_platform.short, "rh5-32")
-
-            with mock.patch("platform.machine", lambda: "x86_64"):
-                with mock_architecture_64bit:
-                    epd_platform = _guess_epd_platform()
-                    self.assertEqual(epd_platform.short, "rh5-64")
-
-        with mock_centos_6_3:
-            epd_platform = _guess_epd_platform(Arch.from_name("x86"))
-            self.assertEqual(epd_platform.short, "rh6-32")
-
-            epd_platform = _guess_epd_platform(Arch.from_name("amd64"))
-            self.assertEqual(epd_platform.short, "rh6-64")
-
-        with mock_centos_7_6:
-            epd_platform = _guess_epd_platform(Arch.from_name("amd64"))
-            self.assertEqual(epd_platform.short, "rh7-64")
-
     def test_guess_linux2_unsupported(self):
         with mock_ubuntu_raring:
             with self.assertRaises(OkonomiyakiError):
-                _guess_epd_platform()
+                EPDPlatform.from_running_system()
 
     @mock_solaris
     def test_guess_solaris_unsupported(self):
-        self.assertRaises(OkonomiyakiError, _guess_epd_platform)
+        with self.assertRaises(OkonomiyakiError):
+            EPDPlatform.from_running_system()
 
     def test_from_epd_platform_string(self):
         # Given
-        epd_platform_string = "rh5-32"
+        epd_platform_string = "rh5-x86"
 
         # When
         epd_platform = EPDPlatform.from_string(epd_platform_string)
 
         # Then
         platform = epd_platform.platform
         self.assertEqual(platform.os_kind, OSKind.linux)
         self.assertEqual(platform.family_kind, FamilyKind.rhel)
         self.assertEqual(platform.name_kind, NameKind.rhel)
         self.assertEqual(platform.arch, X86)
         self.assertEqual(platform.machine, X86)
 
         # Given
-        epd_platform_string = "win-32"
+        epd_platform_string = "win-x86"
 
         # When
         epd_platform = EPDPlatform.from_string(epd_platform_string)
 
         # Then
         platform = epd_platform.platform
         self.assertEqual(platform.os_kind, OSKind.windows)
         self.assertEqual(platform.family_kind, FamilyKind.windows)
         self.assertEqual(platform.name_kind, NameKind.windows)
         self.assertEqual(platform.arch, X86)
         self.assertEqual(platform.machine, X86)
 
         # Given
-        epd_platform_string = "osx-64"
+        epd_platform_string = "osx-x86_64"
 
         # When
         epd_platform = EPDPlatform.from_string(epd_platform_string)
         platform = epd_platform.platform
 
         # Then
         self.assertEqual(platform.os_kind, OSKind.darwin)
@@ -579,27 +531,26 @@
         # When/Then
         with self.assertRaises(OkonomiyakiError):
             EPDPlatform.from_string(epd_platform_string)
 
     def test_from_platform_tag(self):
         # Given
         inputs_outputs = (
-            ("linux_i686", "rh5-32"),
-            ("linux_i386", "rh5-32"),
-            ("linux_x86_64", "rh5-64"),
-            ("win32", "win-32"),
-            ("win_amd64", "win-64"),
-            ("macosx_10_6_x86_64", "osx-64"),
-            ("macosx_10_6_i386", "osx-32"),
+            ("linux_i686", "rh5_x86"),
+            ("linux_i386", "rh5_x86"),
+            ("linux_x86_64", "rh5_x86_64"),
+            ("win32", "win_x86"),
+            ("win_amd64", "win_x86_64"),
+            ("macosx_10_6_x86_64", "osx_x86_64"),
         )
 
         # When/Then
         for platform_tag, epd_string in inputs_outputs:
             platform = EPDPlatform._from_platform_tag(platform_tag)
-            self.assertEqual(platform.short, epd_string)
+            self.assertEqual(str(platform), epd_string)
 
         # When/Then
         with self.assertRaises(NotImplementedError):
             EPDPlatform._from_platform_tag("openbsd_i386")
 
         with self.assertRaises(ValueError):
             EPDPlatform._from_platform_tag("any")
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_pep425.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_pep425.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import unittest
+import re
 
 from packaging import tags
 
 from ..pep425 import compute_abi_tag, compute_python_tag, compute_platform_tag
 
 
 def _system_tags():
@@ -20,14 +21,16 @@
 
     def setUp(self):
         self.tag = next(
             tag for tag in
             _system_tags()
             # We do not support the manylinux tag
             if 'manylinux' not in tag.platform)
+        self.compatible_platforms = tuple(
+            tag.platform for tag in _system_tags())
 
     def test_abi_tag(self):
         # Given
         executable = sys.executable
 
         # When
         abi_tag = compute_abi_tag(executable)
@@ -63,15 +66,26 @@
         # Given
         executable = sys.executable
 
         # When
         platform_tag = compute_platform_tag(executable)
 
         # Then
-        self.assertEqual(platform_tag, self.tag.platform)
+        if sys.platform.startswith('darwin'):
+            # packaging always sets the minor macos version to 0
+            platform_tag = re.sub('macosx_11_.', 'macosx_11_0', platform_tag)
+            platform_tag = re.sub('macosx_12_.', 'macosx_12_0', platform_tag)
+        else:
+            self.assertIn(platform_tag, self.compatible_platforms)
 
     def test_platform_tag_default(self):
         # When
         platform_tag = compute_platform_tag()
 
         # Then
-        self.assertEqual(platform_tag, self.tag.platform)
+        # Then
+        if sys.platform.startswith('darwin'):
+            # packaging always sets the minor macos version to 0
+            platform_tag = re.sub('macosx_11_.', 'macosx_11_0', platform_tag)
+            platform_tag = re.sub('macosx_12_.', 'macosx_12_0', platform_tag)
+        else:
+            self.assertIn(platform_tag, self.compatible_platforms)
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/tests/test_platform_filters.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/tests/test_platform_filters.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/_arch.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/_arch.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,7 +103,11 @@
         if self._kind == ArchitectureKind.x86_64:
             return "amd64"
         else:
             return self.name
 
     def __str__(self):
         return self.name
+
+
+X86 = Arch(ArchitectureKind.x86)
+X86_64 = Arch(ArchitectureKind.x86_64)
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/_pep425_impl.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/_pep425_impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 _PEP425_IMPL = '''\
 from __future__ import absolute_import, print_function
 
 import sys
 import sysconfig
+import subprocess
 
 
 def get_config_var(var):
     try:
         return sysconfig.get_config_var(var)
     except IOError:
         return None
@@ -99,35 +100,20 @@
     return sys.maxsize == 2147483647
 
 
 def get_platform():
     import distutils.util
     import platform
     """Return our platform name 'win32', 'linux_x86_64'"""
-    if sys.platform == 'darwin':
-        # distutils.util.get_platform() returns the release based on the value
-        # of MACOSX_DEPLOYMENT_TARGET on which Python was built, which may
-        # be significantly older than the user's current machine.
-        release, _, machine = platform.mac_ver()
-        split_ver = release.split('.')
-
-        if machine == "x86_64" and _is_running_32bit():
-            machine = "i386"
-        elif machine == "ppc64" and _is_running_32bit():
-            machine = "ppc"
 
-        return 'macosx_{0}_{1}_{2}'.format(split_ver[0], split_ver[1], machine)
-
-    # XXX remove distutils dependency
     result = distutils.util.get_platform().replace('.', '_').replace('-', '_')
     if result == "linux_x86_64" and _is_running_32bit():
         # 32 bit Python program (running on a 64 bit Linux): pip should only
         # install and run 32 bit compiled extensions in that case.
         result = "linux_i686"
-
     return result
 
 
 if __name__ == "__main__":
     import argparse
 
     p = argparse.ArgumentParser()
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/_platform.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/_platform.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import absolute_import
 
 import platform
 import sys
+import subprocess
 
 import enum
 import six
-
 from attr import attr, attributes
 from attr.validators import instance_of
 
 from okonomiyaki.errors import OkonomiyakiError
+from okonomiyaki.versions import SemanticVersion
 
-from ._arch import Arch
+from ._arch import Arch, X86
 
 
 @enum.unique
 class OSKind(enum.Enum):
     darwin = 0
     linux = 1
     solaris = 2
@@ -29,30 +30,34 @@
     mac_os_x = 2
     windows = 3
     solaris = 4
 
 
 @enum.unique
 class NameKind(enum.Enum):
+    unknown = -1
     centos = 0
     debian = 1
     rhel = 2
     ubuntu = 3
     mac_os_x = 4
     windows = 5
     solaris = 6
+    rocky = 7
 
 
 NAME_KIND_TO_PRETTY_NAMES = {
     NameKind.windows: "Windows",
     NameKind.mac_os_x: "Mac OS X",
     NameKind.centos: "CentOS",
     NameKind.rhel: "RedHat",
     NameKind.ubuntu: "Ubuntu",
     NameKind.debian: "Debian",
+    NameKind.unknown: "Unknown distribution",
+    NameKind.rocky: "Rocky Linux",
 }
 
 
 @six.python_2_unicode_compatible
 @attributes(repr=False, frozen=True)
 class Platform(object):
     """
@@ -93,26 +98,31 @@
     """
 
     @classmethod
     def from_running_python(cls):
         """ Guess the platform, using the running python to guess the
         architecture.
         """
-        return _guess_platform()
+        arch = Arch.from_running_python()
+        return _guess_platform(arch)
 
     @classmethod
     def from_running_system(cls, arch_string=None):
         """ Guess the platform, with an optional architecture string.
 
         Parameters
         ----------
         arch_string: str, None
             If given, should be a valid architecture name (e.g. 'x86')
         """
-        return _guess_platform(arch_string)
+        if arch_string is None:
+            arch = Arch.from_running_system()
+        else:
+            arch = Arch.from_name(arch_string)
+        return _guess_platform(arch)
 
     @property
     def family(self):
         return self.family_kind.name
 
     @property
     def name(self):
@@ -121,22 +131,20 @@
     @property
     def os(self):
         return self.os_kind.name
 
     def __repr__(self):
         return (
             "Platform(os={0.os!r}, name={0.name!r}, family={0.family!r}, "
-            "release='{0.release}', arch='{0.arch}', machine='{0.machine}')".format(self)
-        )
+            "release='{0.release}', arch='{0.arch}', machine='{0.machine}')".format(self))
 
     def __str__(self):
         return u"{0} {1.release} on {1.machine}".format(
             NAME_KIND_TO_PRETTY_NAMES[self.name_kind],
-            self
-        )
+            self)
 
 
 def _guess_os_kind():
     if sys.platform == "win32":
         return OSKind.windows
     elif sys.platform == "darwin":
         return OSKind.darwin
@@ -145,54 +153,80 @@
     else:
         msg = "Could not guess platform from sys.platform: {0!r}"
         raise OkonomiyakiError(msg.format(sys.platform))
 
 
 def _guess_platform_details(os_kind):
     if os_kind == OSKind.windows:
-        return FamilyKind.windows, NameKind.windows, platform.win32_ver()[0]
+        return FamilyKind.windows, NameKind.windows, _windows_version()
     elif os_kind == OSKind.darwin:
-        return FamilyKind.mac_os_x, NameKind.mac_os_x, platform.mac_ver()[0]
+        return FamilyKind.mac_os_x, NameKind.mac_os_x, _macos_release()
     elif os_kind == OSKind.linux:
-        name, release = _linux_distribution()
+        name, release, like = _linux_distribution()
         try:
             name_kind = NameKind[name]
         except KeyError:
-            raise OkonomiyakiError(
-                "Unsupported platform: {0!r}".format(name)
-            )
-        else:
-            if name_kind in (NameKind.ubuntu, NameKind.debian):
-                family_kind = FamilyKind.debian
-            elif name_kind in (NameKind.centos, NameKind.rhel):
-                family_kind = FamilyKind.rhel
+            for name in like:
+                try:
+                    name_kind = NameKind[name]
+                except KeyError:
+                    continue
+                else:
+                    name_kind = NameKind.unknown
+                    break
             else:
-                raise OkonomiyakiError("Unsupported platform: {0!r}".format(name))
-            return family_kind, name_kind, release
+                raise OkonomiyakiError(
+                    "Unsupported platform: {0!r}".format(name))
 
+        if name_kind in (NameKind.ubuntu, NameKind.debian):
+            family_kind = FamilyKind.debian
+        elif name_kind in (NameKind.centos, NameKind.rhel, NameKind.rocky):
+            family_kind = FamilyKind.rhel
+        elif name_kind == NameKind.unknown and 'rhel' in like:
+            family_kind = FamilyKind.rhel
+        elif name_kind == NameKind.unknown and 'debian' in like:
+            family_kind = FamilyKind.debian
+        else:
+            raise OkonomiyakiError("Unsupported platform: {0!r}".format(name))
+        return family_kind, name_kind, release
 
-def _guess_platform(arch_string=None):
-    if arch_string is None:
-        arch = Arch.from_running_python()
-    else:
-        arch = Arch.from_name(arch_string)
 
+def _guess_platform(arch):
     machine = Arch.from_running_system()
+    if machine == X86 and arch.bits == 64:
+        raise OkonomiyakiError("Incompatible 32bit machine with a 64bit architecture")
     os_kind = _guess_os_kind()
     family_kind, name_kind, release = _guess_platform_details(os_kind)
-
     return Platform(os_kind, name_kind, family_kind, release, arch, machine)
 
 
 def _linux_distribution():
     """ Get the linux distribution of the running system.
 
     """
-    try:
-        name, release, _ = platform.linux_distribution()
-    except AttributeError:
-        # We are probably running on Python > 3.8
-        # see https://docs.python.org/3.6/library/platform.html?highlight=linux_distribution#unix-platforms
-        import distro
-        name, release, _ = distro.linux_distribution()
+    import distro
+    name = distro.name()
+    release = distro.version()
+    like = distro.like().lower()
     name = name.split()[0]
-    return name.lower(), release
+    return name.lower(), release, like.split()
+
+
+def _macos_release():
+    release = platform.mac_ver()[0]
+    if release == '10.16':
+        # need to verify since sometimes python reports a compatibility version
+        cmd = [
+            sys.executable, '-sS', '-c',
+            'import platform; print(platform.mac_ver()[0])']
+        release = subprocess.check_output(
+            cmd, env={"SYSTEM_VERSION_COMPAT": "0"},
+            universal_newlines=True).strip()
+    return release
+
+
+def _windows_version():
+    version, release, _, _ = platform.win32_ver()
+    release = SemanticVersion.from_string(release)
+    if release > SemanticVersion.from_string('10.0.22000'):
+        version = '11'
+    return version
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/abi.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,16 @@
             return _PLATFORM_ABI_NONE
         else:
             return abi.pep425_tag
 
 
 def _default_cpython_abi(platform, implementation_version):
     msg = (
-        "Unsupported platform/version combo for cpython: {0!r}/{1!r}".
-        format(platform, implementation_version)
-    )
+        "Unsupported combo of {0!r} and cpython version {1!s}".
+        format(platform, implementation_version))
 
     if platform.os_kind == OSKind.darwin:
         return u"darwin"
     elif platform.os_kind == OSKind.linux:
         return u"gnu"
     elif platform.os_kind == OSKind.windows:
         abi = None
@@ -44,14 +43,16 @@
                 abi = u"msvc2008"
             elif implementation_version.minor <= 4:
                 abi = u"msvc2010"
             elif implementation_version.minor <= 6:
                 abi = u"msvc2015"
             elif implementation_version.minor <= 8:
                 abi = u"msvc2019"
+            elif implementation_version.minor <= 11:
+                abi = u"msvc2022"
 
         if abi is None:
             raise OkonomiyakiError(msg)
 
         return abi
     else:
         raise OkonomiyakiError(msg)
@@ -112,9 +113,8 @@
             return u"gnu"
         elif platform.os_kind == OSKind.darwin:
             return u"darwin"
         else:
             raise OkonomiyakiError(msg)
     else:
         raise OkonomiyakiError(
-            "Unsupported implementation: {0!r}".format(implementation)
-        )
+            "Unsupported implementation: {0!r}".format(implementation))
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/epd_platform.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/epd_platform.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import six
 
 from attr import attributes, attr
 from attr.validators import instance_of
 
 from okonomiyaki.versions import RuntimeVersion
 from okonomiyaki.errors import OkonomiyakiError, InvalidPEP440Version
-from ._arch import Arch, ArchitectureKind
+from ._arch import Arch, ArchitectureKind, X86, X86_64
 from ._platform import OSKind, FamilyKind, NameKind, Platform
 
 # the string used in EGG-INFO/spec/depend. Only used during normalization
 # operations.
 _X86_64_LEGACY_SPEC = "amd64"
 
 # Those lists are redundant with legacy spec. We check the consistency in our
@@ -22,23 +22,21 @@
 _ARCHBITS_TO_ARCH = {
     "32": ArchitectureKind.x86.name,
     "64": _X86_64_LEGACY_SPEC,
     ArchitectureKind.x86: ArchitectureKind.x86.name,
     ArchitectureKind.x86_64: _X86_64_LEGACY_SPEC,
 }
 
-X86 = Arch(ArchitectureKind.x86)
-X86_64 = Arch(ArchitectureKind.x86_64)
-
 PLATFORM_NAMES = (
     "osx",
     "rh3",
     "rh5",
     "rh6",
     "rh7",
+    "rh8",
     "sol",
     "win",
 )
 
 EPD_PLATFORM_SHORT_NAMES = (
     "osx-32",
     "osx-64",
@@ -72,16 +70,15 @@
 
 
 def platform_validator():
     def wrapper(inst, attr, value):
         instance_of(Platform)(inst, attr, value)
         if not _is_supported(value):
             raise OkonomiyakiError(
-                "Platform {0} not supported".format(value)
-            )
+                "Platform {0} not supported by EPD".format(value))
     return wrapper
 
 
 @six.python_2_unicode_compatible
 @attributes(frozen=True)
 class EPDPlatform(object):
     """
@@ -106,36 +103,33 @@
             return _ANY_PLATFORM_STRING
         else:
             return platform.pep425_tag
 
     @classmethod
     def from_running_python(cls):
         """
-        Attempt to create an EPDPlatform instance by guessing the running
+        Attempt to create an EPDPlatform instance based on the running
         python. May raise an OkonomiyakiError exception
         """
         return cls(Platform.from_running_python())
 
     @classmethod
     def from_running_system(cls, arch_name=None):
         """
-        Attempt to create an EPDPlatform instance by guessing the running
-        platform. May raise an OkonomiyakiError exception
+        Attempt to create an EPDPlatform instance based on the running platform.
+        May raise an OkonomiyakiError exception
 
         Parameters
         ----------
         arch_name: str, None
             If given, must be a valid architecture string (e.g. 'x86'). If
             None, will be guessed from the running platform.
         """
-        if arch_name is not None:
-            arch = Arch.from_name(arch_name)
-        else:
-            arch = Arch.from_running_system()
-        return _guess_epd_platform(arch)
+        platform = Platform.from_running_system(arch_name)
+        return cls(platform)
 
     @classmethod
     def from_string(cls, s, runtime_version=None):
         """ Create a new instance from an epd platform string.
 
         Parameters:
         s : string
@@ -169,16 +163,15 @@
         """
         Create a new instance from an epd platform string (e.g. 'win-32')
 
         DEPRECATED: use from_string instead.
         """
         warnings.warn(
             "Deprecated: use EPDPlatform.from_string instead",
-            DeprecationWarning
-        )
+            DeprecationWarning)
         return cls.from_string(s, runtime_version)
 
     @classmethod
     def _from_spec_depend_data(
             cls, platform, osdist, arch_name,
             platform_tag, python_version, platform_abi):
         msg = ("Unrecognized platform/osdist combination: {0!r}/{1!r}"
@@ -193,14 +186,16 @@
                 epd_name = "rh3"
             elif osdist in (None, "RedHat_5"):
                 epd_name = "rh5"
             elif osdist == "RedHat_6":
                 epd_name = "rh6"
             elif osdist == "RedHat_7":
                 epd_name = "rh7"
+            elif osdist == "RedHat_8":
+                epd_name = "rh8"
             else:
                 raise ValueError(msg)
         else:
             raise ValueError(msg)
 
         if python_version is not None:
             try:
@@ -222,16 +217,15 @@
     @classmethod
     def _from_platform_tag(cls, platform_tag):
         """
         Attempt to create an EPDPlatform instance from a PEP 425 platform tag.
         """
         if platform_tag is None or platform_tag == _ANY_PLATFORM_STRING:
             raise ValueError(
-                "Invalid platform_tag for platform: '{}'".format(platform_tag)
-            )
+                "Invalid platform_tag for platform: '{}'".format(platform_tag))
         else:
             if platform_tag.startswith("linux"):
                 m = _LINUX_TAG_R.match(platform_tag)
                 assert m, platform_tag
                 arch_string = m.group("arch")
                 epd_string = u"rh5_" + str(Arch.from_name(arch_string))
             elif platform_tag.startswith("macosx"):
@@ -245,16 +239,15 @@
                 arch_string = m.group("arch")
                 if arch_string == "32":
                     epd_string = u"win_i386"
                 else:
                     epd_string = u"win_" + str(Arch.from_name(arch_string))
             else:
                 raise NotImplementedError(
-                    "Unsupported platform '{0}'".format(platform_tag)
-                )
+                    "Unsupported platform '{0}'".format(platform_tag))
 
             return cls.from_epd_string(epd_string)
 
     @property
     def arch(self):
         return self.platform.arch
 
@@ -263,15 +256,15 @@
         """
         The number of bits (as a string) of this epd platform.
         """
         return self.arch._arch_bits
 
     @property
     def pep425_tag(self):
-        msg = "Cannot guess platform tag for platform {0!r}"
+        msg = "Cannot generate pep425 tag for platform {0!r}"
 
         platform = self.platform
         if platform.os_kind == OSKind.darwin:
             release = platform.release.replace('.', '_')
             if platform.arch == X86:
                 return u"macosx_{}_i386".format(release)
             elif platform.arch == X86_64:
@@ -311,14 +304,16 @@
                     base = u"rh3"
                 elif parts[0] == "5":
                     base = u"rh5"
                 elif parts[0] == "6":
                     base = u"rh6"
                 elif parts[0] == "7":
                     base = u"rh7"
+                elif parts[0] == "8":
+                    base = u"rh8"
                 else:
                     msg = ("Unsupported rhel release: {0!r}".format(release))
                     raise OkonomiyakiError(msg)
                 return base
             else:
                 msg = "Unsupported distribution: {0!r}".format(family_kind)
                 raise OkonomiyakiError(msg)
@@ -348,14 +343,15 @@
     def __hash__(self):
         return hash(self.platform)
 
 
 def applies(platform_string, to='current'):
     """ Returns True if the given platform string applies to the platform
     specified by 'to'."""
+
     def _parse_component(component):
         component = component.strip()
 
         parts = component.split("-")
         if len(parts) == 1:
             if parts[0] in VALID_PLATFORMS_FILTER:
                 return parts[0], None
@@ -427,23 +423,28 @@
         return not any(conditions)
     else:
         return any(conditions)
 
 
 def _epd_name_and_python_to_quadruplet(name, runtime_version=None):
     py38 = RuntimeVersion.from_string('3.8')
+    py311 = RuntimeVersion.from_string('3.11')
+    if name == "rh8":
+        return (OSKind.linux, NameKind.rhel, FamilyKind.rhel, "8.8")
     if name == "rh7":
         return (OSKind.linux, NameKind.rhel, FamilyKind.rhel, "7.1")
     if name == "rh6":
         return (OSKind.linux, NameKind.rhel, FamilyKind.rhel, "6.5")
     elif name == "rh5":
         return (OSKind.linux, NameKind.rhel, FamilyKind.rhel, "5.8")
     elif name == "rh3":
         return (OSKind.linux, NameKind.rhel, FamilyKind.rhel, "3.8")
     elif name == "osx":
+        if runtime_version is not None and runtime_version >= py311:
+            return (OSKind.darwin, NameKind.mac_os_x, FamilyKind.mac_os_x, "12.0")
         if runtime_version is not None and runtime_version >= py38:
             return (OSKind.darwin, NameKind.mac_os_x, FamilyKind.mac_os_x, "10.14")
         else:
             return (OSKind.darwin, NameKind.mac_os_x, FamilyKind.mac_os_x, "10.6")
     elif name == "sol":
         return (OSKind.solaris, NameKind.solaris, FamilyKind.solaris, "")
     elif name == "win":
@@ -452,34 +453,26 @@
         else:
             return (OSKind.windows, NameKind.windows, FamilyKind.windows, "")
     else:
         msg = "Invalid epd platform string name: {0!r}".format(name)
         raise OkonomiyakiError(msg)
 
 
-def _guess_epd_platform(arch=None):
-    if arch is None:
-        arch = Arch.from_running_python()
-
-    platform = Platform.from_running_system(str(arch))
-    return EPDPlatform(platform)
-
-
 def _is_supported(platform):
     arch_and_machine_are_intel = (
         platform.arch in (X86, X86_64)
-        and platform.machine in (X86, X86_64)
-    )
+        and platform.machine in (X86, X86_64))
     if platform.os_kind == OSKind.windows:
         return arch_and_machine_are_intel
     if platform.os_kind == OSKind.darwin:
         return arch_and_machine_are_intel
     if platform.os_kind == OSKind.solaris:
         return arch_and_machine_are_intel
     if platform.os_kind == OSKind.linux:
         if platform.family_kind != FamilyKind.rhel:
             return False
         parts = platform.release.split(".")
-        return parts[0] in ("3", "5", "6", "7") \
-            and arch_and_machine_are_intel
+        return (
+            parts[0] in ("3", "5", "6", "7", "8")
+            and arch_and_machine_are_intel)
 
     return False
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/legacy.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/legacy.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/pep425.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/pep425.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/platform_filters.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/platform_filters.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/platforms/python_implementation.py` & `okonomiyaki-1.4.0/okonomiyaki/platforms/python_implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,22 +64,23 @@
         m = _TAG_RE.match(s)
         if m is None:
             raise generic_exc
         else:
             d = m.groupdict()
             kind = d["interpreter"]
             version = d["version"]
-            if len(version) < 2:
-                raise generic_exc
-            elif len(version) > 2:
-                raise generic_exc
-            else:
+            if '_' in version:
+                major, minor = map(int, version.split('_'))
+                return cls(kind, major, minor)
+            elif 1 < len(version) < 4:
                 major = int(version[0])
-                minor = int(version[1])
+                minor = int(version[1:])
                 return cls(kind, major, minor)
+            else:
+                raise generic_exc
 
     def __init__(self, kind, major, minor):
         self.kind = _ABBREVIATED_TO_KIND.get(kind, kind)
         self.major = major
         self.minor = minor
 
     @property
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/broken_legacy_eggs/mccabe-0.2.1-2.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/broken_legacy_eggs/mccabe-0.2.1-2.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/_osx64app-1.0-1.egg`

 * *Files 21% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      1562 (000000000000061Ah)
-  Actual end-cent-dir record offset:          1540 (0000000000000604h)
-  Expected end-cent-dir record offset:        1540 (0000000000000604h)
+  Zip archive file size:                      1209 (00000000000004B9h)
+  Actual end-cent-dir record offset:          1187 (00000000000004A3h)
+  Expected end-cent-dir record offset:        1187 (00000000000004A3h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 6 entries.
-  The central directory is 525 (000000000000020Dh) bytes long,
+  central directory contains 5 entries.
+  The central directory is 442 (00000000000001BAh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1015 (00000000000003F7h).
+  is 745 (00000000000002E9h).
 
 
 Central directory entry #1:
 ---------------------------
 
   EGG-INFO/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Jun 4 02:09:38
-  file last modified on (UT extra field modtime): 2015 Jun 3 17:09:37 local
-  file last modified on (UT extra field modtime): 2015 Jun 3 17:09:37 UTC
+  file last modified on (DOS date/time):          2015 Jun 10 17:00:56
+  file last modified on (UT extra field modtime): 2015 Jun 10 08:00:55 local
+  file last modified on (UT extra field modtime): 2015 Jun 10 08:00:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -50,33 +50,33 @@
     01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  EGG-INFO/PKG-INFO
+  EGG-INFO/post_egginst.py
 
   offset of local header from start of archive:   67
                                                   (0000000000000043h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2011 Jan 14 19:13:12
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:12 local
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:12 UTC
-  32-bit CRC value (hex):                         109b3c19
-  compressed size:                                258 bytes
-  uncompressed size:                              376 bytes
-  length of filename:                             17 characters
+  file last modified on (DOS date/time):          2012 Jan 13 09:21:42
+  file last modified on (UT extra field modtime): 2012 Jan 13 00:21:42 local
+  file last modified on (UT extra field modtime): 2012 Jan 13 00:21:42 UTC
+  32-bit CRC value (hex):                         3735a991
+  compressed size:                                141 bytes
+  uncompressed size:                              191 bytes
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
@@ -87,147 +87,111 @@
     01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  EGG-INFO/spec/
-
-  offset of local header from start of archive:   400
-                                                  (0000000000000190h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2015 Jun 4 02:09:34
-  file last modified on (UT extra field modtime): 2015 Jun 3 17:09:34 local
-  file last modified on (UT extra field modtime): 2015 Jun 3 17:09:34 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #4:
----------------------------
-
-  EGG-INFO/spec/depend
+  EGG-INFO/pre_egguninst.py
 
-  offset of local header from start of archive:   472
-                                                  (00000000000001D8h) bytes
+  offset of local header from start of archive:   290
+                                                  (0000000000000122h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2011 Jan 14 19:13:44
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 local
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 UTC
-  32-bit CRC value (hex):                         0e945864
-  compressed size:                                115 bytes
-  uncompressed size:                              143 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2012 Jan 13 09:26:12
+  file last modified on (UT extra field modtime): 2012 Jan 13 00:26:12 local
+  file last modified on (UT extra field modtime): 2012 Jan 13 00:26:12 UTC
+  32-bit CRC value (hex):                         015e2ae6
+  compressed size:                                102 bytes
+  uncompressed size:                              122 bytes
+  length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #4:
 ---------------------------
 
-  EGG-INFO/spec/lib-depend
+  EGG-INFO/spec/
 
-  offset of local header from start of archive:   665
-                                                  (0000000000000299h) bytes
+  offset of local header from start of archive:   475
+                                                  (00000000000001DBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2011 Jan 14 19:13:44
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 local
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 UTC
-  32-bit CRC value (hex):                         9114a66f
-  compressed size:                                153 bytes
-  uncompressed size:                              506 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2012 Jan 13 08:45:50
+  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:50 local
+  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:50 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
-  MS-DOS file attributes (00 hex):                none
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 f5 01 00 00 04 14 00 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #5:
 ---------------------------
 
-  EGG-INFO/spec/summary
+  EGG-INFO/spec/depend
 
-  offset of local header from start of archive:   900
-                                                  (0000000000000384h) bytes
+  offset of local header from start of archive:   547
+                                                  (0000000000000223h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2011 Jan 14 19:13:44
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 local
-  file last modified on (UT extra field modtime): 2011 Jan 14 10:13:44 UTC
-  32-bit CRC value (hex):                         10aca43e
-  compressed size:                                36 bytes
-  uncompressed size:                              36 bytes
-  length of filename:                             21 characters
+  file last modified on (DOS date/time):          2012 Jan 13 08:45:46
+  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:45 local
+  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:45 UTC
+  32-bit CRC value (hex):                         b72a9986
+  compressed size:                                120 bytes
+  uncompressed size:                              149 bytes
+  length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 f5 01 00 00 04 14 00 00 00.
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmp5sipovoz_.zip

```diff
@@ -1,19 +1,16 @@
 Filename: EGG-INFO/
 Comment: 
 
-Filename: EGG-INFO/PKG-INFO
+Filename: EGG-INFO/post_egginst.py
 Comment: 
 
-Filename: EGG-INFO/spec/
-Comment: 
-
-Filename: EGG-INFO/spec/depend
+Filename: EGG-INFO/pre_egguninst.py
 Comment: 
 
-Filename: EGG-INFO/spec/lib-depend
+Filename: EGG-INFO/spec/
 Comment: 
 
-Filename: EGG-INFO/spec/summary
+Filename: EGG-INFO/spec/depend
 Comment: 
 
 Zip file comment:
```

#### EGG-INFO/spec/depend

```diff
@@ -1,10 +1,10 @@
 metadata_version = '1.1'
-name = 'MKL'
-version = '10.3'
+name = '_osx64app'
+version = '1.0'
 build = 1
 
 arch = 'amd64'
 platform = 'darwin'
 osdist = None
-python = None
+python = '2.7'
 packages = []
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/PySide-1.1.0-3.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/PySide-1.1.0-3.egg`

 * *Files 14% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,163 +1,131 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      5316 (00000000000014C4h)
-  Actual end-cent-dir record offset:          5294 (00000000000014AEh)
-  Expected end-cent-dir record offset:        5294 (00000000000014AEh)
+  Zip archive file size:                      5108 (00000000000013F4h)
+  Actual end-cent-dir record offset:          5086 (00000000000013DEh)
+  Expected end-cent-dir record offset:        5086 (00000000000013DEh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 4 entries.
-  The central directory is 340 (0000000000000154h) bytes long,
+  The central directory is 244 (00000000000000F4h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 4954 (000000000000135Ah).
+  is 4842 (00000000000012EAh).
 
 
 Central directory entry #1:
 ---------------------------
 
   EGG-INFO/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
+  minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Aug 24 17:18:44
-  file last modified on (UT extra field modtime): 2015 Aug 24 16:18:44 local
-  file last modified on (UT extra field modtime): 2015 Aug 24 16:18:44 UTC
+  file last modified on (DOS date/time):          2023 May 12 16:18:46
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040775 octal):            drwxrwxr-x
   MS-DOS file attributes (10 hex):                dir 
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
-
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  EGG-INFO/PKG-INFO
+  EGG-INFO/spec/
 
-  offset of local header from start of archive:   67
-                                                  (0000000000000043h) bytes
+  offset of local header from start of archive:   39
+                                                  (0000000000000027h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2012 Jan 11 10:25:12
-  file last modified on (UT extra field modtime): 2012 Jan 11 10:25:12 local
-  file last modified on (UT extra field modtime): 2012 Jan 11 10:25:12 UTC
-  32-bit CRC value (hex):                         a79868ed
-  compressed size:                                4543 bytes
-  uncompressed size:                              11703 bytes
-  length of filename:                             17 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:18:46
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+  apparent file type:                             binary
+  Unix file attributes (040775 octal):            drwxrwxr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  EGG-INFO/spec/
+  EGG-INFO/spec/depend
 
-  offset of local header from start of archive:   4685
-                                                  (000000000000124Dh) bytes
+  offset of local header from start of archive:   83
+                                                  (0000000000000053h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Aug 24 17:18:30
-  file last modified on (UT extra field modtime): 2015 Aug 24 16:18:30 local
-  file last modified on (UT extra field modtime): 2015 Aug 24 16:18:30 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:18:46
+  32-bit CRC value (hex):                         51074fe8
+  compressed size:                                119 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             20 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040775 octal):            drwxrwxr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  EGG-INFO/spec/depend
+  EGG-INFO/PKG-INFO
 
-  offset of local header from start of archive:   4757
-                                                  (0000000000001295h) bytes
+  offset of local header from start of archive:   252
+                                                  (00000000000000FCh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2012 Apr 11 15:16:06
-  file last modified on (UT extra field modtime): 2012 Apr 11 14:16:06 local
-  file last modified on (UT extra field modtime): 2012 Apr 11 14:16:06 UTC
-  32-bit CRC value (hex):                         51074fe8
-  compressed size:                                119 bytes
-  uncompressed size:                              148 bytes
-  length of filename:                             20 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:18:46
+  32-bit CRC value (hex):                         a79868ed
+  compressed size:                                4543 bytes
+  uncompressed size:                              11703 bytes
+  length of filename:                             17 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
-
   There is no file comment.
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmpydbu0j63_.zip

```diff
@@ -1,13 +1,13 @@
 Filename: EGG-INFO/
 Comment: 
 
-Filename: EGG-INFO/PKG-INFO
-Comment: 
-
 Filename: EGG-INFO/spec/
 Comment: 
 
 Filename: EGG-INFO/spec/depend
 Comment: 
 
+Filename: EGG-INFO/PKG-INFO
+Comment: 
+
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=store
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/_osx64app-1.0-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/MKL-10.3-1.egg`

 * *Files 27% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,200 +1,127 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      1209 (00000000000004B9h)
-  Actual end-cent-dir record offset:          1187 (00000000000004A3h)
-  Expected end-cent-dir record offset:        1187 (00000000000004A3h)
+  Zip archive file size:                       917 (0000000000000395h)
+  Actual end-cent-dir record offset:           895 (000000000000037Fh)
+  Expected end-cent-dir record offset:         895 (000000000000037Fh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 5 entries.
-  The central directory is 442 (00000000000001BAh) bytes long,
+  central directory contains 3 entries.
+  The central directory is 268 (000000000000010Ch) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 745 (00000000000002E9h).
+  is 627 (0000000000000273h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  EGG-INFO/
+  EGG-INFO/PKG-INFO
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2015 Jun 10 17:00:56
-  file last modified on (UT extra field modtime): 2015 Jun 10 08:00:55 local
-  file last modified on (UT extra field modtime): 2015 Jun 10 08:00:55 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             9 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #2:
----------------------------
-
-  EGG-INFO/post_egginst.py
-
-  offset of local header from start of archive:   67
-                                                  (0000000000000043h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2012 Jan 13 09:21:42
-  file last modified on (UT extra field modtime): 2012 Jan 13 00:21:42 local
-  file last modified on (UT extra field modtime): 2012 Jan 13 00:21:42 UTC
-  32-bit CRC value (hex):                         3735a991
-  compressed size:                                141 bytes
-  uncompressed size:                              191 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2023 Jun 29 15:28:12
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:28:12 local
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:28:12 UTC
+  32-bit CRC value (hex):                         f209c767
+  compressed size:                                207 bytes
+  uncompressed size:                              292 bytes
+  length of filename:                             17 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #2:
 ---------------------------
 
-  EGG-INFO/pre_egguninst.py
+  EGG-INFO/spec/depend
 
-  offset of local header from start of archive:   290
-                                                  (0000000000000122h) bytes
+  offset of local header from start of archive:   282
+                                                  (000000000000011Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2012 Jan 13 09:26:12
-  file last modified on (UT extra field modtime): 2012 Jan 13 00:26:12 local
-  file last modified on (UT extra field modtime): 2012 Jan 13 00:26:12 UTC
-  32-bit CRC value (hex):                         015e2ae6
-  compressed size:                                102 bytes
-  uncompressed size:                              122 bytes
-  length of filename:                             25 characters
+  file last modified on (DOS date/time):          2023 Jun 29 15:21:28
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:21:28 local
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:21:28 UTC
+  32-bit CRC value (hex):                         e41e3492
+  compressed size:                                152 bytes
+  uncompressed size:                              235 bytes
+  length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100666 octal):            -rw-rw-rw-
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #3:
 ---------------------------
 
-  EGG-INFO/spec/
+  EGG-INFO/spec/summary
 
-  offset of local header from start of archive:   475
-                                                  (00000000000001DBh) bytes
+  offset of local header from start of archive:   512
+                                                  (0000000000000200h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2012 Jan 13 08:45:50
-  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:50 local
-  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:50 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #5:
----------------------------
-
-  EGG-INFO/spec/depend
-
-  offset of local header from start of archive:   547
-                                                  (0000000000000223h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2012 Jan 13 08:45:46
-  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:45 local
-  file last modified on (UT extra field modtime): 2012 Jan 12 23:45:45 UTC
-  32-bit CRC value (hex):                         b72a9986
-  compressed size:                                120 bytes
-  uncompressed size:                              149 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2023 Jun 29 15:28:18
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:28:17 local
+  file last modified on (UT extra field modtime): 2023 Jun 29 14:28:17 UTC
+  32-bit CRC value (hex):                         10aca43e
+  compressed size:                                36 bytes
+  uncompressed size:                              36 bytes
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100600 octal):            -rw-------
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmpwt3p6p03_.zip

```diff
@@ -1,16 +1,10 @@
-Filename: EGG-INFO/
+Filename: EGG-INFO/PKG-INFO
 Comment: 
 
-Filename: EGG-INFO/post_egginst.py
-Comment: 
-
-Filename: EGG-INFO/pre_egguninst.py
-Comment: 
-
-Filename: EGG-INFO/spec/
+Filename: EGG-INFO/spec/depend
 Comment: 
 
-Filename: EGG-INFO/spec/depend
+Filename: EGG-INFO/spec/summary
 Comment: 
 
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

#### EGG-INFO/spec/depend

```diff
@@ -1,10 +1,16 @@
-metadata_version = '1.1'
-name = '_osx64app'
-version = '1.0'
+metadata_version = '1.4'
+name = 'MKL'
+version = '10.3'
 build = 1
 
 arch = 'amd64'
-platform = 'darwin'
-osdist = None
-python = '2.7'
+platform = 'linux2'
+osdist = 'RedHat_8'
+python = None
+
+python_tag = None
+abi_tag = None
+platform_tag = 'linux_x86_64'
+platform_abi = 'gnu'
+
 packages = []
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/enstaller-4.5.0-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/enstaller-4.5.0-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/ets-4.3.0-3.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/ets-4.3.0-3.egg`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 10027 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     4395 b- defN 13-Jun-21 17:27 ets_docs.pyc
--rw-rw-r--  2.0 unx     3791 b- defN 13-Jun-21 17:27 ets.pyc
--rw-rw-r--  2.0 unx     6137 b- defN 13-Mar-28 16:23 ets_docs.py
--rw-rw-r--  2.0 unx     5138 b- defN 13-Mar-28 16:23 ets.py
--rw-rw-r--  2.0 unx      363 b- defN 13-Jun-21 17:27 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx       59 b- defN 13-Jun-21 17:27 EGG-INFO/entry_points.txt
-?rw-------  2.0 unx     1923 b- defN 13-Jun-21 17:27 EGG-INFO/PKG-INFO
-?rw-------  2.0 unx       55 b- defN 13-Jun-21 17:27 EGG-INFO/spec/summary
-?rw-------  2.0 unx      514 b- defN 13-Jun-21 17:27 EGG-INFO/spec/depend
-9 files, 22375 bytes uncompressed, 9041 bytes compressed:  59.6%
+Zip file size: 10225 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx     3791 b- defN 23-May-12 16:10 ets.pyc
+-rw-rw-r--  2.0 unx     4395 b- defN 23-May-12 16:10 ets_docs.pyc
+-rw-rw-r--  2.0 unx     5138 b- defN 23-May-12 16:10 ets.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:10 EGG-INFO/
+-rw-rw-r--  2.0 unx       59 b- defN 23-May-12 16:10 EGG-INFO/entry_points.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-12 16:10 EGG-INFO/spec/
+-rw-rw-r--  2.0 unx      514 b- defN 23-May-12 16:10 EGG-INFO/spec/depend
+-rw-rw-r--  2.0 unx       55 b- defN 23-May-12 16:10 EGG-INFO/spec/summary
+-rw-rw-r--  2.0 unx      363 b- defN 23-May-12 16:10 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx     1923 b- defN 23-May-12 16:10 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx     6137 b- defN 23-May-12 16:10 ets_docs.py
+11 files, 22375 bytes uncompressed, 9041 bytes compressed:  59.6%
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmpm1zfnd8g_.zip

```diff
@@ -1,28 +1,34 @@
-Filename: ets_docs.pyc
-Comment: 
-
 Filename: ets.pyc
 Comment: 
 
-Filename: ets_docs.py
+Filename: ets_docs.pyc
 Comment: 
 
 Filename: ets.py
 Comment: 
 
-Filename: EGG-INFO/requires.txt
+Filename: EGG-INFO/
 Comment: 
 
 Filename: EGG-INFO/entry_points.txt
 Comment: 
 
-Filename: EGG-INFO/PKG-INFO
+Filename: EGG-INFO/spec/
+Comment: 
+
+Filename: EGG-INFO/spec/depend
 Comment: 
 
 Filename: EGG-INFO/spec/summary
 Comment: 
 
-Filename: EGG-INFO/spec/depend
+Filename: EGG-INFO/requires.txt
+Comment: 
+
+Filename: EGG-INFO/PKG-INFO
+Comment: 
+
+Filename: ets_docs.py
 Comment: 
 
 Zip file comment:
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pip-6.0.8-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pip-6.0.8-1.egg`

 * *Files 22% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,310 +1,247 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      2386 (0000000000000952h)
-  Actual end-cent-dir record offset:          2364 (000000000000093Ch)
-  Expected end-cent-dir record offset:        2364 (000000000000093Ch)
+  Zip archive file size:                      1971 (00000000000007B3h)
+  Actual end-cent-dir record offset:          1949 (000000000000079Dh)
+  Expected end-cent-dir record offset:        1949 (000000000000079Dh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 8 entries.
-  The central directory is 704 (00000000000002C0h) bytes long,
+  The central directory is 512 (0000000000000200h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1660 (000000000000067Ch).
+  is 1437 (000000000000059Dh).
 
 
 Central directory entry #1:
 ---------------------------
 
   EGG-INFO/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
+  minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 May 18 16:10:28
-  file last modified on (UT extra field modtime): 2015 May 18 07:10:27 local
-  file last modified on (UT extra field modtime): 2015 May 18 07:10:27 UTC
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
+  Unix file attributes (040775 octal):            drwxrwxr-x
   MS-DOS file attributes (10 hex):                dir 
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
   EGG-INFO/entry_points.txt
 
-  offset of local header from start of archive:   67
-                                                  (0000000000000043h) bytes
+  offset of local header from start of archive:   39
+                                                  (0000000000000027h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 19 10:22:56
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 UTC
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
   32-bit CRC value (hex):                         f034f165
   compressed size:                                42 bytes
   uncompressed size:                              68 bytes
   length of filename:                             25 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  EGG-INFO/pbr.json
+  EGG-INFO/spec/
 
-  offset of local header from start of archive:   192
-                                                  (00000000000000C0h) bytes
+  offset of local header from start of archive:   136
+                                                  (0000000000000088h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
+  minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 4 18:28:16
-  file last modified on (UT extra field modtime): 2015 Feb 4 09:28:16 local
-  file last modified on (UT extra field modtime): 2015 Feb 4 09:28:16 UTC
-  32-bit CRC value (hex):                         7d25c07d
-  compressed size:                                46 bytes
-  uncompressed size:                              46 bytes
-  length of filename:                             17 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+  apparent file type:                             binary
+  Unix file attributes (040775 octal):            drwxrwxr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  EGG-INFO/PKG-INFO
+  EGG-INFO/spec/depend
 
-  offset of local header from start of archive:   313
-                                                  (0000000000000139h) bytes
+  offset of local header from start of archive:   180
+                                                  (00000000000000B4h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 19 10:22:56
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 UTC
-  32-bit CRC value (hex):                         93882d3e
-  compressed size:                                744 bytes
-  uncompressed size:                              1969 bytes
-  length of filename:                             17 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         4b17b9a4
+  compressed size:                                118 bytes
+  uncompressed size:                              145 bytes
+  length of filename:                             20 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  EGG-INFO/requires.txt
+  EGG-INFO/spec/summary
 
-  offset of local header from start of archive:   1132
-                                                  (000000000000046Ch) bytes
+  offset of local header from start of archive:   348
+                                                  (000000000000015Ch) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 19 10:22:56
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:56 UTC
-  32-bit CRC value (hex):                         554175aa
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         cc3bcbdb
   compressed size:                                51 bytes
-  uncompressed size:                              56 bytes
+  uncompressed size:                              52 bytes
   length of filename:                             21 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  EGG-INFO/spec/
+  EGG-INFO/pbr.json
 
-  offset of local header from start of archive:   1262
-                                                  (00000000000004EEh) bytes
+  offset of local header from start of archive:   450
+                                                  (00000000000001C2h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 May 18 16:10:28
-  file last modified on (UT extra field modtime): 2015 May 18 07:10:27 local
-  file last modified on (UT extra field modtime): 2015 May 18 07:10:27 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         7d25c07d
+  compressed size:                                47 bytes
+  uncompressed size:                              46 bytes
+  length of filename:                             17 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  EGG-INFO/spec/depend
+  EGG-INFO/requires.txt
 
-  offset of local header from start of archive:   1334
-                                                  (0000000000000536h) bytes
+  offset of local header from start of archive:   544
+                                                  (0000000000000220h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 19 10:22:58
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:58 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:58 UTC
-  32-bit CRC value (hex):                         4b17b9a4
-  compressed size:                                118 bytes
-  uncompressed size:                              145 bytes
-  length of filename:                             20 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         554175aa
+  compressed size:                                51 bytes
+  uncompressed size:                              56 bytes
+  length of filename:                             21 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  EGG-INFO/spec/summary
+  EGG-INFO/PKG-INFO
 
-  offset of local header from start of archive:   1530
-                                                  (00000000000005FAh) bytes
+  offset of local header from start of archive:   646
+                                                  (0000000000000286h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 19 10:22:58
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:58 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 01:22:58 UTC
-  32-bit CRC value (hex):                         cc3bcbdb
-  compressed size:                                51 bytes
-  uncompressed size:                              52 bytes
-  length of filename:                             21 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:14:22
+  32-bit CRC value (hex):                         93882d3e
+  compressed size:                                744 bytes
+  uncompressed size:                              1969 bytes
+  length of filename:                             17 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmppks8uu_9_.zip

```diff
@@ -1,25 +1,25 @@
 Filename: EGG-INFO/
 Comment: 
 
 Filename: EGG-INFO/entry_points.txt
 Comment: 
 
-Filename: EGG-INFO/pbr.json
+Filename: EGG-INFO/spec/
 Comment: 
 
-Filename: EGG-INFO/PKG-INFO
+Filename: EGG-INFO/spec/depend
 Comment: 
 
-Filename: EGG-INFO/requires.txt
+Filename: EGG-INFO/spec/summary
 Comment: 
 
-Filename: EGG-INFO/spec/
+Filename: EGG-INFO/pbr.json
 Comment: 
 
-Filename: EGG-INFO/spec/depend
+Filename: EGG-INFO/requires.txt
 Comment: 
 
-Filename: EGG-INFO/spec/summary
+Filename: EGG-INFO/PKG-INFO
 Comment: 
 
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=store
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pip-7.0.3-py3.4.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pip-7.0.3-py3.4.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pymongo-2.8-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pymongo-2.8-1.egg`

 * *Files 27% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,236 +1,189 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      3825 (0000000000000EF1h)
-  Actual end-cent-dir record offset:          3803 (0000000000000EDBh)
-  Expected end-cent-dir record offset:        3803 (0000000000000EDBh)
+  Zip archive file size:                      3515 (0000000000000DBBh)
+  Actual end-cent-dir record offset:          3493 (0000000000000DA5h)
+  Expected end-cent-dir record offset:        3493 (0000000000000DA5h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 6 entries.
-  The central directory is 525 (000000000000020Dh) bytes long,
+  The central directory is 381 (000000000000017Dh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 3278 (0000000000000CCEh).
+  is 3112 (0000000000000C28h).
 
 
 Central directory entry #1:
 ---------------------------
 
   EGG-INFO/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
+  minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 May 29 12:44:28
-  file last modified on (UT extra field modtime): 2015 May 29 03:44:27 local
-  file last modified on (UT extra field modtime): 2015 May 29 03:44:27 UTC
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
+  Unix file attributes (040775 octal):            drwxrwxr-x
   MS-DOS file attributes (10 hex):                dir 
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  EGG-INFO/PKG-INFO
+  EGG-INFO/spec/
 
-  offset of local header from start of archive:   67
-                                                  (0000000000000043h) bytes
+  offset of local header from start of archive:   39
+                                                  (0000000000000027h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 20 08:48:20
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 UTC
-  32-bit CRC value (hex):                         10acccc9
-  compressed size:                                2655 bytes
-  uncompressed size:                              7529 bytes
-  length of filename:                             17 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+  apparent file type:                             binary
+  Unix file attributes (040775 octal):            drwxrwxr-x
+  MS-DOS file attributes (10 hex):                dir 
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  EGG-INFO/spec/
+  EGG-INFO/spec/depend
 
-  offset of local header from start of archive:   2797
-                                                  (0000000000000AEDh) bytes
+  offset of local header from start of archive:   83
+                                                  (0000000000000053h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 May 29 12:44:28
-  file last modified on (UT extra field modtime): 2015 May 29 03:44:27 local
-  file last modified on (UT extra field modtime): 2015 May 29 03:44:27 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             14 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
+  32-bit CRC value (hex):                         4d19f16f
+  compressed size:                                119 bytes
+  uncompressed size:                              147 bytes
+  length of filename:                             20 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  EGG-INFO/spec/depend
+  EGG-INFO/spec/summary
 
-  offset of local header from start of archive:   2869
-                                                  (0000000000000B35h) bytes
+  offset of local header from start of archive:   252
+                                                  (00000000000000FCh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 20 08:48:20
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 UTC
-  32-bit CRC value (hex):                         4d19f16f
-  compressed size:                                119 bytes
-  uncompressed size:                              147 bytes
-  length of filename:                             20 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
+  32-bit CRC value (hex):                         6ba2afa7
+  compressed size:                                28 bytes
+  uncompressed size:                              26 bytes
+  length of filename:                             21 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
   EGG-INFO/spec/lib-depend
 
-  offset of local header from start of archive:   3066
-                                                  (0000000000000BFAh) bytes
+  offset of local header from start of archive:   331
+                                                  (000000000000014Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 20 08:48:20
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 UTC
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
   32-bit CRC value (hex):                         f946d228
   compressed size:                                25 bytes
   uncompressed size:                              27 bytes
   length of filename:                             24 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  EGG-INFO/spec/summary
+  EGG-INFO/PKG-INFO
 
-  offset of local header from start of archive:   3173
-                                                  (0000000000000C65h) bytes
+  offset of local header from start of archive:   410
+                                                  (000000000000019Ah) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2015 Feb 20 08:48:20
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 local
-  file last modified on (UT extra field modtime): 2015 Feb 19 23:48:20 UTC
-  32-bit CRC value (hex):                         6ba2afa7
-  compressed size:                                26 bytes
-  uncompressed size:                              26 bytes
-  length of filename:                             21 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2023 May 12 16:15:58
+  32-bit CRC value (hex):                         10acccc9
+  compressed size:                                2655 bytes
+  uncompressed size:                              7529 bytes
+  length of filename:                             17 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
```

#### zipnote «TEMP»/diffoscope_mb3a2trt_/tmpoy3beauo_.zip

```diff
@@ -1,19 +1,19 @@
 Filename: EGG-INFO/
 Comment: 
 
-Filename: EGG-INFO/PKG-INFO
-Comment: 
-
 Filename: EGG-INFO/spec/
 Comment: 
 
 Filename: EGG-INFO/spec/depend
 Comment: 
 
+Filename: EGG-INFO/spec/summary
+Comment: 
+
 Filename: EGG-INFO/spec/lib-depend
 Comment: 
 
-Filename: EGG-INFO/spec/summary
+Filename: EGG-INFO/PKG-INFO
 Comment: 
 
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=store
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/pymongo_description.txt` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/pymongo_description.txt`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/setuptools-16.0-py3.4.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/setuptools-16.0-py3.4.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/setuptools-40.8.0-py2.7.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/setuptools-40.8.0-py2.7.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/supervisor-3.0-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/supervisor-3.0-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-4.6.0.dev235-py2.7-macosx-10.10-intel.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-4.6.0.dev235-py2.7-macosx-10.10-intel.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-linux-x86_64.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-linux-x86_64.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-macosx-10.14-x86_64.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-macosx-10.14-x86_64.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-win-amd64.egg` & `okonomiyaki-1.4.0/okonomiyaki/repositories/tests/data/traits-6.3.0.dev1702-py3.8-win-amd64.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime_info.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/tests/test_runtime_metadata.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/tests/test_runtime_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import os.path
 import shutil
 import sys
 
 import zipfile2
+from hypothesis import given
+from hypothesis.strategies import sampled_from
+
 
 from okonomiyaki.errors import (
     InvalidMetadata, MissingMetadata, UnsupportedMetadata)
 from okonomiyaki.utils import tempdir
 from okonomiyaki.utils.test_data import (
     INVALID_RUNTIME_NO_METADATA_VERSION, JULIA_DEFAULT_0_3_11_RH5_X86_64,
     PYTHON_CPYTHON_2_7_10_RH5_X86_64, PYTHON_CPYTHON_2_7_10_RH5_X86_64_INVALID,
     PYTHON_PYPY_2_6_0_RH5_X86_64, R_DEFAULT_3_0_0_RH5_X86_64,
     PYTHON_CPYTHON_3_8_8_RH7_X86_64, PYTHON_CPYTHON_3_8_8_OSX_X86_64,
-    PYTHON_CPYTHON_3_8_8_WIN_X86_64, PYTHON_CPYTHON_3_8_8_WIN_X86
-
+    PYTHON_CPYTHON_3_8_8_WIN_X86_64, PYTHON_CPYTHON_3_8_8_WIN_X86,
+    PYTHON_CPYTHON_3_11_2_RH8_X86_64, PYTHON_CPYTHON_3_11_2_OSX_X86_64,
+    PYTHON_CPYTHON_3_11_2_WIN_X86_64
 )
 from okonomiyaki.versions import MetadataVersion
 from okonomiyaki.platforms import Platform, OSKind, FamilyKind, NameKind, X86_64, X86
 
 from ..runtime_metadata import (
     JuliaRuntimeMetadataV1, PythonRuntimeMetadataV1, RuntimeVersion,
     is_runtime_path_valid, runtime_metadata_factory
@@ -26,310 +30,249 @@
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
 
 
 class TestPythonMetadataV1(unittest.TestCase):
-    def test_simple(self):
-        # Given
-        path = PYTHON_CPYTHON_2_7_10_RH5_X86_64
-
-        # When
-        metadata = PythonRuntimeMetadataV1._from_path(path)
-
-        # Then
-        self.assertTrue(is_runtime_path_valid(path))
-        self.assertEqual(metadata.filename, os.path.basename(path))
-        self.assertEqual(
-            metadata.metadata_version, MetadataVersion.from_string("1.0"))
-        self.assertEqual(metadata.implementation, "cpython")
-        self.assertEqual(
-            metadata.version, RuntimeVersion.from_string("2.7.10+1"))
-        self.assertEqual(
-            metadata.language_version, RuntimeVersion.from_string("2.7.10"))
-        self.assertEqual(metadata.build_revision, "2.1.0-dev570")
-        self.assertEqual(metadata.executable, "${prefix}/bin/python")
-        self.assertEqual(metadata.paths, ("${prefix}/bin",))
-        self.assertEqual(
-            metadata.post_install,
-            ("${executable}",
-             "${prefix}/lib/python2.7/custom_tools/fix-scripts.py"))
-        self.assertEqual(metadata.scriptsdir, "${prefix}/bin")
-        self.assertEqual(
-            metadata.site_packages, "${prefix}/lib/python2.7/site-packages")
-        self.assertEqual(metadata.python_tag, "cp27")
-        self.assertEqual(
-            metadata.platform,
-            Platform(
-                os_kind=OSKind.linux,
-                family_kind=FamilyKind.rhel,
-                name_kind=NameKind.rhel,
-                release='5.8',
-                arch=X86_64,
-                machine=X86_64))
 
-    def test_simple_pypy(self):
+    def test_pypy(self):
         # Given
         path = PYTHON_PYPY_2_6_0_RH5_X86_64
 
         # When
         metadata = PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertTrue(is_runtime_path_valid(path))
         self.assertEqual(metadata.filename, os.path.basename(path))
 
         self.assertEqual(
             metadata.metadata_version,
-            MetadataVersion.from_string("1.0")
+            MetadataVersion.from_string('1.0')
         )
-        self.assertEqual(metadata.implementation, "pypy")
+        self.assertEqual(metadata.implementation, 'pypy')
         self.assertEqual(
             metadata.version,
-            RuntimeVersion.from_string("2.6.0+1")
+            RuntimeVersion.from_string('2.6.0+1')
         )
         self.assertEqual(
             metadata.language_version,
-            RuntimeVersion.from_string("2.7.9")
+            RuntimeVersion.from_string('2.7.9')
         )
-        self.assertEqual(metadata.build_revision, "")
-        self.assertEqual(metadata.executable, "${prefix}/bin/pypy")
-        self.assertEqual(metadata.paths, ("${prefix}/bin",))
+        self.assertEqual(metadata.build_revision, '')
+        self.assertEqual(metadata.executable, '${prefix}/bin/pypy')
+        self.assertEqual(metadata.paths, ('${prefix}/bin',))
         self.assertEqual(metadata.post_install, tuple())
-        self.assertEqual(metadata.scriptsdir, "${prefix}/bin")
-        self.assertEqual(metadata.site_packages, "${prefix}/site-packages")
-        self.assertEqual(metadata.python_tag, "pp27")
+        self.assertEqual(metadata.scriptsdir, '${prefix}/bin')
+        self.assertEqual(metadata.site_packages, '${prefix}/site-packages')
+        self.assertEqual(metadata.python_tag, 'pp27')
 
     def test_invalid(self):
         # Given
-        path = "python-cpython-2.7.10-1-rh5_64.zip"
+        path = 'python-cpython-2.7.10-1-rh5_64.zip'
 
         # When/Then
         with self.assertRaises(InvalidMetadata):
             PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertFalse(is_runtime_path_valid(path))
 
         # Given
-        path = "python_cpython_2.7.10-1_rh5_64.runtime"
+        path = 'python_cpython_2.7.10-1_rh5_64.runtime'
 
         # When/Then
         with self.assertRaises(InvalidMetadata):
             PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertFalse(is_runtime_path_valid(path))
 
         # Given
-        path = "python-cpython-2.7.10_rh5_x86_64.runtime"
+        path = 'python-cpython-2.7.10_rh5_x86_64.runtime'
 
         # When/Then
         with self.assertRaises(InvalidMetadata):
             PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertFalse(is_runtime_path_valid(path))
 
         # When/Then
         with tempdir() as d:
-            path = os.path.join(d, "foo.zip")
-            with zipfile2.ZipFile(path, "w") as zp:
+            path = os.path.join(d, 'foo.zip')
+            with zipfile2.ZipFile(path, 'w') as zp:
                 pass
 
             with self.assertRaises(InvalidMetadata):
                 PythonRuntimeMetadataV1._from_path(path)
 
-            with zipfile2.ZipFile(path, "w") as zp:
+            with zipfile2.ZipFile(path, 'w') as zp:
                 with self.assertRaises(InvalidMetadata):
                     PythonRuntimeMetadataV1._from_path(zp)
 
-
-class TestCPython38RuntimeMetadataV1(unittest.TestCase):
-
-    def test_gnu(self):
-        # Given
-        path = PYTHON_CPYTHON_3_8_8_RH7_X86_64
+    @given(
+        sampled_from([
+            (PYTHON_CPYTHON_2_7_10_RH5_X86_64, '2.7.10+1', '5.8'),
+            (PYTHON_CPYTHON_3_8_8_RH7_X86_64, '3.8.8+1', '7.1'),
+            (PYTHON_CPYTHON_3_11_2_RH8_X86_64, '3.11.2+2', '8.8')]))
+    def test_cpython_gnu(self, options):
+        # Given
+        path, release, os_release = options
+        version = RuntimeVersion.from_string(release.split('+')[0])
+        release = RuntimeVersion.from_string(release)
+        lib = '${{prefix}}/lib/python{0}.{1}'.format(version.major, version.minor)
+        tag = 'cp{0}{1}'.format(version.major, version.minor)
 
         # When
         metadata = PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertTrue(is_runtime_path_valid(path))
         self.assertEqual(metadata.filename, os.path.basename(path))
         self.assertEqual(
-            metadata.metadata_version, MetadataVersion.from_string("1.0"))
-        self.assertEqual(metadata.implementation, "cpython")
-        self.assertEqual(
-            metadata.version, RuntimeVersion.from_string("3.8.8+1"))
-        self.assertEqual(
-            metadata.language_version, RuntimeVersion.from_string("3.8.8"))
-        self.assertEqual(metadata.build_revision, "2.1.0-dev570")
-        self.assertEqual(metadata.executable, "${prefix}/bin/python")
-        self.assertEqual(metadata.paths, ("${prefix}/bin",))
+            metadata.metadata_version, MetadataVersion.from_string('1.0'))
+        self.assertEqual(metadata.implementation, 'cpython')
+        self.assertEqual(metadata.version, release)
+        self.assertEqual(metadata.language_version, version)
+        self.assertEqual(metadata.build_revision, '2.1.0-dev570')
+        self.assertEqual(metadata.executable, '${prefix}/bin/python')
+        self.assertEqual(metadata.paths, ('${prefix}/bin',))
         self.assertEqual(
             metadata.post_install,
-            ("${executable}",
-             "${prefix}/lib/python3.8/custom_tools/fix-scripts.py"))
-        self.assertEqual(metadata.scriptsdir, "${prefix}/bin")
+            ('${executable}', f'{lib}/custom_tools/fix-scripts.py'))
+        self.assertEqual(metadata.scriptsdir, '${prefix}/bin')
         self.assertEqual(
-            metadata.site_packages, "${prefix}/lib/python3.8/site-packages")
-        self.assertEqual(metadata.python_tag, "cp38")
+            metadata.site_packages, f'{lib}/site-packages')
+        self.assertEqual(metadata.python_tag, tag)
         self.assertEqual(
             metadata.platform,
             Platform(
                 os_kind=OSKind.linux,
                 family_kind=FamilyKind.rhel,
                 name_kind=NameKind.rhel,
-                release='7.1',
+                release=os_release,
                 arch=X86_64,
                 machine=X86_64))
 
-    def test_darwin(self):
-        # Given
-        path = PYTHON_CPYTHON_3_8_8_OSX_X86_64
+    @given(
+        sampled_from([
+            (PYTHON_CPYTHON_3_8_8_OSX_X86_64, '3.8.8+1', '10.14'),
+            (PYTHON_CPYTHON_3_11_2_OSX_X86_64, '3.11.2+2', '12.0')]))
+    def test_cpython_darwin(self, options):
+        # Given
+        path, release, os_release = options
+        version = RuntimeVersion.from_string(release.split('+')[0])
+        release = RuntimeVersion.from_string(release)
+        lib = '${{prefix}}/lib/python{0}.{1}'.format(version.major, version.minor)
+        tag = 'cp{0}{1}'.format(version.major, version.minor)
 
         # When
         metadata = PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertTrue(is_runtime_path_valid(path))
         self.assertEqual(metadata.filename, os.path.basename(path))
         self.assertEqual(
-            metadata.metadata_version, MetadataVersion.from_string("1.0"))
-        self.assertEqual(metadata.implementation, "cpython")
-        self.assertEqual(
-            metadata.version, RuntimeVersion.from_string("3.8.8+1"))
-        self.assertEqual(
-            metadata.language_version, RuntimeVersion.from_string("3.8.8"))
-        self.assertEqual(metadata.build_revision, "2.1.0-dev570")
-        self.assertEqual(metadata.executable, "${prefix}/bin/python")
-        self.assertEqual(metadata.paths, ("${prefix}/bin",))
+            metadata.metadata_version, MetadataVersion.from_string('1.0'))
+        self.assertEqual(metadata.implementation, 'cpython')
+        self.assertEqual(metadata.version, release)
+        self.assertEqual(metadata.language_version, version)
+        self.assertEqual(metadata.build_revision, '2.1.0-dev570')
+        self.assertEqual(metadata.executable, '${prefix}/bin/python')
+        self.assertEqual(metadata.paths, ('${prefix}/bin',))
         self.assertEqual(
             metadata.post_install,
-            ("${executable}",
-             "${prefix}/lib/python3.8/custom_tools/fix-scripts.py"))
-        self.assertEqual(metadata.scriptsdir, "${prefix}/bin")
+            ('${executable}', f'{lib}/custom_tools/fix-scripts.py'))
+        self.assertEqual(metadata.scriptsdir, '${prefix}/bin')
         self.assertEqual(
-            metadata.site_packages, "${prefix}/lib/python3.8/site-packages")
-        self.assertEqual(metadata.python_tag, "cp38")
+            metadata.site_packages, f'{lib}/site-packages')
+        self.assertEqual(metadata.python_tag, tag)
         self.assertEqual(
             metadata.platform,
             Platform(
                 os_kind=OSKind.darwin,
                 family_kind=FamilyKind.mac_os_x,
                 name_kind=NameKind.mac_os_x,
-                release='10.14',
-                arch=X86_64,
-                machine=X86_64))
-
-    def test_win64(self):
-        # Given
-        path = PYTHON_CPYTHON_3_8_8_WIN_X86_64
-
-        # When
-        metadata = PythonRuntimeMetadataV1._from_path(path)
-
-        # Then
-        self.assertTrue(is_runtime_path_valid(path))
-        self.assertEqual(metadata.filename, os.path.basename(path))
-        self.assertEqual(
-            metadata.metadata_version, MetadataVersion.from_string("1.0"))
-        self.assertEqual(metadata.implementation, "cpython")
-        self.assertEqual(
-            metadata.version, RuntimeVersion.from_string("3.8.8+1"))
-        self.assertEqual(
-            metadata.language_version, RuntimeVersion.from_string("3.8.8"))
-        self.assertEqual(metadata.build_revision, "2.1.0-dev570")
-        self.assertEqual(metadata.executable, "${prefix}\\python.exe")
-        self.assertEqual(metadata.paths, ("${prefix}", "${prefix}\\Scripts"))
-        self.assertEqual(
-            metadata.post_install,
-            ("${executable}",
-             "${prefix}\\Lib\\custom_tools\\fix-scripts.py"))
-        self.assertEqual(metadata.scriptsdir, "${prefix}\\Scripts")
-        self.assertEqual(
-            metadata.site_packages, "${prefix}\\Lib\\site-packages")
-        self.assertEqual(metadata.python_tag, "cp38")
-        self.assertEqual(
-            metadata.platform,
-            Platform(
-                os_kind=OSKind.windows,
-                family_kind=FamilyKind.windows,
-                name_kind=NameKind.windows,
-                release='10',
+                release=os_release,
                 arch=X86_64,
                 machine=X86_64))
 
-    def test_win32(self):
-        # Given
-        path = PYTHON_CPYTHON_3_8_8_WIN_X86
+    @given(
+        sampled_from([
+            (PYTHON_CPYTHON_3_11_2_WIN_X86_64, '3.11.2+2', '10', X86_64),
+            (PYTHON_CPYTHON_3_8_8_WIN_X86_64, '3.8.8+1', '10', X86_64),
+            (PYTHON_CPYTHON_3_8_8_WIN_X86, '3.8.8+1', '10', X86)]))
+    def test_cpython_windows(self, options):
+        # Given
+        path, release, os_release, arch = options
+        version = RuntimeVersion.from_string(release.split('+')[0])
+        release = RuntimeVersion.from_string(release)
+        tag = 'cp{0}{1}'.format(version.major, version.minor)
 
         # When
         metadata = PythonRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertTrue(is_runtime_path_valid(path))
         self.assertEqual(metadata.filename, os.path.basename(path))
         self.assertEqual(
-            metadata.metadata_version, MetadataVersion.from_string("1.0"))
-        self.assertEqual(metadata.implementation, "cpython")
-        self.assertEqual(
-            metadata.version, RuntimeVersion.from_string("3.8.8+1"))
-        self.assertEqual(
-            metadata.language_version, RuntimeVersion.from_string("3.8.8"))
-        self.assertEqual(metadata.build_revision, "2.1.0-dev570")
-        self.assertEqual(metadata.executable, "${prefix}\\python.exe")
-        self.assertEqual(metadata.paths, ("${prefix}", "${prefix}\\Scripts"))
+            metadata.metadata_version, MetadataVersion.from_string('1.0'))
+        self.assertEqual(metadata.implementation, 'cpython')
+        self.assertEqual(metadata.version, release)
+        self.assertEqual(metadata.language_version, version)
+        self.assertEqual(metadata.build_revision, '2.1.0-dev570')
+        self.assertEqual(metadata.executable, '${prefix}\\python.exe')
+        self.assertEqual(metadata.paths, ('${prefix}', '${prefix}\\Scripts'))
         self.assertEqual(
             metadata.post_install,
-            ("${executable}",
-             "${prefix}\\Lib\\custom_tools\\fix-scripts.py"))
-        self.assertEqual(metadata.scriptsdir, "${prefix}\\Scripts")
+            ('${executable}',
+             '${prefix}\\Lib\\custom_tools\\fix-scripts.py'))
+        self.assertEqual(metadata.scriptsdir, '${prefix}\\Scripts')
         self.assertEqual(
-            metadata.site_packages, "${prefix}\\Lib\\site-packages")
-        self.assertEqual(metadata.python_tag, "cp38")
+            metadata.site_packages, '${prefix}\\Lib\\site-packages')
+        self.assertEqual(metadata.python_tag, tag)
         self.assertEqual(
             metadata.platform,
             Platform(
                 os_kind=OSKind.windows,
                 family_kind=FamilyKind.windows,
                 name_kind=NameKind.windows,
-                release='10',
-                arch=X86,
-                machine=X86))
+                release=os_release,
+                arch=arch,
+                machine=arch))
 
 
 class TestJuliaRuntimeMetadataV1(unittest.TestCase):
     def test_simple(self):
         # Given
         path = JULIA_DEFAULT_0_3_11_RH5_X86_64
 
         # When
         metadata = JuliaRuntimeMetadataV1._from_path(path)
 
         # Then
         self.assertEqual(
             metadata.metadata_version,
-            MetadataVersion.from_string("1.0")
+            MetadataVersion.from_string('1.0')
         )
         self.assertEqual(metadata.filename, os.path.basename(path))
-        self.assertEqual(metadata.implementation, "julia")
+        self.assertEqual(metadata.implementation, 'julia')
         self.assertEqual(
             metadata.version,
-            RuntimeVersion.from_string("0.3.11+1")
+            RuntimeVersion.from_string('0.3.11+1')
         )
         self.assertEqual(
             metadata.language_version,
-            RuntimeVersion.from_string("0.3.11")
+            RuntimeVersion.from_string('0.3.11')
         )
-        self.assertEqual(metadata.build_revision, "483dbf5279")
-        self.assertEqual(metadata.executable, "${prefix}/bin/julia")
-        self.assertEqual(metadata.paths, ("${prefix}/bin",))
+        self.assertEqual(metadata.build_revision, '483dbf5279')
+        self.assertEqual(metadata.executable, '${prefix}/bin/julia')
+        self.assertEqual(metadata.paths, ('${prefix}/bin',))
         self.assertEqual(metadata.post_install, tuple())
 
 
 class TestRuntimeMetadataFactory(unittest.TestCase):
     def test_simple(self):
         # Given
         path = PYTHON_CPYTHON_2_7_10_RH5_X86_64
@@ -371,36 +314,35 @@
 
         # Given
         path = PYTHON_CPYTHON_2_7_10_RH5_X86_64_INVALID
 
         # When/Then
         with tempdir() as d:
             target = os.path.join(
-                d, os.path.basename(path).replace(".invalid", "")
+                d, os.path.basename(path).replace('.invalid', '')
             )
             shutil.copy(path, target)
 
             with self.assertRaises(InvalidMetadata):
                 runtime_metadata_factory(target)
 
         # Given
         path = PYTHON_CPYTHON_2_7_10_RH5_X86_64
 
         # When/Then
         with tempdir() as d:
             target = os.path.join(d, os.path.basename(path))
             # One needs to add an archive for the zipfile to be valid on 2.6.
-            with zipfile2.ZipFile(target, "w") as zp:
-                zp.writestr("dummy", b"dummy data")
+            with zipfile2.ZipFile(target, 'w') as zp:
+                zp.writestr('dummy', b'dummy data')
             with self.assertRaises(MissingMetadata):
                 runtime_metadata_factory(target)
 
     def test_missing_metadata(self):
         # Given
         path = INVALID_RUNTIME_NO_METADATA_VERSION
 
         # When/Then
         with self.assertRaisesRegexp(
-            MissingMetadata,
-            r"^Missing runtime metadata field 'metadata_version'$"
-        ):
+                MissingMetadata,
+                r"^Missing runtime metadata field 'metadata_version'$"):
             runtime_metadata_factory(path)
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_info.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_info.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_metadata.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_metadata.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/runtimes/runtime_schemas.py` & `okonomiyaki-1.4.0/okonomiyaki/runtimes/runtime_schemas.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/osx_x86_64/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/osx_x86_64/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh5_x86_64/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh5_x86_64/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh6_x86_64/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh6_x86_64/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/rh7_x86_64/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/rh7_x86_64/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/MKL-10.3-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/MKL-10.3-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/nose-1.3.4-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/nose-1.3.4-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/eggs/win_x86_64/numpy-1.9.2-1.egg` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/eggs/win_x86_64/numpy-1.9.2-1.egg`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/wheels/okonomiyaki-0.17.0.dev799-py2-none-any.whl` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/wheels/okonomiyaki-0.17.0.dev799-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/__init__.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,14 +116,27 @@
     _HERE, "cpython-3.8.8+1-win_x86_64-msvc2019.runtime",
 )
 PYTHON_CPYTHON_3_8_8_WIN_X86 = os.path.join(
     _HERE, "cpython-3.8.8+1-win_x86-msvc2019.runtime",
 )
 
 
+# 3.11.2
+PYTHON_CPYTHON_3_11_2_RH8_X86_64 = os.path.join(
+    _HERE, "cpython-3.11.2+2-rh8_x86_64-gnu.runtime",
+)
+PYTHON_CPYTHON_3_11_2_OSX_X86_64 = os.path.join(
+    _HERE, "cpython-3.11.2+2-osx_x86_64-darwin.runtime",
+)
+PYTHON_CPYTHON_3_11_2_WIN_X86_64 = os.path.join(
+    _HERE, "cpython-3.11.2+2-win_x86_64-msvc2022.runtime",
+)
+
+
+# Misc
 PYTHON_CPYTHON_2_7_10_RH5_X86_64_INVALID = os.path.join(
     _HERE, "cpython-2.7.10+1-rh5_x86_64-gnu.runtime.invalid",
 )
 PYTHON_PYPY_2_6_0_RH5_X86_64 = os.path.join(
     _HERE, "pypy-2.6.0+1-rh5_x86_64-gnu.runtime",
 )
 JULIA_DEFAULT_0_3_11_RH5_X86_64 = os.path.join(
@@ -224,7 +237,39 @@
     NUMPY_1_9_2_RH7_X86_64_cp38,
     NOSE_1_3_4_WIN_X86_64_cp38,
     MKL_10_3_WIN_X86_64_cp38,
     NUMPY_1_9_2_WIN_X86_64_cp38,
     NOSE_1_3_4_OSX_X86_64_cp38,
     MKL_10_3_OSX_X86_64_cp38,
     NUMPY_1_9_2_OSX_X86_64_cp38]
+
+# cp38 eggs for testing
+
+_RH8_X86_64_cp311 = os.path.join(_HERE, "eggs", "rh8_x86_64", "cp311")
+
+NOSE_1_3_4_RH7_X86_64_cp311 = os.path.join(_RH8_X86_64_cp311, "nose-1.3.4-1.egg")
+MKL_10_3_RH7_X86_64_cp311 = os.path.join(_RH8_X86_64_cp311, "MKL-10.3-1.egg")
+NUMPY_1_9_2_RH7_X86_64_cp311 = os.path.join(_RH8_X86_64_cp311, "numpy-1.9.2-1.egg")
+
+_WIN_X86_64_cp311 = os.path.join(_HERE, "eggs", "win_x86_64", "cp311")
+
+NOSE_1_3_4_WIN_X86_64_cp311 = os.path.join(_WIN_X86_64_cp311, "nose-1.3.4-1.egg")
+MKL_10_3_WIN_X86_64_cp311 = os.path.join(_WIN_X86_64_cp311, "MKL-10.3-1.egg")
+NUMPY_1_9_2_WIN_X86_64_cp311 = os.path.join(_WIN_X86_64_cp311, "numpy-1.9.2-1.egg")
+
+_OSX_X86_64_cp311 = os.path.join(_HERE, "eggs", "osx_x86_64", "cp311")
+
+NOSE_1_3_4_OSX_X86_64_cp311 = os.path.join(_OSX_X86_64_cp311, "nose-1.3.4-1.egg")
+MKL_10_3_OSX_X86_64_cp311 = os.path.join(_OSX_X86_64_cp311, "MKL-10.3-1.egg")
+NUMPY_1_9_2_OSX_X86_64_cp311 = os.path.join(_OSX_X86_64_cp311, "numpy-1.9.2-1.egg")
+
+
+CP311_EGGS = [
+    NOSE_1_3_4_RH7_X86_64_cp311,
+    MKL_10_3_RH7_X86_64_cp311,
+    NUMPY_1_9_2_RH7_X86_64_cp311,
+    NOSE_1_3_4_WIN_X86_64_cp311,
+    MKL_10_3_WIN_X86_64_cp311,
+    NUMPY_1_9_2_WIN_X86_64_cp311,
+    NOSE_1_3_4_OSX_X86_64_cp311,
+    MKL_10_3_OSX_X86_64_cp311,
+    NUMPY_1_9_2_OSX_X86_64_cp311]
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime.invalid` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh5_x86_64-gnu.runtime.invalid`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh6_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh6_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86_64-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.10+1-win_x86_64-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh6_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh6_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86_64-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86_64-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime.invalid` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime.invalid`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh6_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh6_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86_64-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86_64-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh6_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh6_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86_64-msvc2008.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.5.1+1-win_x86_64-msvc2008.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh6_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh6_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86-msvc2015.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86-msvc2015.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86_64-msvc2015.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.6.5+1-win_x86_64-msvc2015.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-osx_x86_64-darwin.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-osx_x86_64-darwin.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-rh7_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-rh7_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86-msvc2019.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86-msvc2019.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86_64-msvc2019.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/cpython-3.8.8+1-win_x86_64-msvc2019.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/julia-0.3.11+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/julia-0.3.11+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/julia-0.3.11+1-win_x86_64-mingw.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/julia-0.3.11+1-win_x86_64-mingw.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/test_data/pypy-2.6.0+1-rh5_x86_64-gnu.runtime` & `okonomiyaki-1.4.0/okonomiyaki/utils/test_data/pypy-2.6.0+1-rh5_x86_64-gnu.runtime`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_eggs.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_eggs.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from hypothesis import given
 from hypothesis.strategies import sampled_from
 
 from okonomiyaki.file_formats import EggMetadata
 from okonomiyaki.platforms import PlatformABI
 
-from ..test_data import CP38_EGGS, CP27_EGGS
+from ..test_data import CP38_EGGS, CP27_EGGS, CP311_EGGS
 
 
 class TestDummyEggs(unittest.TestCase):
 
     @given(sampled_from(CP38_EGGS))
     def test_cp38_egg_metadata_valid(self, filepath):
         # when
@@ -30,14 +30,37 @@
         elif 'win_x86_64' in filepath:
             self.assertEqual(metadata.platform_tag, 'win_amd64')
             self.assertEqual(metadata.platform_abi, PlatformABI(u'msvc2019'))
         else:
             self.assertEqual(metadata.platform_tag, 'linux_x86_64')
             self.assertEqual(metadata.platform_abi, PlatformABI(u'gnu'))
 
+    @given(sampled_from(CP311_EGGS))
+    def test_cp311_egg_metadata_valid(self, filepath):
+        # when
+        metadata = EggMetadata.from_egg(filepath)
+        filepath = filepath.lower()
+
+        # then
+        if 'mkl' in metadata.name:
+            self.assertEqual(metadata.python_tag, None)
+            self.assertEqual(metadata.abi_tag, None)
+        else:
+            self.assertEqual(metadata.python_tag, 'cp311')
+            self.assertEqual(metadata.abi_tag, 'cp311')
+        if 'osx_x86_64' in filepath:
+            self.assertEqual(metadata.platform_tag, 'macosx_12_0_x86_64')
+            self.assertEqual(metadata.platform_abi, PlatformABI(u'darwin'))
+        elif 'win_x86_64' in filepath:
+            self.assertEqual(metadata.platform_tag, 'win_amd64')
+            self.assertEqual(metadata.platform_abi, PlatformABI(u'msvc2022'))
+        else:
+            self.assertEqual(metadata.platform_tag, 'linux_x86_64')
+            self.assertEqual(metadata.platform_abi, PlatformABI(u'gnu'))
+
     @given(sampled_from(CP27_EGGS))
     def test_cp27_egg_metadata_valid(self, filepath):
         # when
         metadata = EggMetadata.from_egg(filepath)
         filepath = filepath.lower()
 
         # then
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_main.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_misc.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/tests/test_test_data.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/tests/test_runtimes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import glob
 from os.path import join
 import sys
+
 import zipfile2
+from hypothesis import given
+from hypothesis.strategies import sampled_from
+
 
 from okonomiyaki.runtimes.runtime_metadata import IRuntimeMetadata
-from okonomiyaki.errors import UnsupportedMetadata
 
 from ..test_data import DUMMY_RUNTIMES_DIRECTORY
 
 if sys.version_info < (2, 7):
     import unittest2 as unittest
 else:
     import unittest
 
 
+runtime_paths = [
+    join(DUMMY_RUNTIMES_DIRECTORY, f) for f
+    in glob.glob(join(DUMMY_RUNTIMES_DIRECTORY, '*.runtime'))
+    if 'r-3.0.0' not in f]
+
+
 class TestDummyPythonRuntimes(unittest.TestCase):
 
     def _get_contents_of_runtime(self, runtime):
         with zipfile2.ZipFile(runtime) as zp:
             return zp.namelist()
 
-    def test_pythonw_in_dummy_runtime(self):
-        """
-        Ensure that pythonw.exe is included in all Windows runtimes
-        """
-
-        # Given
-        runtime_paths = [join(DUMMY_RUNTIMES_DIRECTORY, f) for f
-                         in glob.glob(join(DUMMY_RUNTIMES_DIRECTORY, '*.runtime'))]
-        win_cpy_runtimes = []
-        for runtime_path in runtime_paths:
-            try:
-                runtime_metadata = IRuntimeMetadata.factory_from_path(runtime_path)
-                if (runtime_metadata.platform.os == 'windows'
-                   and runtime_metadata.implementation == 'cpython'):
-                    win_cpy_runtimes.append(runtime_path)
-            except UnsupportedMetadata:
-                continue
-
-        # When/Then
-        self.assertGreaterEqual(len(win_cpy_runtimes), 1)
-        for win_runtime in win_cpy_runtimes:
-            files_in_runtime = self._get_contents_of_runtime(win_runtime)
+    @given(sampled_from(runtime_paths))
+    def test_reading_dummy_runtimes(self, runtime):
+        # Then check the runtime is valid
+        runtime_metadata = IRuntimeMetadata.factory_from_path(runtime)
+
+        # additional checks for windows runtimes:
+        if 'cpython-' in runtime and 'win_' in runtime:
+            self.assertEqual(runtime_metadata.platform.os, 'windows')
+            self.assertEqual(runtime_metadata.implementation, 'cpython')
+            files_in_runtime = self._get_contents_of_runtime(runtime)
             self.assertIn(
                 'pythonw.exe', files_in_runtime,
-                msg="'pythonw.exe' is not in {0}".format(win_runtime)
-            )
+                msg="'pythonw.exe' is not in {0}".format(runtime))
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/__init__.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/misc.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/misc.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/py3compat.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/py3compat.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/utils/testing.py` & `okonomiyaki-1.4.0/okonomiyaki/utils/testing.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_enpkg_version.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_enpkg_version.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_metadata_version.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_metadata_version.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_pep386_workaround.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_pep386_workaround.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_pep440.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_pep440.py`

 * *Files 5% similar despite different names*

```diff
@@ -181,14 +181,25 @@
         # Given
         v1 = V("1.2.0")
         v2 = V("1.2.0")
 
         # When/Then
         self.assertEqual(hash(v1), hash(v2))
 
+    def test_repr(self):
+        # Given
+        v1 = V("1.2.0")
+
+        # When
+        result = repr(v1)
+
+        # Then
+        self.assertEqual(result, "PEP440Version.from_string('1.2.0')")
+        self.assertEqual(eval(result), v1)
+
     def test_invalid(self):
         # Given
         left = V("1.0")
         right = "1.0"
 
         # When/Then
         with self.assertRaises(TypeError):
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_runtime_version.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_runtime_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,25 @@
 
         self.assertEqual(hash(v1), hash(v2))
 
     def test_str(self):
         self.assertEqual(str(V("1.2.0")), "1.2.0")
         self.assertEqual(V("1.2.0").normalized_string, "1.2")
 
+    def test_repr(self):
+        # given
+        v1 = V("1.2.0")
+
+        # when
+        result = repr(v1)
+
+        # then
+        self.assertEqual(result, "RuntimeVersion.from_string('1.2.0')")
+        self.assertEqual(eval(result), v1)
+
     def test_simple(self):
         self.assertTrue(V("1.2.0") == V("1.2"))
         self.assertFalse(V("1.2.0") == V("1.2.3"))
         self.assertTrue(V("1.2.0") != V("1.2.3"))
         self.assertTrue(V("1.2.0") < V("1.2.3"))
         self.assertFalse(V("1.2.3") < V("1.2.0"))
         self.assertTrue(V("1.2.0") <= V("1.2.3"))
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/tests/test_semver.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/enpkg.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/enpkg.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/metadata_version.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/metadata_version.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/pep386.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/pep386.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This module implements PEP 386
 # 2010-04-20: hg clone http://bitbucket.org/tarek/distutilsversion/
 
 """
 "Rational" version definition and parsing for DistutilsVersionFight
 discussion at PyCon 2009.
 """
-import sys
 import re
 
 
 class IrrationalVersionError(Exception):
     """This is an irrational version."""
     pass
 
+
 class HugeMajorVersionNumError(IrrationalVersionError):
     """An irrational version because the major version number is huge
     (often because a year or date was used).
 
     See `error_on_huge_major_num` option in `NormalizedVersion` for details.
     This guard can be disabled by setting that option False.
     """
     pass
 
+
 # A marker used in the second and third parts of the `parts` tuple, for
 # versions that don't have those segments, to sort properly. An example
 # of versions in sort order ('highest' last):
 #   1.0b1                 ((1,0), ('b',1), ('f',))
 #   1.0.dev345            ((1,0), ('dev', 345), ('f',))
 #   1.0                   ((1,0), ('f',),  ('f',))
 #   1.0.post256.dev345    ((1,0), ('f',),  ('f', 'post', 256, 'dev', 345))
@@ -48,14 +49,15 @@
                                    # '.dev'=dev version (e.g. pre-alpha)
                                    # 'rc'= alias for release candidate
         (?P<prerelversion>\d+(?:\.\d+)*)
     )?
     (?P<postdev>(\.post(?P<post>\d+))?(\.dev(?P<dev>\d+))?)?
     $''', re.VERBOSE)
 
+
 class NormalizedVersion(object):
     """A rational version.
 
     Good:
         1.2         # equivalent to "1.2.0"
         1.2.0
         1.2a1
@@ -131,15 +133,16 @@
             if dev is not None:
                 postdev.extend(['dev', int(dev)])
             parts.append(tuple(postdev))
         else:
             parts.append(FINAL_MARKER)
         self.parts = tuple(parts)
         if error_on_huge_major_num and self.parts[0][0] > 1980:
-            raise HugeMajorVersionNumError("huge major version number, %r, "
+            raise HugeMajorVersionNumError(
+                "huge major version number, %r, "
                 "which might cause future problems: %r" % (self.parts[0][0], s))
 
     def _parse_numdots(self, s, full_ver_str, drop_trailing_zeros=False,
                        pad_zeros_length=0):
         """Parse 'N.N.N' sequences, return a list of ints.
 
         @param s {str} 'N.N.N..." sequence to be parsed
@@ -149,15 +152,16 @@
             from the returned list. Default True.
         @param pad_zeros_length {int} The length to which to pad the
             returned list with zeros, if necessary. Default 0.
         """
         nums = []
         for n in s.split("."):
             if len(n) > 1 and n[0] == '0':
-                raise IrrationalVersionError("cannot have leading zero in "
+                raise IrrationalVersionError(
+                    "cannot have leading zero in "
                     "version number segment: '%s' in %r" % (n, full_ver_str))
             nums.append(int(n))
         if drop_trailing_zeros:
             while nums and nums[-1] == 0:
                 nums.pop()
         while len(nums) < pad_zeros_length:
             nums.append(0)
@@ -189,16 +193,17 @@
                 i += 1
         return s
 
     def __repr__(self):
         return "%s('%s')" % (self.__class__.__name__, self)
 
     def _cannot_compare(self, other):
-        raise TypeError("cannot compare %s and %s"
-                % (type(self).__name__, type(other).__name__))
+        raise TypeError(
+            "cannot compare %s and %s"
+            % (type(self).__name__, type(other).__name__))
 
     def __eq__(self, other):
         if not isinstance(other, NormalizedVersion):
             self._cannot_compare(other)
         return self.parts == other.parts
 
     def __lt__(self, other):
@@ -214,14 +219,15 @@
 
     def __le__(self, other):
         return self.__eq__(other) or self.__lt__(other)
 
     def __ge__(self, other):
         return self.__eq__(other) or self.__gt__(other)
 
+
 def suggest_normalized_version(s):
     """Suggest a normalized version close to the given version string.
 
     If you have a version string that isn't rational (i.e. NormalizedVersion
     doesn't like it) then you might be able to get an equivalent (or close)
     rational version from this function.
 
@@ -269,15 +275,15 @@
     rs = re.sub(r"[.~]?([abc])\.?", r"\1", rs)
 
     # Clean: v0.3, v1.0
     if rs.startswith('v'):
         rs = rs[1:]
 
     # Clean leading '0's on numbers.
-    #TODO: unintended side-effect on, e.g., "2003.05.09"
+    # TODO: unintended side-effect on, e.g., "2003.05.09"
     # PyPI stats: 77 (~2%) better
     rs = re.sub(r"\b0+(\d+)(?!\d)", r"\1", rs)
 
     # Clean a/b/c with no version. E.g. "1.0a" -> "1.0a0". Setuptools infers
     # zero.
     # PyPI stats: 245 (7.56%) better
     rs = re.sub(r"(\d+[abc])$", r"\g<1>0", rs)
@@ -315,18 +321,16 @@
     # Clean '.pre' (normalized from '-pre' above) instead of 'c' usage:
     #   0.2.pre1        ->  0.2c1
     #   0.2-c1         ->  0.2c1
     #   1.0preview123   ->  1.0c123
     # PyPI stats: ~21 (0.62%) better
     rs = re.sub(r"\.?(pre|preview|-c)(\d+)$", r"c\g<2>", rs)
 
-
     # Tcl/Tk uses "px" for their post release markers
     rs = re.sub(r"p(\d+)$", r".post\1", rs)
 
     try:
         NormalizedVersion(rs)
         return rs   # already rational
     except IrrationalVersionError:
         pass
     return None
-
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/pep386_workaround.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/pep386_workaround.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/pep440.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/pep440.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         return self._parts >= other._parts
 
     def __gt__(self, other):
         self._ensure_compatible(other)
         return self._parts > other._parts
 
     def __repr__(self):
-        return "{0}('{1}')".format(self.__class__.__name__, str(self))
+        return "{0}.from_string('{1!s}')".format(self.__class__.__name__, self)
 
     def __str__(self):
         if self._string is None:
             nums = self._release_clause
             epoch, _, pre, post, dev, local = self._parts
             self._string = self._compute_string(
                 epoch, nums, pre, post, dev, local
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/runtime_version.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/runtime_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         if not isinstance(other, self.__class__):
             msg = "Cannot compare {0!r} and {1!r}"
             raise TypeError(msg.format(type(self), type(other)))
 
     def __str__(self):
         return str(self._pep440_version)
 
+    def __repr__(self):
+        return "{0}.from_string('{1!s}')".format(self.__class__.__name__, self)
+
     def __hash__(self):
         return hash(self._pep440_version)
 
     def __eq__(self, other):
         self._ensure_can_compare(other)
         return self._pep440_version == other._pep440_version
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki/versions/semver.py` & `okonomiyaki-1.4.0/okonomiyaki/versions/semver.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki/errors.py` & `okonomiyaki-1.4.0/okonomiyaki/errors.py`

 * *Files identical despite different names*

### Comparing `okonomiyaki-1.3.2/okonomiyaki.egg-info/PKG-INFO` & `okonomiyaki-1.4.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,63 @@
-Metadata-Version: 1.1
-Name: okonomiyaki
-Version: 1.3.2
-Summary: ('Self-contained library to deal with metadata in Enthought-specific eggs',)
-Home-page: UNKNOWN
-Author: Enthought, Inc.
-Author-email: info@enthought.com
-License: BSD
-Description: .. image:: https://travis-ci.com/enthought/okonomiyaki.svg?branch=master
-            :target: https://travis-ci.com/enthought/okonomiyaki
-        
-        Okonomiyaki is an experimental library aimed at consolidating a lot of our
-        low-level code used for Enthought's eggs.
-        
-        The library contains code for the following:
-        
-        * producing EDM and enpkg-compatible egg from a tree + metadata
-        * object models for eggs metadata, as well as versions and platform
-          representations
-        
-        It works on both python 2 and 3, and pypy. It is expected to work on pretty
-        much any compliant python implementation.
-        
-        Examples
-        ========
-        
-        Version parsing
-        ---------------
-        
-        To parse versions::
-        
-             from okonomiyaki.versions import EnpkgVersion
-             # Every Version class has a from_string constructor
-             v1 = EnpkgVersion.from_string("1.3.3-1")
-             v2 = EnpkgVersion.from_string("1.3.2-3")
-        
-             assert v1 > v2
-        
-        Version instances are designed to be immutable, and to be used as keys in
-        dictionaries.
-        
-        Platform parsing
-        ----------------
-        
-        To parse epd platform strings (``rh5-64``, ``rh6_x86_64``, etc.) consistently::
-        
-            from okonomiyaki.platforms import EPDPlatform
-            # Internal representation is normalized.
-            rh5_new_name = EPDPlatform.from_string("rh5-x86_64")
-            rh5_old_name = EPDPlatform.from_string("rh5-64")
-        
-            assert rh5_old_name == rh5_new_name
-        
-        As for Version instances, ``EPDPlatform`` instances are designed to be
-        immutable and to be used as keys in dictionaries.
-        
-        Egg metadata
-        ------------
-        
-        To parse Enthought eggs::
-        
-            from okonomiyaki.file_formats import EggMetadata
-        
-            # Only works for Enthought eggs
-            metadata = EggMetadata.from_egg("numpy-1.10.1-1.egg")
-            print(metadata.metadata_version)
-            print(metadata.name)
-            print(metadata.version)
-        
-        This will take care of a lot of low-level, legacy details you don't want to
-        know about.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+.. image:: https://travis-ci.com/enthought/okonomiyaki.svg?branch=master
+    :target: https://travis-ci.com/enthought/okonomiyaki
+
+Okonomiyaki is an experimental library aimed at consolidating a lot of our
+low-level code used for Enthought's eggs.
+
+The library contains code for the following:
+
+* producing EDM and enpkg-compatible egg from a tree + metadata
+* object models for eggs metadata, as well as versions and platform
+  representations
+
+It works on both python 2 and 3, and pypy. It is expected to work on pretty
+much any compliant python implementation.
+
+Examples
+========
+
+Version parsing
+---------------
+
+To parse versions::
+
+     from okonomiyaki.versions import EnpkgVersion
+     # Every Version class has a from_string constructor
+     v1 = EnpkgVersion.from_string("1.3.3-1")
+     v2 = EnpkgVersion.from_string("1.3.2-3")
+
+     assert v1 > v2
+
+Version instances are designed to be immutable, and to be used as keys in
+dictionaries.
+
+Platform parsing
+----------------
+
+To parse epd platform strings (``rh5-64``, ``rh6_x86_64``, etc.) consistently::
+
+    from okonomiyaki.platforms import EPDPlatform
+    # Internal representation is normalized.
+    rh5_new_name = EPDPlatform.from_string("rh5-x86_64")
+    rh5_old_name = EPDPlatform.from_string("rh5-64")
+
+    assert rh5_old_name == rh5_new_name
+
+As for Version instances, ``EPDPlatform`` instances are designed to be
+immutable and to be used as keys in dictionaries.
+
+Egg metadata
+------------
+
+To parse Enthought eggs::
+
+    from okonomiyaki.file_formats import EggMetadata
+
+    # Only works for Enthought eggs
+    metadata = EggMetadata.from_egg("numpy-1.10.1-1.egg")
+    print(metadata.metadata_version)
+    print(metadata.name)
+    print(metadata.version)
+
+This will take care of a lot of low-level, legacy details you don't want to
+know about.
```

### Comparing `okonomiyaki-1.3.2/okonomiyaki.egg-info/SOURCES.txt` & `okonomiyaki-1.4.0/okonomiyaki.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+CHANGELOG
 LICENSE.txt
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 okonomiyaki/__init__.py
 okonomiyaki/__main__.py
 okonomiyaki/_version.py
 okonomiyaki/errors.py
 okonomiyaki.egg-info/PKG-INFO
 okonomiyaki.egg-info/SOURCES.txt
 okonomiyaki.egg-info/dependency_links.txt
+okonomiyaki.egg-info/not-zip-safe
 okonomiyaki.egg-info/requires.txt
 okonomiyaki.egg-info/top_level.txt
 okonomiyaki/_cli/__init__.py
 okonomiyaki/_cli/tests/__init__.py
 okonomiyaki/_cli/tests/test_cli.py
 okonomiyaki/file_formats/__init__.py
 okonomiyaki/file_formats/_egg_info.py
@@ -104,14 +107,17 @@
 okonomiyaki/utils/test_data/cpython-2.7.9+1-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+1-rh6_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+1-rh7_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86-msvc2008.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+1-win_x86_64-msvc2008.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-2.7.9+2-rh5_x86_64-gnu.runtime.invalid
+okonomiyaki/utils/test_data/cpython-3.11.2+2-osx_x86_64-darwin.runtime
+okonomiyaki/utils/test_data/cpython-3.11.2+2-rh8_x86_64-gnu.runtime
+okonomiyaki/utils/test_data/cpython-3.11.2+2-win_x86_64-msvc2022.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-osx_x86_64-darwin.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-rh6_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-rh7_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86-msvc2008.runtime
 okonomiyaki/utils/test_data/cpython-3.4.1+1-win_x86_64-msvc2008.runtime
 okonomiyaki/utils/test_data/cpython-3.5.1+1-osx_x86_64-darwin.runtime
@@ -133,14 +139,17 @@
 okonomiyaki/utils/test_data/julia-0.3.11+1-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/julia-0.3.11+1-win_x86_64-mingw.runtime
 okonomiyaki/utils/test_data/pypy-2.6.0+1-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/r-3.0.0+1-rh5_x86_64-gnu.runtime
 okonomiyaki/utils/test_data/eggs/osx_x86_64/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/osx_x86_64/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/osx_x86_64/numpy-1.9.2-1.egg
+okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/MKL-10.3-1.egg
+okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/nose-1.3.4-1.egg
+okonomiyaki/utils/test_data/eggs/osx_x86_64/cp311/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/osx_x86_64/cp38/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/rh5_x86_64/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/rh5_x86_64/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/rh5_x86_64/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/rh6_x86_64/MKL-10.3-1.egg
@@ -148,26 +157,32 @@
 okonomiyaki/utils/test_data/eggs/rh6_x86_64/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/rh7_x86_64/cp38/numpy-1.9.2-1.egg
+okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/MKL-10.3-1.egg
+okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/nose-1.3.4-1.egg
+okonomiyaki/utils/test_data/eggs/rh8_x86_64/cp311/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/numpy-1.9.2-1.egg
+okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/MKL-10.3-1.egg
+okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/nose-1.3.4-1.egg
+okonomiyaki/utils/test_data/eggs/win_x86_64/cp311/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/MKL-10.3-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/nose-1.3.4-1.egg
 okonomiyaki/utils/test_data/eggs/win_x86_64/cp38/numpy-1.9.2-1.egg
 okonomiyaki/utils/test_data/wheels/okonomiyaki-0.17.0.dev799-py2-none-any.whl
 okonomiyaki/utils/tests/__init__.py
 okonomiyaki/utils/tests/test_eggs.py
 okonomiyaki/utils/tests/test_main.py
 okonomiyaki/utils/tests/test_misc.py
-okonomiyaki/utils/tests/test_test_data.py
+okonomiyaki/utils/tests/test_runtimes.py
 okonomiyaki/versions/__init__.py
 okonomiyaki/versions/enpkg.py
 okonomiyaki/versions/metadata_version.py
 okonomiyaki/versions/pep386.py
 okonomiyaki/versions/pep386_workaround.py
 okonomiyaki/versions/pep440.py
 okonomiyaki/versions/runtime_version.py
```

### Comparing `okonomiyaki-1.3.2/LICENSE.txt` & `okonomiyaki-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

