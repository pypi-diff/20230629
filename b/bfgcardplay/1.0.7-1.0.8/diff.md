# Comparing `tmp/bfgcardplay-1.0.7.tar.gz` & `tmp/bfgcardplay-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.0.7.tar", last modified: Thu Jun 29 13:59:58 2023, max compression
+gzip compressed data, was "bfgcardplay-1.0.8.tar", last modified: Thu Jun 29 14:58:22 2023, max compression
```

## Comparing `bfgcardplay-1.0.7.tar` & `bfgcardplay-1.0.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4007 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.7/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.468568 bfgcardplay-1.0.7/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      215 2023-06-29 13:52:00.000000 bfgcardplay-1.0.7/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.7/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/bfgcardplay/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2305 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19594 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4661 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12247 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3976 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9753 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16135 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17433 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    21989 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16445 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1989 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6553 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5369 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      664 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43274 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    24438 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3025 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10003 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7231 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3638 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1880 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17664 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14321 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6542 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/bfgcardplay/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      558 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15003 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      587 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_utilities.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      294 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.468568 bfgcardplay-1.0.7/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4007 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1589 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.7/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4050 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.8/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.204541 bfgcardplay-1.0.8/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      215 2023-06-29 13:52:00.000000 bfgcardplay-1.0.8/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.8/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.207874 bfgcardplay-1.0.8/bfgcardplay/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3446 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2303 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    19533 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4663 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12296 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3976 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9753 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16201 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17433 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    21952 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16445 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2026 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6553 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5369 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      665 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6982 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43274 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    24438 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3025 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9986 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7231 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3638 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1880 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17664 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14321 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6542 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/src/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/bfgcardplay/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      558 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    15003 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      587 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/test_utilities.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      294 2023-06-29 14:57:34.000000 bfgcardplay-1.0.8/bfgcardplay/tests/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 14:58:22.204541 bfgcardplay-1.0.8/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4050 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1589 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-29 14:58:22.000000 bfgcardplay-1.0.8/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 14:58:22.211207 bfgcardplay-1.0.8/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.8/setup.py
```

### Comparing `bfgcardplay-1.0.7/PKG-INFO` & `bfgcardplay-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.7
+Version: 1.0.8
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
-Version 1.0.7 29 Jun 2023
+Version 1.0.8 29 Jun 2023
 
-1. xxx
+1. Linting
 
 ------
 
 Version 1.0.7 29 Jun 2023
 
-1. xxx
+1. General modifications and enhanced testing
 
 ------
 
 Version 1.0.6 26 Jun 2023
 
 1. xxx
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/logger.py` & `bfgcardplay-1.0.8/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/card_player_components.py` & `bfgcardplay-1.0.8/bfgcardplay/src/card_player_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,8 +88,9 @@
 
     def __init__(self, name, selection_reason='000', *args, **kwargs):
         super().__init__(name, *args, **kwargs)
         self.selection_reason = selection_reason
 
     def __str__(self):
         """Return the str value."""
-        return f'Card("{self.name}"), {self.selection_reason}, {CARD_SELECTION_REASON[self.selection_reason]}'
+        selection_reason = CARD_SELECTION_REASON[self.selection_reason]
+        return f'Card("{self.name}"), {self.selection_reason}, {selection_reason}'
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/cards.py` & `bfgcardplay-1.0.8/bfgcardplay/src/cards.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 # from types import list
 from termcolor import cprint
 
 import random
 
 from bridgeobjects import Suit, Card, SUITS
-from bfgsupport import Hand
+from bfgbidding import Hand
 
 import bfgcardplay.src.global_variables as global_vars
 from .utilities import get_list_of_best_scores
 
 global_vars.initialize()
 
 MODULE_COLOUR = 'magenta'
 
 
 class Cards():
     """A class representing a set of cards."""
-    def __init__(self, input: list[str] | list[Card] | Hand]):
+    def __init__(self, input: list[str] | list[Card] | Hand):
         self.list = []
         self.longest_suit = None
         by_suit = {suit: [] for key, suit in SUITS.items()}
         by_suit_name = {key: [] for key, suit in SUITS.items()}
         self.by_suit = {**by_suit, **by_suit_name}
         self._value = 0
         self._create(input)
 
     def count(self) -> int:
         """Return the number of cards."""
         return len(self.list)
 
