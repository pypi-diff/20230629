# Comparing `tmp/ecghelper-0.6.0.tar.gz` & `tmp/ecghelper-0.6.1.tar.gz`

## Comparing `ecghelper-0.6.0.tar` & `ecghelper-0.6.1.tar`

### file list

```diff
@@ -1,61 +1,56 @@
--rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.6.0/82000.xml
--rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.6.0/Untitled.ipynb
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 ecghelper-0.6.0/debug.py
--rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.ipynb_checkpoints/debug-checkpoint.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ecghelper-0.6.0/examples/convert_cpsc_2018.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/__main__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/convert.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/utils.py
--rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 ecghelper-0.6.0/src/ecghelper/waveform.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/test_timing.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/test_waveform.py
--rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/binary.csv
--rw-r--r--   0        0        0   624965 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.csv
--rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.edf
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.hea
--rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.mat
--rw-r--r--   0        0        0   249304 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0001.xml
--rw-r--r--   0        0        0   420392 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.csv
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.mat
--rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0002.xml
--rw-r--r--   0        0        0   420107 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.csv
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.mat
--rw-r--r--   0        0        0   169347 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0003.xml
--rw-r--r--   0        0        0   505976 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.csv
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.hea
--rw-r--r--   0        0        0   143400 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.mat
--rw-r--r--   0        0        0   200488 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0004.xml
--rw-r--r--   0        0        0  1058258 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.csv
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.hea
--rw-r--r--   0        0        0   300024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.mat
--rw-r--r--   0        0        0   409351 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0005.xml
--rw-r--r--   0        0        0   593141 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.csv
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.hea
--rw-r--r--   0        0        0   168024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.mat
--rw-r--r--   0        0        0   233317 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0006.xml
--rw-r--r--   0        0        0   415932 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.csv
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.mat
--rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0007.xml
--rw-r--r--   0        0        0   646884 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.csv
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.hea
--rw-r--r--   0        0        0   182136 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.mat
--rw-r--r--   0        0        0   252148 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0008.xml
--rw-r--r--   0        0        0   677928 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.csv
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.hea
--rw-r--r--   0        0        0   192024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.mat
--rw-r--r--   0        0        0   265336 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0009.xml
--rw-r--r--   0        0        0   413829 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.csv
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.hea
--rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.mat
--rw-r--r--   0        0        0   169334 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/A0010.xml
--rw-r--r--   0        0        0  1368843 2020-02-02 00:00:00.000000 ecghelper-0.6.0/tests/data/cpsc_2018/challenge_data_as_xml.zip
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.6.0/.gitignore
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ecghelper-0.6.0/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ecghelper-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ecghelper-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ecghelper-0.6.1/examples/convert_cpsc_2018.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.6.1/src/ecghelper/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.6.1/src/ecghelper/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.6.1/src/ecghelper/convert.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.6.1/src/ecghelper/utils.py
+-rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 ecghelper-0.6.1/src/ecghelper/waveform.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/test_timing.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/test_waveform.py
+-rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/binary.csv
+-rw-r--r--   0        0        0   624965 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0001.csv
+-rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0001.edf
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0001.hea
+-rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0001.mat
+-rw-r--r--   0        0        0   249304 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0001.xml
+-rw-r--r--   0        0        0   420392 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0002.csv
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0002.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0002.mat
+-rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0002.xml
+-rw-r--r--   0        0        0   420107 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0003.csv
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0003.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0003.mat
+-rw-r--r--   0        0        0   169347 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0003.xml
+-rw-r--r--   0        0        0   505976 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0004.csv
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0004.hea
+-rw-r--r--   0        0        0   143400 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0004.mat
+-rw-r--r--   0        0        0   200488 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0004.xml
+-rw-r--r--   0        0        0  1058258 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0005.csv
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0005.hea
+-rw-r--r--   0        0        0   300024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0005.mat
+-rw-r--r--   0        0        0   409351 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0005.xml
+-rw-r--r--   0        0        0   593141 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0006.csv
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0006.hea
+-rw-r--r--   0        0        0   168024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0006.mat
+-rw-r--r--   0        0        0   233317 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0006.xml
+-rw-r--r--   0        0        0   415932 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0007.csv
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0007.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0007.mat
+-rw-r--r--   0        0        0   169335 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0007.xml
+-rw-r--r--   0        0        0   646884 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0008.csv
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0008.hea
+-rw-r--r--   0        0        0   182136 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0008.mat
+-rw-r--r--   0        0        0   252148 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0008.xml
+-rw-r--r--   0        0        0   677928 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0009.csv
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0009.hea
+-rw-r--r--   0        0        0   192024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0009.mat
+-rw-r--r--   0        0        0   265336 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0009.xml
+-rw-r--r--   0        0        0   413829 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0010.csv
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0010.hea
+-rw-r--r--   0        0        0   120024 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0010.mat
+-rw-r--r--   0        0        0   169334 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/A0010.xml
+-rw-r--r--   0        0        0  1368843 2020-02-02 00:00:00.000000 ecghelper-0.6.1/tests/data/cpsc_2018/challenge_data_as_xml.zip
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.6.1/.gitignore
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ecghelper-0.6.1/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ecghelper-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ecghelper-0.6.1/PKG-INFO
```

