# Comparing `tmp/receptor_utils-0.0.4.tar.gz` & `tmp/receptor_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_utils-0.0.4.tar", last modified: Thu Dec 30 16:28:23 2021, max compression
+gzip compressed data, was "receptor_utils-0.0.5.tar", last modified: Thu Jan 20 10:22:49 2022, max compression
```

## Comparing `receptor_utils-0.0.4.tar` & `receptor_utils-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-12-30 16:28:23.293831 receptor_utils-0.0.4/
--rw-rw-rw-   0        0        0      240 2021-12-29 13:38:03.000000 receptor_utils-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3218 2021-12-30 16:28:23.293831 receptor_utils-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2021-12-30 11:12:28.000000 receptor_utils-0.0.4/README.md
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_utils-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      943 2021-12-30 16:28:23.296833 receptor_utils-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-12-30 16:28:23.253831 receptor_utils-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2021-12-30 16:28:23.279832 receptor_utils-0.0.4/src/receptor_utils/
--rw-rw-rw-   0        0        0        0 2021-12-30 16:26:06.000000 receptor_utils-0.0.4/src/receptor_utils/__init__.py
--rw-rw-rw-   0        0        0     1174 2021-12-30 16:05:03.000000 receptor_utils-0.0.4/src/receptor_utils/extract_refs.py
--rw-rw-rw-   0        0        0     1124 2021-12-30 15:57:33.000000 receptor_utils-0.0.4/src/receptor_utils/gap_inferred.py
--rw-rw-rw-   0        0        0      947 2021-12-30 16:05:03.000000 receptor_utils-0.0.4/src/receptor_utils/identical_seqs.py
--rw-rw-rw-   0        0        0     5679 2021-12-29 15:43:06.000000 receptor_utils-0.0.4/src/receptor_utils/novel_allele_name.py
--rw-rw-rw-   0        0        0    12194 2021-12-29 15:41:46.000000 receptor_utils-0.0.4/src/receptor_utils/number_ighv.py
--rw-rw-rw-   0        0        0     3878 2021-12-12 16:10:58.000000 receptor_utils-0.0.4/src/receptor_utils/simple_bio_seq.py
-drwxrwxrwx   0        0        0        0 2021-12-30 16:28:23.292831 receptor_utils-0.0.4/src/receptor_utils.egg-info/
--rw-rw-rw-   0        0        0     3218 2021-12-30 16:28:23.000000 receptor_utils-0.0.4/src/receptor_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2021-12-30 16:28:23.000000 receptor_utils-0.0.4/src/receptor_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-30 16:28:23.000000 receptor_utils-0.0.4/src/receptor_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2021-12-30 16:28:23.000000 receptor_utils-0.0.4/src/receptor_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2021-12-30 16:28:23.000000 receptor_utils-0.0.4/src/receptor_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.330403 receptor_utils-0.0.5/
+-rw-rw-rw-   0        0        0      240 2021-12-29 13:38:03.000000 receptor_utils-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3218 2022-01-20 10:22:49.330403 receptor_utils-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2022-01-20 10:18:59.000000 receptor_utils-0.0.5/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_utils-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      943 2022-01-20 10:22:49.332403 receptor_utils-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.176113 receptor_utils-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.314403 receptor_utils-0.0.5/src/receptor_utils/
+-rw-rw-rw-   0        0        0        0 2021-12-30 16:26:06.000000 receptor_utils-0.0.5/src/receptor_utils/__init__.py
+-rw-rw-rw-   0        0        0     1218 2022-01-19 12:24:36.000000 receptor_utils-0.0.5/src/receptor_utils/extract_refs.py
+-rw-rw-rw-   0        0        0     1749 2022-01-20 09:38:18.000000 receptor_utils-0.0.5/src/receptor_utils/gap_inferred.py
+-rw-rw-rw-   0        0        0      993 2022-01-19 12:07:22.000000 receptor_utils-0.0.5/src/receptor_utils/identical_seqs.py
+-rw-rw-rw-   0        0        0     6174 2022-01-11 09:48:59.000000 receptor_utils-0.0.5/src/receptor_utils/novel_allele_name.py
+-rw-rw-rw-   0        0        0    12364 2022-01-20 09:23:34.000000 receptor_utils-0.0.5/src/receptor_utils/number_ighv.py
+-rw-rw-rw-   0        0        0     3878 2021-12-12 16:10:58.000000 receptor_utils-0.0.5/src/receptor_utils/simple_bio_seq.py
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.329403 receptor_utils-0.0.5/src/receptor_utils.egg-info/
+-rw-rw-rw-   0        0        0     3218 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/top_level.txt
```

### Comparing `receptor_utils-0.0.4/PKG-INFO` & `receptor_utils-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor_utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some tools I find useful for working with Ig receptor sequences
 Home-page: https://github.com/williamdlees/receptor_utils
 Author: William Lees
 Author-email: william@lees.org.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/williamdlees/receptor_utils/issues
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 # receptor_utils
 
 Some tools I find useful for working with Ig receptor sequences.
 
 # Installation
 
 ```bash
-pip install receptor_utils
+pip install receptor-utils
 ```
 
 The module requires [Biopython](https://biopython.org).
 
 # Overview
 
 Please refer to the files themselves for slightly more detailed documentation.
```

### Comparing `receptor_utils-0.0.4/README.md` & `receptor_utils-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # receptor_utils
 
 Some tools I find useful for working with Ig receptor sequences.
 
 # Installation
 
 ```bash
-pip install receptor_utils
+pip install receptor-utils
 ```
 
 The module requires [Biopython](https://biopython.org).
 
 # Overview
 
 Please refer to the files themselves for slightly more detailed documentation.
```

### Comparing `receptor_utils-0.0.4/setup.cfg` & `receptor_utils-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 7574 696c   = receptor_util
 00000020: 730d 0a76 6572 7369 6f6e 203d 2030 2e30  s..version = 0.0
-00000030: 2e34 0d0a 6175 7468 6f72 203d 2057 696c  .4..author = Wil
+00000030: 2e35 0d0a 6175 7468 6f72 203d 2057 696c  .5..author = Wil
 00000040: 6c69 616d 204c 6565 730d 0a61 7574 686f  liam Lees..autho
 00000050: 725f 656d 6169 6c20 3d20 7769 6c6c 6961  r_email = willia
 00000060: 6d40 6c65 6573 2e6f 7267 2e75 6b0d 0a64  m@lees.org.uk..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2053 6f6d  escription = Som
 00000080: 6520 746f 6f6c 7320 4920 6669 6e64 2075  e tools I find u
 00000090: 7365 6675 6c20 666f 7220 776f 726b 696e  seful for workin
 000000a0: 6720 7769 7468 2049 6720 7265 6365 7074  g with Ig recept
```

### Comparing `receptor_utils-0.0.4/src/receptor_utils/extract_refs.py` & `receptor_utils-0.0.5/src/receptor_utils/extract_refs.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,11 @@
     for seg in segs:
         ungapped[seg] = {}
         for id, seq in refs[args.species_name][seg].items():
             ungapped[seg][id] = seq.replace('.', '')
 
         simple.write_fasta(ungapped[seg], '%s_%s.fasta' % (args.species_name.replace(' ', '_'), seg))
 
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `receptor_utils-0.0.4/src/receptor_utils/identical_seqs.py` & `receptor_utils-0.0.5/src/receptor_utils/identical_seqs.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,7 +26,12 @@
             print(', '.join(names))
 
     print('Sub-sequences:')
     for n1 in seqs:
         for n2 in seqs:
             if n1 != n2 and seqs[n1] != seqs[n2] and n1 in n2:
                 print('%s is a sub-sequence of %s' % (n1, n2))
+
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `receptor_utils-0.0.4/src/receptor_utils/novel_allele_name.py` & `receptor_utils-0.0.5/src/receptor_utils/novel_allele_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,26 @@
 # ref_set: dict of reference genes (gapped in the case of v-genes), in the format returned by read_fasta
 # v_gene: True if we are naming a v_gene
 # gaps in V-sequences are '.', as in the IMGT reference set
 
 
 def name_novel(novel_seq, ref_set, v_gene=True):
     novel_seq = novel_seq.upper()
+    notes = ''
 
-    # gap the sequence if necessary
+    # gap the sequence (even if already gapped) so that we get the notes
+
+    if v_gene:
+        if '.' in novel_seq:
+            novel_seq = novel_seq.replace('.', '')
 
-    if v_gene and '.' not in novel_seq:
         ungapped_ref_set = {}
         for k, v in ref_set.items():
             ungapped_ref_set[k] = v.replace('.', '')
-        novel_seq = number_ighv.gap_sequence(novel_seq, ref_set, ungapped_ref_set)[0]
+        (novel_seq, aa, notes) = number_ighv.gap_sequence(novel_seq, ref_set, ungapped_ref_set)
 
     # Check for truncation at 5' end and construct ambiguous reference set if necessary
 
     if novel_seq[0] == '.':
         for i in range(0, len(novel_seq)):
             if novel_seq[i] != '.':
                 break
@@ -52,27 +56,38 @@
             diffs[i] = d
 
     # trim any diffs that are past the end of the novel sequence
 
     for i in range(len(novel_seq) - 1, 0):
         if novel_seq[i] != '.':
             break
-    end = i
+    novel_end = i
 
     for i in list(diffs.keys()):
-        if i > end:
+        if i > novel_end:
             del diffs[i]
 
+    # add diffs if the closest ref is longer than the novel seq
+
+    if len(closest_ref_seq) > novel_end + 1:
+        for j in range(novel_end, len(closest_ref_seq) - 1):
+            d = Diff()
+            d.pos = j
+            d.ref = closest_ref_seq[j]
+            d.novel = '-'
+            diffs[j] = d
+
+
     # consolidate any adjacent diffs
 
     prev_i = None
     for i, d in list(diffs.items()):
         if prev_i and diffs[prev_i].pos + len(diffs[prev_i].novel) == i:
             diffs[prev_i].ref += closest_ref_seq[i]
-            diffs[prev_i].novel += novel_seq[i]
+            diffs[prev_i].novel += novel_seq[i] if i < len(novel_seq) - 1 else '-'
             del diffs[i]
         else:
             prev_i = i
 
     # split diffs that are too short to consolidate
 
     for i, d in list(diffs.items()):
@@ -92,15 +107,15 @@
         d = diffs[i]
         if len(d.novel) == 1 and d.ref != '.' and d.novel != '.':
             suffs.append('%s%d%s' % (d.ref.lower(), d.pos + 1, d.novel.lower()))
         else:
             suffs.append('%d%s%d' % (d.pos + 1, d.novel.lower(), d.pos + len(d.novel)))
 
     novel_name = closest_ref_name + '_' + '_'.join(suffs) if len(suffs) else closest_ref_name
-    return(novel_name, novel_seq)
+    return(novel_name, novel_seq, notes)
 
 
 # Build (and name) a reference set for sequences truncated at the 5' end
 # Start is 0-based index of first available bp
 
 
 def build_ambiguous_ref(full_ref, start):
```

### Comparing `receptor_utils-0.0.4/src/receptor_utils/number_ighv.py` & `receptor_utils-0.0.5/src/receptor_utils/number_ighv.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,28 +256,33 @@
             diffs = d
 
     res = gap_align(seq, gapped_ref[closest])
     aa = simple.translate(seq)
     aa = gap_align_aa_from_nt(aa, res)
 
     # checks
-    notes = ''
+    notes = check_conserved_residues(aa)
+
+    return (res, aa, notes)
+
 
-    if 'X' in aa or '*' in aa:
+def check_conserved_residues(aa):
+    notes = ''
+    # allow stop codon in final nucleotides without warning
+    if 'X' in aa[:-1] or '*' in aa[:-1]:
         notes = 'Stop codon in V-REGION'
     elif aa[22] != 'C':
         notes = 'First cysteine not found'
     elif aa[40] != 'W':
         notes = 'Conserved Trp not found'
     elif len(aa) < 104:
         notes = 'Sequence truncated before second cysteine'
     elif aa[103] != 'C':
         notes = 'Second cysteine not found'
-
-    return res, aa, notes
+    return notes
 
 
 def run_tests():
     failed = 0
 
     print('1-64')
     query = 'EMQLVQSEAEVKKPGASVKISCKASGYTFTYRYLHWLRQTPGQGLEWMGWITPYNGNTNYAQKFQDRATITRDRSMSTAYMELSSLRSEDTAVYYCAR'
```

### Comparing `receptor_utils-0.0.4/src/receptor_utils/simple_bio_seq.py` & `receptor_utils-0.0.5/src/receptor_utils/simple_bio_seq.py`

 * *Files identical despite different names*

### Comparing `receptor_utils-0.0.4/src/receptor_utils.egg-info/PKG-INFO` & `receptor_utils-0.0.5/src/receptor_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Some tools I find useful for working with Ig receptor sequences
 Home-page: https://github.com/williamdlees/receptor_utils
 Author: William Lees
 Author-email: william@lees.org.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/williamdlees/receptor_utils/issues
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 # receptor_utils
 
 Some tools I find useful for working with Ig receptor sequences.
 
 # Installation
 
 ```bash
-pip install receptor_utils
+pip install receptor-utils
 ```
 
 The module requires [Biopython](https://biopython.org).
 
 # Overview
 
 Please refer to the files themselves for slightly more detailed documentation.
```