-    def _create(self, input: list[str] | list[Card] | Hand]):
+    def _create(self, input: list[str] | list[Card] | Hand):
         """Create a set of cards"""
         if isinstance(input, Hand):
             cards = input.cards
         elif not isinstance(input, list):
             raise TypeError('Cards must be a list of cards')
         else:
             cards = input
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/dashboard.py` & `bfgcardplay-1.0.8/bfgcardplay/src/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     probability: float
     cards: str
 
 
 class Dashboard():
     "Statistics for a player."
     def __init__(self, player) -> None:
-        self.suits = {suit:{} for suit in SUITS}
+        self.suits = {suit: {} for suit in SUITS}
         self.player = player
         self.threats = self._get_threats()
         # self.losers = self._get_losers()
         self.winners = self._get_suit_winners()
-        self.split_winners  = self._get_split_winners()
+        self.split_winners = self._get_split_winners()
         self.winner_count = self._get_winner_count()
         self.suit_lengths = self._suit_lengths()
         self.extra_winners_length = self._extra_winners_length()
         # extra_winners_strength must be generated after winners
         self.extra_winners_strength = self._extra_winners_strength()
         self.tricks_needed = 6 + int(player.board.contract.name[0])
 
@@ -243,15 +243,16 @@
                         skip_card = False
 
                         # No more cards to lose
                         if winners > missing:
                             break
                     else:
                         threats[suit].append(ranking_card)
-                        # skip card means that the next card in the suit is assumed to have been beaten
+                        # skip card means that the next card in the suit is assumed
+                        # to have been beaten
                         skip_card = True
 
                     # threats only in long hand
                     if index + 1 >= len(long_cards):
                         break
                 if len(opponents_cards) <= index + 1:
                     break
@@ -291,15 +292,16 @@
                             break
 
                         # No more cards to lose
                         if winners > missing:
                             break
                     else:
                         threats[suit].append(ranking_card)
-                        # skip card means that the next card in the suit is assumed to have been beaten
+                        # skip card means that the next card in the suit is assumed
+                        # to have been beaten
                         skip_card = True
 
                     # threats only in long hand
                     if index + 1 >= len(long_cards):
                         break
                 if len(opponents_cards) <= index + 1:
                     break
@@ -336,17 +338,14 @@
         # return (long_unplayed_cards, short_unplayed_cards)
 
     def _get_losers(self) -> dict[str, Card]:
         """Return a dict of losing cards by suit in players cards."""
         player = self.player
         (long_hand, short_hand) = self.get_long_short_trump_hands()
         unplayed_cards = player.cards_by_suit(long_hand)
-        long_cards = unplayed_cards[player.trump_suit.name]
-
-        losers = {suit: [] for suit in SUITS}
         ranks = [rank for rank in RANKS]
         ranks.reverse()
         sorted_ranks = ranks[:-1]
 
         for suit in SUITS:
             our_cards = player.our_unplayed_cards[suit]
 
@@ -384,26 +383,26 @@
         our_cards = player.our_unplayed_cards
         our_length = self._get_our_length(player, suit)
         opponents_cards = player.opponents_unplayed_cards
         split_winners = SplitWinners(split, SPLIT_PROBABILITIES[split], '')
         opps_suit_cards = opponents_cards[suit][:int(split[0])]
         for index, card in enumerate(our_cards[suit]):
             split_winners.cards += self._split_winner(index, card, opps_suit_cards,
-                                                        split_winners.cards, our_length)
+                                                      split_winners.cards, our_length)
         return split_winners
 
     @staticmethod
     def _split_winner(index, card, opps_suit_cards, cards, our_length):
         if index < len(opps_suit_cards):
             if len(cards) < our_length:
                 if opps_suit_cards:
                     if card.value > opps_suit_cards[0].value:
                         return card.rank
         elif index < our_length:
-                return card.rank
+            return card.rank
         return ''
 
     @staticmethod
     def _get_our_length(player: object, suit: str) -> int:
         my_cards = player.unplayed_cards
         partners_cards = player.partners_unplayed_cards
         if len(my_cards[suit]) > len(partners_cards[suit]):
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/data_classes.py` & `bfgcardplay-1.0.8/bfgcardplay/src/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 
 MODULE_COLOUR = 'yellow'
 
 
 class Cards():
     """A class representing a set of cards."""
-    def __init__(self, input: list[str] | list[Card]| Hand):
+    def __init__(self, input: list[str] | list[Card] | Hand):
         self.list = []
         self.longest_suit = None
         by_suit = {suit: [] for key, suit in SUITS.items()}
         by_suit_name = {key: [] for key, suit in SUITS.items()}
         self.by_suit = {**by_suit, **by_suit_name}
         self._value = 0
         self._create(input)
 
     def count(self) -> int:
         """Return the number of cards."""
         return len(self.list)
 