### Comparing `ecghelper-0.6.0/debug.py` & `ecghelper-0.6.1/tests/test_waveform.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,106 @@
 import os
+import pytest
 import numpy as np
 from pathlib import Path
+import csv
 
 from ecghelper.waveform import WaveformRecord
 
-"""
-<WaveformType>Rhythm</WaveformType>
-<WaveformStartTime>0</WaveformStartTime>
-<NumberofLeads>8</NumberofLeads>
-<SampleType>CONTINUOUS_SAMPLES</SampleType>
-<SampleBase>500</SampleBase>
-<SampleExponent>0</SampleExponent>
-<HighPassFilter>5</HighPassFilter>
-<LowPassFilter>100</LowPassFilter>
-<ACFilter>60</ACFilter>
-<LeadData>
-    <LeadByteCountTotal>10000</LeadByteCountTotal>
-    <LeadTimeOffset>0</LeadTimeOffset>
-    <LeadSampleCountTotal>5000</LeadSampleCountTotal>
-    <LeadAmplitudeUnitsPerBit>4.88</LeadAmplitudeUnitsPerBit>
-    <LeadAmplitudeUnits>MICROVOLTS</LeadAmplitudeUnits>
-    <LeadHighLimit>32767</LeadHighLimit>
-    <LeadLowLimit>-32768</LeadLowLimit>
-    <LeadID>I</LeadID>
-    <LeadOffsetFirstSample>0</LeadOffsetFirstSample>
-    <FirstSampleBaseline>0</FirstSampleBaseline>
-    <LeadSampleSize>2</LeadSampleSize>
-    <LeadOff>FALSE</LeadOff>
-    <BaselineSway>FALSE</BaselineSway>
-    <LeadDataCRC32>4002389123</LeadDataCRC32>
-</LeadData>
-"""
-
-def test_write():
-    # inputs
-    data_path = Path('tests/data').resolve()
-    filename = '82000'
 
