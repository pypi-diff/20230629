# Comparing `tmp/hebpipe-3.0.0.4.tar.gz` & `tmp/hebpipe-3.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hebpipe-3.0.0.4.tar", last modified: Thu Jun 29 14:15:50 2023, max compression
+gzip compressed data, was "dist\hebpipe-3.0.0.5.tar", last modified: Thu Jun 29 14:45:16 2023, max compression
```

## Comparing `hebpipe-3.0.0.4.tar` & `hebpipe-3.0.0.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:50.017022 hebpipe-3.0.0.4/
--rw-rw-rw-   0        0        0      708 2023-06-29 14:15:50.015027 hebpipe-3.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6418 2023-03-23 13:46:54.000000 hebpipe-3.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.651156 hebpipe-3.0.0.4/hebpipe/
--rw-rw-rw-   0        0        0       47 2020-05-26 16:17:29.000000 hebpipe-3.0.0.4/hebpipe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.661128 hebpipe-3.0.0.4/hebpipe/bin/
--rw-rw-rw-   0        0        0       10 2018-09-15 20:02:00.000000 hebpipe-3.0.0.4/hebpipe/bin/binary_dependencies_go_here.txt
--rw-rw-rw-   0        0        0      364 2023-02-16 15:29:32.000000 hebpipe-3.0.0.4/hebpipe/check_len.py
--rw-rw-rw-   0        0        0      990 2021-07-30 01:20:38.000000 hebpipe-3.0.0.4/hebpipe/clean_meta.py
--rw-rw-rw-   0        0        0    27773 2021-08-01 21:43:53.000000 hebpipe-3.0.0.4/hebpipe/conll18_ud_eval.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.888986 hebpipe-3.0.0.4/hebpipe/data/
--rw-rw-rw-   0        0        0   154395 2018-05-08 20:43:27.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_dev_gold.tab
--rw-rw-rw-   0        0        0    75818 2018-05-08 20:45:47.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_dev_plain.tab
--rw-rw-rw-   0        0        0   226455 2018-05-08 20:27:59.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_test_gold.tab
--rw-rw-rw-   0        0        0   111130 2018-05-08 20:45:12.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_test_plain.tab
--rw-rw-rw-   0        0        0  1704715 2018-04-18 17:10:59.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_train_gold.tab
--rw-rw-rw-   0        0        0   835656 2018-05-08 20:45:33.000000 hebpipe-3.0.0.4/hebpipe/data/SPMRL_train_plain.tab
--rw-rw-rw-   0        0        0    92942 2018-05-09 15:16:41.000000 hebpipe-3.0.0.4/hebpipe/data/Wiki5K_test_gold.tab
--rw-rw-rw-   0        0        0    45564 2018-05-09 15:19:14.000000 hebpipe-3.0.0.4/hebpipe/data/Wiki5K_test_plain.tab
--rw-rw-rw-   0        0        0   850542 2021-05-24 20:56:43.000000 hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-dev.conllu
--rw-rw-rw-   0        0        0   916918 2021-05-24 20:56:45.000000 hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-test.conllu
--rw-rw-rw-   0        0        0 10302649 2021-05-26 18:53:25.000000 hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-train_and_geek.conllu
--rw-rw-rw-   0        0        0   152953 2021-08-21 19:05:45.000000 hebpipe-3.0.0.4/hebpipe/data/heb.binyan
--rw-rw-rw-   0        0        0     1054 2018-08-24 20:56:59.000000 hebpipe-3.0.0.4/hebpipe/data/heb.conf
--rw-rw-rw-   0        0        0   224818 2018-05-09 15:37:49.000000 hebpipe-3.0.0.4/hebpipe/data/heb.frq
--rw-rw-rw-   0        0        0  7800623 2021-07-30 15:58:05.000000 hebpipe-3.0.0.4/hebpipe/data/heb.lemma
--rw-rw-rw-   0        0        0 24143089 2021-07-29 20:36:37.000000 hebpipe-3.0.0.4/hebpipe/data/heb.lex
--rw-rw-rw-   0        0        0      743 2018-08-24 13:22:23.000000 hebpipe-3.0.0.4/hebpipe/data/heb_abbr.tab
--rw-rw-rw-   0        0        0  2448363 2018-08-25 05:46:11.000000 hebpipe-3.0.0.4/hebpipe/data/heb_lemma_lex.tab
--rw-rw-rw-   0        0        0  2178509 2018-08-24 18:17:55.000000 hebpipe-3.0.0.4/hebpipe/data/heb_train_seg_all.tab
--rw-rw-rw-   0        0        0  9145481 2018-01-30 00:39:46.000000 hebpipe-3.0.0.4/hebpipe/data/heb_train_tb.conll10
--rw-rw-rw-   0        0        0      339 2021-07-29 19:11:27.000000 hebpipe-3.0.0.4/hebpipe/data/make_lemma_lex.py
--rw-rw-rw-   0        0        0      184 2021-05-19 15:27:35.000000 hebpipe-3.0.0.4/hebpipe/data/postprocess_parsed.ini
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.897935 hebpipe-3.0.0.4/hebpipe/eval/
--rw-rw-rw-   0        0        0        0 2017-06-22 07:38:42.000000 hebpipe-3.0.0.4/hebpipe/eval/__init__.py
--rw-rw-rw-   0        0        0     3083 2018-08-17 13:07:30.000000 hebpipe-3.0.0.4/hebpipe/eval/eval_parsing.py
--rw-rw-rw-   0        0        0     3483 2018-08-21 05:33:30.000000 hebpipe-3.0.0.4/hebpipe/eval/eval_tokenization.py
--rw-rw-rw-   0        0        0     3394 2018-08-14 09:04:14.000000 hebpipe-3.0.0.4/hebpipe/eval/f_score_segs.py
--rw-rw-rw-   0        0        0     4433 2021-07-28 22:32:17.000000 hebpipe-3.0.0.4/hebpipe/eval_morph.py
--rw-rw-rw-   0        0        0    32298 2022-10-18 13:57:43.000000 hebpipe-3.0.0.4/hebpipe/heb_pipe.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.940596 hebpipe-3.0.0.4/hebpipe/lib/
--rw-rw-rw-   0        0        0      489 2023-01-20 21:19:48.000000 hebpipe-3.0.0.4/hebpipe/lib/__init__.py
--rw-rw-rw-   0        0        0      180 2023-06-29 14:11:49.000000 hebpipe-3.0.0.4/hebpipe/lib/_version.py
--rw-rw-rw-   0        0        0     2443 2021-07-22 17:50:33.000000 hebpipe-3.0.0.4/hebpipe/lib/append_column.py
--rw-rw-rw-   0        0        0     1436 2018-07-31 18:01:39.000000 hebpipe-3.0.0.4/hebpipe/lib/binarize_tags.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.946397 hebpipe-3.0.0.4/hebpipe/lib/crfutils/
--rw-rw-rw-   0        0        0        0 2023-02-20 19:45:29.000000 hebpipe-3.0.0.4/hebpipe/lib/crfutils/__init__.py
--rw-rw-rw-   0        0        0     2268 2022-09-30 14:56:17.000000 hebpipe-3.0.0.4/hebpipe/lib/crfutils/crf.py
--rw-rw-rw-   0        0        0    11135 2022-09-30 14:56:17.000000 hebpipe-3.0.0.4/hebpipe/lib/crfutils/viterbi.py
--rw-rw-rw-   0        0        0    32435 2018-08-17 12:58:11.000000 hebpipe-3.0.0.4/hebpipe/lib/depedit.py
--rw-rw-rw-   0        0        0     1786 2022-09-30 14:56:17.000000 hebpipe-3.0.0.4/hebpipe/lib/dropout.py
--rw-rw-rw-   0        0        0     1232 2018-06-08 18:55:21.000000 hebpipe-3.0.0.4/hebpipe/lib/harvest_tt_sgml.py
--rw-rw-rw-   0        0        0      394 2021-07-17 05:59:39.000000 hebpipe-3.0.0.4/hebpipe/lib/morph_trankit.py
--rw-rw-rw-   0        0        0    65977 2023-01-20 21:19:06.000000 hebpipe-3.0.0.4/hebpipe/lib/mtlmodel.py
--rw-rw-rw-   0        0        0     9199 2022-10-17 18:39:18.000000 hebpipe-3.0.0.4/hebpipe/lib/partial_morph.ini
--rw-rw-rw-   0        0        0    11225 2018-07-29 12:49:00.000000 hebpipe-3.0.0.4/hebpipe/lib/preprocess.py
--rw-rw-rw-   0        0        0     3683 2020-06-19 19:21:29.000000 hebpipe-3.0.0.4/hebpipe/lib/reorder_sgml.py
--rw-rw-rw-   0        0        0      567 2021-07-22 20:11:46.000000 hebpipe-3.0.0.4/hebpipe/lib/sent_split.py
--rw-rw-rw-   0        0        0      805 2021-06-10 14:55:27.000000 hebpipe-3.0.0.4/hebpipe/lib/timing.py
--rw-rw-rw-   0        0        0     3993 2021-05-17 19:04:13.000000 hebpipe-3.0.0.4/hebpipe/lib/tt2conll.py
--rw-rw-rw-   0        0        0    12198 2021-10-18 13:52:17.000000 hebpipe-3.0.0.4/hebpipe/lib/whitespace_tokenize.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.951385 hebpipe-3.0.0.4/hebpipe/lib/xrenner/
--rw-rw-rw-   0        0        0      154 2020-02-21 01:17:43.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:50.006050 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/
--rw-rw-rw-   0        0        0      156 2017-02-21 16:55:35.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/__init__.py
--rw-rw-rw-   0        0        0    33982 2020-02-25 15:19:28.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/depedit.py
--rw-rw-rw-   0        0        0     1135 2020-02-27 00:48:58.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/get_models.py
--rw-rw-rw-   0        0        0      677 2017-12-26 17:31:32.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/timing.py
--rw-rw-rw-   0        0        0    13406 2020-02-20 22:48:44.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_classes.py
--rw-rw-rw-   0        0        0     2921 2020-02-25 17:33:50.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_classify.py
--rw-rw-rw-   0        0        0    28099 2020-02-24 14:32:38.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_compatible.py
--rw-rw-rw-   0        0        0    11367 2020-02-25 19:57:24.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_coref.py
--rw-rw-rw-   0        0        0    24875 2020-02-26 20:41:51.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_lex.py
--rw-rw-rw-   0        0        0    37745 2020-02-24 14:26:02.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_marker.py
--rw-rw-rw-   0        0        0     6228 2016-12-14 21:38:54.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_ontoreader.py
--rw-rw-rw-   0        0        0    28875 2020-02-27 19:07:18.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_out.py
--rw-rw-rw-   0        0        0     8597 2021-05-17 19:42:56.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_postprocess.py
--rw-rw-rw-   0        0        0     5249 2020-02-21 00:54:34.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_preprocess.py
--rw-rw-rw-   0        0        0     3304 2016-05-31 21:01:58.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_propagate.py
--rw-rw-rw-   0        0        0     7694 2018-01-16 21:19:45.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_rule.py
--rw-rw-rw-   0        0        0     3144 2020-02-25 17:15:11.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_sequence.py
--rw-rw-rw-   0        0        0    10980 2020-02-23 18:55:41.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_test.py
--rw-rw-rw-   0        0        0    32247 2020-02-26 22:07:21.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_xrenner.py
--rw-rw-rw-   0        0        0     8302 2020-02-27 00:35:48.000000 hebpipe-3.0.0.4/hebpipe/lib/xrenner/xrenner.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:50.009043 hebpipe-3.0.0.4/hebpipe/models/
--rw-rw-rw-   0        0        0       10 2018-09-15 20:02:00.000000 hebpipe-3.0.0.4/hebpipe/models/models_go_here.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:50.012051 hebpipe-3.0.0.4/hebpipe/models/stanza/
--rw-rw-rw-   0        0        0        1 2021-07-29 19:15:49.000000 hebpipe-3.0.0.4/hebpipe/models/stanza/stanza_models_here.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 14:15:49.659137 hebpipe-3.0.0.4/hebpipe.egg-info/
--rw-rw-rw-   0        0        0      708 2023-06-29 14:15:49.000000 hebpipe-3.0.0.4/hebpipe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2679 2023-06-29 14:15:49.000000 hebpipe-3.0.0.4/hebpipe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:15:49.000000 hebpipe-3.0.0.4/hebpipe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-29 14:15:49.000000 hebpipe-3.0.0.4/hebpipe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 14:15:49.000000 hebpipe-3.0.0.4/hebpipe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:15:50.018019 hebpipe-3.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-06-29 14:11:35.000000 hebpipe-3.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.462327 hebpipe-3.0.0.5/
+-rw-rw-rw-   0        0        0      708 2023-06-29 14:45:16.461332 hebpipe-3.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6418 2023-03-23 13:46:54.000000 hebpipe-3.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.266558 hebpipe-3.0.0.5/hebpipe/
+-rw-rw-rw-   0        0        0       47 2020-05-26 16:17:29.000000 hebpipe-3.0.0.5/hebpipe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.278548 hebpipe-3.0.0.5/hebpipe/bin/
+-rw-rw-rw-   0        0        0       10 2018-09-15 20:02:00.000000 hebpipe-3.0.0.5/hebpipe/bin/binary_dependencies_go_here.txt
+-rw-rw-rw-   0        0        0      364 2023-02-16 15:29:32.000000 hebpipe-3.0.0.5/hebpipe/check_len.py
+-rw-rw-rw-   0        0        0      990 2021-07-30 01:20:38.000000 hebpipe-3.0.0.5/hebpipe/clean_meta.py
+-rw-rw-rw-   0        0        0    27773 2021-08-01 21:43:53.000000 hebpipe-3.0.0.5/hebpipe/conll18_ud_eval.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.382541 hebpipe-3.0.0.5/hebpipe/data/
+-rw-rw-rw-   0        0        0   154395 2018-05-08 20:43:27.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_dev_gold.tab
+-rw-rw-rw-   0        0        0    75818 2018-05-08 20:45:47.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_dev_plain.tab
+-rw-rw-rw-   0        0        0   226455 2018-05-08 20:27:59.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_test_gold.tab
+-rw-rw-rw-   0        0        0   111130 2018-05-08 20:45:12.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_test_plain.tab
+-rw-rw-rw-   0        0        0  1704715 2018-04-18 17:10:59.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_train_gold.tab
+-rw-rw-rw-   0        0        0   835656 2018-05-08 20:45:33.000000 hebpipe-3.0.0.5/hebpipe/data/SPMRL_train_plain.tab
+-rw-rw-rw-   0        0        0    92942 2018-05-09 15:16:41.000000 hebpipe-3.0.0.5/hebpipe/data/Wiki5K_test_gold.tab
+-rw-rw-rw-   0        0        0    45564 2018-05-09 15:19:14.000000 hebpipe-3.0.0.5/hebpipe/data/Wiki5K_test_plain.tab
+-rw-rw-rw-   0        0        0   850542 2021-05-24 20:56:43.000000 hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-dev.conllu
+-rw-rw-rw-   0        0        0   916918 2021-05-24 20:56:45.000000 hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-test.conllu
+-rw-rw-rw-   0        0        0 10302649 2021-05-26 18:53:25.000000 hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-train_and_geek.conllu
+-rw-rw-rw-   0        0        0   152953 2021-08-21 19:05:45.000000 hebpipe-3.0.0.5/hebpipe/data/heb.binyan
+-rw-rw-rw-   0        0        0     1054 2018-08-24 20:56:59.000000 hebpipe-3.0.0.5/hebpipe/data/heb.conf
+-rw-rw-rw-   0        0        0   224818 2018-05-09 15:37:49.000000 hebpipe-3.0.0.5/hebpipe/data/heb.frq
+-rw-rw-rw-   0        0        0  7800623 2021-07-30 15:58:05.000000 hebpipe-3.0.0.5/hebpipe/data/heb.lemma
+-rw-rw-rw-   0        0        0 24143089 2021-07-29 20:36:37.000000 hebpipe-3.0.0.5/hebpipe/data/heb.lex
+-rw-rw-rw-   0        0        0      743 2018-08-24 13:22:23.000000 hebpipe-3.0.0.5/hebpipe/data/heb_abbr.tab
+-rw-rw-rw-   0        0        0  2448363 2018-08-25 05:46:11.000000 hebpipe-3.0.0.5/hebpipe/data/heb_lemma_lex.tab
+-rw-rw-rw-   0        0        0  2178509 2018-08-24 18:17:55.000000 hebpipe-3.0.0.5/hebpipe/data/heb_train_seg_all.tab
+-rw-rw-rw-   0        0        0  9145481 2018-01-30 00:39:46.000000 hebpipe-3.0.0.5/hebpipe/data/heb_train_tb.conll10
+-rw-rw-rw-   0        0        0      339 2021-07-29 19:11:27.000000 hebpipe-3.0.0.5/hebpipe/data/make_lemma_lex.py
+-rw-rw-rw-   0        0        0      184 2021-05-19 15:27:35.000000 hebpipe-3.0.0.5/hebpipe/data/postprocess_parsed.ini
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.388525 hebpipe-3.0.0.5/hebpipe/eval/
+-rw-rw-rw-   0        0        0        0 2017-06-22 07:38:42.000000 hebpipe-3.0.0.5/hebpipe/eval/__init__.py
+-rw-rw-rw-   0        0        0     3083 2018-08-17 13:07:30.000000 hebpipe-3.0.0.5/hebpipe/eval/eval_parsing.py
+-rw-rw-rw-   0        0        0     3483 2018-08-21 05:33:30.000000 hebpipe-3.0.0.5/hebpipe/eval/eval_tokenization.py
+-rw-rw-rw-   0        0        0     3394 2018-08-14 09:04:14.000000 hebpipe-3.0.0.5/hebpipe/eval/f_score_segs.py
+-rw-rw-rw-   0        0        0     4433 2021-07-28 22:32:17.000000 hebpipe-3.0.0.5/hebpipe/eval_morph.py
+-rw-rw-rw-   0        0        0    32298 2022-10-18 13:57:43.000000 hebpipe-3.0.0.5/hebpipe/heb_pipe.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.414455 hebpipe-3.0.0.5/hebpipe/lib/
+-rw-rw-rw-   0        0        0      489 2023-01-20 21:19:48.000000 hebpipe-3.0.0.5/hebpipe/lib/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-06-29 14:44:41.000000 hebpipe-3.0.0.5/hebpipe/lib/_version.py
+-rw-rw-rw-   0        0        0     2443 2021-07-22 17:50:33.000000 hebpipe-3.0.0.5/hebpipe/lib/append_column.py
+-rw-rw-rw-   0        0        0     1436 2018-07-31 18:01:39.000000 hebpipe-3.0.0.5/hebpipe/lib/binarize_tags.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.418444 hebpipe-3.0.0.5/hebpipe/lib/crfutils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 19:45:29.000000 hebpipe-3.0.0.5/hebpipe/lib/crfutils/__init__.py
+-rw-rw-rw-   0        0        0     2268 2022-09-30 14:56:17.000000 hebpipe-3.0.0.5/hebpipe/lib/crfutils/crf.py
+-rw-rw-rw-   0        0        0    11135 2022-09-30 14:56:17.000000 hebpipe-3.0.0.5/hebpipe/lib/crfutils/viterbi.py
+-rw-rw-rw-   0        0        0    32435 2018-08-17 12:58:11.000000 hebpipe-3.0.0.5/hebpipe/lib/depedit.py
+-rw-rw-rw-   0        0        0     1786 2022-09-30 14:56:17.000000 hebpipe-3.0.0.5/hebpipe/lib/dropout.py
+-rw-rw-rw-   0        0        0     1232 2018-06-08 18:55:21.000000 hebpipe-3.0.0.5/hebpipe/lib/harvest_tt_sgml.py
+-rw-rw-rw-   0        0        0      394 2021-07-17 05:59:39.000000 hebpipe-3.0.0.5/hebpipe/lib/morph_trankit.py
+-rw-rw-rw-   0        0        0    65977 2023-01-20 21:19:06.000000 hebpipe-3.0.0.5/hebpipe/lib/mtlmodel.py
+-rw-rw-rw-   0        0        0     9199 2022-10-17 18:39:18.000000 hebpipe-3.0.0.5/hebpipe/lib/partial_morph.ini
+-rw-rw-rw-   0        0        0    11225 2018-07-29 12:49:00.000000 hebpipe-3.0.0.5/hebpipe/lib/preprocess.py
+-rw-rw-rw-   0        0        0     3683 2020-06-19 19:21:29.000000 hebpipe-3.0.0.5/hebpipe/lib/reorder_sgml.py
+-rw-rw-rw-   0        0        0      567 2021-07-22 20:11:46.000000 hebpipe-3.0.0.5/hebpipe/lib/sent_split.py
+-rw-rw-rw-   0        0        0      805 2021-06-10 14:55:27.000000 hebpipe-3.0.0.5/hebpipe/lib/timing.py
+-rw-rw-rw-   0        0        0     3993 2021-05-17 19:04:13.000000 hebpipe-3.0.0.5/hebpipe/lib/tt2conll.py
+-rw-rw-rw-   0        0        0    12198 2021-10-18 13:52:17.000000 hebpipe-3.0.0.5/hebpipe/lib/whitespace_tokenize.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.422434 hebpipe-3.0.0.5/hebpipe/lib/xrenner/
+-rw-rw-rw-   0        0        0      154 2020-02-21 01:17:43.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.455345 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/
+-rw-rw-rw-   0        0        0      156 2017-02-21 16:55:35.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/__init__.py
+-rw-rw-rw-   0        0        0    33982 2020-02-25 15:19:28.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/depedit.py
+-rw-rw-rw-   0        0        0     1135 2020-02-27 00:48:58.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/get_models.py
+-rw-rw-rw-   0        0        0      677 2017-12-26 17:31:32.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/timing.py
+-rw-rw-rw-   0        0        0    13406 2020-02-20 22:48:44.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_classes.py
+-rw-rw-rw-   0        0        0     2921 2020-02-25 17:33:50.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_classify.py
+-rw-rw-rw-   0        0        0    28099 2020-02-24 14:32:38.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_compatible.py
+-rw-rw-rw-   0        0        0    11367 2020-02-25 19:57:24.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_coref.py
+-rw-rw-rw-   0        0        0    24875 2020-02-26 20:41:51.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_lex.py
+-rw-rw-rw-   0        0        0    37745 2020-02-24 14:26:02.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_marker.py
+-rw-rw-rw-   0        0        0     6228 2016-12-14 21:38:54.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_ontoreader.py
+-rw-rw-rw-   0        0        0    28875 2020-02-27 19:07:18.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_out.py
+-rw-rw-rw-   0        0        0     8597 2021-05-17 19:42:56.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_postprocess.py
+-rw-rw-rw-   0        0        0     5249 2020-02-21 00:54:34.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_preprocess.py
+-rw-rw-rw-   0        0        0     3304 2016-05-31 21:01:58.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_propagate.py
+-rw-rw-rw-   0        0        0     7694 2018-01-16 21:19:45.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_rule.py
+-rw-rw-rw-   0        0        0     3144 2020-02-25 17:15:11.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_sequence.py
+-rw-rw-rw-   0        0        0    10980 2020-02-23 18:55:41.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_test.py
+-rw-rw-rw-   0        0        0    32247 2020-02-26 22:07:21.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_xrenner.py
+-rw-rw-rw-   0        0        0     8302 2020-02-27 00:35:48.000000 hebpipe-3.0.0.5/hebpipe/lib/xrenner/xrenner.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.456343 hebpipe-3.0.0.5/hebpipe/models/
+-rw-rw-rw-   0        0        0       10 2018-09-15 20:02:00.000000 hebpipe-3.0.0.5/hebpipe/models/models_go_here.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.458337 hebpipe-3.0.0.5/hebpipe/models/stanza/
+-rw-rw-rw-   0        0        0        1 2021-07-29 19:15:49.000000 hebpipe-3.0.0.5/hebpipe/models/stanza/stanza_models_here.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:16.275556 hebpipe-3.0.0.5/hebpipe.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-06-29 14:45:16.000000 hebpipe-3.0.0.5/hebpipe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2679 2023-06-29 14:45:16.000000 hebpipe-3.0.0.5/hebpipe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:45:16.000000 hebpipe-3.0.0.5/hebpipe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-29 14:45:16.000000 hebpipe-3.0.0.5/hebpipe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 14:45:16.000000 hebpipe-3.0.0.5/hebpipe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:45:16.462327 hebpipe-3.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-06-29 14:44:36.000000 hebpipe-3.0.0.5/setup.py
```

### Comparing `hebpipe-3.0.0.4/PKG-INFO` & `hebpipe-3.0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: hebpipe
-Version: 3.0.0.4
+Version: 3.0.0.5
 Summary: A pipeline for Hebrew NLP
 Home-page: https://github.com/amir-zeldes/HebPipe
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/HebPipe/releases/tag/v3.0.0.3
+Download-URL: https://github.com/amir-zeldes/HebPipe/releases/tag/v3.0.0.5
 Description: UNKNOWN
 Keywords: NLP,Hebrew,segmentation,tokenization,tagging,parsing,morphology,POS,lemmatization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hebpipe-3.0.0.4/README.md` & `hebpipe-3.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/clean_meta.py` & `hebpipe-3.0.0.5/hebpipe/clean_meta.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/conll18_ud_eval.py` & `hebpipe-3.0.0.5/hebpipe/conll18_ud_eval.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_dev_gold.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_dev_gold.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_dev_plain.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_dev_plain.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_test_gold.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_test_gold.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_test_plain.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_test_plain.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_train_gold.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_train_gold.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/SPMRL_train_plain.tab` & `hebpipe-3.0.0.5/hebpipe/data/SPMRL_train_plain.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/Wiki5K_test_gold.tab` & `hebpipe-3.0.0.5/hebpipe/data/Wiki5K_test_gold.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/Wiki5K_test_plain.tab` & `hebpipe-3.0.0.5/hebpipe/data/Wiki5K_test_plain.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-dev.conllu` & `hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-dev.conllu`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-test.conllu` & `hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-test.conllu`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/he_htb-ud-train_and_geek.conllu` & `hebpipe-3.0.0.5/hebpipe/data/he_htb-ud-train_and_geek.conllu`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb.binyan` & `hebpipe-3.0.0.5/hebpipe/data/heb.binyan`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb.conf` & `hebpipe-3.0.0.5/hebpipe/data/heb.conf`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb.frq` & `hebpipe-3.0.0.5/hebpipe/data/heb.frq`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb.lemma` & `hebpipe-3.0.0.5/hebpipe/data/heb.lemma`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb.lex` & `hebpipe-3.0.0.5/hebpipe/data/heb.lex`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb_abbr.tab` & `hebpipe-3.0.0.5/hebpipe/data/heb_abbr.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb_lemma_lex.tab` & `hebpipe-3.0.0.5/hebpipe/data/heb_lemma_lex.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb_train_seg_all.tab` & `hebpipe-3.0.0.5/hebpipe/data/heb_train_seg_all.tab`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/data/heb_train_tb.conll10` & `hebpipe-3.0.0.5/hebpipe/data/heb_train_tb.conll10`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/eval/eval_parsing.py` & `hebpipe-3.0.0.5/hebpipe/eval/eval_parsing.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/eval/eval_tokenization.py` & `hebpipe-3.0.0.5/hebpipe/eval/eval_tokenization.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/eval/f_score_segs.py` & `hebpipe-3.0.0.5/hebpipe/eval/f_score_segs.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/eval_morph.py` & `hebpipe-3.0.0.5/hebpipe/eval_morph.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/heb_pipe.py` & `hebpipe-3.0.0.5/hebpipe/heb_pipe.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/append_column.py` & `hebpipe-3.0.0.5/hebpipe/lib/append_column.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/binarize_tags.py` & `hebpipe-3.0.0.5/hebpipe/lib/binarize_tags.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/crfutils/crf.py` & `hebpipe-3.0.0.5/hebpipe/lib/crfutils/crf.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/crfutils/viterbi.py` & `hebpipe-3.0.0.5/hebpipe/lib/crfutils/viterbi.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/depedit.py` & `hebpipe-3.0.0.5/hebpipe/lib/depedit.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/dropout.py` & `hebpipe-3.0.0.5/hebpipe/lib/dropout.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/harvest_tt_sgml.py` & `hebpipe-3.0.0.5/hebpipe/lib/harvest_tt_sgml.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/mtlmodel.py` & `hebpipe-3.0.0.5/hebpipe/lib/mtlmodel.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/partial_morph.ini` & `hebpipe-3.0.0.5/hebpipe/lib/partial_morph.ini`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/preprocess.py` & `hebpipe-3.0.0.5/hebpipe/lib/preprocess.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/reorder_sgml.py` & `hebpipe-3.0.0.5/hebpipe/lib/reorder_sgml.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/sent_split.py` & `hebpipe-3.0.0.5/hebpipe/lib/sent_split.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/timing.py` & `hebpipe-3.0.0.5/hebpipe/lib/timing.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/tt2conll.py` & `hebpipe-3.0.0.5/hebpipe/lib/tt2conll.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/whitespace_tokenize.py` & `hebpipe-3.0.0.5/hebpipe/lib/whitespace_tokenize.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/depedit.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/depedit.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/get_models.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/get_models.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/timing.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/timing.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_classes.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_classes.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_classify.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_classify.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_compatible.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_compatible.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_coref.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_coref.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_lex.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_lex.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_marker.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_marker.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_ontoreader.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_ontoreader.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_out.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_out.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_postprocess.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_postprocess.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_preprocess.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_preprocess.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_propagate.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_propagate.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_rule.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_rule.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_sequence.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_sequence.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_test.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_test.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/modules/xrenner_xrenner.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/modules/xrenner_xrenner.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe/lib/xrenner/xrenner.py` & `hebpipe-3.0.0.5/hebpipe/lib/xrenner/xrenner.py`

 * *Files identical despite different names*

### Comparing `hebpipe-3.0.0.4/hebpipe.egg-info/PKG-INFO` & `hebpipe-3.0.0.5/hebpipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: hebpipe
-Version: 3.0.0.4
+Version: 3.0.0.5
 Summary: A pipeline for Hebrew NLP
 Home-page: https://github.com/amir-zeldes/HebPipe
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/HebPipe/releases/tag/v3.0.0.3
+Download-URL: https://github.com/amir-zeldes/HebPipe/releases/tag/v3.0.0.5
 Description: UNKNOWN
 Keywords: NLP,Hebrew,segmentation,tokenization,tagging,parsing,morphology,POS,lemmatization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `hebpipe-3.0.0.4/hebpipe.egg-info/SOURCES.txt` & `hebpipe-3.0.0.5/hebpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