-    def _create(self, input: list[str] | list[Card]| Hand):
+    def _create(self, input: list[str] | list[Card] | Hand):
         """Create a set of cards"""
         if isinstance(input, Hand):
             cards = input.cards
         elif not isinstance(input, list):
             raise TypeError('Cards must be a list of cards')
         else:
             cards = input
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/declarer_play.py` & `bfgcardplay-1.0.8/bfgcardplay/src/declarer_play.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,21 +130,23 @@
     elif our_card_count == 8:
         return _missing_king_with_eight_cards(player, suit)
     elif 5 <= our_card_count <= 8:
         return _missing_king_with_five_to_eight_cards(player, suit)
 
     return None
 
+
 def _missing_king_with_eleven_cards(player, suit):
     my_cards = player.unplayed_cards[suit]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
     if ace in my_cards:
         return log(inspect.stack(), ace)
     return log(inspect.stack(), my_cards[-1])
 
+
 def _missing_king_with_ten_cards(player, suit):
     my_cards = player.unplayed_cards[suit]
     partners_cards = player.partners_unplayed_cards[suit]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
 
     # Partner holds A and Q
     if ace in partners_cards and queen in partners_cards:
@@ -163,14 +165,15 @@
         return log(inspect.stack(), my_cards[-1])
 
     # A and Q in this hand
     if ace in my_cards and queen in my_cards:
         return None
     return None
 
+
 def _missing_king_with_nine_cards(player, suit):
     my_cards = player.unplayed_cards[suit]
     partners_cards = player.partners_unplayed_cards[suit]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
     # Partner holds A and Q and this hand holds JT
     if (ace in partners_cards and queen in partners_cards and
             jack in my_cards and ten in my_cards):
@@ -190,23 +193,25 @@
         return log(inspect.stack(), ace)
 
     # Partner holds A
     if ace in partners_cards:
         return log(inspect.stack(), my_cards[-1])
     return None
 
+
 def _missing_king_with_eight_cards(player, suit):
     my_cards = player.unplayed_cards[suit]
     partners_cards = player.partners_unplayed_cards[suit]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
     # Partner holds A and Q
     if ace in partners_cards and queen in partners_cards:
         return log(inspect.stack(), my_cards[-1])
     return None
 
+
 def _missing_king_with_five_to_eight_cards(player, suit):
     my_cards = player.unplayed_cards[suit]
     partners_cards = player.partners_unplayed_cards[suit]
     # We hold AQJT9
     our_cards = my_cards + partners_cards
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
     nine = Card('9', suit)
@@ -300,11 +305,12 @@
             else:
                 return log(inspect.stack(), my_suit_cards[-1])
 
     for card in my_suit_cards[::-1]:
         if player.is_winner_declarer(card):
             return log(inspect.stack(), card)
         else:
-            manager.card_to_play[player.partner_seat] = player.partners_unplayed_cards[suit.name][-1]
+            partners_cards = player.partners_unplayed_cards[suit.name]
+            manager.card_to_play[player.partner_seat] = partners_cards[-1]
             return log(inspect.stack(), my_suit_cards[0])
     print(colored(f'missing_queen return None {suit}', MODULE_COLOUR))
     return None
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/defender_play.py` & `bfgcardplay-1.0.8/bfgcardplay/src/defender_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/first_seat.py` & `bfgcardplay-1.0.8/bfgcardplay/src/first_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer.py` & `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         if player.trump_suit and not player.opponents_trumps:
             long_suits = player.partnership_long_suits()
             for suit in long_suits:
                 if player.can_lead_toward_tenace(suit):
                     return Suit(suit)
 
-        return(player.longest_suit)
+        return player.longest_suit
 
     def _select_suit_for_nt_contract(self, manager) -> Suit:
         """Return the trick lead suit for the declarer in  a suit contract."""
         player = self.player
 
         winners = player.get_winners()
         target = player.declarers_target
@@ -147,15 +147,16 @@
         long_suits_to_develop = []
 
         lead_to_this_hand = False
         for suit_name in suits_to_develop:
             declarers_suit_cards = player.declarers_suit_cards[suit_name]
             dummys_suit_cards = player.dummys_suit_cards[suit_name]
             total_cards = len(declarers_suit_cards) + len(dummys_suit_cards)
