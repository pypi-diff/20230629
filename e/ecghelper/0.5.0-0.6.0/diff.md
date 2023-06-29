# Comparing `tmp/ecghelper-0.5.0.tar.gz` & `tmp/ecghelper-0.6.0.tar.gz`

## Comparing `ecghelper-0.5.0.tar` & `ecghelper-0.6.0.tar`

### file list

```diff
@@ -1,68 +1,61 @@
--rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.5.0/82000.xml
--rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.5.0/Untitled.ipynb
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 ecghelper-0.5.0/debug.py
--rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.5.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.5.0/.ipynb_checkpoints/debug-checkpoint.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ecghelper-0.5.0/examples/convert_cpsc_2018.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((12500, 12)).json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((5000, 12)).json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((5974, 12)).json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((7000, 12)).json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((7500, 12)).json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((7588, 12)).json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ecghelper-0.5.0/output/WaveformRecord((8000, 12)).json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.5.0/src/ecghelper/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.5.0/src/ecghelper/__main__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.5.0/src/ecghelper/convert.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.5.0/src/ecghelper/utils.py
--rw-r--r--   0        0        0    24473 2020-02-02 00:00:00.000000 ecghelper-0.5.0/src/ecghelper/waveform.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/test_timing.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/test_waveform.py
--rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/binary.csv
--rw-r--r--   0        0        0   624965 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0001.csv
--rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0001.edf
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0001.hea
--rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0001.mat
--rw-r--r--   0        0        0   249304 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0001.xml
--rw-r--r--   0        0        0   420392 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0002.csv
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0002.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0002.mat
--rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0002.xml
--rw-r--r--   0        0        0   420107 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0003.csv
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0003.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0003.mat
--rw-r--r--   0        0        0   169347 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0003.xml
--rw-r--r--   0        0        0   505976 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0004.csv
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0004.hea
--rw-r--r--   0        0        0   143400 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0004.mat
--rw-r--r--   0        0        0   200488 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0004.xml
--rw-r--r--   0        0        0  1058258 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0005.csv
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0005.hea
--rw-r--r--   0        0        0   300024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0005.mat
--rw-r--r--   0        0        0   409351 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0005.xml
--rw-r--r--   0        0        0   593141 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0006.csv
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0006.hea
--rw-r--r--   0        0        0   168024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0006.mat
--rw-r--r--   0        0        0   233317 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0006.xml
--rw-r--r--   0        0        0   415932 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0007.csv
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0007.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0007.mat
--rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0007.xml
--rw-r--r--   0        0        0   646884 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0008.csv
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0008.hea
--rw-r--r--   0        0        0   182136 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0008.mat
--rw-r--r--   0        0        0   252148 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0008.xml
--rw-r--r--   0        0        0   677928 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0009.csv
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0009.hea
--rw-r--r--   0        0        0   192024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0009.mat
--rw-r--r--   0        0        0   265336 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0009.xml
--rw-r--r--   0        0        0   413829 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0010.csv
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0010.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0010.mat
--rw-r--r--   0        0        0   169334 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/A0010.xml
--rw-r--r--   0        0        0  1368843 2020-02-02 00:00:00.000000 ecghelper-0.5.0/tests/data/cpsc_2018/challenge_data_as_xml.zip
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.5.0/.gitignore
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ecghelper-0.5.0/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ecghelper-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 ecghelper-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.6.0/82000.xml
+-rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.6.0/Untitled.ipynb
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 ecghelper-0.6.0/debug.py
+-rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.ipynb_checkpoints/debug-checkpoint.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ecghelper-0.6.0/examples/convert_cpsc_2018.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/convert.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/utils.py
+-rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/waveform.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/test_timing.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/test_waveform.py
+-rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/binary.csv
+-rw-r--r--   0        0        0   624965 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.csv
+-rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.edf
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.hea
+-rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.mat
+-rw-r--r--   0        0        0   249304 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.xml
+-rw-r--r--   0        0        0   420392 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.csv
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.mat
+-rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.xml
+-rw-r--r--   0        0        0   420107 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.csv
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.mat
+-rw-r--r--   0        0        0   169347 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.xml
+-rw-r--r--   0        0        0   505976 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.csv
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.hea
+-rw-r--r--   0        0        0   143400 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.mat
+-rw-r--r--   0        0        0   200488 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.xml
+-rw-r--r--   0        0        0  1058258 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.csv
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.hea
+-rw-r--r--   0        0        0   300024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.mat
+-rw-r--r--   0        0        0   409351 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.xml
+-rw-r--r--   0        0        0   593141 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.csv
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.hea
+-rw-r--r--   0        0        0   168024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.mat
+-rw-r--r--   0        0        0   233317 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.xml
+-rw-r--r--   0        0        0   415932 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.csv
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.mat
+-rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.xml
+-rw-r--r--   0        0        0   646884 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.csv
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.hea
+-rw-r--r--   0        0        0   182136 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.mat
+-rw-r--r--   0        0        0   252148 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.xml
+-rw-r--r--   0        0        0   677928 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.csv
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.hea
+-rw-r--r--   0        0        0   192024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.mat
+-rw-r--r--   0        0        0   265336 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.xml
+-rw-r--r--   0        0        0   413829 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.csv
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.mat
+-rw-r--r--   0        0        0   169334 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.xml
+-rw-r--r--   0        0        0  1368843 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/challenge_data_as_xml.zip
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.gitignore
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ecghelper-0.6.0/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ecghelper-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ecghelper-0.6.0/PKG-INFO
```

