# Comparing `tmp/nanomonsv-0.6.0.tar.gz` & `tmp/nanomonsv-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomonsv-0.6.0.tar", last modified: Wed Jun 14 10:11:09 2023, max compression
+gzip compressed data, was "nanomonsv-0.7.0.tar", last modified: Thu Jun 29 06:36:54 2023, max compression
```

## Comparing `nanomonsv-0.6.0.tar` & `nanomonsv-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/cluster_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20284 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/count_sread_by_alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv/data/
--rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/filt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/gather_support_read_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/generate_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/insert_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/locate_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/locate_bp_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/long_read_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/merge_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/my_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/post_proc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/pyssw.py
--rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/smith_waterman.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/ssw_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/swalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/vcf_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.809836 nanomonsv-0.7.0/nanomonsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/cluster_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/count_sread_by_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/nanomonsv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/gather_support_read_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/generate_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/insert_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/locate_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/locate_bp_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/long_read_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/merge_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/my_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/post_proc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/pyssw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/smith_waterman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/ssw_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/swalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/vcf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.809836 nanomonsv-0.7.0/nanomonsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/setup.py
```

### Comparing `nanomonsv-0.6.0/LICENSE` & `nanomonsv-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/PKG-INFO` & `nanomonsv-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following paper. **When you use nanomonsv or any resource of this repository, please kindly site this paper**.
 
-Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
+Precise characterization of somatic complex structural variations from tumor/control paired long-read sequencing data with nanomonsv, Shiraishi et al., Nucleic Acids Research, 2023, [[link]](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946).
 
 The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
 
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
```

### Comparing `nanomonsv-0.6.0/README.md` & `nanomonsv-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following paper. **When you use nanomonsv or any resource of this repository, please kindly site this paper**.
 
-Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
+Precise characterization of somatic complex structural variations from tumor/control paired long-read sequencing data with nanomonsv, Shiraishi et al., Nucleic Acids Research, 2023, [[link]](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946).
 
 The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
 
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
```

### Comparing `nanomonsv-0.6.0/nanomonsv/arg_parser.py` & `nanomonsv-0.7.0/nanomonsv/arg_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 
     ##########
     # parse
     parse = subparsers.add_parser("parse",
                                 help = "Parse supporting reads for candidate structural variations")
 
 
-    parse.add_argument("bam_file", default = None, type = str,
-                     help = "Path to input BAM file")
+    parse.add_argument("alignment_file", default = None, type = str,
+                     help = "Path to input BAM or CRAM file")
 
     parse.add_argument("output_prefix", type = str,
                        help = "Prefix of output files")
 
+    parse.add_argument("--reference_fasta", metavar = "reference.fa", default = None, type = str,
+                     help = "the path to the reference genome sequence")
+
     parse.add_argument("--debug", default = False, action = 'store_true', help = "keep intermediate files")
 
     parse.add_argument("--split_alignment_check_margin", default = 50, type = int,
                        help = "Two split alignments whose margin sizes are no more than this value is counted as candidate breakpoint (default: 50)")
 
     parse.add_argument("--minimum_breakpoint_ambiguity", default = 20, type = int,
                        help = "Sizes of ambiguities of breakpoint positions from the observed ones (default: 20)") 
@@ -55,24 +58,24 @@
     get = subparsers.add_parser("get",
                                 help = "List up reliable structural variations with refined breakpoint positions")
 
     get.add_argument("tumor_prefix", type = str,
                       help = "Prefix of tumor data processed in parse step")
        
     get.add_argument("tumor_bam", default = None, type = str,
-                      help = "Path to tumor BAM file")
+                      help = "Path to tumor alignment (BAM or CRAM) file")
  
     get.add_argument("reference_fasta", metavar = "reference.fa", default = None, type = str,
                      help = "the path to the reference genome sequence")
 
     get.add_argument("--control_prefix", type = str, # required = True,
                      help = "Prefix of matched control data processed in parse step")
 
     get.add_argument("--control_bam", type = str, # required = True,
-                     help = "Path to control BAM file")
+                     help = "Path to control alignment (BAM or CRAM) file")
 
     get.add_argument("--control_panel_prefix", type = str, 
                      help = "Prefix of non-matched control panel data processed in merge_control step")
 
     get.add_argument("--min_tumor_variant_read_num", default = 3, type = int,
                      help = "Minimum required supporting read number for a tumor sample (default: 3)")
 
@@ -105,37 +108,52 @@
 
     get.add_argument("--check_read_max_num", default = 500, type = int,
                      help = "The maximum number of reads to check per breakpoint in the phase of realignment validation (default: 500)")
 
     get.add_argument("--var_read_min_mapq", default = 0, type = int,
                      help = "Threshould for mapping quality in validate step (default: 0)")
 
+    get.add_argument("--validation_score_ratio_thres", default = 1.2, type = float,
+                     help = "Threshould for threshould for SV segment validation by alignment")
+
     get.add_argument("--use_ssw_lib", default = False, action = 'store_true',
                      help = "Use SSW Library. This is for backward comaptibility, and may be removed in the future (default: False)")
 