-    # read in the record
-    record = WaveformRecord.from_xml(data_path / f"{filename}.xml")
+def test_waveform_binary_read(data_path):
+    """Load 82000 data converted into a CSV"""
+    with open(data_path / 'binary.csv', 'r') as fp:
+        csvreader = csv.DictReader(fp)
+        lead_data = []
+        columns = []
+        for row in csvreader:
+            lead_data.append(row['WaveFormData'])
+            columns.append(row['LeadID'])
+
+            # assume various parameters don't change from lead to lead
+            sampling_frequency = int(row['SamplingFrequency'])
+            sample_size = int(row['LeadSampleSize'])
+            amplitude_units_per_bit = float(row['LeadAmplitudeUnitsPerBit'])
+            baseline = int(row['FirstSampleBaseline'])
+            units = str(row['LeadAmplitudeUnits'])
+
+    # expect 8 leads of data in the source binary data
+    assert len(lead_data) == 8
+
+    binary = WaveformRecord.from_binary(
+        lead_data, columns, sampling_frequency,
+        sample_size, amplitude_units_per_bit, baseline, units
+    )
+    assert binary.data.shape[0] > 0
+
+    # expect 12 leads of data after being loaded into a WaveformRecord
+    assert binary.data.shape[1] == 12
+
+@pytest.mark.parametrize(
+        "ext,load_fcn",
+        [
+            (".xml", WaveformRecord.from_xml),
+            (".hea", WaveformRecord.from_wfdb),
+            (".edf", WaveformRecord.from_edf)
+        ])
+def test_waveform_read(cpsc_2018_path, ext, load_fcn):
+    """Tests that we can read signals without changing the data."""
+    files = cpsc_2018_path.glob(f'*{ext}')
+    filenames = [x.stem for x in files]
+    for filename in filenames:
+        if ext == '.hea':
+            record = load_fcn(cpsc_2018_path / f"{filename}")
+        else:
+            record = load_fcn(cpsc_2018_path / f"{filename}{ext}")
 
-    fcns = [
-        (".xml", record.to_xml, WaveformRecord.from_xml),
-        (".hea", record.to_wfdb, WaveformRecord.from_wfdb),
-        # TODO: edf is failing!
-        # (".edf", record.to_edf, WaveformRecord.from_edf),
-        (".csv",record.to_csv, WaveformRecord.from_csv),
-    ]
-    # test fcn
-    for ext, to_fcn, load_fcn in fcns:
-        # EDF precision is 8 chars
-        signal = np.around(record.data, 5)
-        output_file = Path(f'{filename}{ext}')
-        to_fcn(output_file)
-        assert os.path.exists(output_file)
-
-        # re-load, compare to original signal
-        record_reloaded = load_fcn(output_file)
-        signal_reloaded = record_reloaded.data
-        assert signal_reloaded.shape == signal.shape
-
-        # assert approximately equal
-        assert (abs(signal_reloaded - signal) < 0.01).all()
-
-        assert signal_reloaded.shape[0] > 0
-        assert signal_reloaded.shape[1] == 8
-
-        # units should be between -2 and 5 millivolts
-        assert signal_reloaded.min() > -2
-        assert signal_reloaded.max() < 5
-
-def test_read():
-    # inputs
-    data_path = Path('tests/data').resolve()
-    fcns = [
-        (".xml", WaveformRecord.from_xml),
-        # (".hea", WaveformRecord.from_wfdb),
-        # (".edf", WaveformRecord.from_edf),
-        # (".csv", WaveformRecord.from_csv),
-    ]
-    filename = '82000'
-
-    # test fcn
-    for ext, load_fcn in fcns:
-        record = load_fcn(data_path / f"{filename}{ext}")
         assert record.data.shape[0] > 0
         assert record.data.shape[1] == 12
 
-        # units should be between -2 and 5 millivolts
-        assert record.data.min() > -2
+        # units should be between -2.5 and 5 millivolts
+        assert record.data.min() > -2.5
         assert record.data.max() < 5
-    
-    xml_output = record._serialize_to_xml()
 
-def main():
-    test_read()
+@pytest.mark.parametrize(
+        "format,ext",
+        [
+            ("xml"),
+            ("wfdb"),
+            # ("edf"),
+            ("csv"),
+        ])
+def test_write(cpsc_2018_path, tmp_path, format):
+    # load in a waveform record from the CPSC-2018 dataset
+    files = cpsc_2018_path.glob('*.hea')
+    filename = [x.stem for x in files][0]
+
+    # read in the record
+    record = WaveformRecord.from_wfdb(cpsc_2018_path / f"{filename}")
+
+    to_fcn = record.write_methods[format]
+    load_fcn = record.from_methods[format]
 