### Comparing `ecghelper-0.5.0/82000.xml` & `ecghelper-0.6.0/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/Untitled.ipynb` & `ecghelper-0.6.0/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/debug.py` & `ecghelper-0.6.0/debug.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `ecghelper-0.6.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/.ipynb_checkpoints/debug-checkpoint.py` & `ecghelper-0.6.0/.ipynb_checkpoints/debug-checkpoint.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/examples/convert_cpsc_2018.py` & `ecghelper-0.6.0/examples/convert_cpsc_2018.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/src/ecghelper/__main__.py` & `ecghelper-0.6.0/src/ecghelper/__main__.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/src/ecghelper/convert.py` & `ecghelper-0.6.0/src/ecghelper/convert.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/src/ecghelper/utils.py` & `ecghelper-0.6.0/src/ecghelper/utils.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/src/ecghelper/waveform.py` & `ecghelper-0.6.0/src/ecghelper/waveform.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     @classmethod
     def from_wfdbz(cls, record_filename: Union[str, Path]):
         """Load a WFDB record."""
         return cls.from_wfdb(record_filename)
 
     @classmethod
-    def _parse_xml_data(cls, etree: _ElementTree[_Element]) -> WaveformRecord:
+    def _parse_xml_data(cls, root: _Element) -> WaveformRecord:
         """Load waveform data from an XML record.
         
         This function assumes the following XML structure is present:
             <Waveform>
                 <WaveformType>Rhythm</WaveformType>
                 <LeadData>
                     <LeadByteCountTotal>1200</LeadByteCountTotal>
@@ -217,28 +217,30 @@
                     <BaselineSway>FALSE</BaselineSway>
                     <LeadDataCRC32>1391929279</LeadDataCRC32>
                     <WaveFormData> ... </WaveFormData>
                 </LeadData>
                 ... (repeats for each lead)
             </Waveform>
         """
-        root = etree.getroot()
-
         # the 12-lead ECG is assumed stored in the Rhythm waveform type
+        waveform = None
         for waveform in root.iter('Waveform'):
             waveform_type = waveform.find('WaveformType').text
             if waveform_type == 'Rhythm':
                 break
             if waveform_type is None:
                 raise ValueError('WaveformType = "Rhythm" not found')
 
         # the Waveform tag has multiple LeadData tags, each of which
         # contains a base64-encoded string of the waveform data
         signal = []
         columns = []
+        if waveform is None:
+            raise ValueError('Waveform tag not found')
+
         for lead in waveform.iter('LeadData'):
             # lead_name = lead.find('LeadID').text
             sample_size = int(lead.find('LeadSampleSize').text)
             if sample_size > 8:
                 raise ValueError(f'byte size expected to be no higher than 8')
 
             # extract the string with the waveform data and decode into bytes
@@ -274,22 +276,23 @@
             columns=columns,
             sampling_frequency=fs,
         )
 
     @classmethod
     def from_xml_string(cls, xml_string: str) -> WaveformRecord:
         # parse the element tree
-        etree = ET.fromstring(xml_string, parser=None)
-        return cls._parse_xml_data(etree)
+        root = ET.fromstring(xml_string, parser=None)
+        return cls._parse_xml_data(root)
 
     @classmethod
     def from_xml(cls, record_filename: Union[str, Path]) -> WaveformRecord:
         # parse the element tree
         etree = ET.parse(record_filename, parser=None)