+    get.add_argument("--qv10", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5")
+
+    get.add_argument("--qv15", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.")
+
+    get.add_argument("--qv20", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 20. Recommended for ONT data with Q20+ chemistry.")
+
+    get.add_argument("--qv25", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality above 25. Recommended for PacBio Hifi data.")
+
     get.add_argument("--use_racon", default = False, action = 'store_true',
                      help = "Use racon for error correction of clustered putative supporting reads (default: False)")
 
     get.add_argument("--single_bnd", default = False, action = 'store_true',
                      help = "Generate single end breakpoints (default: False)")
 
     # get.add_argument("--control_read_num_thres", default = 0, type = int,
     #                  help = "Filter if the number of supporting reads for the control sample is larger than this value")
 
-    get.add_argument("--threads", default = 1, type = int,
-                     help = "Number of parallel threads to use (not recommended) (default: 1)")
+    # get.add_argument("--threads", default = 1, type = int,
+    #                  help = "Number of parallel threads to use (not recommended) (default: 1)")
 
     get.add_argument("--processes", default = 1, type = int,
                      help = "Number of parallel processes to use (default: 1)")
 
-    get.add_argument("--sort_option", metavar = "-S 1G", type = str, default = "-S 1G", 
+    get.add_argument("--sort_option", type = str, default = "-S 1G", 
                      help = "Options for Linux sort command (default: '-S 1G')")
 
-    get.add_argument("--max_memory_minimap2", metavar = 1, type = int, default = 1, 
-                     help = "Maximum memory size (Gbyte) for minimap2 (default: 1)")
+    get.add_argument("--max_memory_minimap2", type = int, default = 2, 
+                     help = "Maximum memory size (Gbyte) for minimap2 (default: 2)")
 
     get.add_argument("--debug", default = False, action = 'store_true', help = "keep intermediate files (default: False)")
 
     get.set_defaults(func = get_main)
     ##########
 
     ##########
@@ -157,18 +175,30 @@
 
     validate.add_argument("--control_bam", default = None, type = str,
                           help = "Path to control BAM file")
 
     validate.add_argument("--var_read_min_mapq", default = 40, type = int,
                           help = "Threshould for mapping quality in validate step")
 
-    validate.add_argument("--use_ssw_lib", default = False, action = 'store_true',
-                          help = "Use SSW Library. This is for backward comaptibility, and may be removed in the future")
+    validate.add_argument("--validation_score_ratio_thres", default = 1.2, type = float, 
+                     help = "Threshould for threshould for SV segment validation by alignment")
+
+    validate.add_argument("--qv10", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5")
+    
+    validate.add_argument("--qv15", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.")
+    
+    validate.add_argument("--qv20", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality of around 20. Recommended for ONT data with Q20+ chemistry.")
+
+    validate.add_argument("--qv25", default = False, action = 'store_true',
+                     help = "Parameter preset for sequencing data with a base quality above 25. Recommended for PacBio Hifi data.")
 
-    validate.add_argument("--sort_option", metavar = "-S 1G", type = str, default = "-S 1G", 
+    validate.add_argument("--sort_option", metavar = "-S 1G", type = str, default = "-S 2G", 
                      help = "options for sort command")
 
     validate.add_argument("--debug", default = False, action = 'store_true', help = "keep intermediate files")
 
     validate.set_defaults(func = validate_main)
     ##########
```

### Comparing `nanomonsv-0.6.0/nanomonsv/cluster.py` & `nanomonsv-0.7.0/nanomonsv/cluster.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/cluster_sbnd.py` & `nanomonsv-0.7.0/nanomonsv/cluster_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/count_sread_by_alignment.py` & `nanomonsv-0.7.0/nanomonsv/count_sread_by_alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 #! /usr/bin/env python3
 
-import sys, os, subprocess, shutil, random
+import sys, os, subprocess, shutil, random, copy
 import pysam
 import parasail
 
 from .pyssw import *
 from .my_seq import reverse_complement
+from .utils import get_alignment_object
 
 # when the total read number exceeds max_read_num, then max_read_num reads are randomly selected
-def bam_subsample_fetch(bam_ps, tchr, tstart, tend, max_read_num = 500):
+def bam_subsample_fetch(alignment_h, tchr, tstart, tend, max_read_num = 500):
 
     rec = 0
-    for read in bam_ps.fetch(tchr, tstart, tend):
+    for read in alignment_h.fetch(tchr, tstart, tend):
         rec = rec + 1
 
     selected_inds = random.sample(range(rec), min(max_read_num, rec))
 
     rec2 = 0
-    for read in bam_ps.fetch(tchr, tstart, tend):
+    for read in alignment_h.fetch(tchr, tstart, tend):
         if rec2 in selected_inds:
             yield read
         rec2 = rec2 + 1
 
 # function for gathering sequence read for realignment validation
-def gather_local_read_for_realignment(sv_file, bam_file, output_file,
+def gather_local_read_for_realignment(sv_file, alignment_file, output_file, reference_fasta,
     sbnd_file = None, output_file_sbnd = None, validate_sequence_length = 200, check_read_max_num = 500,
     sort_option = None):
 
-    bam_ps = pysam.AlignmentFile(bam_file, "rb")
+    alignment_h = get_alignment_object(alignment_file, reference_fasta)
 
     rname2key = {}
     key2rname2mapq = {}
     with open(sv_file, 'r') as hin:
         for line in hin:
             if line.startswith("#") or line.startswith("Chr_1"): continue
             F = line.rstrip('\n').split('\t')
             tchr1, tpos1, tdir1, tchr2, tpos2, tdir2, tinseq, tid = F[0], int(F[1]), F[2], F[3], int(F[4]), F[5], F[6], F[7]
             # if tinseq == "---": tinseq = ''
             key = f"{tchr1},{tpos1},{tdir1},{tchr2},{tpos2},{tdir2},{tinseq},{tid}"
 
             if key not in key2rname2mapq: key2rname2mapq[key] = {}
 
-            # for read in bam_ps.fetch(tchr1, max(tpos1 - 100, 0), tpos1 + 100):
-            for read in bam_subsample_fetch(bam_ps, tchr1, max(tpos1 - 100, 0), tpos1 + 100):
+            for read in bam_subsample_fetch(alignment_h, tchr1, max(tpos1 - 100, 0), tpos1 + 100):
     
                 if read.qname not in rname2key: rname2key[read.qname] = []
                 rname2key[read.qname].append(key)
 
                 if read.qname not in key2rname2mapq[key]: key2rname2mapq[key][read.qname] = [None, None]
                 key2rname2mapq[key][read.qname][0] = read.mapping_quality
 
-            # for read in bam_ps.fetch(tchr2, max(tpos2 - 100, 0), tpos2 + 100):
-            for read in bam_subsample_fetch(bam_ps, tchr2, max(tpos2 - 100, 0), tpos2 + 100):
+            for read in bam_subsample_fetch(alignment_h, tchr2, max(tpos2 - 100, 0), tpos2 + 100):
 
                 if read.qname not in rname2key: rname2key[read.qname] = []
                 rname2key[read.qname].append(key)
 
                 if read.qname not in key2rname2mapq[key]: key2rname2mapq[key][read.qname] = [None, None]
                 key2rname2mapq[key][read.qname][1] = read.mapping_quality
 
@@ -73,31 +72,30 @@
                 if line.startswith("#") or line.startswith("Chr_1"): continue
                 F = line.rstrip('\n').split('\t')
                 tchr, tpos, tdir, tseq, tid = F[0], int(F[1]), F[2], F[3][:validate_sequence_length], F[4]
                 key = f"{tchr},{tpos},{tdir},{tseq},{tid}"
 
                 if key not in key2rname2mapq_sbnd: key2rname2mapq_sbnd[key] = {}
 
-                # for read in bam_ps.fetch(tchr, max(tpos - 100, 0), tpos + 100):
-                for read in bam_subsample_fetch(bam_ps, tchr, max(tpos - 100, 0), tpos + 100):
+                for read in bam_subsample_fetch(alignment_h, tchr, max(tpos - 100, 0), tpos + 100):
 
                     if read.qname not in rname2key_sbnd: rname2key_sbnd[read.qname] = []
                     rname2key_sbnd[read.qname].append(key)
                     
                     key2rname2mapq_sbnd[key][read.qname] = read.mapping_quality
 
         # remove duplicated keys
         for rname in rname2key_sbnd:
             keys = list(set(rname2key_sbnd[rname]))
             rname2key_sbnd[rname] = keys
 
  
     hout = open(output_file + ".tmp.unsorted", 'w')
     if sbnd_file is not None: hout_sbnd = open(output_file_sbnd + ".tmp.unsorted", 'w')
-    for read in bam_ps.fetch():
+    for read in alignment_h.fetch():
 
         flags = format(int(read.flag), "#014b")[:1:-1]
 
         # skip supplementary alignment
         if flags[8] == "1" or flags[11] == "1": continue
 
         # skip duplicated reads             
@@ -129,15 +127,15 @@
     os.remove(output_file + ".tmp.unsorted")
 
     if sbnd_file is not None:
         with open(output_file_sbnd, 'w') as hout:
             subprocess.call(["sort", "-k1,1"] + sort_option.split(" ") + [output_file_sbnd + ".tmp.unsorted"], stdout = hout)
         os.remove(output_file_sbnd + ".tmp.unsorted")
 
-    bam_ps.close()
+    alignment_h.close()
 
 
 def ssw_check(query, target, use_ssw = False):
 
     user_matrix = parasail.matrix_create("ACGT", 2, -2)
 
     alignment_info = {}
@@ -165,16 +163,16 @@
 
     return(alignment_info)
 
 
 class Alignment_counter(object):
 
     def __init__(self, output_count_file, output_alignment_info_file, reference_fasta,
-        var_read_min_mapq, use_ssw_lib, debug, validate_sequence_length = 200,  
-        score_ratio_thres = 1.2, start_pos_thres = 0.1, end_pos_thres = 0.9, var_ref_margin_thres = 20):
+        var_read_min_mapq, score_ratio_thres, use_ssw_lib, debug, validate_sequence_length = 200,  
+        start_pos_thres = 0.1, end_pos_thres = 0.9, var_ref_margin_thres = 20):
 
         self.temp_key = None
         self.temp_key2 = None # here, the insertion sequence is converted to its length. this is to shorten file names.
         self.hout_count = open(output_count_file, 'w')
         self.hout_ainfo = open(output_alignment_info_file, 'w')
         self.reference_fasta_h = pysam.FastaFile(reference_fasta)
 
@@ -193,14 +191,15 @@
         self.use_ssw_lib = use_ssw_lib
         self.debug = debug
 
         self.tmp_dir = output_count_file + ".tmp_dir"
         os.makedirs(self.tmp_dir, exist_ok = True)
 
 
+
     def __del__(self):
 
         self.hout_count.close()
         self.hout_ainfo.close()
         self.reference_fasta_h.close()
         if not self.debug:
             shutil.rmtree(self.tmp_dir)
@@ -208,14 +207,25 @@
     def initialize(self, key, is_sbnd = False):
         self.temp_key = key
         # the insertion sequence is converted to its length. this is to shorten file names.
         tkeys = self.temp_key.split(',')
         tkeys[-2] = '' if tkeys[-2] == '---' else tkeys[-1]
         tkeys[-2] = str(len(tkeys[-2]))
         self.temp_key2 = ','.join(tkeys)
+
+        self.is_inseq = True if tkeys[-2] != '' else False
+
+        if is_sbnd == False:
+            self.is_short_del_dup = False
+            if tkeys[6] == "---": tkeys[6] = ''
+            if tkeys[0] == tkeys[3] and tkeys[2] == '+' and tkeys[5] == '-' and int(tkeys[4]) - int(tkeys[1]) + len(tkeys[6]) < 300:
+                self.is_short_del_dup = True
+            elif tkeys[0] == tkeys[3] and tkeys[2] == '-' and tkeys[5] == '+' and int(tkeys[4]) - int(tkeys[1]) + len(tkeys[6]) < 300:
+                self.is_short_del_dup = True
+
         self.readid2mapq = {}
         self.temp_long_read_seq_file_h = open(self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", 'w')
         if is_sbnd:
             self.generate_segment_fasta_files_sbnd()
         else:
             self.generate_segment_fasta_files()
 
@@ -284,60 +294,71 @@
         # close file hundle for writing long_read_seq.fa if it is open
         if self.temp_long_read_seq_file_h is not None: self.temp_long_read_seq_file_h.close()
 
         with open(self.tmp_dir + '/' + self.temp_key2 + ".variant_seg_1.fa", 'w') as hout:
             print('>' + self.temp_key2 + '\n' + self.variant_segment_1, file = hout)
         with open(self.tmp_dir + '/' + self.temp_key2 + ".variant_seg_2.fa", 'w') as hout:
             print('>' + self.temp_key2 + '\n' + self.variant_segment_2, file = hout)
-        with open(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_1.fa", 'w') as hout:
-            print('>' + self.temp_key2 + '\n' + self.reference_segment_1, file = hout)
-        with open(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_2.fa", 'w') as hout:
-            print('>' + self.temp_key2 + '\n' + self.reference_segment_2, file = hout)
 
         alignment_info_var_1 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".variant_seg_1.fa",
             self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
-        alignment_info_var_2 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".variant_seg_2.fa", 
-            self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib) 
 
-        # if is_short_del_dup(self.temp_key):
-        alignment_info_ref_1 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_1.fa",
-            self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
-        alignment_info_ref_2 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_2.fa",
-            self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
+        if self.is_inseq:
+            alignment_info_var_2 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".variant_seg_2.fa",
+                self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
+        else:
+            alignment_info_var_2 = copy.copy(alignment_info_var_1)
+
+
+        if self.is_short_del_dup:
+            with open(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_1.fa", 'w') as hout:
+                print('>' + self.temp_key2 + '\n' + self.reference_segment_1, file = hout)
+
+            with open(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_2.fa", 'w') as hout:
+                print('>' + self.temp_key2 + '\n' + self.reference_segment_2, file = hout)
+
+            alignment_info_ref_1 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_1.fa",
+                self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
+            alignment_info_ref_2 = ssw_check(self.tmp_dir + '/' + self.temp_key2 + ".reference_seg_2.fa",
+                self.tmp_dir + '/' + self.temp_key2 + ".long_read_seq.fa", self.use_ssw_lib)
+
 
         all_rnames = list(set(list(alignment_info_var_1.keys()) + list(alignment_info_var_2.keys())))
 
         supporting_reads = [rname for rname in all_rnames if \
             (alignment_info_var_1[rname][0] > self.score_ratio_thres * len(self.variant_segment_1) and \
             alignment_info_var_1[rname][1] < self.start_pos_thres * len(self.variant_segment_1) and \
             alignment_info_var_1[rname][2] > self.end_pos_thres * len(self.variant_segment_1)) or \
             (alignment_info_var_2[rname][0] > self.score_ratio_thres * len(self.variant_segment_2) and \
             alignment_info_var_2[rname][1] < self.start_pos_thres * len(self.variant_segment_2) and \
             alignment_info_var_2[rname][2] > self.end_pos_thres * len(self.variant_segment_2))]
 
         # for short deletion or insertion
-        # if is_short_del_dup(self.temp_key):
-        supporting_reads = [rname for rname in supporting_reads if \
-            (alignment_info_var_1[rname][0] >= alignment_info_ref_1[rname][0] + self.var_ref_margin_thres and \
-            alignment_info_var_1[rname][0] >= alignment_info_ref_2[rname][0] + self.var_ref_margin_thres) or \
-            (alignment_info_var_2[rname][0] >= alignment_info_ref_1[rname][0] + self.var_ref_margin_thres and \
-             alignment_info_var_2[rname][0] >= alignment_info_ref_1[rname][0] + self.var_ref_margin_thres)]
+        if self.is_short_del_dup:
+            supporting_reads = [rname for rname in supporting_reads if \
+                (alignment_info_var_1[rname][0] >= alignment_info_ref_1[rname][0] + self.var_ref_margin_thres and \
+                alignment_info_var_1[rname][0] >= alignment_info_ref_2[rname][0] + self.var_ref_margin_thres) or \
+                (alignment_info_var_2[rname][0] >= alignment_info_ref_1[rname][0] + self.var_ref_margin_thres and \
+                alignment_info_var_2[rname][0] >= alignment_info_ref_2[rname][0] + self.var_ref_margin_thres)]
 
         # filtering by mapping qualities
         supporting_reads = [rname for rname in supporting_reads if \
             self.readid2mapq[rname][0] is not None and self.readid2mapq[rname][0] >= self.var_read_min_mapq and \
             self.readid2mapq[rname][1] is not None and self.readid2mapq[rname][1] >= self.var_read_min_mapq]
 
 
         tchr1, tpos1, tdir1, tchr2, tpos2, tdir2, tinseq, tid = self.temp_key.split(',')
         print(f"{tchr1}\t{tpos1}\t{tdir1}\t{tchr2}\t{tpos2}\t{tdir2}\t{tinseq}\t{tid}\t{len(all_rnames)}\t{len(supporting_reads)}", file = self.hout_count)
         
         sread_info = { rname: alignment_info_var_1[rname] + alignment_info_var_2[rname] for rname in supporting_reads}
         for rname in supporting_reads:
-            sinfo = '\t'.join([str(x) for x in alignment_info_var_1[rname] + alignment_info_var_2[rname] + alignment_info_ref_1[rname] + alignment_info_ref_2[rname]])
+            if self.is_short_del_dup:
+                sinfo = '\t'.join([str(x) for x in alignment_info_var_1[rname] + alignment_info_var_2[rname] + alignment_info_ref_1[rname] + alignment_info_ref_2[rname]])
+            else:
+                sinfo = '\t'.join([str(x) for x in alignment_info_var_1[rname] + alignment_info_var_2[rname] + ["None"] * 12])
             print(f"{tchr1}\t{tpos1}\t{tdir1}\t{tchr2}\t{tpos2}\t{tdir2}\t{tinseq}\t{tid}\t{rname}\t{sinfo}", file = self.hout_ainfo)
 
 
     def count_alignment_and_print_sbnd(self):
 
         # close file hundle for writing long_read_seq.fa if it is open
         if self.temp_long_read_seq_file_h is not None: self.temp_long_read_seq_file_h.close()
@@ -373,26 +394,26 @@
         sread_info = { rname: alignment_info_var_1[rname] for rname in supporting_reads}
         for rname in supporting_reads:
             sinfo = '\t'.join([str(x) for x in alignment_info_var_1[rname] ])
             print(f"{tchr}\t{tpos}\t{tdir}\t{tcontig}\t{tid}\t{rname}\t{sinfo}", file = self.hout_ainfo)
 
 
 
-def count_sread_by_alignment(sv_file, bam_file, output_count_file, output_alignment_info_file, reference_fasta, 
+def count_sread_by_alignment(sv_file, alignment_file, output_count_file, output_alignment_info_file, reference_fasta, 
     sbnd_file = None, output_count_file_sbnd = None, output_alignment_info_file_sbnd = None,
-    check_read_max_num = 500, var_read_min_mapq = 0, use_ssw_lib = False, sort_option = None, debug = False):
+    check_read_max_num = 500, var_read_min_mapq = 0, score_ratio_thres = 1.2, use_ssw_lib = False, sort_option = None, debug = False):
 
-    gather_local_read_for_realignment(sv_file, bam_file, output_count_file + ".tmp.local_read_for_realignment",
+    gather_local_read_for_realignment(sv_file, alignment_file, output_count_file + ".tmp.local_read_for_realignment", reference_fasta,
         sbnd_file = sbnd_file, 
         output_file_sbnd = output_count_file_sbnd + ".tmp.local_read_for_realignment" if output_count_file_sbnd is not None else None,
         check_read_max_num = check_read_max_num,
         sort_option = sort_option)
 
     alignment_counter = Alignment_counter(output_count_file, output_alignment_info_file, reference_fasta,
-        var_read_min_mapq, use_ssw_lib, debug)
+        var_read_min_mapq, score_ratio_thres, use_ssw_lib, debug)
 
     with open(output_count_file + ".tmp.local_read_for_realignment", 'r') as hin:
         for line in hin:
             tkey, treadid, tmapq1, tmpaq2, tseq = line.rstrip('\n').split('\t')
             if alignment_counter.temp_key != tkey:
                 if alignment_counter.temp_key is not None:
                     alignment_counter.count_alignment_and_print()
@@ -406,15 +427,15 @@
 
     if not debug:
         os.remove(output_count_file + ".tmp.local_read_for_realignment")
 
     if sbnd_file is None: return
 
     alignment_counter_sbnd = Alignment_counter(output_count_file_sbnd, output_alignment_info_file_sbnd, reference_fasta,
-        var_read_min_mapq, use_ssw_lib, debug)
+        var_read_min_mapq, score_ratio_thres, use_ssw_lib, debug)
 
     with open(output_count_file_sbnd + ".tmp.local_read_for_realignment", 'r') as hin:
         for line in hin:
             tkey, treadid, tmapq1, tmapq2, tseq = line.rstrip('\n').split('\t')
             tmapq2 = "None"
             if alignment_counter_sbnd.temp_key != tkey:
                 if alignment_counter_sbnd.temp_key is not None:
```

### Comparing `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz` & `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi` & `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz` & `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi` & `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/filt.py` & `nanomonsv-0.7.0/nanomonsv/filt.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/gather_support_read_seq.py` & `nanomonsv-0.7.0/nanomonsv/gather_support_read_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python3
 
 import sys, os, subprocess, statistics 
 import pysam
 
 from .logger import get_logger
 from .my_seq import reverse_complement
+from .utils import get_alignment_object
 
 logger = get_logger(__name__)
 
  
 def set_readid2alignment(readid2alignment, input_file, mode, alignment_margin):
 
     # readid2alignment = {}
@@ -83,34 +84,35 @@
                     readid2alignment_sbnd[readids[i]].append((tkey, max(1, qpos - alignment_margin), qlen, qstrand, '*'))
                 else:
                     readid2alignment_sbnd[readids[i]].append((tkey, 1, min(qpos + alignment_margin, qlen), qstrand, '*'))
 
             cid = cid + 1
 
 
-def gather_support_read_seq(rearrangement_file, insertion_file, deletion_file, output_file, tumor_bam, 
+def gather_support_read_seq(rearrangement_file, insertion_file, deletion_file, output_file, tumor_alignment_file, reference_fasta, 
     single_breakend_file = None, output_file_sbind = None, alignment_margin = 300):
 
     is_sbnd = True if single_breakend_file is not None else False
 
-    bamfile = pysam.AlignmentFile(tumor_bam, "rb")
+    
+    alignment_h = get_alignment_object(tumor_alignment_file, reference_fasta)
 
     readid2alignment = {}
     set_readid2alignment(readid2alignment, rearrangement_file, 'r', alignment_margin)
     set_readid2alignment(readid2alignment, insertion_file, 'i', alignment_margin)
     set_readid2alignment(readid2alignment, deletion_file, 'd', alignment_margin)
     
     hout = open(output_file + ".tmp.unsorted", 'w')
 
     if is_sbnd:
         readid2alignment_sbnd = {}
         set_readid2alignment_sbnd(readid2alignment_sbnd, single_breakend_file, alignment_margin)
         hout_sbnd = open(output_file + ".sbnd.tmp.unsorted", 'w')
 
-    for read in bamfile.fetch():
+    for read in alignment_h.fetch():
 
         if read.is_secondary or read.is_supplementary: continue
 
         if read.query_name in readid2alignment:
 
             for talignment in readid2alignment[read.query_name]:
 
@@ -133,14 +135,15 @@
                 read_seq = reverse_complement(read.query_sequence) if read.is_reverse else read.query_sequence
                 part_seq = read_seq[(astart - 1):aend]
                 if astrand != tstrand: part_seq = reverse_complement(part_seq)
 
                 print('\t'.join([akey, read.query_name, asize, part_seq]), file = hout_sbnd)
 
 
+    alignment_h.close()
     hout.close()
     if is_sbnd: hout_sbnd.close()
 
     with open(output_file, 'w') as hout:
         subprocess.check_call(["sort", "-k1,1", output_file + ".tmp.unsorted"], stdout = hout)
     os.remove(output_file + ".tmp.unsorted")
```

### Comparing `nanomonsv-0.6.0/nanomonsv/generate_consensus.py` & `nanomonsv-0.7.0/nanomonsv/generate_consensus.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,19 +211,24 @@
         elif "RLIMIT_VMEM" in resource.__dict__:
             resource.setrlimit(resource.RLIMIT_VMEM, (limit, limit))
 
     def print_consensus_sbnd(self):
 
         if self.temp_support_read_file_h is not None: self.temp_support_read_file_h.close()
 
-        with open(self.tmp_dir + '/' + self.temp_key + "_ava_minimap2.paf", 'w') as hout:
-            subprocess.check_call(["minimap2", "-x", "ava-ont", 
-                self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa",
-                self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
-                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        try:
+            with open(self.tmp_dir + '/' + self.temp_key + "_ava_minimap2.paf", 'w') as hout:
+                subprocess.check_call(["minimap2", "-x", "ava-ont", 
+                    self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa",
+                    self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
+                    stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        except Exception as e:
+            logger.warning(f'{e}')
+            return
+
 
         readid2inclusion_count = {}
         with open(self.tmp_dir + '/' + self.temp_key + "_ava_minimap2.paf") as hin:
             for line in hin:
                 row = line.rstrip('\n').split('\t')
                 if int(row[2]) <= self.start_margin and (float(row[3]) - float(row[2])) / float(row[1]) >= self.min_inclusion_ratio:
                     if row[5] not in readid2inclusion_count: readid2inclusion_count[row[5]] = 0
@@ -247,18 +252,22 @@
                     print(f">{tid}\n{tseq}", file = hout)
                     break
                 seq_read_count = seq_read_count + 1
                 if tid == '' or seq_read_count > 10000: 
                     logger.warning(f"Something inconsistent happend when choosing template reads for {self.temp_key}")
                     return
 
-        with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2.paf", 'w') as hout:
-            subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref.fa",
-                self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"], 
-                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        try:
+            with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2.paf", 'w') as hout:
+                subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref.fa",
+                    self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"], 
+                    stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        except Exception as e:
+            logger.warning(f'{e}')
+            return
 
         paf_rec_count = 0
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2.paf", 'r') as hin:
             for line in hin:
                 paf_rec_count = paf_rec_count + 1
 
         if paf_rec_count < 3:
@@ -283,18 +292,22 @@
 
         if len(consensus) < 1000: return
                         
         # second round racon
         with open(self.tmp_dir + '/' + self.temp_key + "_ref_2nd.fa", 'w') as hout:
             print(f">{self.temp_key}_1st_polished_seq\n{consensus}", file = hout)
 
-        with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2_2nd.paf", 'w') as hout:
-            subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref_2nd.fa",
-                self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
-                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        try:
+            with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2_2nd.paf", 'w') as hout:
+                subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref_2nd.fa",
+                    self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
+                    stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
+        except Exception as e:
+            logger.warning(f'{e}')
+            return
 
         paf_rec_count = 0
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2_2nd.paf", 'r') as hin:
             for line in hin:
                 paf_rec_count = paf_rec_count + 1
             
         if paf_rec_count < 3:
```

### Comparing `nanomonsv-0.6.0/nanomonsv/insert_classify.py` & `nanomonsv-0.7.0/nanomonsv/insert_classify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/locate_bp.py` & `nanomonsv-0.7.0/nanomonsv/locate_bp.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/locate_bp_sbnd.py` & `nanomonsv-0.7.0/nanomonsv/locate_bp_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/long_read_validate.py` & `nanomonsv-0.7.0/nanomonsv/long_read_validate.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/merge_control.py` & `nanomonsv-0.7.0/nanomonsv/merge_control.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/my_seq.py` & `nanomonsv-0.7.0/nanomonsv/my_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/parse.py` & `nanomonsv-0.7.0/nanomonsv/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #! /usr/bin/env python3
 
-import sys, subprocess, itertools
+import sys, os, subprocess, itertools
 import pysam
 
 from .logger import get_logger
+from .utils import get_alignment_object 
 logger = get_logger(__name__)
 
-def parse_alignment_info(input_bam, deletion_output_file, insertion_output_file, rearrangement_output_file,
+def parse_alignment_info(input_alignment_file, reference_fasta, deletion_output_file, insertion_output_file, rearrangement_output_file,
     breakpoint_output_file, min_ins_size = 20, min_del_size = 30, min_clipping_size_for_bp = 200):
 
     """Parse BAM file to obtain putative SV supporting reads and their associated info."""
 
     hout_d = open(deletion_output_file, 'w')
     hout_i = open(insertion_output_file, 'w')
     hout_r = open(rearrangement_output_file, 'w') 
     hout_b = open(breakpoint_output_file, 'w')
 
-    bamfile = pysam.AlignmentFile(input_bam, "rb")
+    alignment_h = get_alignment_object(input_alignment_file, reference_fasta)
     
-    for read in bamfile.fetch():
+    for read in alignment_h.fetch():
 
         # if read.is_secondary: continue
 
         query_name = read.query_name
         query_strand = '-' if read.is_reverse else '+'
         query_length = read.infer_read_length()
 
@@ -177,15 +178,15 @@
                 file = hout_b)
 
 
     hout_d.close()
     hout_i.close()
     hout_r.close()
     hout_b.close()
-    bamfile.close()
+    alignment_h.close()
 
 
 def extract_bedpe_junction(input_file, output_file, split_alignment_check_margin1 = 50, split_alignment_check_margin2 = 50, minimum_ambiguity = 20):
 
    
     def print_bedpe_junction(query2target, hout):
```

### Comparing `nanomonsv-0.6.0/nanomonsv/post_proc.py` & `nanomonsv-0.7.0/nanomonsv/post_proc.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/pyssw.py` & `nanomonsv-0.7.0/nanomonsv/pyssw.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/run.py` & `nanomonsv-0.7.0/nanomonsv/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,40 +11,39 @@
 from .locate_bp_sbnd import *
 from .count_sread_by_alignment import *
 from .post_proc import *
 from .vcf_convert import *
 from .insert_classify import *
 from .utils import *
 from .logger import get_logger
-
+from .utils import *
 
 logger = get_logger(__name__)
 
 def parse_main(args):
 
     # check if the executables exist
     is_tool("tabix")
     is_tool("bgzip")
 
     # check input file existences
-    is_exists_bam(args.bam_file)
+    is_exists_bam(args.alignment_file)
 
     # BAM format check
-    bam_format_check(args.bam_file)
+    bam_cram_format_check(args.alignment_file, args.reference_fasta)
 
     # make directory for the output prefix
     output_dir = os.path.dirname(args.output_prefix)
     if output_dir != '' and not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     ####################
-    parse_alignment_info(args.bam_file, args.output_prefix + ".tmp.deletion_info.txt", 
-                                        args.output_prefix + ".tmp.insertion_info.txt", 
-                                        args.output_prefix + ".tmp.rearrangement_info.txt",
-                                        args.output_prefix + ".tmp.bp_info.txt")
+    parse_alignment_info(args.alignment_file, args.reference_fasta, 
+        args.output_prefix + ".tmp.deletion_info.txt", args.output_prefix + ".tmp.insertion_info.txt", 
+        args.output_prefix + ".tmp.rearrangement_info.txt", args.output_prefix + ".tmp.bp_info.txt")
 
     ####################
     # deletion processing
     hout = open(args.output_prefix + ".tmp.deletion.sorted.bed", 'w')
     subprocess.check_call(["sort", "-k1,1", "-k2,2n", "-k3,3n", "-k5,5n", args.output_prefix + ".tmp.deletion_info.txt"], stdout = hout)
     hout.close()
 
@@ -71,16 +70,16 @@
     ####################
     # rearrangement processing
     hout = open(args.output_prefix + ".tmp.rearrangement_info.name_sorted.txt", 'w')
     subprocess.check_call(["sort", "-k1,1", "-k2,2n", args.output_prefix + ".tmp.rearrangement_info.txt"], stdout = hout)
     hout.close()
 
     extract_bedpe_junction(args.output_prefix + ".tmp.rearrangement_info.name_sorted.txt", 
-                           args.output_prefix + ".tmp.rearrangement.bedpe") # ,
-                           # args.split_alignment_check_margin, args.minimum_breakpoint_ambiguity)
+                           args.output_prefix + ".tmp.rearrangement.bedpe",
+                           args.split_alignment_check_margin, args.split_alignment_check_margin, args.minimum_breakpoint_ambiguity)
 
     hout = open(args.output_prefix + ".tmp.rearrangement.sorted.bedpe", 'w')
     subprocess.check_call(["sort", "-k1,1", "-k2,2n", "-k3,3n", "-k4,4", "-k5,5n", "-k6,6n", 
                            args.output_prefix + ".tmp.rearrangement.bedpe"], stdout = hout)
     hout.close()
   
     hout = open(args.output_prefix + ".rearrangement.sorted.bedpe.gz", 'w')
@@ -121,105 +120,127 @@
     merge_control_from_parse_files(args.prefix_list_file, args.output_prefix)
 
 
 def call_slow_request(args, index):
     ret_code = 1
     err_message = ""
     try:
-        logger.info("Generate consensus sequences (%d)" % (index))
-        generate_consensus(args.tumor_prefix + ".support_read_seq.%d.txt" % (index),
-            args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
-            use_racon = args.use_racon, debug = args.debug)
-        generate_consensus_sbnd(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (index),
-            args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
-            use_racon = args.use_racon, debug = args.debug, max_memory_minimap2 = args.max_memory_minimap2)
-
-        logger.info("Locating single-base resolution break points for candidate SVs (%d)" % (index))
-        locate_bp(args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
-            args.tumor_prefix + ".refined_bp.%d.txt" % (index),
-            args.reference_fasta, args.debug)
-        locate_bp_sbnd(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
-            args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index),
-            args.reference_fasta, args.debug)
+        call_slow_request_main(args, index)
+        ret_code = 0
+    except Exception as e:
+        err_message = str(e)
+    
+    logger.info("End Process (%d): ret_code=%d" % (index, ret_code))
+    return (ret_code, err_message)
+
+
+def call_slow_request_main(args, index):
 
-        logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments (%d)" % (index))
+    logger.info("Generate consensus sequences (%d)" % (index))
+    generate_consensus(args.tumor_prefix + ".support_read_seq.%d.txt" % (index),
+        args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
+        use_racon = args.use_racon, debug = args.debug)
+    generate_consensus_sbnd(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (index),
+        args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
+        use_racon = args.use_racon, debug = args.debug, max_memory_minimap2 = args.max_memory_minimap2)
+
+    logger.info("Locating single-base resolution break points for candidate SVs (%d)" % (index))
+    locate_bp(args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
+        args.tumor_prefix + ".refined_bp.%d.txt" % (index),
+        args.reference_fasta, args.debug)
+    locate_bp_sbnd(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
+        args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index),
+        args.reference_fasta, args.debug)
+
+    logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments (%d)" % (index))
+    count_sread_by_alignment(
+        args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
+        args.tumor_bam, 
+        args.tumor_prefix + ".realignment.tumor.sread_count.%d.txt" % (index), 
+        args.tumor_prefix + ".realignment.tumor.sread_info.%d.txt" % (index), 
+        args.reference_fasta,
+        sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
+        output_count_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.%d.txt" % (index),
+        output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_info.sbnd.%d.txt" % (index),
+        check_read_max_num = args.check_read_max_num, 
+        var_read_min_mapq = args.var_read_min_mapq, score_ratio_thres = args.validation_score_ratio_thres, use_ssw_lib = False, 
+        sort_option = args.sort_option, debug = args.debug
+    )
+     
+    if args.control_bam is not None:
+        logger.info("Counting the number of supporting read for the control by realignment of SV candidate segments (%d)" % (index))
         count_sread_by_alignment(
             args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
-            args.tumor_bam, 
-            args.tumor_prefix + ".realignment.tumor.sread_count.%d.txt" % (index), 
-            args.tumor_prefix + ".realignment.tumor.sread_info.%d.txt" % (index), 
+            args.control_bam, 
+            args.tumor_prefix + ".realignment.control.sread_count.%d.txt" % (index), 
+            args.tumor_prefix + ".realignment.control.sread_info.%d.txt" % (index), 
             args.reference_fasta,
             sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
-            output_count_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.%d.txt" % (index),
-            output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_info.sbnd.%d.txt" % (index),
+            output_count_file_sbnd = args.tumor_prefix + ".realignment.control.sread_count.sbnd.%d.txt" % (index),
+            output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.control.sread_info.sbnd.%d.txt" % (index),
             check_read_max_num = args.check_read_max_num, 
-            var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
+            var_read_min_mapq = args.var_read_min_mapq, score_ratio_thres = args.validation_score_ratio_thres, use_ssw_lib = False, 
             sort_option = args.sort_option, debug = args.debug
         )
-     
-        if args.control_bam is not None:
-            logger.info("Counting the number of supporting read for the control by realignment of SV candidate segments (%d)" % (index))
-            count_sread_by_alignment(
-                args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
-                args.control_bam, 
-                args.tumor_prefix + ".realignment.control.sread_count.%d.txt" % (index), 
-                args.tumor_prefix + ".realignment.control.sread_info.%d.txt" % (index), 
-                args.reference_fasta,
-                sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
-                output_count_file_sbnd = args.tumor_prefix + ".realignment.control.sread_count.sbnd.%d.txt" % (index),
-                output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.control.sread_info.sbnd.%d.txt" % (index),
-                check_read_max_num = args.check_read_max_num, 
-                var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
-                sort_option = args.sort_option, debug = args.debug
-            )
-        ret_code = 0
-    except Exception as e:
-        err_message = str(e)
-    
-    logger.info("End Process (%d): ret_code=%d" % (index, ret_code))
-    return (ret_code, err_message)
+
 
 def get_main(args):
 
     # check if the executables exist
     if args.use_racon: 
         is_tool("racon")
     else:
         is_tool("mafft")
-    if args.use_ssw_lib: libssw_check()
+    if False: libssw_check()
 
     if args.single_bnd: 
         is_tool("minimap2")
         if not args.use_racon:
             logger.error("single_bnd option has to be used with use_racon option")
             sys.exit(1)
 
     parallel_num = 1
-    if args.threads > 1:
-        if args.processes > 1:
-            logger.error("threads option has to be used with processes option")
-            sys.exit(1)
-        parallel_num = args.threads
-    elif args.processes > 1:
+    # if args.threads > 1:
+    #     if args.processes > 1:
+    #         logger.error("--threads option sholud not be used with processes option")
+    #         sys.exit(1)
+    #     logger.warning("--threads option is not recommended. Please consider using --processes option")
+    #     parallel_num = args.threads
+    # elif args.processes > 1:
+    if args.processes > 1:
         parallel_num = args.processes
 
+    # parameter preset 
+    if sum([int(x == True) for x in [args.qv10, args.qv15, args.qv20, args.qv25]]) > 1:
+        logger.error("Parameter preset (qv10, qv15, qv20, qv25) should be set only once")
+        sys.exit(1)
+
+    if args.qv10:
+        args.validation_score_ratio_thres = 1.2
+    elif args.qv15:
+        args.validation_score_ratio_thres = 1.4
+    elif args.qv20: 
+        args.validation_score_ratio_thres = 1.6
+    elif args.qv25:
+        args.validation_score_ratio_thres = 1.8
+
     # check existences
     is_exists_bam(args.tumor_bam)
     is_exists(args.reference_fasta)
     if args.control_bam is not None: is_exists_bam(args.control_bam)
    
     # check parsed files existences
     is_exists_parsed_files(args.tumor_prefix)
     if args.control_prefix is not None: is_exists_parsed_files(args.control_prefix)
     if args.control_panel_prefix is not None: is_exists_parsed_files(args.control_panel_prefix)
  
     # BAM format check
-    bam_format_check(args.tumor_bam)
+    bam_cram_format_check(args.tumor_bam, args.reference_fasta)
     fasta_format_check(args.reference_fasta)
-    if args.control_bam is not None: bam_format_check(args.control_bam)
+    if args.control_bam is not None: bam_cram_format_check(args.control_bam, args.reference_fasta)
 
     control_rearrangement_bedpe = None
     control_deletion_bed = None
     control_insertion_bed = None
     control_bp_bed = None
     if args.control_prefix is not None: 
         control_rearrangement_bedpe = args.control_prefix + ".rearrangement.sorted.bedpe.gz"
@@ -287,15 +308,15 @@
             pass
 
     logger.info("Gathering sequences of supporting reads")
     gather_support_read_seq(args.tumor_prefix + ".rearrangement.sorted.clustered.bedpe",
         args.tumor_prefix + ".insertion.sorted.clustered.bedpe",
         args.tumor_prefix + ".deletion.sorted.clustered.bedpe",
         args.tumor_prefix + ".support_read_seq.txt",
-        args.tumor_bam, single_breakend_file = args.tumor_prefix + ".singlebreakend.sorted.clustered.bed",
+        args.tumor_bam, args.reference_fasta, single_breakend_file = args.tumor_prefix + ".singlebreakend.sorted.clustered.bed",
         output_file_sbind = args.tumor_prefix + ".support_read_seq.sbnd.txt" )
     
     logger.info("Preparation for parallel execution")
     fw_support_read_seqs = []
     fw_support_read_seq_sbnds = []
     for i in range(parallel_num):
         fw_support_read_seqs.append(open(args.tumor_prefix + ".support_read_seq.%d.txt" % (i), "w"))
@@ -328,17 +349,15 @@
             fw_support_read_seq_sbnds[last_tpos].write(row)
 
     for i in range(parallel_num):
         fw_support_read_seqs[i].close()
         fw_support_read_seq_sbnds[i].close()
 
     if parallel_num == 1:
-        ret_code, err_message = call_slow_request(args, 0)
-        if ret_code != 0:
-            raise Exception(err_message)
+        call_slow_request_main(args, 0)
     else:
         import concurrent.futures
 
         if args.processes > 1:
             with concurrent.futures.ProcessPoolExecutor(max_workers=parallel_num) as executor:
                 features = [executor.submit(call_slow_request, args, i) for i in range(parallel_num)]
                 for feature in features:
@@ -441,63 +460,66 @@
         if not args.single_bnd:
             os.remove(args.tumor_prefix + ".nanomonsv.sbnd.result.txt")   
 
 
 def validate_main(args):
    
     # executable check
-    if args.use_ssw_lib: libssw_check()
+    # if False: libssw_check()
+
+    # parameter preset 
+    if sum([int(x == True) for x in [args.qv10, args.qv15, args.qv20, args.qv25]]) > 1:
+        logger.error("Parameter preset (qv10, qv15, qv20, qv25) should be set only once")
+        sys.exit(1)
+
+    if args.qv10:
+        args.validation_score_ratio_thres = 1.2
+    elif args.qv15:
+        args.validation_score_ratio_thres = 1.4
+    elif args.qv20: 
+        args.validation_score_ratio_thres = 1.6
+    elif args.qv25:
+        args.validation_score_ratio_thres = 1.8
+
+    # check existences
+    is_exists_bam(args.tumor_bam)
+    is_exists(args.reference_fasta)
+    if args.control_bam is not None: is_exists_bam(args.control_bam)
+
+    # BAM format check
+    bam_cram_format_check(args.tumor_bam, args.reference_fasta)
+    fasta_format_check(args.reference_fasta)
+    if args.control_bam is not None: bam_cram_format_check(args.control_bam, args.reference_fasta)
 
     
     logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments")
     count_sread_by_alignment(args.sv_list_file, args.tumor_bam,
         args.output + ".realignment.tumor.sread_count.txt", args.output + ".realignment.tumor.sread_info.txt",
-        args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
+        args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = False, 
         sort_option = args.sort_option, debug = args.debug)
 
     if args.control_bam is not None:
         logger.info("Counting the number of supporting read for the control by realignment of SV candidate segments")
         count_sread_by_alignment(args.sv_list_file, args.control_bam,
             args.output + ".realignment.control.sread_count.txt", args.output + ".realignment.control.sread_info.txt",
-            args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
+            args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = False, 
             sort_option = args.sort_option, debug = args.debug)
 
     logger.info("Final processing")
     control_sread_count_file = args.output + ".realignment.control.sread_count.txt" if args.control_bam is not None else None
     integrate_realignment_result(args.output + ".realignment.tumor.sread_count.txt", control_sread_count_file, args.output,
-        args.reference_fasta, 0, 0, float("inf"), float("inf"))
+        args.reference_fasta, min_indel_size = 0, min_tumor_variant_read_num = 0, min_tumor_VAF = 0,
+        max_control_variant_read_num = float("inf"), max_control_VAF = float("inf"))
 
     if not args.debug:
         os.remove(args.output + ".realignment.tumor.sread_count.txt")
         os.remove(args.output + ".realignment.tumor.sread_info.txt")
         os.remove(args.output + ".realignment.control.sread_count.txt")
         os.remove(args.output + ".realignment.control.sread_info.txt")
     ####################
-    """
-    long_read_validate_main(args.sv_list_file,
-                            args.tumor_bam,
-                            args.output + ".validated.txt",
-                            args.output + ".validated.tumor_sread.txt",
-                            args.reference_fasta,
-                            args.control_bam, 
-                            args.var_read_min_mapq,
-                            args.use_ssw_lib, args.debug)
-
-    is_control = True if args.control_bam is not None else False
-
-    filt_final(args.output + ".validated.txt",
-               args.output + ".validated.tumor_sread.txt",
-               args.output, 
-               args.output + ".supporting_read.txt",
-               0, 0, float("inf"), float("inf"), True, is_control)
-
-    if not args.debug:
-        subprocess.check_call(["rm", "-rf", args.output + ".validated.txt"])
-        subprocess.check_call(["rm", "-rf", args.output + ".validated.tumor_sread.txt"])
-    """
     
 
 def insert_classify_main(args):
 
     import tempfile
     import annot_utils.exon
```

### Comparing `nanomonsv-0.6.0/nanomonsv/smith_waterman.py` & `nanomonsv-0.7.0/nanomonsv/smith_waterman.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/ssw_lib.py` & `nanomonsv-0.7.0/nanomonsv/ssw_lib.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/swalign.py` & `nanomonsv-0.7.0/nanomonsv/swalign.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv/vcf_convert.py` & `nanomonsv-0.7.0/nanomonsv/vcf_convert.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.6.0/nanomonsv.egg-info/PKG-INFO` & `nanomonsv-0.7.0/nanomonsv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following paper. **When you use nanomonsv or any resource of this repository, please kindly site this paper**.
 
-Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
+Precise characterization of somatic complex structural variations from tumor/control paired long-read sequencing data with nanomonsv, Shiraishi et al., Nucleic Acids Research, 2023, [[link]](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946).
 
 The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
 
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
```

### Comparing `nanomonsv-0.6.0/nanomonsv.egg-info/SOURCES.txt` & `nanomonsv-0.7.0/nanomonsv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 nanomonsv/arg_parser.py
 nanomonsv/cluster.py
 nanomonsv/cluster_sbnd.py
 nanomonsv/count_sread_by_alignment.py
 nanomonsv/filt.py
 nanomonsv/gather_support_read_seq.py
 nanomonsv/generate_consensus.py
-nanomonsv/identify.py
 nanomonsv/insert_classify.py
 nanomonsv/locate_bp.py
 nanomonsv/locate_bp_sbnd.py
 nanomonsv/logger.py
 nanomonsv/long_read_validate.py
 nanomonsv/merge_control.py
 nanomonsv/my_seq.py
```

### Comparing `nanomonsv-0.6.0/setup.py` & `nanomonsv-0.7.0/setup.py`

 * *Files identical despite different names*

