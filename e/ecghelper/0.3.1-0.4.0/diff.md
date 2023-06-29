# Comparing `tmp/ecghelper-0.3.1.tar.gz` & `tmp/ecghelper-0.4.0.tar.gz`

## Comparing `ecghelper-0.3.1.tar` & `ecghelper-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.csv
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.dat
--rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.edf
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.hea
--rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000.xml
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000_wfdb.dat
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ecghelper-0.3.1/82000_wfdb.hea
--rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.3.1/Untitled.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.1/debug.py
--rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.ipynb_checkpoints/debug-checkpoint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/__main__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/convert.py
--rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/io.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/utils.py
--rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 ecghelper-0.3.1/src/ecghelper/waveform.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_io.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_timing.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/test_waveform.py
--rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/82000.xml
--rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.edf
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.hea
--rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.mat
--rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/A0001.xml
--rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.3.1/tests/data/binary.csv
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.3.1/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ecghelper-0.3.1/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ecghelper-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 ecghelper-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000.csv
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000.dat
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000.edf
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000.hea
+-rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000.xml
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000_wfdb.dat
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ecghelper-0.4.0/82000_wfdb.hea
+-rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.4.0/Untitled.ipynb
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 ecghelper-0.4.0/debug.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 ecghelper-0.4.0/xml.patch
+-rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.4.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.4.0/.ipynb_checkpoints/debug-checkpoint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.4.0/src/ecghelper/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.4.0/src/ecghelper/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.4.0/src/ecghelper/convert.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.4.0/src/ecghelper/utils.py
+-rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 ecghelper-0.4.0/src/ecghelper/waveform.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/test_timing.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/test_waveform.py
+-rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/82000.xml
+-rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/A0001.edf
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/A0001.hea
+-rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/A0001.mat
+-rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/A0001.xml
+-rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.4.0/tests/data/binary.csv
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.4.0/.gitignore
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ecghelper-0.4.0/README.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ecghelper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 ecghelper-0.4.0/PKG-INFO
```

### Comparing `ecghelper-0.3.1/82000.csv` & `ecghelper-0.4.0/82000.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000.dat` & `ecghelper-0.4.0/82000.dat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000.edf` & `ecghelper-0.4.0/82000.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000.hea` & `ecghelper-0.4.0/82000.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000.xml` & `ecghelper-0.4.0/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000_wfdb.dat` & `ecghelper-0.4.0/82000_wfdb.dat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/82000_wfdb.hea` & `ecghelper-0.4.0/82000_wfdb.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/Untitled.ipynb` & `ecghelper-0.4.0/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/debug.py` & `ecghelper-0.4.0/.ipynb_checkpoints/debug-checkpoint.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `ecghelper-0.4.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/.ipynb_checkpoints/debug-checkpoint.py` & `ecghelper-0.4.0/tests/test_waveform.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,100 @@
 import os
+import pytest
 import numpy as np
 from pathlib import Path
+import csv
 
 from ecghelper.waveform import WaveformRecord
 
-def test_write():
+
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
+@pytest.mark.parametrize('filename', ['82000'])
+@pytest.mark.parametrize(
+        "ext,load_fcn",
+        [
+            (".xml", WaveformRecord.from_xml),
+            # (".hea", WaveformRecord.from_wfdb),
+            # (".edf", WaveformRecord.from_edf)
+        ])
+def test_waveform_read(data_path, filename, ext, load_fcn):
+    """Tests that we can read signals without changing the data."""
+    record = load_fcn(data_path / f"{filename}{ext}")
+    assert record.data.shape[0] > 0
+    assert record.data.shape[1] == 12
+
+    # units should be between -2 and 5 millivolts
+    assert record.data.min() > -2
+    assert record.data.max() < 5
+
+
+@pytest.mark.parametrize(
+        "format",
+        [
+            ("xml"),
+            ("wfdb"),
+            # ("edf"),
+            ("csv"),
+        ])
+def test_write(data_path, tmp_path, format):
     # inputs
-    data_path = Path('tests/data').resolve()
     filename = '82000'
 
     # read in the record
     record = WaveformRecord.from_xml(data_path / f"{filename}.xml")
 
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
-
-def main():
-    test_write()
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

### Comparing `ecghelper-0.3.1/src/ecghelper/__main__.py` & `ecghelper-0.4.0/src/ecghelper/__main__.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/src/ecghelper/convert.py` & `ecghelper-0.4.0/src/ecghelper/convert.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/src/ecghelper/utils.py` & `ecghelper-0.4.0/src/ecghelper/utils.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/src/ecghelper/waveform.py` & `ecghelper-0.4.0/src/ecghelper/waveform.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,21 @@
 from dataclasses import dataclass, field
 import json
 from pathlib import Path
 from typing import Union, List, Optional
 from inspect import getmembers
 
 import lxml.etree as ET