-            if (total_cards >= 6 and (len(declarers_suit_cards) >= 4 or len(dummys_suit_cards) >= 4)):
+            if (total_cards >= 6 and
+                    (len(declarers_suit_cards) >= 4 or len(dummys_suit_cards) >= 4)):
                 long_suits_to_develop.append(suit_name)
                 my_touching_honours = player.hand.touching_honours()
                 partner_touching_honours = player.partners_hand.touching_honours()
                 for suit_name in suits_to_develop:
 
                     suit_cards = player.partners_suit_cards[suit_name]
                     if player.get_suit_tenaces(suit_cards):
@@ -179,15 +180,16 @@
                     entry = partners_entries[suit_name][0]
                     break
         if entry:
             if suit_to_develop:
                 manager.suit_to_develop[player.declarer] = suit_to_develop
                 manager.suit_to_develop[player.dummy] = suit_to_develop
                 manager.card_to_play[player.partner_seat].append(entry)
-                manager.card_to_play[player.partner_seat].append(player.partners_suit_cards[suit_to_develop][-1])
+                card = player.partners_suit_cards[suit_to_develop][-1]
+                manager.card_to_play[player.partner_seat].append(card)
                 manager.card_to_play[player.seat].append(player.suit_cards[entry.suit.name][-1])
                 return Suit(suit_to_develop)
         return None
 
     def _select_lead_card(self, manager, suit: Suit) -> Card:
         """Return the selected lead card for declarer."""
         player = self.player
@@ -267,15 +269,16 @@
         """Return True if declarer should draw trumps."""
         player = self.player
         if not player.trump_cards:
             return False
 
         declarers_trumps = Cards(player.declarers_hand.cards).by_suit[player.trump_suit]
         dummys_trumps = Cards(player.dummys_hand.cards).by_suit[player.trump_suit]
-        if len(declarers_trumps) + len(dummys_trumps) <= 7 and max(len(declarers_trumps), len(dummys_trumps)) == 4:
+        if (len(declarers_trumps) + len(dummys_trumps) <= 7 and
+                max(len(declarers_trumps), len(dummys_trumps)) == 4):
             return False
 
         declarers_trumps = player.unplayed_cards_by_suit(player.trump_suit, player.declarer)
         dummys_trumps = player.unplayed_cards_by_suit(player.trump_suit, player.dummy)
         if len(declarers_trumps) + len(dummys_trumps) >= 9:  # TODO too simplistic - determine losers first
             return True
 
@@ -296,15 +299,15 @@
             # else:
             #     short_suit_cards = player.unplayed_cards_by_suit(suit, player.declarer)
 
             declarers_cards = player.unplayed_cards_by_suit(suit, player.declarer)
             dummys_cards = player.unplayed_cards_by_suit(suit, player.dummy)
             suit_cards = declarers_cards + dummys_cards
 
-            if not(Card('A', suit.name) in suit_cards or Card('K', suit.name) in suit_cards):
+            if (Card('A', suit.name) not in suit_cards or Card('K', suit.name) in suit_cards):
                 return False
         return True
 
     def _long_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on length (long)."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name in SUITS}
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_nt.py` & `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_nt.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_suit.py` & `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_declarer_suit.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
                         card = player.unplayed_cards[suit_to_develop.name][0]
                         return log(inspect.stack(), card)
         return None
 
     def _select_suit(self) -> Suit:
         """Return the trick lead suit for the declarer in  a suit contract."""
         player = self.player
-        dashboard = player.dashboard
         manager = global_vars.manager
 
         # Draw trumps?
         can_draw_trumps = self._can_draw_trumps()
         if player.opponents_trumps and can_draw_trumps:
             return log(inspect.stack(), player.trump_suit)
 
@@ -149,15 +148,15 @@
             return suit
 
         # Select best suit
         score_reasons = self._get_score_reasons()
         best_suit = self._best_suit(score_reasons)
         return log(inspect.stack(), best_suit)
 