-        return cls._parse_xml_data(etree)
+        root = etree.getroot()
+        return cls._parse_xml_data(root)
 
     @classmethod
     def from_csv(cls, record_filename: Union[str, Path]) -> WaveformRecord:
         """Load a CSV record.
         
         CSV must have a header row. The first column must be a time
         column, in seconds, in order to calculate the sampling frequency.
@@ -567,39 +570,64 @@
             data['dx'] = [int(x) for x in data['dx'].split(',')]
 
         data['arrhythmia'] = data.pop('dx')
 
         return cls(**data)
 
     @classmethod
-    def from_xml(cls, record_filename: Union[str, Path]):
-        """Load metadata from a GE MUSE XML record."""
-        etree = ET.parse(record_filename, parser=None)
-        # root is RestingECG tag
-        root = etree.getroot()
-        demographics = root.find('PatientDemographics')
+    def _parse_xml_data(cls, root: _Element) -> WaveformMetadata:
+        """Load waveform metadata from an XML record. The XML record is
+        assumed to be in a GE MUSE XML format."""
         data = {}
-        data['age'] = demographics.find('PatientAge').text
-        data['sex'] = demographics.find('Gender').text
-        data['race'] = demographics.find('Race').text
+        
+        demographics = root.find('PatientDemographics')
+        if demographics is not None:
+            data['age'] = demographics.find('PatientAge')
+            data['sex'] = demographics.find('Gender')
+            data['race'] = demographics.find('Race')
+
+        for key in ['age', 'sex', 'race']:
+            if data[key] is not None:
+                data[key] = data[key].text
 
         # TODO: some thought here once the data actually comes in
         dx = root.find('Diagnosis')
         # iterate through the DiagnosisStatement elements under diagnosis
         # and get the StmtText attribute under it
-        dx = [x.find('StmtText').text for x in dx.iter('DiagnosisStatement')]
-
+        if dx is None:
+            data['arrythmia'] = None
+            return cls(**data)
+
+        dx_output = []
+        for stmt in dx.iter('DiagnosisStatement'):
+            stmt_text = stmt.find('StmtText')
+            if stmt_text is not None:
+                dx_output.append(stmt_text.text)
+        dx_output = ', '.join(dx_output)
         # TODO: above dx is free text
         # need to convert to a list of codes
         # for now, just return the free text
-        data['arrythmia'] = dx
+        data['arrythmia'] = dx_output
 
         return cls(**data)
 
     @classmethod
+    def from_xml_string(cls, xml_string: str) -> WaveformMetadata:
+        # parse the element tree
+        root = ET.fromstring(xml_string, parser=None)
+        return cls._parse_xml_data(root)
+
+    @classmethod
+    def from_xml(cls, record_filename: Union[str, Path]) -> WaveformMetadata:
+        # parse the element tree
+        etree = ET.parse(record_filename, parser=None)
+        root = etree.getroot()
+        return cls._parse_xml_data(root)
+
+    @classmethod
     def from_csv(cls, record_name: Union[str, Path]):
         """Load metadata for a CSV record. Not implemented."""
         raise NotImplementedError('Cannot load metadata from CSV.')
 
     @classmethod
     def from_json(cls, record_name: Union[str, Path]):
         """Load metadata for a JSON record."""
```

### Comparing `ecghelper-0.5.0/tests/conftest.py` & `ecghelper-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/test_timing.py` & `ecghelper-0.6.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/test_waveform.py` & `ecghelper-0.6.0/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/binary.csv` & `ecghelper-0.6.0/tests/data/binary.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0001.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0001.edf` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0001.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0001.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0001.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0002.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0002.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0002.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0002.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0003.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0003.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0003.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0003.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0004.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0004.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0004.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0004.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0005.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0005.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0005.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0005.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0006.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0006.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0006.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0006.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0007.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0007.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0007.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0007.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0008.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0008.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0008.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0008.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0009.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0009.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0009.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0009.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0010.csv` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0010.hea` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0010.mat` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/A0010.xml` & `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/tests/data/cpsc_2018/challenge_data_as_xml.zip` & `ecghelper-0.6.0/tests/data/cpsc_2018/challenge_data_as_xml.zip`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/.gitignore` & `ecghelper-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/README.md` & `ecghelper-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecghelper-0.5.0/pyproject.toml` & `ecghelper-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecghelper"
-version = "0.5.0"
+version = "0.6.0"
 description = "Tools to load and process electrocardiogram data."
 author = "Alistair Johnson"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
@@ -24,11 +24,11 @@
     "wfdb>=4.1.2",
     "pyEDFlib>=0.1.32",
     "lxml>=4.9.2",
     "types-lxml>=2023.3.28"
 ]
 
 [project.optional-dependencies]
-dev = ["pytest"]
+dev = ["pytest", "build", "twine"]
 
 [tool.hatchling]
 src = "src/ecghelper"
```

### Comparing `ecghelper-0.5.0/PKG-INFO` & `ecghelper-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecghelper
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools to load and process electrocardiogram data.
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: cython>=0.29.34
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: lxml>=4.9.2
@@ -13,15 +13,17 @@
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: types-lxml>=2023.3.28
 Requires-Dist: wfdb>=4.1.2
 Requires-Dist: xgboost>=1.7.4
 Provides-Extra: dev
+Requires-Dist: build; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ecghelper
 
 A utility package for working with electrocardiograms, particularly 12-lead electrocardiograms.
 
 ## Quickstart
```

