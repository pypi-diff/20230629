# Comparing `tmp/receptor_digger-0.5.0.tar.gz` & `tmp/receptor_digger-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_digger-0.5.0.tar", last modified: Thu Apr  6 16:35:57 2023, max compression
+gzip compressed data, was "receptor_digger-0.5.3.tar", last modified: Thu Jun 29 10:13:20 2023, max compression
```

## Comparing `receptor_digger-0.5.0.tar` & `receptor_digger-0.5.3.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.483522 receptor_digger-0.5.0/
--rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0      804 2023-04-06 16:35:57.484521 receptor_digger-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-06 16:34:18.000000 receptor_digger-0.5.0/README.md
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0     1176 2023-04-06 16:35:57.487521 receptor_digger-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.111522 receptor_digger-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.271521 receptor_digger-0.5.0/src/digger/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.0/src/digger/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.0/src/digger/blastresults_to_csv.py
--rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.0/src/digger/calc_motifs.py
--rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/cirelli_contig_matches.py
--rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/cirelli_to_fasta.py
--rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.0/src/digger/compare_annotations.py
--rw-rw-rw-   0        0        0     8440 2023-03-28 08:13:03.000000 receptor_digger-0.5.0/src/digger/digger.py
--rw-rw-rw-   0        0        0    47492 2023-04-05 17:05:33.000000 receptor_digger-0.5.0/src/digger/find_alignments.py
--rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.0/src/digger/motif.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.110522 receptor_digger-0.5.0/src/digger/motifs/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.109521 receptor_digger-0.5.0/src/digger/motifs/human/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.307520 receptor_digger-0.5.0/src/digger/motifs/human/IGH/
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.335521 receptor_digger-0.5.0/src/digger/motifs/human/IGK/
--rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
--rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGK/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.357523 receptor_digger-0.5.0/src/digger/motifs/human/IGL/
--rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.0/src/digger/motifs/human/IGL/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.111522 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.383520 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.426521 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
--rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/features.csv
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.465521 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/features.csv
--rw-rw-rw-   0        0        0    14499 2023-04-01 08:42:36.000000 receptor_digger-0.5.0/src/digger/parse_imgt_annotations.py
--rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.0/src/digger/slugify.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:35:57.481521 receptor_digger-0.5.0/src/receptor_digger.egg-info/
--rw-rw-rw-   0        0        0      804 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3906 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      298 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 16:35:57.000000 receptor_digger-0.5.0/src/receptor_digger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.085569 receptor_digger-0.5.3/
+-rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1121 2023-06-29 10:13:20.086568 receptor_digger-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-06-29 10:12:31.000000 receptor_digger-0.5.3/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1218 2023-06-29 10:13:20.087568 receptor_digger-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.850944 receptor_digger-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.986403 receptor_digger-0.5.3/src/digger/
+-rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.3/src/digger/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.3/src/digger/blastresults_to_csv.py
+-rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.3/src/digger/calc_motifs.py
+-rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/cirelli_contig_matches.py
+-rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/cirelli_to_fasta.py
+-rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.3/src/digger/compare_annotations.py
+-rw-rw-rw-   0        0        0     9824 2023-06-27 10:55:29.000000 receptor_digger-0.5.3/src/digger/dig_sequence.py
+-rw-rw-rw-   0        0        0    14103 2023-06-28 10:25:18.000000 receptor_digger-0.5.3/src/digger/dig_utils.py
+-rw-rw-rw-   0        0        0     8440 2023-03-28 08:13:03.000000 receptor_digger-0.5.3/src/digger/digger.py
+-rw-rw-rw-   0        0        0    18523 2023-06-29 09:28:28.000000 receptor_digger-0.5.3/src/digger/find_alignments.py
+-rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.3/src/digger/motif.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.848944 receptor_digger-0.5.3/src/digger/motifs/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.848944 receptor_digger-0.5.3/src/digger/motifs/human/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.001404 receptor_digger-0.5.3/src/digger/motifs/human/IGH/
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.013403 receptor_digger-0.5.3/src/digger/motifs/human/IGK/
+-rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
+-rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGK/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.023444 receptor_digger-0.5.3/src/digger/motifs/human/IGL/
+-rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.3/src/digger/motifs/human/IGL/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:19.850944 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.039562 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.057825 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
+-rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/features.csv
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.074825 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/features.csv
+-rw-rw-rw-   0        0        0    40658 2023-06-28 10:49:28.000000 receptor_digger-0.5.3/src/digger/parse_genes.py
+-rw-rw-rw-   0        0        0    14499 2023-04-01 08:42:36.000000 receptor_digger-0.5.3/src/digger/parse_imgt_annotations.py
+-rw-rw-rw-   0        0        0    12271 2023-06-27 11:37:05.000000 receptor_digger-0.5.3/src/digger/search_motifs.py
+-rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.3/src/digger/slugify.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:13:20.084569 receptor_digger-0.5.3/src/receptor_digger.egg-info/
+-rw-rw-rw-   0        0        0     1121 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4011 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 10:13:19.000000 receptor_digger-0.5.3/src/receptor_digger.egg-info/top_level.txt
```

### Comparing `receptor_digger-0.5.0/MANIFEST.in` & `receptor_digger-0.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/setup.cfg` & `receptor_digger-0.5.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 6469 6767   = receptor_digg
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 302e  er..version = 0.
-00000030: 352e 300d 0a61 7574 686f 7220 3d20 5769  5.0..author = Wi
+00000030: 352e 330d 0a61 7574 686f 7220 3d20 5769  5.3..author = Wi
 00000040: 6c6c 6961 6d20 4c65 6573 0d0a 6175 7468  lliam Lees..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696c 6c69  or_email = willi
 00000060: 616d 406c 6565 732e 6f72 672e 756b 0d0a  am@lees.org.uk..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 546f  description = To
 00000080: 6f6c 7320 666f 7220 6465 206e 6f76 6f20  ols for de novo 
 00000090: 6469 7363 6f76 6572 7920 6f66 2067 656e  discovery of gen
 000000a0: 6f6d 6963 2067 6572 6d6c 696e 6520 4947  omic germline IG
@@ -64,11 +64,14 @@
 000003f0: 6669 6e64 5f61 6c69 676e 6d65 6e74 733a  find_alignments:
 00000400: 6d61 696e 0d0a 0970 6172 7365 5f69 6d67  main...parse_img
 00000410: 745f 616e 6e6f 7461 7469 6f6e 7320 3d20  t_annotations = 
 00000420: 6469 6767 6572 2e70 6172 7365 5f69 6d67  digger.parse_img
 00000430: 745f 616e 6e6f 7461 7469 6f6e 733a 6d61  t_annotations:ma
 00000440: 696e 0d0a 0963 616c 635f 6d6f 7469 6673  in...calc_motifs
 00000450: 203d 2064 6967 6765 722e 6361 6c63 5f6d   = digger.calc_m