-    def _get_score_reasons(self) ->dict[str, int]:
+    def _get_score_reasons(self) -> dict[str, int]:
         controls = self.player.get_controls()
         score_reasons = {
             'trumps': self._deprecate_trumps(),
             'shortage': self._shortage_score(controls),
             'void': self._deprecate_suits(),
             'all_winners': self._all_winners_score(),
             'frozen': self._frozen_suits(),
@@ -250,15 +249,14 @@
         for suit in SUITS:
             can_lead_to_dummy = (player.touching_honours_in_hand(player.dummys_hand, suit) and
                                  player.unplayed_cards[suit])
             if player.touching_honours_in_hand(player.hand, suit) or can_lead_to_dummy:
                 return log(inspect.stack(), Suit(suit))
         return None
 
-
     def _update_manager_with_threats(self):
         player = self.player
         dashboard = player.dashboard
         manager = global_vars.manager
         for suit, threat_cards in dashboard.threats.items():
             ace = Card('A', suit)
             king = Card('K', suit)
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/src/first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat.py` & `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         elif player.trump_cards:
             for card in player.trump_cards[::-1]:
                 if card.value + 13 > values[2]:
                     log(inspect.stack(), f'{card}')
                     return card
         return None
 
-    def _second_player_winning_trick(self, cards: list[Card], trick: Trick, trumps: Denomination) -> bool:
+    def _second_player_winning_trick(self, cards: list[Card],
+                                     trick: Trick, trumps: Denomination) -> bool:
         """Return True if the second player is winning the trick."""
         values = trick_card_values(trick, trumps)
         if values[1] > values[0] and values[1] > values[2]:
             return True
         return False
 
     def can_win_trick(self, player, card) -> bool:
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_declarer.py` & `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/src/fourth_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/manager.py` & `bfgcardplay-1.0.8/bfgcardplay/src/manager.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead.py` & `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .opening_lead_card import opening_lead_card
 from .opening_lead_suit import opening_lead_suit
 
 import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'green'
 
+
 def opening_lead(board):
     """Return the proposed opening lead for the board."""
 
     manager = global_vars.manager
     manager.initialise()
 
     if not board.contract.declarer:
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_card.py` & `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         return None
     for index in range(len(cards) - 2):
         card = _find_internal_sequence(cards, index)
         if card:
             return card
     return None
 
+
 def _find_internal_sequence(cards, index):
     for offset in range(2, 5):  # Check Q, J and T
         if (cards[index].value == cards[index+1].value + offset and
                 cards[index+1].value == cards[index+2].value + 1 and
                 cards[index+1].is_honour):
             return cards[index+1]
     return None
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_suit.py` & `bfgcardplay-1.0.8/bfgcardplay/src/opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/player.py` & `bfgcardplay-1.0.8/bfgcardplay/src/player.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/second_seat.py` & `bfgcardplay-1.0.8/bfgcardplay/src/second_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/second_seat_declarer.py` & `bfgcardplay-1.0.8/bfgcardplay/src/second_seat_declarer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import inspect
 
 from ..logger import log
 
 from bridgeobjects import Card, SUITS, Suit
 from bfgdealer import Trick
 from .player import Player
-from .utilities import get_list_of_best_scores, get_suit_strength, play_to_unblock
+from .utilities import get_list_of_best_scores, get_suit_strength
 from .second_seat import SecondSeat
 import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'green'
 
 
 class SecondSeatDeclarer(SecondSeat):
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/second_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/src/second_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/suggested_card.py` & `bfgcardplay-1.0.8/bfgcardplay/src/suggested_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/third_seat.py` & `bfgcardplay-1.0.8/bfgcardplay/src/third_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/third_seat_declarer.py` & `bfgcardplay-1.0.8/bfgcardplay/src/third_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/third_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/src/third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/src/utilities.py` & `bfgcardplay-1.0.8/bfgcardplay/src/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/tests/test_first_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/tests/test_first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_card.py` & `bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_suit.py` & `bfgcardplay-1.0.8/bfgcardplay/tests/test_opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/tests/test_third_seat_defender.py` & `bfgcardplay-1.0.8/bfgcardplay/tests/test_third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay/tests/test_utilities.py` & `bfgcardplay-1.0.8/bfgcardplay/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.0.8/bfgcardplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.7
+Version: 1.0.8
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
-Version 1.0.7 29 Jun 2023
+Version 1.0.8 29 Jun 2023
 
-1. xxx
+1. Linting
 
 ------
 
 Version 1.0.7 29 Jun 2023
 
-1. xxx
+1. General modifications and enhanced testing
 
 ------
 
 Version 1.0.6 26 Jun 2023
 
 1. xxx
```

### Comparing `bfgcardplay-1.0.7/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.0.8/bfgcardplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.7/setup.py` & `bfgcardplay-1.0.8/setup.py`

 * *Files identical despite different names*