+from lxml.etree import _ElementTree, _Element
 import numpy as np
 import wfdb
 import pyedflib
 
 from .utils import remove_wfdb_suffix
 
-_LEADS = (
-    'I', 'II', 'III', 'aVR', 'aVL', 'aVF',
-    'V1', 'V2', 'V3', 'V4', 'V5', 'V6'
-)
-
 @dataclass
 class WaveformRecord:
     data: np.ndarray
     columns: List[str]
     sampling_frequency: float
 
     def __post_init__(self):
@@ -40,18 +36,64 @@
                 self.from_methods[method[0][5:]] = method[1]
         
         # similar approach for writing data out
         self.write_methods = {}
         for method in methods:
             if method[0].startswith('to_') and callable(method[1]):
                 self.write_methods[method[0][3:]] = method[1]
+        
+        # convert 8-lead ECGs to 12-lead
+        _LEADS = (
+            'I', 'II', 'III', 'aVR', 'aVL', 'aVF',
+            'V1', 'V2', 'V3', 'V4', 'V5', 'V6'
+        )
+        if self.data.shape[1] == 8:
+            self._convert_8_to_12_lead(_LEADS)
+        elif self.data.shape[1] != 12:
+            raise ValueError('Input data for WaveformRecord must have 8 or 12 leads')
+
+        # ensure that the columns are always in the standard 12-lead order
+        idx = [self.columns.index(lead) for lead in _LEADS]
+        self.data = self.data[:, idx]
+        self.columns = list(_LEADS)
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.data.shape})'
 