-00000460: 6f74 6966 733a 6d61 696e 0d0a 0d0a 5b65  otifs:main....[e
-00000470: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000480: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000490: 203d 2030 0d0a 0d0a                       = 0....
+00000460: 6f74 6966 733a 6d61 696e 0d0a 0964 6967  otifs:main...dig
+00000470: 5f73 6571 7565 6e63 6520 3d20 6469 6767  _sequence = digg
+00000480: 6572 2e64 6967 5f73 6571 7565 6e63 653a  er.dig_sequence:
+00000490: 6d61 696e 0d0a 0d0a 5b65 6767 5f69 6e66  main....[egg_inf
+000004a0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+000004b0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004c0: 0d0a                                     ..
```

### Comparing `receptor_digger-0.5.0/src/digger/blastresults_to_csv.py` & `receptor_digger-0.5.3/src/digger/blastresults_to_csv.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/calc_motifs.py` & `receptor_digger-0.5.3/src/digger/calc_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/cirelli_contig_matches.py` & `receptor_digger-0.5.3/src/digger/cirelli_contig_matches.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/compare_annotations.py` & `receptor_digger-0.5.3/src/digger/compare_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/digger.py` & `receptor_digger-0.5.3/src/digger/digger.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/find_alignments.py` & `receptor_digger-0.5.3/src/digger/parse_genes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,75 @@
-from operator import attrgetter, itemgetter
-
-from Bio import pairwise2
-import csv
 from collections import defaultdict
-from importlib.resources import files
-
-from receptor_utils.number_ighv import number_ighv, gap_nt_from_aa, nt_diff, gap_sequence
 from math import ceil
-import glob
-import os.path
-import argparse
+from operator import attrgetter
+
+from Bio import pairwise2
 from receptor_utils import simple_bio_seq as simple
+from receptor_utils.number_ighv import gap_sequence, number_ighv, gap_nt_from_aa
+
 try:
     from motif import Motif
+    from search_motifs import find_compound_motif, MotifResult, SingleMotifResult
 except:
     from digger.motif import Motif
-
-try:
-    from slugify import slugify
-except:
-    from digger.slugify import slugify
-
-
-def get_parser():
-    parser = argparse.ArgumentParser(description='Find valid genes in a contig given blast matches')
-    parser.add_argument('germline_file', help='reference set used to produce the blast matches')
-    parser.add_argument('assembly_file', help='assembly or contig provided to blast')
-    parser.add_argument('blast_file', help='results from blast in the format provided by blastresults_to_csv (can contain wildcards if there are multiple files, will be matched by glob)')
-    parser.add_argument('-species', help='use motifs for the specified species provided with the package')
-    parser.add_argument('-motif_dir', help='use motif probability files present in the specified directory')
-    parser.add_argument('-ref', help='ungapped reference to compare to: name and reference file separated by comma eg mouse,mouse.fasta (may be repeated multiple times)', action='append')
-    parser.add_argument('-align', help='gapped reference file to use for V gene alignments (should contain V genes only), otherwise de novo alignment will be attempted')
-    parser.add_argument('-locus', help='locus (default is IGH)')
-    parser.add_argument('-sense', help='sense in which to read the assembly (forward or reverse) (will select automatically)')
-    parser.add_argument('-debug', help='produce parsing_errors file with debug information', action='store_true')
-    parser.add_argument('output_file', help='output file (csv)')
-    return parser
-
-# global variables initialised in main()
-
-args = None
-germlines = None
-locus = None
-manual_sense = None
-J_TRP_MOTIF = None
-J_TRP_OFFSET = None
-J_SPLICE = None
-V_RSS_SPACING = None
-reference_sets = []
-v_gapped_ref = {}
-v_ungapped_ref = {}
-assembly = ''
-assembly_rc = ''
-assembly_length = 0
-motifs = {}
-conserved_motif_seqs = {}
-
-
-def find_all_matches(seq, pattern, thresh=0.7):
-    dists = []
-    pattern_length = len(pattern)
-
-    significant_bps = len([x for x in pattern if x != 'X'])
-    min_result = ceil((1.0-thresh) * significant_bps)
-
-    for i in range(len(seq) - len(pattern)):
-        d = nt_diff(seq[i:i+pattern_length], pattern)
-        if d <= min_result:
-            dists.append((i, d))
-
-    return dists
+    from digger.search_motifs import find_compound_motif, MotifResult, SingleMotifResult
 
 
 class DAnnotation:
-    def __init__(self, start, end, left_motif, right_motif):
+    """
+    Represents an annotation for a D-segment.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param start: The starting position of the D-segment.
+    :type start: int
+    :param end: The ending position of the D-segment.
+    :type end: int
+    :param left_motif: The left motif information.
+    :type left_motif: MotifResult
+    :param right_motif: The right motif information.
+    :type right_motif: MotifResult
+
+    :ivar start: The starting position of the D-segment.
+    :vartype start: int
+    :ivar end: The ending position of the D-segment.
+    :vartype end: int
+    :ivar seq: The sequence of the D-segment.
+    :vartype seq: str
+    :ivar notes: List of notes related to the D-segment.
+    :vartype notes: list
+    :ivar functionality: The functionality of the D-segment.
+    :vartype functionality: str
+    :ivar d_5_nonamer: The 5' nonamer sequence of the D-segment.
+    :vartype d_5_nonamer: str
+    :ivar d_5_heptamer: The 5' heptamer sequence of the D-segment.
+    :vartype d_5_heptamer: str
+    :ivar d_3_nonamer: The 3' nonamer sequence of the D-segment.
+    :vartype d_3_nonamer: str
+    :ivar d_3_heptamer: The 3' heptamer sequence of the D-segment.
+    :vartype d_3_heptamer: str
+    :ivar d_5_rss_start: The starting position of the 5' RSS of the D-segment.
+    :vartype d_5_rss_start: int
+    :ivar d_5_rss_end: The ending position of the 5' RSS of the D-segment.
+    :vartype d_5_rss_end: int
+    :ivar d_3_rss_start: The starting position of the 3' RSS of the D-segment.
+    :vartype d_3_rss_start: int
+    :ivar d_3_rss_end: The ending position of the 3' RSS of the D-segment.
+    :vartype d_3_rss_end: int
+    :ivar likelihood: The likelihood of the D-segment.
+    :vartype likelihood: float
+
+    :method annotate: Annotate the D-segment by determining its functionality.
+
+    .. note::
+        The class represents an annotation for a D-segment in the assembly sequence.
+        It provides information about the D-segment's start and end positions, sequence,
+        notes, functionality, motif sequences, RSS positions, and likelihood.
+    """
+    def __init__(self, assembly, start, end, left_motif, right_motif):
         self.start = start
         self.end = end
         self.seq = assembly[start-1:end]
         self.notes = []
         left_motif.notes = [f"5' {n}" for n in left_motif.notes]
         right_motif.notes = [f"3' {n}" for n in right_motif.notes]
         self.notes.extend(left_motif.notes)
@@ -90,47 +82,86 @@
         self.d_5_rss_start = left_motif.start
         self.d_5_rss_end = left_motif.end
         self.d_3_rss_start = right_motif.start
         self.d_3_rss_end = right_motif.end
         self.likelihood = left_motif.likelihood * right_motif.likelihood
 
     def annotate(self):
+        """
+        Annotate the D-segment by determining its functionality.
+
+        :return: None
+        """
         self.functionality = 'Functional'
         for note in self.notes:
             note = note.lower()
             if 'not found' in note or 'conserved' in note:
                 self.functionality = 'ORF'
                 break
 
 
-def process_d(start, end, best, matches):
+def process_d(assembly, assembly_rc, germlines, conserved_motif_seqs, motifs, start, end, best, matches):
+    """
+    Process D-segment annotations.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param assembly_rc: The reverse complement of the assembly sequence.
+    :type assembly_rc: str
+    :param germlines: Dictionary containing the germline sequences.
+    :type germlines: dict
+    :param conserved_motif_seqs: Dictionary containing conserved motif sequences.
+    :type conserved_motif_seqs: dict
+    :param motifs: Dictionary containing motifs.
+    :type motifs: dict
+    :param start: The starting position of the D-segment search.
+    :type start: int
+    :param end: The ending position of the D-segment search.
+    :type end: int
+    :param best: The best match information.
+    :type best: dict
+    :param matches: List of matches.
+    :type matches: list
+
+    :return: List of processed D-segment annotations.
+    :rtype: list of dict
+
+    .. note::
+        The function processes D-segment annotations based on the provided parameters.
+        It returns a list of dictionaries representing the processed D-segment annotations.
+
+    .. seealso::
+        - `find_compound_motif`: Function for finding compound motifs.
+        - `calc_best_match_score`: Function for calculating the best match score.
+        - `check_seq`: Function for checking a sequence.
+   """
     #if start == 1678577:
     #   breakpoint()
 
-    left_rss = find_compound_motif("5'D-NONAMER", "5'D-HEPTAMER", 12, 12, 15, end=start-1)
-    right_rss = find_compound_motif("3'D-HEPTAMER", "3'D-NONAMER", 12, 12, 15, start=end)
+    left_rss = find_compound_motif(assembly, conserved_motif_seqs, motifs["5'D-NONAMER"], motifs["5'D-HEPTAMER"], 12, 12, 15, end=start-1)
+    right_rss = find_compound_motif(assembly, conserved_motif_seqs, motifs["3'D-HEPTAMER"], motifs["3'D-NONAMER"], 12, 12, 15, start=end)
 
     results = []
 
     for left in left_rss:
         for right in right_rss:
-            annot = DAnnotation(left.end + 1, right.start - 1, left, right)
+            annot = DAnnotation(assembly, left.end + 1, right.start - 1, left, right)
             if annot.likelihood:
                 results.append(annot)    # explicitly don't add Ds with missing RSS components, there are too many
 
     rows = []
     for result in results:
         result.annotate()
-        best_match, best_score, best_nt_diffs = calc_best_match_score(best, result.seq)
+        best_match, best_score, best_nt_diffs = calc_best_match_score(germlines, best, result.seq)
 
         row = {
             'start': result.start,
             'end': result.end,
-            'end_rev': assembly_length - result.start + 1,
-            'start_rev': assembly_length - result.end + 1,
+            'end_rev': len(assembly) - result.start + 1,
+            'start_rev': len(assembly) - result.end + 1,
             'evalue': best['evalue'],
             'matches': len(matches),
             'blast_match': best_match,
             'blast_score': best_score,
             'blast_nt_diffs': best_nt_diffs,
             'functional': result.functionality,
             'notes': ', '.join(result.notes),
@@ -140,116 +171,240 @@
             'd_5_heptamer': result.d_5_heptamer,
             'd_5_nonamer': result.d_5_nonamer,
             'likelihood': result.likelihood,
         }
 
         row['3_rss_start'] = result.d_3_rss_start
         row['3_rss_end'] = result.d_3_rss_end
-        row['3_rss_start_rev'], row['3_rss_end_rev'] = assembly_length - row['3_rss_end'] + 1, assembly_length - row['3_rss_start'] + 1
+        row['3_rss_start_rev'], row['3_rss_end_rev'] = len(assembly) - row['3_rss_end'] + 1, len(assembly) - row['3_rss_start'] + 1
 
         row['5_rss_start'] = result.d_5_rss_start
         row['5_rss_end'] = result.d_5_rss_end
-        row['5_rss_start_rev'], row['5_rss_end_rev'] = assembly_length - row['5_rss_end'] + 1, assembly_length - row['5_rss_start'] + 1
+        row['5_rss_start_rev'], row['5_rss_end_rev'] = len(assembly) - row['5_rss_end'] + 1, len(assembly) - row['5_rss_start'] + 1
 
+        add_gene_coords(row, assembly)
         rows.append(row)
 
     for row in rows:
-        check_seq(row['seq'], row['start'], row['end'], False)
-        check_seq(row['seq'], row['start_rev'], row['end_rev'], True)
-        check_seq(row['d_5_nonamer'], row['5_rss_start'], row['5_rss_start'] + 8, False)
-        check_seq(row['d_5_heptamer'], row['5_rss_end'] - 6, row['5_rss_end'], False)
-        check_seq(assembly[row['5_rss_start'] - 1:row['5_rss_end']], row['5_rss_start_rev'], row['5_rss_end_rev'], True)
-        check_seq(row['d_3_heptamer'], row['3_rss_start'], row['3_rss_start'] + 6, False)
-        check_seq(row['d_3_nonamer'], row['3_rss_end'], row['3_rss_end'] - 8, False)
-        check_seq(assembly[row['3_rss_start'] - 1:row['3_rss_end']], row['3_rss_start_rev'], row['3_rss_end_rev'], True)
+        check_seq(assembly, assembly_rc, row['seq'], row['start'], row['end'], False)
+        check_seq(assembly, assembly_rc, row['seq'], row['start_rev'], row['end_rev'], True)
+        check_seq(assembly, assembly_rc, row['d_5_nonamer'], row['5_rss_start'], row['5_rss_start'] + 8, False)
+        check_seq(assembly, assembly_rc, row['d_5_heptamer'], row['5_rss_end'] - 6, row['5_rss_end'], False)
+        check_seq(assembly, assembly_rc, assembly[row['5_rss_start'] - 1:row['5_rss_end']], row['5_rss_start_rev'], row['5_rss_end_rev'], True)
+        check_seq(assembly, assembly_rc, row['d_3_heptamer'], row['3_rss_start'], row['3_rss_start'] + 6, False)
+        check_seq(assembly, assembly_rc, row['d_3_nonamer'], row['3_rss_end'], row['3_rss_end'] - 8, False)
+        check_seq(assembly, assembly_rc, assembly[row['3_rss_start'] - 1:row['3_rss_end']], row['3_rss_start_rev'], row['3_rss_end_rev'], True)
 
     return rows
 
 class CAnnotation:
-    def __init__(self, start, end):
+    """
+    Represents an annotation for a C-segment.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param start: The starting position of the C-segment.
+    :type start: int
+    :param end: The ending position of the C-segment.
+    :type end: int
+
+    :ivar start: The starting position of the C-segment.
+    :vartype start: int
+    :ivar end: The ending position of the C-segment.
+    :vartype end: int
+    :ivar seq: The sequence of the C-segment.
+    :vartype seq: str
+    :ivar notes: List of notes related to the C-segment.
+    :vartype notes: list
+    :ivar functionality: The functionality of the C-segment.
+    :vartype functionality: str
+
+    :method annotate: Annotate the C-segment by determining its functionality.
+
+    .. note::
+        The class represents an annotation for a C-segment in the assembly sequence.
+        It provides information about the C-segment's start and end positions, sequence,
+        notes, and functionality.
+    """
+    def __init__(self, assembly, start, end):
         self.start = start
         self.end = end
         self.seq = assembly[start-1:end]
         self.notes = []
         self.functionality = None
 
+    """
+    Annotate the C-segment by determining its functionality.
+
+    :return: None
+    """
     def annotate(self):
         self.functionality = 'Functional'
         self.notes = []
 
 
-def process_c(start, end, best, matches):
+def process_c(assembly, assembly_rc, germlines, start, end, best, matches):
+    """
+    Process C-segment annotations.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param assembly_rc: The reverse complement of the assembly sequence.
+    :type assembly_rc: str
+    :param germlines: The germline sequences.
+    :type germlines: dict
+    :param start: The starting position of the C-segment.
+    :type start: int
+    :param end: The ending position of the C-segment.
+    :type end: int
+    :param best: The best match information.
+    :type best: dict
+    :param matches: List of matches.
+    :type matches: list
+
+    :return: List of processed C-segment annotations.
+    :rtype: list of dict
+
+    .. note::
+        The function processes C-segment annotations based on the provided parameters.
+        It returns a list of dictionaries representing the processed C-segment annotations.
+
+    .. seealso::
+        - `calc_best_match_score`: Function for calculating the best match score.
+        - `check_seq`: Function for checking a sequence.
+    """
     # find optimal starting point for ungapped alignment
 
     best_match = -1
     best_match_score = 999
     for i in range(start - (int(best['s start'])) - 10, start - (int(best['s start'])) + 10):
         score = simple.nt_diff(assembly[i - 1:i + len(germlines[best['subject']]) - 1], germlines[best['subject']])
         if score < best_match_score:
             best_match_score = score
             best_match = i
 
     result_start = best_match
     result_end = best_match + len(germlines[best['subject']]) - 1
     result_seq = assembly[best_match - 1:best_match + len(germlines[best['subject']]) - 1]
 
-    best_match, best_score, best_nt_diffs = calc_best_match_score(best, result_seq)
+    best_match, best_score, best_nt_diffs = calc_best_match_score(germlines, best, result_seq)
 
     if best_score < 0.1: # just too many Ns
         return []
 
     row = {
         'start': result_start,
         'end': result_end,
-        'end_rev': assembly_length - result_start + 1,
-        'start_rev': assembly_length - result_end + 1,
+        'end_rev': len(assembly) - result_start + 1,
+        'start_rev': len(assembly) - result_end + 1,
         'matches': len(matches),
         'blast_match': best_match,
         'blast_score': best_score,
         'blast_nt_diffs': best_nt_diffs,
         'functional': 'Functional',
         'notes': '',
         'seq': result_seq,
     }
 
+    add_gene_coords(row, assembly)
 
-    check_seq(row['seq'], row['start'], row['end'], False)
-    check_seq(row['seq'], row['start_rev'], row['end_rev'], True)
+    check_seq(assembly, assembly_rc, row['seq'], row['start'], row['end'], False)
+    check_seq(assembly, assembly_rc, row['seq'], row['start_rev'], row['end_rev'], True)
 
     return[row]
 
 class JAnnotation:
-    def __init__(self, start, end, motif):
+    """
+    Represents an annotation for a J-segment.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param start: The starting position of the J-segment.
+    :type start: int
+    :param end: The ending position of the J-segment.
+    :type end: int
+    :param motif: The motif representing the J-segment.
+    :type motif: MotifResult
+
+    :ivar start: The starting position of the J-segment.
+    :vartype start: int
+    :ivar end: The ending position of the J-segment.
+    :vartype end: int
+    :ivar aa: The translated amino acid sequence of the J-segment.
+    :vartype aa: str
+    :ivar seq: The sequence of the J-segment.
+    :vartype seq: str
+    :ivar assembly: The assembly sequence.
+    :vartype assembly: str
+    :ivar notes: List of notes related to the J-segment.
+    :vartype notes: list
+    :ivar functionality: The functionality of the J-segment.
+    :vartype functionality: str
+    :ivar j_frame: The reading frame of the J-segment.
+    :vartype j_frame: int
+    :ivar nonamer: The nonamer sequence of the J-segment.
+    :vartype nonamer: str
+    :ivar heptamer: The heptamer sequence of the J-segment.
+    :vartype heptamer: str
+    :ivar rss_start: The start position of the RSS associated with the J-segment.
+    :vartype rss_start: int
+    :ivar rss_end: The end position of the RSS associated with the J-segment.
+    :vartype rss_end: int
+    :ivar likelihood: The likelihood of the J-segment.
+    :vartype likelihood: float
+
+    :method annotate: Annotate the J-segment by determining its functionality.
+
+    .. note::
+        The class represents an annotation for a J-segment in the assembly sequence.
+        It provides information about the J-segment's start and end positions, amino acid
+        sequence, sequence, assembly sequence, notes, functionality, reading frame, nonamer,
+        heptamer, RSS positions, and likelihood.
+    """
+    def __init__(self, assembly, start, end, motif):
         self.start = start
         self.end = end
         self.aa = ''
         self.seq = assembly[start-1:end]
+        self.assembly = assembly
         self.notes = motif.notes
         self.functionality = None
         self.j_frame = None
         self.nonamer = motif.left
         self.heptamer = motif.right
         self.rss_start = motif.start
         self.rss_end = motif.end
         self.likelihood = motif.likelihood
 
-    def annotate(self):
+    def annotate(self, J_TRP_MOTIF, J_TRP_OFFSET, J_SPLICE):
+        """
+        Annotate the J-segment by determining its functionality.
+
+        :param J_TRP_MOTIF: The J-TRP motif to search for.
+        :type J_TRP_MOTIF: str
+        :param J_TRP_OFFSET: The offset for the J-TRP motif.
+        :type J_TRP_OFFSET: int
+        :param J_SPLICE: The J-splice sequence to search for.
+        :type J_SPLICE: str
+
+        :return: None
+        """
         # consider each frame
         hit = 0
         for i in range(0, 3):
             j_codons = self.seq[i:]
             self.aa = simple.translate(j_codons)
             hit = find_best_match(self.aa, J_TRP_MOTIF, thresh=1.0)
             if hit >= 0:
                 break
 
         if hit >= 0:
             self.end = self.start + i + (hit + J_TRP_OFFSET)*3      # include the donor splice
-            self.seq = assembly[self.start - 1:self.end]
-            if assembly[self.end - 1:self.end + 2] != J_SPLICE:
+            self.seq = self.assembly[self.start - 1:self.end]
+            if self.assembly[self.end - 1:self.end + 2] != J_SPLICE:
                 self.notes.append('Donor splice not found')
                 self.j_frame = 0
                 self.functionality = 'pseudo'
             else:
                 self.j_frame = i
                 self.functionality = 'Functional'
                 for note in self.notes:
@@ -257,37 +412,72 @@
                         self.functionality = 'ORF'
                         break
         else:
             self.notes.append('J-TRP not found')
             self.j_frame = 0
             self.functionality = 'pseudo'
 
-def process_j(start, end, best, matches):
-    j_rss = find_compound_motif('J-NONAMER', 'J-HEPTAMER', 22, 23, 15, end=start-1)
+def process_j(assembly, assembly_rc, germlines, conserved_motif_seqs, motifs, start, end, best, matches, J_TRP_MOTIF, J_TRP_OFFSET, J_SPLICE, J_RSS_SPACING):
+    """
+    Process J-segment annotations.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param assembly_rc: The reverse complement of the assembly sequence.
+    :type assembly_rc: str
+    :param germlines: The germline sequences.
+    :type germlines: dict
+    :param conserved_motif_seqs: Dictionary containing conserved motif sequences.
+    :type conserved_motif_seqs: dict
+    :param motifs: Dictionary containing motifs.
+    :type motifs: dict
+    :param start: The starting position of the J-segment search.
+    :type start: int
+    :param end: The ending position of the J-segment search.
+    :type end: int
+    :param best: The best match information.
+    :type best: dict
+    :param matches: List of matches.
+    :type matches: list
+
+    :return: List of processed J-segment annotations.
+    :rtype: list of dict
+
+    .. note::
+        The function processes J-segment annotations based on the provided parameters.
+        It returns a list of dictionaries representing the processed J-segment annotations.
+
+    .. seealso::
+        - `find_compound_motif`: Function for finding compound motifs.
+        - `calc_best_match_score`: Function for calculating the best match score.
+        - `check_seq`: Function for checking a sequence.
+
+    """
+    j_rss = find_compound_motif(assembly, conserved_motif_seqs, motifs['J-NONAMER'], motifs['J-HEPTAMER'], J_RSS_SPACING-1, J_RSS_SPACING, 15, end=start-1)
 
     if len(j_rss) == 0:
         return []
 
 
     # we need to make a call between the rss on the basis of likelihood
     # otherwise we'll get overlapping rss and call js that only differ in a bp or two at the 5' end
 
     j_rss.sort(key=attrgetter('likelihood'), reverse=True)
     j_rs = j_rss[0]
 
-    result = (JAnnotation(j_rs.end + 1, end, j_rs))
-    result.annotate()
+    result = (JAnnotation(assembly, j_rs.end + 1, end, j_rs))
+    result.annotate(J_TRP_MOTIF, J_TRP_OFFSET, J_SPLICE)
 
-    best_match, best_score, best_nt_diffs = calc_best_match_score(best, result.seq)
+    best_match, best_score, best_nt_diffs = calc_best_match_score(germlines, best, result.seq)
 
     row = {
         'start': result.start,
         'end': result.end,
-        'end_rev': assembly_length - result.start + 1,
-        'start_rev': assembly_length - result.end + 1,
+        'end_rev': len(assembly) - result.start + 1,
+        'start_rev': len(assembly) - result.end + 1,
         'evalue': best['evalue'],
         'matches': len(matches),
         'blast_match': best_match,
         'blast_score': best_score,
         'blast_nt_diffs': best_nt_diffs,
         'functional': result.functionality,
         'notes': ', '.join(result.notes),
@@ -297,27 +487,69 @@
         'j_frame': result.j_frame,
         'aa': result.aa,
         'likelihood': result.likelihood,
     }
 
     row['5_rss_start'] = result.rss_start
     row['5_rss_end'] = result.rss_end
-    row['5_rss_start_rev'], row['5_rss_end_rev'] = assembly_length - row['5_rss_end'] + 1, assembly_length - row['5_rss_start'] + 1
+    row['5_rss_start_rev'], row['5_rss_end_rev'] = len(assembly) - row['5_rss_end'] + 1, len(assembly) - row['5_rss_start'] + 1
+
+    add_gene_coords(row, assembly)
 
-    check_seq(row['seq'], row['start'], row['end'], False)
-    check_seq(row['seq'], row['start_rev'], row['end_rev'], True)
-    check_seq(row['j_nonamer'], row['5_rss_start'], row['5_rss_start'] + 8, False)
-    check_seq(row['j_heptamer'], row['5_rss_end'] - 6, row['5_rss_end'], False)
-    check_seq(assembly[row['5_rss_start'] - 1:row['5_rss_end']], row['5_rss_start_rev'], row['5_rss_end_rev'], True)
+    check_seq(assembly, assembly_rc, row['seq'], row['start'], row['end'], False)
+    check_seq(assembly, assembly_rc, row['seq'], row['start_rev'], row['end_rev'], True)
+    check_seq(assembly, assembly_rc, row['j_nonamer'], row['5_rss_start'], row['5_rss_start'] + 8, False)
+    check_seq(assembly, assembly_rc, row['j_heptamer'], row['5_rss_end'] - 6, row['5_rss_end'], False)
+    check_seq(assembly, assembly_rc, assembly[row['5_rss_start'] - 1:row['5_rss_end']], row['5_rss_start_rev'], row['5_rss_end_rev'], True)
 
     return [row]
 
 
 class VAnnotation:
-    def __init__(self, start, end, refs=None):
+    """
+    Represents a V-segment annotation.
+
+    :param assembly: The assembly sequence.
+    :type assembly: str
+    :param start: The starting position of the V-segment annotation (1-based coordinate).
+    :type start: int
+    :param end: The ending position of the V-segment annotation (1-based coordinate).
+    :type end: int
+    :param refs: Optional references for sequence alignment.
+    :type refs: list, optional
+
+    :ivar start: The starting position of the V-segment annotation.
+    :vartype start: int
+    :ivar end: The ending position of the V-segment annotation.
+    :vartype end: int
+    :ivar ungapped: The ungapped sequence of the V-segment annotation.
+    :vartype ungapped: str
+    :ivar gapped: The gapped sequence of the V-segment annotation.
+    :vartype gapped: str
+    :ivar gapped_aa: The gapped amino acid sequence of the V-segment annotation.
+    :vartype gapped_aa: str
+    :ivar notes: List of additional notes related to the V-segment annotation.
+    :vartype notes: list
+    :ivar functionality: The functionality of the V-segment annotation ('Functional', 'ORF', 'pseudo').
+    :vartype functionality: str
+    :ivar likelihood: The likelihood value of the V-segment annotation.
+    :vartype likelihood: None or float
+    :ivar align_refs: Indicates if references are used for sequence alignment.
+    :vartype align_refs: bool
+    :ivar v_gapped_ref: The gapped reference sequence for alignment.
+    :vartype v_gapped_ref: str or None
+    :ivar v_ungapped_ref: The ungapped reference sequence for alignment.
+    :vartype v_ungapped_ref: str or None
+
+    .. note::
+        If `refs` parameter is provided, the references for sequence alignment will be used.
+        Otherwise, the alignment process will be skipped.
+
+    """
+    def __init__(self, assembly, start, end, refs=None):
         self.start = start
         self.end = end
         self.ungapped = assembly[start-1:end]
         self.gapped = None
         self.gapped_aa = None
         self.notes = []
         self.functionality = None
@@ -326,14 +558,20 @@
             self.align_refs = True
             self.v_gapped_ref = refs[0]
             self.v_ungapped_ref = refs[1]
         else:
             self.align_refs = False
 
     def annotate(self):
+        """
+        Annotate the V-segment.
+
+        This method performs sequence alignment and annotation of the V-segment.
+        It updates the `gapped`, `gapped_aa`, `functionality`, and `notes` attributes.
+        """
         v_p = simple.translate(self.ungapped)
 
         if self.align_refs:
             self.gapped, self.gapped_aa, errors = gap_sequence(self.ungapped, self.v_gapped_ref, self.v_ungapped_ref)
         else:
             self.gapped_aa, errors = number_ighv(str(v_p))
             if self.gapped_aa is not None and len(self.gapped_aa) > 0:
@@ -350,73 +588,135 @@
             self.functionality = 'Functional'
 
 
 # assembly is now forward-sense
 # want to find all possible leaders within a range, with their probs
 # then find all possible rss within range
 # evaluate every combination - joint prob and functionality
-def process_v(start, end, best, matches, v_parsing_errors):
-    #if start == 80078:
-    #    breakpoint()
-
-    leaders = find_compound_motif('L-PART1', 'L-PART2', 10, 600, 8, end=start-1, right_force=start-len(motifs['L-PART2'].consensus))
+def process_v(assembly, assembly_rc, germlines, v_gapped_ref, v_ungapped_ref, conserved_motif_seqs, motifs, start, end, best, matches, align, V_RSS_SPACING, v_parsing_errors):
+    """
+     Process V-segment annotations.
+
+     :param assembly: The assembly sequence.
+     :type assembly: str
+     :param assembly_rc: The reverse complement of the assembly sequence.
+     :type assembly_rc: str
+     :param germlines: The germline sequences.
+     :type germlines: dict
+     :param v_gapped_ref: The gapped reference sequence for V-segment alignment.
+     :type v_gapped_ref: str
+     :param v_ungapped_ref: The ungapped reference sequence for V-segment alignment.
+     :type v_ungapped_ref: str
+     :param conserved_motif_seqs: Dictionary containing conserved motif sequences.
+     :type conserved_motif_seqs: dict
+     :param motifs: Dictionary containing motifs.
+     :type motifs: dict
+     :param start: The starting position of the V-segment search (1-based).
+     :type start: int
+     :param end: The ending position of the V-segment search (1-based).
+     :type end: int
+     :param best: The best match information.
+     :type best: dict
+     :param matches: List of matches.
+     :type matches: list
+     :param align: Flag indicating whether sequence alignment should be performed.
+     :type align: bool
+     :param V_RSS_SPACING: The spacing between V-segment RSS motifs.
+     :type V_RSS_SPACING: int
+     :param v_parsing_errors: Dictionary for storing V-segment parsing errors.
+     :type v_parsing_errors: dict
+
+     :return: List of processed V-segment annotations.
+     :rtype: list of dict
+
+     .. note::
+         The function processes V-segment annotations based on the provided parameters.
+         It returns a list of dictionaries representing the processed V-segment annotations.
+
+     .. seealso::
+         - `find_compound_motif`: Function for finding compound motifs.
+         - `VAnnotation`: Class representing V-segment annotations.
+         - `calc_best_match_score`: Function for calculating the best match score.
+         - `check_seq`: Function for checking a sequence.
+   """
+    leaders = find_compound_motif(assembly, conserved_motif_seqs, motifs['L-PART1'], motifs['L-PART2'], 10, 800, 8, end=start-1, right_force=start-len(motifs['L-PART2'].consensus))
 
     # restrain length to between 270 and 320 nt, allow a window anywhere within that range
-    rights = find_compound_motif('V-HEPTAMER', 'V-NONAMER', V_RSS_SPACING-1, V_RSS_SPACING, 25, start=start+295)
+    rights = find_compound_motif(assembly, conserved_motif_seqs, motifs['V-HEPTAMER'], motifs['V-NONAMER'], V_RSS_SPACING-1, V_RSS_SPACING, 25, start=start+295)
 
     # put in a dummy leader if we found an RSS but no leader
 
     if rights and not leaders:
-        leaders.append(MotifResult(motifs['L-PART1'],
-                                   0,
-                                   start-len(motifs['L-PART2'].consensus)-10-len(motifs['L-PART2'].consensus),
-                                   motifs['L-PART2'],
-                                   0,
-                                   start-len(motifs['L-PART2'].consensus),
-                                   ['Leader not found']))
+        leaders.append(
+            MotifResult(assembly,
+                   SingleMotifResult(assembly, conserved_motif_seqs, motifs['L-PART1'], start-len(motifs['L-PART1'].consensus)-10-len(motifs['L-PART2'].consensus), 0),
+                   SingleMotifResult(assembly, conserved_motif_seqs, motifs['L-PART2'], start-len(motifs['L-PART2'].consensus), 0),
+                   ['Leader not found'])
+        )
+
+    # put in a dummy RSS if we found leader but no RSS
+
+    if leaders and not rights:
+        rights.append(
+            MotifResult(assembly,
+                   SingleMotifResult(assembly, conserved_motif_seqs, motifs['V-HEPTAMER'], end+1, 0),
+                   SingleMotifResult(assembly, conserved_motif_seqs, motifs['V-NONAMER'], end+V_RSS_SPACING+1, 0),
+                   ['RSS not found'])
+        )
 
     best_rights = find_best_rss(rights)
-    best_leaders = find_best_leaders(leaders)
+    best_leaders = find_best_leaders(assembly, leaders)
 
     max_likelihood_rec = None
+    max_likelihood_rec_at_start = None
     results = []
 
     # report one or more functional V-GENEs found between the identified leaders and rss.
     # if none, report the non-functional sequence with highest combined (leader, rss) likelihood
 
     if len(best_leaders) == 0:
-        v_parsing_errors[start] = ((start, end, best['subject'], 'leader not found', assembly[start-500:start]))
+        err_seq = assembly[max(start-500, 0):start]
+        v_parsing_errors[start] = ((start, end, best['subject'], 'leader not found', err_seq))
 
     if len(best_rights) == 0:
-        v_parsing_errors[start] = ((start, end, best['subject'], 'rss not found', assembly[end+1:end+24]))
+        if len(assembly) >= end+24:
+            err_seq = assembly[end+1:end+24]
+        else:
+            err_seq = assembly[end+1:]
+        v_parsing_errors[start] = ((start, end, best['subject'], 'rss not found', err_seq))
 
     # if we have multiple possible rights, discard any that are substantially weaker than the best
 
     if len(best_rights) > 1:
         best_rl = max([x.likelihood for x in best_rights.values()])
         for k in list(best_rights.keys()):
             if best_rights[k].likelihood < (best_rl / 100):
                 del best_rights[k]
 
     for left in best_leaders.values():
         #if left.end == 1114541:
         #    breakpoint()
         for right in best_rights.values():
-            if args.align:
-                v_annot = VAnnotation(left.end + 1, right.start - 1, refs=[v_gapped_ref, v_ungapped_ref])
+            if align:
+                v_annot = VAnnotation(assembly, left.end + 1, right.start - 1, refs=[v_gapped_ref, v_ungapped_ref])
             else:
-                v_annot = VAnnotation(left.end + 1, right.start - 1)
+                v_annot = VAnnotation(assembly, left.end + 1, right.start - 1)
             v_annot.annotate()
             v_annot.likelihood = left.likelihood * right.likelihood
 
             if v_annot.functionality == 'Functional':
                 results.append((left, v_annot, right))
             if max_likelihood_rec is None or v_annot.likelihood > max_likelihood_rec[1].likelihood:
                 max_likelihood_rec = (left, v_annot, right)
+            if v_annot.start == start + 1 and (max_likelihood_rec_at_start is None or v_annot.likelihood > max_likelihood_rec[1].likelihood):
+                max_likelihood_rec_at_start = (left, v_annot, right)
 
+    # If we don't have any functional results, favour the one with the suggested start position.
+    if len(results) == 0 and max_likelihood_rec_at_start is not None:
+        results = [max_likelihood_rec_at_start]
 
     if len(results) == 0 and max_likelihood_rec is not None:
         results = [max_likelihood_rec]
 
     #if len(results) == 0:
     #    breakpoint()
 
@@ -435,24 +735,24 @@
                 if 'conserved' in note or 'not found' in note:
                     v_gene.functionality = 'ORF'
             for note in leader.notes:
                 note = note.lower()
                 if 'stop codon' in note or 'atg' in note or 'donor-splice' in note or 'acceptor-splice' in note:
                     v_gene.functionality = 'pseudo'
 
-        best_match, best_score, best_nt_diffs = calc_best_match_score(best, v_gene.ungapped)
+        best_match, best_score, best_nt_diffs = calc_best_match_score(germlines, best, v_gene.ungapped)
 
         #if '1-56' in best_match:
         #    breakpoint()
 
         row = {
             'start': v_gene.start,
             'end': v_gene.end,
-            'end_rev': assembly_length - v_gene.start + 1,
-            'start_rev': assembly_length - v_gene.end + 1,
+            'end_rev': len(assembly) - v_gene.start + 1,
+            'start_rev': len(assembly) - v_gene.end + 1,
             'evalue': best['evalue'],
             'matches': len(matches),
             'blast_match': best_match,
             'blast_score': best_score,
             'blast_nt_diffs': best_nt_diffs,
             'l_part1': leader.left,
             'l_part2': leader.right,
@@ -463,48 +763,49 @@
             'v-gene_aligned_aa': v_gene.gapped_aa,
             'seq': v_gene.ungapped,
             'seq_gapped': v_gene.gapped,
             'likelihood': v_gene.likelihood,
         }
 
         row['3_rss_start'] = rss.start
-        row['3_rss_start_rev'] = assembly_length - rss.end + 1
+        row['3_rss_start_rev'] = len(assembly) - rss.end + 1
         row['3_rss_end'] = rss.end
-        row['3_rss_end_rev'] = assembly_length - rss.start + 1
+        row['3_rss_end_rev'] = len(assembly) - rss.start + 1
 
         row['l_part1_start'] = leader.start
         row['l_part1_end'] = leader.start + len(leader.left) - 1
-        row['l_part1_start_rev'], row['l_part1_end_rev'] = assembly_length - row['l_part1_end'] + 1, assembly_length - row['l_part1_start'] + 1
+        row['l_part1_start_rev'], row['l_part1_end_rev'] = len(assembly) - row['l_part1_end'] + 1, len(assembly) - row['l_part1_start'] + 1
 
         row['l_part2_start'] = leader.end - len(leader.right) + 1
         row['l_part2_end'] = leader.end
-        row['l_part2_start_rev'], row['l_part2_end_rev'] = assembly_length - row['l_part2_end'] + 1, assembly_length - row['l_part2_start'] + 1
+        row['l_part2_start_rev'], row['l_part2_end_rev'] = len(assembly) - row['l_part2_end'] + 1, len(assembly) - row['l_part2_start'] + 1
 
         row['aa'] = simple.translate(v_gene.ungapped)
 
+        add_gene_coords(row, assembly)
         rows.append(row)
 
     for row in rows:
-        check_seq(row['seq'], row['start'], row['end'], False)
-        check_seq(row['seq'], row['start_rev'], row['end_rev'], True)
-        check_seq(row['v_heptamer'], row['3_rss_start'], row['3_rss_start'] + 6, False)
-        check_seq(row['v_nonamer'], row['3_rss_end'], row['3_rss_end'] - 8, False)
-        check_seq(assembly[row['3_rss_start'] - 1:row['3_rss_end']], row['3_rss_start_rev'], row['3_rss_end_rev'], True)
-        check_seq(row['l_part1'], row['l_part1_start'], row['l_part1_end'], False)
-        check_seq(assembly[row['l_part1_start'] - 1:row['l_part1_end']], row['l_part1_start_rev'], row['l_part1_end_rev'], True)
-        check_seq(row['l_part2'], row['l_part2_start'], row['l_part2_end'], False)
-        check_seq(assembly[row['l_part2_start'] - 1:row['l_part2_end']], row['l_part2_start_rev'], row['l_part2_end_rev'], True)
+        check_seq(assembly, assembly_rc, row['seq'], row['start'], row['end'], False)
+        check_seq(assembly, assembly_rc, row['seq'], row['start_rev'], row['end_rev'], True)
+        check_seq(assembly, assembly_rc, row['v_heptamer'], row['3_rss_start'], row['3_rss_start'] + 6, False)
+        check_seq(assembly, assembly_rc, row['v_nonamer'], row['3_rss_end'], row['3_rss_end'] - 8, False)
+        check_seq(assembly, assembly_rc, assembly[row['3_rss_start'] - 1:row['3_rss_end']], row['3_rss_start_rev'], row['3_rss_end_rev'], True)
+        check_seq(assembly, assembly_rc, row['l_part1'], row['l_part1_start'], row['l_part1_end'], False)
+        check_seq(assembly, assembly_rc, assembly[row['l_part1_start'] - 1:row['l_part1_end']], row['l_part1_start_rev'], row['l_part1_end_rev'], True)
+        check_seq(assembly, assembly_rc, row['l_part2'], row['l_part2_start'], row['l_part2_end'], False)
+        check_seq(assembly, assembly_rc, assembly[row['l_part2_start'] - 1:row['l_part2_end']], row['l_part2_start_rev'], row['l_part2_end_rev'], True)
 
     return rows
 
 
 # check co-ordinates of each element for sanity
 # all co-ordinates should be 1-based!
 
-def check_seq(seq, start, end, rev):
+def check_seq(assembly, assembly_rc, seq, start, end, rev):
     if len(seq) == 0:
         return  #   allow empty sequences which may occur if the assembly is truncated
 
     if end < start:
         end, start = start, end
 
     if end >= len(assembly) or start <= 0:
@@ -515,167 +816,37 @@
         if seq != assembly[start-1:end]:
             print('Error: sequence at (%d, %d) failed co-ordinate check.' % (start, end))
     else:
         if simple.reverse_complement(seq) != assembly_rc[start-1:end]:
             print('Error: reverse sequence at (%d, %d) failed co-ordinate check.' % (start, end))
 
 
-# Look for a single motif within the specified range of start positions
-# return a list of all discovered motifs, and their likelihoods
-# min_start, max_start - 1-based co-ords of allowed start positions
-def find_single_motif(motif, min_start, max_start):
-    res = []
-    max_found = 0
-    max_hit = ''
-    # print('looking for single motif %s in %s' % (motif.consensus, assembly[min_start-1:min_start + len(motif.consensus) + (max_start-min_start)]))
-    consensus_len = len(motif.consensus)
-
-    for p in range(min_start, max_start+1):
-        seq = assembly[p-1:p-1 + consensus_len]
-        likelihood = motif.calc_likelihood(seq)
-
-        if likelihood > max_found:
-            max_found = likelihood
-
-        if likelihood >= motif.likelihood_threshold:
-            res.append(SingleMotifResult(motif, p, likelihood))
-
-    return res
-
-
-class SingleMotifResult:
-    def __init__(self, motif, position, likelihood):
-        self.start = position
-        self.name = motif.name
-        self.end = position + len(motif.consensus) - 1
-        self.seq = assembly[position - 1:position - 1 + len(motif.consensus)]
-        self.likelihood = likelihood
-        self.notes = []
-
-        if likelihood:      # don't check dummy motifs
-            self.check_motif_consensus()
-
-
-    # check residues that are strongly conserved across all loci
-    def check_motif_consensus(self):
-        cons = None
-
-        if self.name in conserved_motif_seqs:
-            cons = conserved_motif_seqs[self.name]
-
-            non_conserved = 0
-            res = ''
-            if cons:
-                for s, ref in zip(list(self.seq), list(cons)):
-                    if ref != '-' and s != ref:
-                        res += s
-                        non_conserved += 1
-                    else:
-                        res += '-'
-
-            if non_conserved:
-                self.notes.append(f'{self.name} has variation at strongly conserved residue(s): {res}')
-
-
-# Find compound motifs - ie heptamer plus nonamer, or l-part1 and l-part2.
-# left, right - the two motifs
-# min_gap, max_gap - the gap between them
-# start co-ord, end co-ord: 1-based co-ordinates of either the desired ending position of left, or starting position of right (specify ome or the other)
-# window - the function will look either for a left that ends at end +/- window, or a right that starts at start +/- window
-# returns [{start, end, left_seq, gap_seq, right_seq, likelihood}] for each left, right combination that meets the threshold criterion
-# If force has a value, always report a right starting at that position, with the best available left. This is used to force an L-PART2 to be discovered
-# at the point that the BLAST alignment indicates the v-region should start
-def find_compound_motif(left_motif_name, right_motif_name, min_gap, max_gap, window, start=None, end=None, right_force=None):
-    left_motif = motifs[left_motif_name]
-    right_motif = motifs[right_motif_name]
-    max_length = len(left_motif.consensus) + max_gap + len(right_motif.consensus)
-    min_length = len(left_motif.consensus) + min_gap + len(right_motif.consensus)
-
-    if start is None:
-        min_start = end - max_length - window
-    else:
-        min_start = start - window
-    max_start = min_start + (max_length - min_length) + 2 * window
-
-    min_end = min_start + min_length
-    max_end = max_start + max_length
-
-    if min_end > len(assembly):
-        return []
-
-    if max_end > len(assembly):
-        max_end = len(assembly)
-
-    # start by finding the motif with the highest threshold
-
-    res = []
-
-    if left_motif.likelihood_threshold > right_motif.likelihood_threshold:
-        # use the specified start position if we have one, otherwise extrapolate from the end and min/max gaps - less accurate
-        if start is not None:
-            left_results = find_single_motif(left_motif, start - window, start + window)
-        else:
-            left_results = find_single_motif(left_motif, min_start, min_start + 2*window)
-
-        right_results = []
-        for left_result in left_results:
-            right_results = find_single_motif(right_motif, left_result.start + len(left_motif.consensus) + min_gap, left_result.start + len(left_result.seq) + max_gap)
-            for right_result in right_results:
-                res.append(MotifResult(left_result, right_result))
-
-        # put in a dummy if we missed the lower likelihood motif
-        if left_results and not right_results:
-            best_left = sorted(left_results, key=attrgetter('likelihood'), reverse=True)[0]
-            res.append(MotifResult(best_left, SingleMotifResult(right_motif, best_left.start + len(best_left.seq) + min_gap, 0), notes=[f'{right_motif.name} not found']))
-    else:
-        if end is not None:
-            right_results = find_single_motif(right_motif, end - len(right_motif.consensus) - window, end + window)
-        else:
-            right_results = find_single_motif(right_motif, min_end - len(right_motif.consensus), max_end - len(right_motif.consensus))
-
-        # if right_force is set, if necessary, force discovery of a right motif at the forced position
-
-        if right_force and right_force not in [r.start for r in right_results]:
-            right_results.append(SingleMotifResult(right_motif, right_force, 0))
-
-        left_results = []
-        for right_result in right_results:
-            left_results = find_single_motif(left_motif, right_result.start - max_gap - len(left_motif.consensus), right_result.start - min_gap - len(left_motif.consensus))
-            for left_result in left_results:
-                res.append(MotifResult(left_result, right_result))
-
-        # put in a dummy if we missed the lower likelihood motif
-        if right_results and not left_results:
-            best_right = sorted(right_results, key=attrgetter('likelihood'), reverse=True)[0]
-            res.append(MotifResult(SingleMotifResult(left_motif, best_right.start - min_gap - len(left_motif.consensus), 0), best_right, notes=[f'{left_motif.name} not found']))
-
-    return res
-
-
-class MotifResult:
-    def __init__(self, left_motif, right_motif, notes=None):
-        self.start = left_motif.start
-        self.end = right_motif.start + len(right_motif.seq) - 1
-        self.left = left_motif.seq
-        self.gap = assembly[self.start + len(self.left):right_motif.start - 1]
-        self.right = right_motif.seq
-        self.likelihood = left_motif.likelihood * right_motif.likelihood
-        if notes:
-            self.notes = [n for n in notes]
-        else:
-            self.notes = []
-        self.notes.extend(left_motif.notes)
-        self.notes.extend(right_motif.notes)
-
+# Find all 'start' or 'end' coords in a record
+def find_coords(rec, keyword):
+    coords = []
+
+    for k in rec.keys():
+        if keyword in k and 'rev' not in k:
+            coords.append(int(rec[k]))
+
+    return coords
+
+
+# Add overall gene coordinates to a row
+def add_gene_coords(row, assembly):
+    row['gene_start'] = max(min(find_coords(row, 'start')), 1)
+    row['gene_end'] = min(max(find_coords(row, 'end')), len(assembly))
+    row['gene_start_rev'], row['gene_end_rev'] = len(assembly) - row['gene_end'] + 1, len(assembly) - row['gene_start'] + 1
+    row['gene_seq'] = assembly[row['gene_start'] - 1:row['gene_end']]
 
 
 # find the best leader PART1 for each PART2 starting position:
 # if PART2 is in-frame: the in-frame PART1 giving best likelihood
 # otherwise, the PART1 giving best likelihood regardless of frame
-def find_best_leaders(leaders):
+def find_best_leaders(assembly, leaders):
     def spread(n, inc=1):
         ret = []
         for i in range(0, n, inc):
             ret.append(i)
             if i != 0:
                 ret.append(0 - i)
         return ret
@@ -773,374 +944,46 @@
     for position, choice in right_choices.items():
         choice.sort(key=attrgetter('likelihood'), reverse=True)
         best_rights[position] = choice[0]
 
     return best_rights
 
 
-def calc_matched_refs(row):
-    for ref in reference_sets:
-        row[ref['name'] + '_match'] = ''
-        row[ref['name'] + '_score'] = 0
-        row[ref['name'] + '_nt_diffs'] = 999
-
-        for ref_name, ref_seq in ref['seqs'].items():
-            if row['gene_type'] in ref_name:
-                score = pairwise2.align.globalms(row['seq'], ref_seq, 1, 0, -1, -1, score_only=True)
-                if isinstance(score, float) and score > row[ref['name'] + '_score']:
-                    row[ref['name'] + '_score'] = score
-                    row[ref['name'] + '_match'] = ref_name
-
-                if 'V' in row['gene_type'] and len(row['seq']) > 290 and len(ref_seq) > 290:
-                    score = nt_diff(row['seq'][:291], ref_seq[:291])
-                else:
-                    score = nt_diff(row['seq'], ref_seq)
-                if score < row[ref['name'] + '_nt_diffs']:
-                    row[ref['name'] + '_nt_diffs'] = score
-
-        if row[ref['name'] + '_nt_diffs'] == 999:
-            row[ref['name'] + '_nt_diffs'] = 0
-
-        if row[ref['name'] + '_score'] > 0:
-            row[ref['name'] + '_score'] = round(row[ref['name'] + '_score'] * 100.0 / len(row['seq']), 2)
-
-
-def calc_best_match_score(best, seq):
+def calc_best_match_score(germlines, best, seq):
     score = pairwise2.align.globalms(seq, germlines[best['subject']], 1, 0, -1, -1, score_only=True)
     if isinstance(score, float) and score > 0:
         best_score = round(100 * score / len(seq), 2)
         best_match = best['subject']
     else:
         best_score = 0.0
         best_match = ''
 
-    best_nt_diffs = nt_diff(seq, germlines[best['subject']])
+    best_nt_diffs = simple.nt_diff(seq, germlines[best['subject']])
 
     return best_match, best_score, best_nt_diffs
 
 
-def strings_to_num(row, fields):
-    for field in fields:
-        if '.' in row[field]:
-            row[field] = float(row[field])
-        else:
-            row[field] = int(row[field])
-    return row
-
-
 def find_best_match(seq, pattern, thresh=0.7):
     dists = find_all_matches(seq, pattern, thresh)
 
     if len(dists) == 0:
         return -1
 
     scores = [d[1] for d in dists]
 
     return dists[scores.index(min(scores))][0]
 
+def find_all_matches(seq, pattern, thresh=0.7):
+    dists = []
+    pattern_length = len(pattern)
 
-def reverse_coords(row):
-    start_revs = [x for x in row.keys() if 'start_rev' in x]
-    for start_rev in start_revs:
-        end_rev = start_rev.replace('start', 'end')
-        start = start_rev.replace('_rev', '')
-        end = end_rev.replace('_rev', '')
-        row[start], row[end_rev] = row[end_rev], row[start]
-        row[end], row[start_rev] = row[start_rev], row[end]
-
-
-def process_file(this_blast_file, writer, write_parsing_errors):
-    global assembly
-    global assembly_rc
-    global J_TRP_MOTIF
-    global J_TRP_OFFSET
-    global J_SPLICE
-
-    assembly_rc = simple.reverse_complement(assembly)
-
-    with open(this_blast_file, 'r') as fi:
-        print('Processing %s' % this_blast_file)
-        this_contig_name = None
-        forward_gene_alignments = defaultdict(list)
-        reverse_gene_alignments = defaultdict(list)
-
-        reader = csv.DictReader(fi, dialect='excel')
-        for row in reader:
-            if not this_contig_name:
-                this_contig_name = row['query']
-            if row['subject'] not in germlines:
-                print('%s is not defined in %s. Please make sure the file has definitions for all sequences used by BLAST.' % (row['subject'], args.germline_file))
-                quit()
-
-            row = strings_to_num(row, ['identity', 'alignment length', 'mismatches', 'gap opens', 'q start', 'q end', 's start', 's end', 'evalue', 'bit score'])
-
-            if row['s end'] < row['s start']:
-                row['sense'] = '-'
-                row['q start'], row['q end'] = assembly_length - row['q end'] + 1, assembly_length - row['q start'] + 1
-                row['s start'], row['s end'] = row['s end'], row['s start']
-                row['q start'] -= row['s start'] - 1
-                row['q end'] = row['q start'] + len(germlines[row['subject']]) -1
-                reverse_gene_alignments[row['q end']].append(row)
-            else:
-                row['sense'] = '+'
-                row['q start'] -= row['s start'] - 1
-                row['q end'] = row['q start'] + len(germlines[row['subject']]) -1
-                forward_gene_alignments[row['q end']].append(row)
-
-        # calculate mean of the best evalue for hits at each position
-
-        def mean_score(gene_alignment):
-            total = 0.0
-            count = 0
-
-            for end, matches in gene_alignment.items():
-                scores = [match['evalue'] if abs(match['s start'] - match['s end']) > 0.9 * len(germlines[match['subject']]) else 100 for match in matches]
-                if min(scores) < 100:
-                    total += min(scores)
-                    count += 1
-
-            return count, (total / count) if count > 0 else 99
-
-        fw_count, fw_score = mean_score(forward_gene_alignments)
-        rev_count, rev_score = mean_score(reverse_gene_alignments)
-
-        print('%d forward alignments, mean evalue %0.2g' % (fw_count, fw_score))
-        print('%d reverse alignments, mean evalue %0.2g' % (rev_count, rev_score))
-
-        if manual_sense:
-            print(f"Using {manual_sense} sense by request")
-
-        co_ordinates_reversed = False
-
-        if manual_sense == 'forward' or (manual_sense is None and fw_count > rev_count):
-            gene_alignments = forward_gene_alignments
-            print('Using forward alignments')
-        else:
-            gene_alignments = reverse_gene_alignments
-            assembly = simple.reverse_complement(assembly)
-            assembly_rc = simple.reverse_complement(assembly)
-            co_ordinates_reversed = True
-            print('Using reverse alignments')
-
-        results = {}
-
-        # the best match for a location is a complete match against a reference sequence
-        # (see overlap reconciliation at the bottom of the loop)
-        # otherwise the lowest e-val for a reasonable length
-        def match_score(match):
-            if match['s end'] - match['s start'] + 1 == len(germlines[match['subject']]) and match['mismatches'] == '0':
-                return 0
-            elif match['s end'] - match['s start'] + 1 > 0.4 * len(germlines[match['subject']]):
-                return match['evalue']
-            else:
-                return 100
-
-        v_parsing_errors = {}
-
-        for end, matches in gene_alignments.items():
-            notes = []
-            scores = [match_score(match) for match in matches]
-            best = matches[scores.index(min(scores))]
-
-            # make sure we take an alignment length of 90% or more if available, otherwise flag a warning
-
-            #if min(scores) > 99:
-            #    notes.append('BLAST alignment was truncated')
-
-            if locus not in best['subject']:
-                print(f"Locus {locus} not found in allele name {best['subject']} - was it specified correctly?")
-                quit(1)
-
-            if locus + 'C' not in best['subject']:
-                gene_type = locus + best['subject'].split(locus)[1][0]
-            else:
-                gene_type = locus + 'C'
-
-            start = best['q start']
-
-            #print('processing match to %s at %d' % (best['subject'], best['q start']))
-
-            add_rows = True
-
-            if 'V' in gene_type:
-                # don't process obviously very truncated records
-                if abs(end - start) < 250:
-                    continue
-                rows = process_v(start, end, best, matches, v_parsing_errors)
-            elif 'J' in gene_type:
-                rows = process_j(start, end, best, matches)
-            elif 'D' in gene_type:
-                rows = process_d(start, end, best, matches)
-            elif 'C' in gene_type:
-                rows = process_c(start, end, best, matches)
-            else:
-                add_rows = False
-
-            if add_rows:
-                for row in rows:
-                    row['gene_type'] = gene_type
-
-                    if len(notes) > 0:
-                        if len(row['notes']) > 0:
-                            row['notes'] = ', '.join(row['notes'].split(', ') + notes)
-                        else:
-                            row['notes'] = ', '.join(notes)
-
-                    add_rec = True
-                    for k, result in list(results.items()):
-                        # if this row overlaps with one already stored in results, keep the one that is longer provided it is functional and there are no 'not found' elements
-                        if result['start'] <= row['start'] <= result['end'] or result['start'] <= row['end'] <= result['end']:
-                            # if row['likelihood'] > result['likelihood']:
-
-                            #if 'not found' in results[k]['notes'] or 'not found' in row['notes']:
-                            #    breakpoint()
-
-                            if row['functional'] == 'Functional' \
-                                    and (row['end'] - row['start'] > result['end'] - result['start'] or result['functional'] != 'Functional')\
-                                    and ('not found' in results[k]['notes'] or 'not found' not in row['notes']):
-                                del(results[k])
-                            else:
-                                add_rec = False
-                                break
-
-                    if add_rec:
-                        row['sense'] = '-' if co_ordinates_reversed else '+'
-                        if co_ordinates_reversed:
-                            reverse_coords(row)
-                        results[row['start']] = row
-
-        for row in results.values():
-            calc_matched_refs(row)
-            row['contig'] = this_contig_name
-
-        for key in sorted(results.keys()):
-            writer.writerow(results[key])
-
-        if write_parsing_errors:
-            with open(this_blast_file.replace('.', '_v_parsing_errors.'), 'w', newline='') as fo:
-                writer = csv.writer(fo)
-                for start in sorted(v_parsing_errors.keys()):
-                    writer.writerow(v_parsing_errors[start])
-
-
-def main():
-    global args, assembly, assembly_length, germlines, locus, manual_sense, J_TRP_MOTIF, J_TRP_OFFSET,  J_SPLICE, V_RSS_SPACING, reference_sets, conserved_motif_seqs
-    global v_gapped_ref
-
-    args = get_parser().parse_args()
-    assembly_file = args.assembly_file
-    blast_file = args.blast_file
-    match_file = args.output_file
-    germlines = simple.read_fasta(args.germline_file)
-    locus = args.locus if args.locus is not None else 'IGH'
-
-    if args.sense:
-        if args.sense in ['forward', 'reverse']:
-            manual_sense = args.sense
-        else:
-            print("Error - sense must be 'forward' or 'reverse'")
-            exit(0)
-
-    if locus in ['IGK']:
-        J_TRP_MOTIF = 'FGXG'
-        J_TRP_OFFSET = 10
-        J_SPLICE = 'CGT'
-    elif locus in ['IGL']:
-        J_TRP_MOTIF = 'FGXG'
-        J_TRP_OFFSET = 10
-        J_SPLICE = 'GGT'
-    else:
-        J_TRP_MOTIF = 'WGXG'
-        J_TRP_OFFSET = 11
-        J_SPLICE = 'GGT'
-
-    if locus not in ['IGK']:
-        V_RSS_SPACING = 23
-    else:
-        V_RSS_SPACING = 12
-
-    if not args.motif_dir and not args.species:
-        print('Error - please specify either -motif_dir or -species')
-        exit(1)
-
-    if args.motif_dir and args.species:
-        print('Error - please specify either -motif_dir or -species, not both')
-        exit(1)
-
-    motif_dir = args.motif_dir
-
-    if args.species:
-        dm = files('digger')
-        motif_dir = dm.joinpath(f'motifs/{args.species}/{locus}')
-
-    print(f'Using motif files from {motif_dir}')
-
-    for motif_name in ["J-HEPTAMER", "J-NONAMER", 'L-PART1', 'L-PART2', "V-HEPTAMER", "V-NONAMER"]:
-        with open(os.path.join(motif_dir, motif_name + '_prob.csv'), 'r') as fi:
-            motifs[motif_name] = Motif(motif_name, stream=fi)
-
-    if locus in ['IGH', 'TRB', 'TRG']:
-        for motif_name in ["5'D-HEPTAMER", "5'D-NONAMER", "3'D-HEPTAMER", "3'D-NONAMER"]:
-            with open(os.path.join(motif_dir, motif_name + '_prob.csv'), 'r') as fi:
-                motifs[motif_name] = Motif(motif_name, stream=fi)
-
-    conserved_motif_file = os.path.join(motif_dir, 'conserved_motifs.fasta')
-    if os.path.isfile(conserved_motif_file):
-        conserved_motif_seqs = simple.read_fasta(conserved_motif_file)
-
-    for ref in args.ref:
-        if ',' in ref:
-            species, filename = ref.split(',')
-            reference_sets.append({'name': species, 'file': filename})
-        else:
-            print('ref argument should consist of a species name and filename separated by a comma')
+    significant_bps = len([x for x in pattern if x != 'X'])
+    min_result = ceil((1.0-thresh) * significant_bps)
 
-    for ref in reference_sets:
-        ref['seqs'] = simple.read_fasta(ref['file'])
+    for i in range(len(seq) - len(pattern)):
+        d = simple.nt_diff(seq[i:i+pattern_length], pattern)
+        if d <= min_result:
+            dists.append((i, d))
 
-    if args.align is not None:
-        v_gapped_ref = simple.read_fasta(args.align)
-        for name, seq in v_gapped_ref.items():
-            v_ungapped_ref[name] = seq.replace('.', '')
-
-    with open(match_file, 'w', newline='') as fo:
-        fieldnames = ['contig', 'start', 'end', 'start_rev', 'end_rev', 'sense', 'gene_type']
-        for ref in reference_sets:
-            fieldnames.extend([ref['name'] + '_match', ref['name'] + '_score', ref['name'] + '_nt_diffs'])
-
-        fieldnames.extend(
-            ['functional', 'notes', 'likelihood', 'l_part1', 'l_part2', 'v_heptamer', 'v_nonamer', 'j_heptamer', 'j_nonamer', 'j_frame', 'd_3_heptamer', 'd_3_nonamer', 'd_5_heptamer', 'd_5_nonamer',
-            'aa', 'v-gene_aligned_aa', 'seq', 'seq_gapped', '5_rss_start', '5_rss_start_rev', '5_rss_end', '5_rss_end_rev',
-            '3_rss_start', '3_rss_start_rev', '3_rss_end', '3_rss_end_rev', 'l_part1_start', 'l_part1_start_rev', 'l_part1_end', 'l_part1_end_rev',
-            'l_part2_start', 'l_part2_start_rev', 'l_part2_end', 'l_part2_end_rev'])
-
-        fieldnames.extend(['matches', 'blast_match', 'blast_score', 'blast_nt_diffs', 'evalue'])
-
-        writer = csv.DictWriter(fo, fieldnames=fieldnames, restval='')
-        writer.writeheader()
-
-        if '*' not in blast_file:
-            assembly = simple.read_single_fasta(assembly_file)
-            assembly_length = len(assembly)
-            process_file(blast_file, writer, args.debug)
-        else:
-            assemblies = {}
-            for name, seq in simple.read_fasta(assembly_file).items():
-                assemblies[name] = seq
-
-            for blast_file_name in glob.glob(blast_file):
-                suffix = os.path.splitext(os.path.basename(blast_file_name))[0].replace(blast_file.split('*')[0], '')
-                assembly = None
-                for assembly_name in assemblies.keys():
-                    s_name = slugify(assembly_name.split(' ')[0].replace('\n', '').replace('|', '')) + '.csv'
-                    if s_name in blast_file_name or suffix in assembly_name:
-                        assembly = assemblies[assembly_name]
-                        assembly_length = len(assembly)
-                        break
+    return dists
 
-                if assembly is not None:
-                    process_file(blast_file_name, writer, args.debug)
-                else:
-                    print('no corresponding assembly found for output file %s' % blast_file_name)
 
-if __name__ == "__main__":
-    main()
```

### Comparing `receptor_digger-0.5.0/src/digger/motif.py` & `receptor_digger-0.5.3/src/digger/motif.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/human/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/human/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/human/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/human/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv` & `receptor_digger-0.5.3/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/human/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/human/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGK/features.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGK/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/motifs/rhesus_macaque/IGL/features.csv` & `receptor_digger-0.5.3/src/digger/motifs/rhesus_macaque/IGL/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/parse_imgt_annotations.py` & `receptor_digger-0.5.3/src/digger/parse_imgt_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/digger/slugify.py` & `receptor_digger-0.5.3/src/digger/slugify.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.0/src/receptor_digger.egg-info/SOURCES.txt` & `receptor_digger-0.5.3/src/receptor_digger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 setup.cfg
 src/digger/__init__.py
 src/digger/blastresults_to_csv.py
 src/digger/calc_motifs.py
 src/digger/cirelli_contig_matches.py
 src/digger/cirelli_to_fasta.py
 src/digger/compare_annotations.py
+src/digger/dig_sequence.py
+src/digger/dig_utils.py
 src/digger/digger.py
 src/digger/find_alignments.py
 src/digger/motif.py
+src/digger/parse_genes.py
 src/digger/parse_imgt_annotations.py
+src/digger/search_motifs.py
 src/digger/slugify.py
 src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
 src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
 src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
 src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
 src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
 src/digger/motifs/human/IGH/J-NONAMER_prob.csv
```