-if __name__ == '__main__':
-    main()
+    # EDF precision is 8 chars
+    signal = np.around(record.data, 5)
+    output_file = tmp_path /  f'{filename}'
+    if format != 'wfdb':
+        output_file.with_suffix(f'.{format}')
+    to_fcn(output_file)
+
+    if format == 'wfdb':
+        output_file = output_file.with_suffix('.hea')
+    assert output_file.exists()
+
+    # re-load, compare to original signal
+    record_reloaded = load_fcn(output_file)
+    signal_reloaded = record_reloaded.data
+    assert signal_reloaded.shape == signal.shape
+
+    # assert approximately equal
+    assert (abs(signal_reloaded - signal) < 0.01).all()
+
+    assert signal_reloaded.shape[0] > 0
+    assert signal_reloaded.shape[1] == 12
+
+    # units should be between -2 and 5 millivolts
+    assert signal_reloaded.min() > -2
+    assert signal_reloaded.max() < 5
```

### Comparing `ecghelper-0.6.0/.ipynb_checkpoints/debug-checkpoint.py` & `ecghelper-0.6.1/examples/convert_cpsc_2018.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,51 @@
+"""
+Example script converting the first 10 records of CPSC-2018 data
+into various formats.
+"""
 import os
 import numpy as np
 from pathlib import Path
 
 from ecghelper.waveform import WaveformRecord
 
-def test_write():
+def main():
     # inputs
-    data_path = Path('tests/data').resolve()
-    filename = '82000'
-
-    # read in the record
-    record = WaveformRecord.from_xml(data_path / f"{filename}.xml")
+    data_path = Path('tests/data/cpsc_2018').resolve()
+    files = data_path.glob('*.hea')
+    filenames = [x.stem for x in files][:10]
+
+    for filename in filenames:
+        # read in the WFDB format record
+        record = WaveformRecord.from_wfdb(data_path / f"{filename}")
+
+        fcns = [
+            (".xml", record.to_xml, WaveformRecord.from_xml),
+            # TODO: edf is failing!
+            # (".edf", record.to_edf, WaveformRecord.from_edf),
+            (".csv", record.to_csv, WaveformRecord.from_csv),
+        ]
+        for ext, to_fcn, load_fcn in fcns:
+            # precision for these records is 5 digits
+            # rounding is useful for output to EDF, CSV, etc.
+            signal = np.around(record.data, 5)
+
+            output_file = Path(data_path / f'{filename}{ext}')
+            to_fcn(output_file)
+            assert os.path.exists(output_file)
+
+            # re-load, compare to original signal
+            record_reloaded = load_fcn(output_file)
+            signal_reloaded = record_reloaded.data
+            assert signal_reloaded.shape == signal.shape
 
-    fcns = [
-        (".xml", record.to_xml, WaveformRecord.from_xml),
-        (".hea", record.to_wfdb, WaveformRecord.from_wfdb),
-        # TODO: edf is failing!
-        # (".edf", record.to_edf, WaveformRecord.from_edf),
-        (".csv",record.to_csv, WaveformRecord.from_csv),
-    ]
-    # test fcn
-    for ext, to_fcn, load_fcn in fcns:
-        # EDF precision is 8 chars
-        signal = np.around(record.data, 5)
-        output_file = Path(f'{filename}{ext}')
-        to_fcn(output_file)
-        assert os.path.exists(output_file)
-
-        # re-load, compare to original signal
-        record_reloaded = load_fcn(output_file)
-        signal_reloaded = record_reloaded.data
-        assert signal_reloaded.shape == signal.shape
-
-        # assert approximately equal
-        assert (abs(signal_reloaded - signal) < 0.01).all()
-
-        assert signal_reloaded.shape[0] > 0
-        assert signal_reloaded.shape[1] == 8
-
-        # units should be between -2 and 5 millivolts
-        assert signal_reloaded.min() > -2
-        assert signal_reloaded.max() < 5
+            # assert approximately equal
+            assert (abs(signal_reloaded - signal) < 0.01).all()
 