+    def _convert_8_to_12_lead(self, _LEADS):
+        """Converts 8-lead ECGs to 12-lead ECGs."""
+        # determine the leads that are missing
+        missing_leads = sorted(list(set(_LEADS) - set(self.columns)))
+
+        # create a new array with the missing leads
+        missing_data = np.zeros((self.data.shape[0], len(missing_leads)))
+        # create an index from lead name to column index
+        lead_idx = {lead: idx for idx, lead in enumerate(self.columns)}
+
+        for i, lead in enumerate(missing_leads):
+            if lead == 'III':
+                # III = II - I
+                missing_data[:, i] = self.data[:, lead_idx["II"]] - self.data[:, lead_idx["I"]]
+            elif lead == 'aVR':
+                # aVR = -(I + II)/2
+                missing_data[:, i] = -(self.data[:, lead_idx["I"]] + self.data[:, lead_idx["II"]])/2
+            elif lead == 'aVL':
+                # aVL = I - II/2
+                missing_data[:, i] = self.data[:, lead_idx["I"]] - self.data[:, lead_idx["II"]]/2
+            elif lead == 'aVF':
+                # aVF = II - I/2
+                missing_data[:, i] = self.data[:, lead_idx["II"]] - self.data[:, lead_idx["I"]]/2
+            else:
+                raise ValueError(f'Unable to impute lead data for {lead}')
+        # concatenate the missing data to the original data
+        self.data = np.concatenate((self.data, missing_data), axis=1)
+
+        # add the missing leads to the list of columns
+        self.columns += missing_leads
+
     @classmethod
     def decode_binary(cls, data: str, sample_size: int, amplitude_units_per_bit: float, baseline: int, units: str):
         lead_data = base64.b64decode(data)
 
         # iterate through to convert each byte into an integer
         lead_data = [
             int.from_bytes(
@@ -147,17 +189,16 @@
         )
 
     @classmethod
     def from_wfdbz(cls, record_filename: Union[str, Path]):
         """Load a WFDB record."""
         return cls.from_wfdb(record_filename)
 
-
     @classmethod
-    def from_xml(cls, record_filename: Union[str, Path]) -> WaveformRecord:
+    def _parse_xml_data(cls, etree: _ElementTree[_Element]) -> WaveformRecord:
         """Load waveform data from an XML record.
         
         This function assumes the following XML structure is present:
             <Waveform>
                 <WaveformType>Rhythm</WaveformType>
                 <LeadData>
                     <LeadByteCountTotal>1200</LeadByteCountTotal>
@@ -175,25 +216,23 @@
                     <BaselineSway>FALSE</BaselineSway>
                     <LeadDataCRC32>1391929279</LeadDataCRC32>
                     <WaveFormData> ... </WaveFormData>
                 </LeadData>
                 ... (repeats for each lead)
             </Waveform>
         """
-        # parse the element tree and navigate to the Waveform record
-        etree = ET.parse(record_filename, parser=None)
         root = etree.getroot()
 
         # the 12-lead ECG is assumed stored in the Rhythm waveform type
         for waveform in root.iter('Waveform'):
             waveform_type = waveform.find('WaveformType').text
             if waveform_type == 'Rhythm':
                 break
             if waveform_type is None:
-                raise ValueError(f'WaveformType = "Rhythm" not found in {record_filename}')
+                raise ValueError('WaveformType = "Rhythm" not found')
 
         # the Waveform tag has multiple LeadData tags, each of which
         # contains a base64-encoded string of the waveform data
         signal = []
         columns = []
         for lead in waveform.iter('LeadData'):
             # lead_name = lead.find('LeadID').text
@@ -225,14 +264,26 @@
         return cls(
             data=signal,
             columns=columns,
             sampling_frequency=fs,
         )
 
     @classmethod
+    def from_xml_string(cls, xml_string: str) -> WaveformRecord:
+        # parse the element tree
+        etree = ET.fromstring(xml_string, parser=None)
+        return cls._parse_xml_data(etree)
+
+    @classmethod
+    def from_xml(cls, record_filename: Union[str, Path]) -> WaveformRecord:
+        # parse the element tree
+        etree = ET.parse(record_filename, parser=None)
+        return cls._parse_xml_data(etree)
+
+    @classmethod
     def from_csv(cls, record_filename: Union[str, Path]) -> WaveformRecord:
         """Load a CSV record.
         
         CSV must have a header row. The first column must be a time
         column, in seconds, in order to calculate the sampling frequency.
         The remaining columns should be leads of the ECG.
         """
```

### Comparing `ecghelper-0.3.1/tests/test_timing.py` & `ecghelper-0.4.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/test_waveform.py` & `ecghelper-0.4.0/debug.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 import os
-import pytest
 import numpy as np
 from pathlib import Path
-import csv
 
 from ecghelper.waveform import WaveformRecord
 
+"""
+<WaveformType>Rhythm</WaveformType>
+<WaveformStartTime>0</WaveformStartTime>
+<NumberofLeads>8</NumberofLeads>
+<SampleType>CONTINUOUS_SAMPLES</SampleType>
+<SampleBase>500</SampleBase>
+<SampleExponent>0</SampleExponent>
+<HighPassFilter>5</HighPassFilter>
+<LowPassFilter>100</LowPassFilter>
+<ACFilter>60</ACFilter>
+<LeadData>
+    <LeadByteCountTotal>10000</LeadByteCountTotal>
+    <LeadTimeOffset>0</LeadTimeOffset>
+    <LeadSampleCountTotal>5000</LeadSampleCountTotal>
+    <LeadAmplitudeUnitsPerBit>4.88</LeadAmplitudeUnitsPerBit>
+    <LeadAmplitudeUnits>MICROVOLTS</LeadAmplitudeUnits>
+    <LeadHighLimit>32767</LeadHighLimit>
+    <LeadLowLimit>-32768</LeadLowLimit>
+    <LeadID>I</LeadID>
+    <LeadOffsetFirstSample>0</LeadOffsetFirstSample>
+    <FirstSampleBaseline>0</FirstSampleBaseline>
+    <LeadSampleSize>2</LeadSampleSize>
+    <LeadOff>FALSE</LeadOff>
+    <BaselineSway>FALSE</BaselineSway>
+    <LeadDataCRC32>4002389123</LeadDataCRC32>
+</LeadData>
+"""
 
-def test_waveform_binary_read(data_path):
-    """Load 82000 data converted into a CSV"""
-    with open(data_path / 'binary.csv', 'r') as fp:
-        csvreader = csv.DictReader(fp)
-        lead_data = []
-        columns = []
-        for row in csvreader:
-            lead_data.append(row['WaveFormData'])
-            columns.append(row['LeadID'])
-
-            # assume various parameters don't change from lead to lead
-            sampling_frequency = int(row['SamplingFrequency'])
-            sample_size = int(row['LeadSampleSize'])
-            amplitude_units_per_bit = float(row['LeadAmplitudeUnitsPerBit'])
-            baseline = int(row['FirstSampleBaseline'])
-            units = str(row['LeadAmplitudeUnits'])
-
-    # expect 8 leads of data
-    assert len(lead_data) == 8
-
-    binary = WaveformRecord.from_binary(
-        lead_data, columns, sampling_frequency, sample_size, amplitude_units_per_bit, baseline, units
-    )
-    assert binary.data.shape[0] > 0
-    # sampling_frequency,LeadAmplitudeUnitsPerBit,LeadAmplitudeUnits,LeadID,LeadSampleSize,LeadDataCRC32,WaveFormData
-
-
-@pytest.mark.parametrize(
-        "ext,load_fcn",
-        [
-            (".xml", WaveformRecord.from_xml),
-            # (".hea", WaveformRecord.from_wfdb),
-            # (".edf", WaveformRecord.from_edf)
-        ])
-def test_waveform_read(data_path, ext, load_fcn):
-    """Tests that we can read signals without changing the data."""
-    filename = '82000'
-    record = load_fcn(data_path / f"{filename}{ext}")
-    assert record.data.shape[0] > 0
-    assert record.data.shape[1] == 8
-
-    # units should be between -2 and 5 millivolts
-    assert record.data.min() > -2
-    assert record.data.max() < 5
-
-
-@pytest.mark.parametrize(
-        "format",
-        [
-            ("xml"),
-            ("wfdb"),
-            # ("edf"),
-            ("csv"),
-        ])
-def test_write(data_path, tmp_path, format):
+def test_write():
     # inputs
+    data_path = Path('tests/data').resolve()
     filename = '82000'
 
     # read in the record
     record = WaveformRecord.from_xml(data_path / f"{filename}.xml")
 
-    to_fcn = record.write_methods[format]
-    load_fcn = record.from_methods[format]
+    fcns = [
+        (".xml", record.to_xml, WaveformRecord.from_xml),
+        (".hea", record.to_wfdb, WaveformRecord.from_wfdb),
+        # TODO: edf is failing!
+        # (".edf", record.to_edf, WaveformRecord.from_edf),
+        (".csv",record.to_csv, WaveformRecord.from_csv),
+    ]
+    # test fcn
+    for ext, to_fcn, load_fcn in fcns:
+        # EDF precision is 8 chars
+        signal = np.around(record.data, 5)
+        output_file = Path(f'{filename}{ext}')
+        to_fcn(output_file)
+        assert os.path.exists(output_file)
+
+        # re-load, compare to original signal
+        record_reloaded = load_fcn(output_file)
+        signal_reloaded = record_reloaded.data
+        assert signal_reloaded.shape == signal.shape
+
+        # assert approximately equal
+        assert (abs(signal_reloaded - signal) < 0.01).all()
+
+        assert signal_reloaded.shape[0] > 0
+        assert signal_reloaded.shape[1] == 8
+
+        # units should be between -2 and 5 millivolts
+        assert signal_reloaded.min() > -2
+        assert signal_reloaded.max() < 5
+
+def test_read():
+    # inputs
+    data_path = Path('tests/data').resolve()
+    fcns = [
+        (".xml", WaveformRecord.from_xml),
+        (".hea", WaveformRecord.from_wfdb),
+        (".edf", WaveformRecord.from_edf),
+        # (".csv", WaveformRecord.from_csv),
+    ]
+    filename = '82000'
+
+    # test fcn
+    for ext, load_fcn in fcns:
+        record = load_fcn(data_path / f"{filename}{ext}")
+        assert record.data.shape[0] > 0
+        assert record.data.shape[1] == 8
+
+        # units should be between -2 and 5 millivolts
+        assert record.data.min() > -2
+        assert record.data.max() < 5
+
+def main():
+    test_write()
 
-    # EDF precision is 8 chars
-    signal = np.around(record.data, 5)
-    output_file = tmp_path /  f'{filename}'
-    if format != 'wfdb':
-        output_file.with_suffix(f'.{format}')
-    to_fcn(output_file)
-
-    if format == 'wfdb':
-        output_file = output_file.with_suffix('.hea')
-    assert output_file.exists()
-
-    # re-load, compare to original signal
-    record_reloaded = load_fcn(output_file)
-    signal_reloaded = record_reloaded.data
-    assert signal_reloaded.shape == signal.shape
-
-    # assert approximately equal
-    assert (abs(signal_reloaded - signal) < 0.01).all()
-
-    assert signal_reloaded.shape[0] > 0
-    assert signal_reloaded.shape[1] == 8
-
-    # units should be between -2 and 5 millivolts
-    assert signal_reloaded.min() > -2
-    assert signal_reloaded.max() < 5
+if __name__ == '__main__':
+    main()
```

### Comparing `ecghelper-0.3.1/tests/data/82000.xml` & `ecghelper-0.4.0/tests/data/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/data/A0001.edf` & `ecghelper-0.4.0/tests/data/A0001.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/data/A0001.hea` & `ecghelper-0.4.0/tests/data/A0001.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/data/A0001.mat` & `ecghelper-0.4.0/tests/data/A0001.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/data/A0001.xml` & `ecghelper-0.4.0/tests/data/A0001.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/tests/data/binary.csv` & `ecghelper-0.4.0/tests/data/binary.csv`

 * *Files identical despite different names*

### Comparing `ecghelper-0.3.1/.gitignore` & `ecghelper-0.4.0/.gitignore`

 * *Files identical despite different names*