-def test_read():
-    # inputs
-    data_path = Path('tests/data').resolve()
-    fcns = [
-        (".xml", WaveformRecord.from_xml),
-        (".hea", WaveformRecord.from_wfdb),
-        (".edf", WaveformRecord.from_edf),
-        # (".csv", WaveformRecord.from_csv),
-    ]
-    filename = '82000'
-
-    # test fcn
-    for ext, load_fcn in fcns:
-        record = load_fcn(data_path / f"{filename}{ext}")
-        assert record.data.shape[0] > 0
-        assert record.data.shape[1] == 8
-
-        # units should be between -2 and 5 millivolts
-        assert record.data.min() > -2
-        assert record.data.max() < 5
+            assert signal_reloaded.shape[0] > 0
+            assert signal_reloaded.shape[1] == 12
 
-def main():
-    test_write()
+            # reloaded signal should be very close
+            np.allclose(signal_reloaded, signal, atol=0.0001)
 
 if __name__ == '__main__':
     main()
```

### Comparing `ecghelper-0.6.0/src/ecghelper/__main__.py` & `ecghelper-0.6.1/src/ecghelper/__main__.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/src/ecghelper/convert.py` & `ecghelper-0.6.1/src/ecghelper/convert.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/src/ecghelper/utils.py` & `ecghelper-0.6.1/src/ecghelper/utils.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/src/ecghelper/waveform.py` & `ecghelper-0.6.1/src/ecghelper/waveform.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,27 +590,27 @@
                 data[key] = data[key].text
 
         # TODO: some thought here once the data actually comes in
         dx = root.find('Diagnosis')
         # iterate through the DiagnosisStatement elements under diagnosis
         # and get the StmtText attribute under it
         if dx is None:
-            data['arrythmia'] = None
+            data['arrhythmia'] = None
             return cls(**data)
 
         dx_output = []
         for stmt in dx.iter('DiagnosisStatement'):
             stmt_text = stmt.find('StmtText')
             if stmt_text is not None:
                 dx_output.append(stmt_text.text)
         dx_output = ', '.join(dx_output)
         # TODO: above dx is free text
         # need to convert to a list of codes
         # for now, just return the free text
-        data['arrythmia'] = dx_output
+        data['arrhythmia'] = dx_output
 
         return cls(**data)
 
     @classmethod
     def from_xml_string(cls, xml_string: str) -> WaveformMetadata:
         # parse the element tree
         root = ET.fromstring(xml_string, parser=None)
```

### Comparing `ecghelper-0.6.0/tests/conftest.py` & `ecghelper-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/test_timing.py` & `ecghelper-0.6.1/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/binary.csv` & `ecghelper-0.6.1/tests/data/binary.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0001.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.edf` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0001.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0001.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0001.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0001.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0001.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0002.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0002.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0002.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0002.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0002.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0003.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0003.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0003.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0003.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0003.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0004.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0004.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0004.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0004.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0004.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0005.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0005.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0005.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0005.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0005.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0006.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0006.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0006.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0006.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0006.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0007.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0007.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0007.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0007.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0007.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0008.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0008.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0008.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0008.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0008.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0009.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0009.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0009.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0009.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0009.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.csv` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0010.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.hea` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0010.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.mat` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0010.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/A0010.xml` & `ecghelper-0.6.1/tests/data/cpsc_2018/A0010.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/tests/data/cpsc_2018/challenge_data_as_xml.zip` & `ecghelper-0.6.1/tests/data/cpsc_2018/challenge_data_as_xml.zip`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/.gitignore` & `ecghelper-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/README.md` & `ecghelper-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ecghelper-0.6.0/pyproject.toml` & `ecghelper-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecghelper"
-version = "0.6.0"
+version = "0.6.1"
 description = "Tools to load and process electrocardiogram data."
 author = "Alistair Johnson"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `ecghelper-0.6.0/PKG-INFO` & `ecghelper-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecghelper
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tools to load and process electrocardiogram data.
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: cython>=0.29.34
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: lxml>=4.9.2
```

