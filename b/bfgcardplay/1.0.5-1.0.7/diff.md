# Comparing `tmp/bfgcardplay-1.0.5.tar.gz` & `tmp/bfgcardplay-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.0.5.tar", last modified: Tue Jun 20 15:19:49 2023, max compression
+gzip compressed data, was "bfgcardplay-1.0.7.tar", last modified: Thu Jun 29 13:59:58 2023, max compression
```

## Comparing `bfgcardplay-1.0.5.tar` & `bfgcardplay-1.0.7.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 15:19:49.584781 bfgcardplay-1.0.5/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3878 2023-06-20 15:19:49.584781 bfgcardplay-1.0.5/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.5/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 15:19:49.578114 bfgcardplay-1.0.5/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      227 2021-10-01 11:09:27.000000 bfgcardplay-1.0.5/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-20 15:18:38.000000 bfgcardplay-1.0.5/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.5/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 15:19:49.584781 bfgcardplay-1.0.5/bfgcardplay/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-12-22 17:41:36.000000 bfgcardplay-1.0.5/bfgcardplay/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2021-12-22 17:41:36.000000 bfgcardplay-1.0.5/bfgcardplay/source/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2347 2023-01-20 16:29:14.000000 bfgcardplay-1.0.5/bfgcardplay/source/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19631 2023-01-05 11:19:24.000000 bfgcardplay-1.0.5/bfgcardplay/source/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4714 2023-05-11 08:43:28.000000 bfgcardplay-1.0.5/bfgcardplay/source/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12323 2023-02-10 13:38:26.000000 bfgcardplay-1.0.5/bfgcardplay/source/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4022 2023-06-20 11:36:59.000000 bfgcardplay-1.0.5/bfgcardplay/source/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9806 2023-02-10 13:38:26.000000 bfgcardplay-1.0.5/bfgcardplay/source/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16175 2023-02-03 17:43:49.000000 bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17044 2023-05-11 08:43:28.000000 bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    22029 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2791 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5957 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5359 2023-06-20 11:36:59.000000 bfgcardplay-1.0.5/bfgcardplay/source/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2021-12-22 17:41:36.000000 bfgcardplay-1.0.5/bfgcardplay/source/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3966 2022-01-04 17:55:18.000000 bfgcardplay-1.0.5/bfgcardplay/source/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      667 2022-06-27 17:02:41.000000 bfgcardplay-1.0.5/bfgcardplay/source/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-01-20 16:49:44.000000 bfgcardplay-1.0.5/bfgcardplay/source/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43277 2023-06-20 15:18:38.000000 bfgcardplay-1.0.5/bfgcardplay/source/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    24518 2023-05-11 08:43:28.000000 bfgcardplay-1.0.5/bfgcardplay/source/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3052 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9977 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7234 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3672 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2428 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17717 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    13898 2023-02-02 07:57:08.000000 bfgcardplay-1.0.5/bfgcardplay/source/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1483 2023-01-20 11:07:39.000000 bfgcardplay-1.0.5/bfgcardplay/source/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 15:19:49.584781 bfgcardplay-1.0.5/bfgcardplay/test/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-10-25 15:12:22.000000 bfgcardplay-1.0.5/bfgcardplay/test/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11741 2023-01-20 16:48:53.000000 bfgcardplay-1.0.5/bfgcardplay/test/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14967 2023-01-20 17:51:03.000000 bfgcardplay-1.0.5/bfgcardplay/test/test_opening_lead_suit.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 15:19:49.578114 bfgcardplay-1.0.5/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3878 2023-06-20 15:19:49.000000 bfgcardplay-1.0.5/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1434 2023-06-20 15:19:49.000000 bfgcardplay-1.0.5/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-20 15:19:49.000000 bfgcardplay-1.0.5/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-20 15:19:49.000000 bfgcardplay-1.0.5/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-20 15:19:49.584781 bfgcardplay-1.0.5/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.5/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4007 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.7/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.468568 bfgcardplay-1.0.7/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      215 2023-06-29 13:52:00.000000 bfgcardplay-1.0.7/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.7/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/bfgcardplay/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2305 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    19594 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4661 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12247 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3976 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9753 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16135 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17433 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    21989 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16445 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1989 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6553 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5369 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      664 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43274 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    24438 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3025 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    10003 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7231 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3638 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1880 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17664 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14321 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6542 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/src/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/bfgcardplay/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      558 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    15003 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      587 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/test_utilities.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      294 2023-06-29 13:57:08.000000 bfgcardplay-1.0.7/bfgcardplay/tests/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:59:58.468568 bfgcardplay-1.0.7/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4007 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1589 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-29 13:59:58.000000 bfgcardplay-1.0.7/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 13:59:58.475234 bfgcardplay-1.0.7/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.7/setup.py
```

### Comparing `bfgcardplay-1.0.5/PKG-INFO` & `bfgcardplay-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.5
+Version: 1.0.7
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.7 29 Jun 2023
+
+1. xxx
+
+------
+
+Version 1.0.7 29 Jun 2023
+
+1. xxx
+
+------
+
+Version 1.0.6 26 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.5 20 Jun 2023
 
 1. Fix bug in opening suit if void in suit
 
 ------
 
 Version 1.0.4 20 Jun 2023
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/logger.py` & `bfgcardplay-1.0.7/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/card_player_components.py` & `bfgcardplay-1.0.7/bfgcardplay/src/card_player_components.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/cards.py` & `bfgcardplay-1.0.7/bfgcardplay/src/cards.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 """Common functionality for cardplay."""
 
-# from types import List
+# from types import list
 from termcolor import cprint
 
-from typing import List, Union
 import random
 
 from bridgeobjects import Suit, Card, SUITS
 from bfgsupport import Hand
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .utilities import get_list_of_best_scores
 
 global_vars.initialize()
 
 MODULE_COLOUR = 'magenta'
 
 
 class Cards():
     """A class representing a set of cards."""
-    def __init__(self, input: Union[List[str], List[Card], Hand]):
+    def __init__(self, input: list[str] | list[Card] | Hand]):
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
 
-    def _create(self, input: Union[List[str], List[Card], Hand]):
+    def _create(self, input: list[str] | list[Card] | Hand]):
         """Create a set of cards"""
         if isinstance(input, Hand):
             cards = input.cards
         elif not isinstance(input, list):
             raise TypeError('Cards must be a list of cards')
         else:
             cards = input
@@ -54,15 +53,15 @@
             suit_name = suit.name
             self.by_suit[suit].append(card)
             self.by_suit[suit_name].append(card)
             self._value += card.value
         self.longest_suit = self._longest_suit()
 
     @staticmethod
-    def sort_cards(cards: List[Card]) -> List[Card]:
+    def sort_cards(cards: list[Card]) -> list[Card]:
         """Return a sorted list of cards."""
         return sorted(cards, reverse=True)
 
     def _longest_suit(self) -> Suit:
         """Return the suit with most cards."""
         suit_dict = {}
         for suit, card_list in self.by_suit.items():
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/dashboard.py` & `bfgcardplay-1.0.7/bfgcardplay/src/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Provide the Dashboard class for bfgcardplay."""
 
-from typing import Dict, List, Tuple
 from termcolor import cprint
 from dataclasses import dataclass
 
 from bridgeobjects import Hand, Card, Suit, SUITS, RANKS
 from .data_classes import SuitCards, CardArray
 
 SPLIT_PROBABILITIES = {
@@ -73,15 +72,15 @@
         cprint(f'{"threats":<10}{self.threats}', MODULE_COLOUR)
         cprint(f'{"winners":<10}{self.winners}', MODULE_COLOUR)
         cprint(f'{"suit_lens":<10}{self.suit_lengths}', MODULE_COLOUR)
         # print(f'{"threats":<10}{self.extra_winners_length}', MODULE_COLOUR)
         # print(f'{"threats":<10}{self.extra_winners_strength}', MODULE_COLOUR)
         return ''
 
-    def _get_current_sure_tricks(self) -> List[Card]:
+    def _get_current_sure_tricks(self) -> list[Card]:
         """Return a list of certain winners based on unplayed cards."""
         player = self.player
         sure_tricks = []
         declarers_cards = player.unplayed_cards
         dummys_cards = player.partners_unplayed_cards
         for suit in SUITS:
             declarer_suit_cards = [card for card in declarers_cards[suit]]
@@ -89,45 +88,45 @@
             our_cards = CardArray.sort_cards(declarer_suit_cards + dummy_suit_cards)
             our_length = max(len(declarer_suit_cards), len(dummy_suit_cards))
             for card in our_cards[:our_length]:
                 if player.is_winner_declarer(card, player.board.tricks[-1]):
                     sure_tricks.append(card)
         return sure_tricks
 
-    def _get_current_probable_tricks(self) -> Tuple[Dict[str, List[Card]]]:
+    def _get_current_probable_tricks(self) -> tuple[dict[str, list[Card]]]:
         """Return a dict of probable winners by suit based on unplayed cards."""
         opponents_length = {
             8: 5,
             7: 4,
             6: 4,
             5: 3,
             4: 3,
             3: 2,
             2: 2,
             1: 1,
             0: 0,
         }
         return self._current_trick_calculation(opponents_length)
 
-    def _get_current_possible_tricks(self) -> Tuple[Dict[str, List[Card]]]:
+    def _get_current_possible_tricks(self) -> tuple[dict[str, list[Card]]]:
         """Return a dict of possible winners by suit based on unplayed cards."""
         opponents_length = {
             8: 4,
             7: 4,
             6: 3,
             5: 3,
             4: 2,
             3: 2,
             2: 1,
             1: 1,
             0: 0,
         }
         return self._current_trick_calculation(opponents_length)
 
-    def _current_trick_calculation(self, opponents_length: Dict[int, int]) -> Tuple[Dict[str, List[Card]]]:
+    def _current_trick_calculation(self, opponents_length: dict[int, int]) -> tuple[dict[str, list[Card]]]:
         """Return a dict of winners by suit based on unplayed cards."""
         player = self.player
         probable_tricks = []
         declarers_cards = player.unplayed_cards
         dummys_cards = player.partners_unplayed_cards
         opponents_cards = player.opponents_unplayed_cards
         for suit in SUITS:
@@ -180,15 +179,15 @@
                 honours = SuitCards(suit).cards('K', 'T')
                 for hand in [declarers_cards[suit], dummys_cards[suit]]:
                     for index, card in enumerate(honours):
                         if check_card(self, hand, card, 2+index):
                             possible_promotions.append(card)
         return possible_promotions
 
-    def _get_current_entries(self) -> Tuple[Dict[str, List[Card]]]:
+    def _get_current_entries(self) -> tuple[dict[str, list[Card]]]:
         """Return a dict of probable entries by suit based on unplayed cards."""
         player = self.player
         my_entries = {suit: [] for suit in SUITS}
         partners_entries = {suit: [] for suit in SUITS}
         for suit in SUITS:
             my_cards = player. unplayed_cards[suit]
             partners_cards = player.partners_unplayed_cards[suit]
@@ -208,22 +207,22 @@
     #         cards = my_cards[suit]
     #         if cards:
     #             if (player.is_winner_declarer(cards[0]) and
     #                     cards[0].value > partners_cards[suit][-1].value):
     #                 entries[suit] = cards[0]
     #     return entries
 
-    def _get_threats(self) -> Dict[str, Card]:
+    def _get_threats(self) -> dict[str, Card]:
         """Return a dict of cards by suit that threaten players cards."""
         if self.player.trump_suit:
             return self._get_threats_suit_contract()
         else:
             return self._get_threats_nt_contract()
 
-    def _get_threats_nt_contract(self) -> Dict[str, Card]:
+    def _get_threats_nt_contract(self) -> dict[str, Card]:
         """Return a dict of cards by suit that threaten players cards."""
         player = self.player
 
         threats = {suit: [] for suit in SUITS}
         ranks = [rank for rank in RANKS]
         ranks.reverse()
         sorted_ranks = ranks[:-1]
@@ -254,15 +253,15 @@
                     # threats only in long hand
                     if index + 1 >= len(long_cards):
                         break
                 if len(opponents_cards) <= index + 1:
                     break
         return threats
 
-    def _get_threats_suit_contract(self) -> Dict[str, Card]:
+    def _get_threats_suit_contract(self) -> dict[str, Card]:
         """Return a dict of cards by suit that threaten players cards."""
         player = self.player
         (long_hand, short_hand) = self.get_long_short_trump_hands()
         unplayed_cards = player.cards_by_suit(long_hand)
         long_cards = unplayed_cards[player.trump_suit.name]
 
         threats = {suit: [] for suit in SUITS}
@@ -302,19 +301,19 @@
                     # threats only in long hand
                     if index + 1 >= len(long_cards):
                         break
                 if len(opponents_cards) <= index + 1:
                     break
         return threats
 
-    def get_long_short_trump_hands(self) -> Tuple[Hand, Hand]:
+    def get_long_short_trump_hands(self) -> tuple[Hand, Hand]:
         """Return the  hands for long and short trump hand between player and partner."""
         return self.get_long_short_hands(self.player.trump_suit)
 
-    def get_long_short_hands(self, suit: Suit) -> Tuple[Hand, Hand]:
+    def get_long_short_hands(self, suit: Suit) -> tuple[Hand, Hand]:
         """Return the  hands for long and short hand between player and partner."""
         player = self.player
         my_unplayed_cards = player.unplayed_cards
         partners_unplayed_cards = player.partners_unplayed_cards
         if len(my_unplayed_cards[suit.name]) >= len(partners_unplayed_cards[suit.name]):
             return (player.hand, player.partners_hand)
         else:
@@ -332,30 +331,30 @@
         #     long_unplayed_cards = player.unplayed_cards
         #     short_unplayed_cards = player.partners_unplayed_cards
         # else:
         #     short_unplayed_cards = player.unplayed_cards
         #     long_unplayed_cards = player.partners_unplayed_cards
         # return (long_unplayed_cards, short_unplayed_cards)
 
-    def _get_losers(self) -> Dict[str, Card]:
+    def _get_losers(self) -> dict[str, Card]:
         """Return a dict of losing cards by suit in players cards."""
         player = self.player
         (long_hand, short_hand) = self.get_long_short_trump_hands()
         unplayed_cards = player.cards_by_suit(long_hand)
         long_cards = unplayed_cards[player.trump_suit.name]
 
         losers = {suit: [] for suit in SUITS}
         ranks = [rank for rank in RANKS]
         ranks.reverse()
         sorted_ranks = ranks[:-1]
 
         for suit in SUITS:
             our_cards = player.our_unplayed_cards[suit]
 
-    def _get_suit_winners(self) -> Dict[str, Card]:
+    def _get_suit_winners(self) -> dict[str, Card]:
         """Return a dict of cards by suit that are certain winners."""
         player = self.player
         winners = {suit: [] for suit in SUITS}
         our_cards = player.our_unplayed_cards
         opponents_cards = player.opponents_unplayed_cards
         for suit in SUITS:
             our_length = self._get_our_length(player, suit)
@@ -364,15 +363,15 @@
                     if opponents_cards[suit]:
                         if card.value > opponents_cards[suit][0].value:
                             winners[suit].append(card)
                     else:
                         winners[suit].append(card)
         return winners
 
-    def _get_split_winners(self) -> Dict[str, Card]:
+    def _get_split_winners(self) -> dict[str, Card]:
         """Return a dict of cards by suit that are certain winners depending on splits."""
         player = self.player
         opponents_cards = player.opponents_unplayed_cards
         split_winners = {suit: [] for suit in SUITS}
         for suit in SUITS:
             if len(opponents_cards[suit]) in SPLITS:
                 splits = SPLITS[len(opponents_cards[suit])]
@@ -407,15 +406,15 @@
     def _get_our_length(player: object, suit: str) -> int:
         my_cards = player.unplayed_cards
         partners_cards = player.partners_unplayed_cards
         if len(my_cards[suit]) > len(partners_cards[suit]):
             return len(my_cards[suit])
         return len(partners_cards[suit])
 
-    def _suit_lengths(self) -> Dict[str, int]:
+    def _suit_lengths(self) -> dict[str, int]:
         """Return a dict of suit_lengths."""
         player = self.player
         suit_lengths = {suit: [] for suit in SUITS}
         our_cards = player.our_unplayed_cards
         for suit in SUITS:
             suit_lengths[suit] = len(our_cards[suit])
         return suit_lengths
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/data_classes.py` & `bfgcardplay-1.0.7/bfgcardplay/src/data_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from termcolor import cprint
-from typing import Tuple, List, Union
 import random
 
 from bridgeobjects import Suit, Card, RANKS, SUITS
 from bfgbidding import Hand
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 from .utilities import get_list_of_best_scores
 
 global_vars.initialize()
 
 
 MODULE_COLOUR = 'yellow'
 
 
 class Cards():
     """A class representing a set of cards."""
-    def __init__(self, input: Union[List[str], List[Card], Hand]):
+    def __init__(self, input: list[str] | list[Card]| Hand):
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
 
-    def _create(self, input: Union[List[str], List[Card], Hand]):
+    def _create(self, input: list[str] | list[Card]| Hand):
         """Create a set of cards"""
         if isinstance(input, Hand):
             cards = input.cards
         elif not isinstance(input, list):
             raise TypeError('Cards must be a list of cards')
         else:
             cards = input
@@ -51,15 +50,15 @@
             suit_name = suit.name
             self.by_suit[suit].append(card)
             self.by_suit[suit_name].append(card)
             self._value += card.value
         self.longest_suit = self._longest_suit()
 
     @staticmethod
-    def sort_cards(cards: List[Card]) -> List[Card]:
+    def sort_cards(cards: list[Card]) -> list[Card]:
         """Return a sorted list of cards."""
         return sorted(cards, reverse=True)
 
     def _longest_suit(self) -> Suit:
         """Return the suit with most cards."""
         suit_dict = {}
         for suit, card_list in self.by_suit.items():
@@ -89,15 +88,15 @@
         self.seven = Card('7', suit)
         self.six = Card('6', suit)
         self.five = Card('5', suit)
         self.four = Card('4', suit)
         self.three = Card('3', suit)
         self.two = Card('2', suit)
 
-    def cards(self, top_rank: str = '', bottom_rank: str = '') -> Tuple[Card]:
+    def cards(self, top_rank: str = '', bottom_rank: str = '') -> tuple[Card]:
         """Return a tuple of the cards requested."""
         if not top_rank:
             top_rank = 'A'
         if not bottom_rank:
             bottom_rank = '2'
 
         cards = []
@@ -120,15 +119,15 @@
         for rank in ranks:
             cards.append(Card(rank, self.suit))
         return cards
 
 
 class CardArray():
     """Data structure for dashboard analyses"""
-    def __init__(self, cards: List[Card]):
+    def __init__(self, cards: list[Card]):
         self.cards = self.sort_cards(cards)
         self.suits = self._suits_from_cards()
 
     def _suits_from_cards(self):
         """Return a dict of suit cards."""
         suits = {}
         for card in self.cards:
@@ -145,10 +144,10 @@
 
     def __repr__(self):
         # cprint(f'{self.cards}', MODULE_COLOUR)
         # cprint(f'{self.suits}', MODULE_COLOUR)
         return ''
 
     @staticmethod
-    def sort_cards(cards: List[Card]) -> List[Card]:
+    def sort_cards(cards: list[Card]) -> list[Card]:
         """Return a sorted list of cards."""
         return sorted(cards, reverse=True)
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/declarer_play.py` & `bfgcardplay-1.0.7/bfgcardplay/src/declarer_play.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Methods to support declarer play."""
-from typing import Union
 from termcolor import colored
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import Card, Suit, CARD_VALUES
 from bfgdealer import Trick
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player
 from .dashboard import SuitCards
 
 MODULE_COLOUR = 'magenta'
 
 
-def card_combinations(player: Player, suit: str = '') -> Union[Card, None]:
+def card_combinations(player: Player, suit: str = '') -> Card | None:
     """Return a card from a defined combination, or None."""
     trick = player.board.tricks[-1]
     if not suit:
         suit = trick.suit.name
     opponents_cards = player.opponents_unplayed_cards[suit]
     our_cards = player.our_unplayed_cards[suit]
     suit_cards = SuitCards(suit).cards('A', 'J')
@@ -35,15 +34,15 @@
             queen in opponents_cards):
         return missing_queen_new(player, suit)
     return None
 
 
 def lead_to_find_missing_ace(player: Player,
                              suit: Suit,
-                             trick: Union[Trick, None] = None) -> Union[Card, None]:
+                             trick: Trick | None = None) -> Card | None:
     """Return the appropriate card if missing the ace."""
     manager = global_vars.manager
     my_suit_cards = player.suit_cards[suit]
     partners_suit_cards = player.partners_suit_cards[suit]
     max_length = max(len(my_suit_cards), len(partners_suit_cards))
     if max_length >= 4:
         if (Card('K', suit.name) in player.our_unplayed_cards[suit.name] and
@@ -72,15 +71,15 @@
         my_entry_cards = player.suit_cards[entry_suit]
         if my_entry_cards:
             manager.win_trick[player.partner_seat] = True
             return my_entry_cards[-1]
     return None
 
 
-def missing_king(player: Player, suit: Suit) -> Union[Card, None]:
+def missing_king(player: Player, suit: Suit) -> Card | None:
     """Return the appropriate card if missing the king."""
     manager = global_vars.manager
     my_suit_cards = player.suit_cards[suit]
     partners_suit_cards = player.partners_suit_cards[suit]
     my_entries = player.get_entries_in_other_suits(player.hand, suit)
     partners_entries = player.get_entries_in_other_suits(player.partners_hand, suit)
 
@@ -112,15 +111,15 @@
         else:
             return log(inspect.stack(), my_suit_cards[0])
 
     print(colored(f'missing_king return None {suit}', MODULE_COLOUR))
     return None
 
 
-def missing_king_new(player: Player, suit: str) -> Union[Card, None]:
+def missing_king_new(player: Player, suit: str) -> Card | None:
     """Return the appropriate card if missing the king."""
     manager = global_vars.manager
     manager.set_missing_king(player.seat, suit, True)
 
     our_card_count = len(player.our_cards[suit])
     if our_card_count >= 11:
         return _missing_king_with_eleven_cards(player, suit)
@@ -216,15 +215,15 @@
         if len(my_cards) > 1:
             return log(inspect.stack(), my_cards[1])
         else:
             return log(inspect.stack(), my_cards[-1])
     return None
 
 
-def missing_queen_new(player: Player, suit: str) -> Union[Card, None]:
+def missing_queen_new(player: Player, suit: str) -> Card | None:
     """Return the appropriate card if missing the queen."""
     trick = player.board.tricks[-1]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
     my_cards = player.unplayed_cards[suit]
     partners_cards = player.partners_unplayed_cards[suit]
 
     # hand holds AJ and partner K
@@ -250,15 +249,15 @@
     elif ace in my_cards and trick.cards and trick.cards[0] != king:
         return log(inspect.stack(), ace)
     return None
 
 
 def missing_queen(player: Player,
                   suit: Suit,
-                  trick: Union[Trick, None] = None) -> Union[Card, None]:
+                  trick: Trick | None = None) -> Card | None:
     """Return the appropriate card if missing the queen."""
     manager = global_vars.manager
     my_suit_cards = player.suit_cards[suit]
     partners_suit_cards = player.partners_suit_cards[suit]
     (ace, king, queen, jack, ten) = SuitCards(suit).cards('A', 'T')
 
     if not partners_suit_cards:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/defender_play.py` & `bfgcardplay-1.0.7/bfgcardplay/src/defender_play.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Methods to support Defender play."""
-from typing import List, Union
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import Card, Suit, CARD_VALUES, SUITS
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .utilities import other_suit_for_signals
 from .player import Player
 
 MODULE_COLOUR = 'cyan'
 
 
 def deduce_partner_void_in_trumps(player: Player) -> bool:
@@ -28,30 +27,30 @@
 
 
 def dummy_is_short_trump_hand(player: Player) -> bool:
     """Return True if dummy is short trump hand."""
     return len(player.hands[player.dummy].cards_by_suit[player.trump_suit.name]) <= 4
 
 
-def get_hilo_signal_card(player, cards: List[Card]) -> Card:
+def get_hilo_signal_card(player, cards: list[Card]) -> Card:
     """Return a signal card denoting even/odd"""
     manager = global_vars.manager
     trick = player.board.tricks[-1]
     if len(cards) % 2 == 0:
         if len(cards) == 2:
             if not cards[-2].is_honour and cards[-2].rank != 'T':
                 manager.set_even_odd(player.seat, trick.suit.name, 0)
                 return log(inspect.stack(), cards[-2])
             return log(inspect.stack(), cards[-1])
 
     manager.set_even_odd(player.seat, trick.suit.name, 1)
     return log(inspect.stack(), cards[-1])
 
 
-def signal_card(player: Player, manager: object, suit: Suit) -> Union[Card, None]:
+def signal_card(player: Player, manager: object, suit: Suit) -> Card | None:
     """Signal suit preference."""
     if not manager.signal_card[player.seat]:
         suit_cards = player.suit_cards[suit.name]
         for card in suit_cards:
             if not card.is_honour:
                 manager.signal_card[player.seat] = card
                 return log(inspect.stack(), card)
@@ -66,15 +65,15 @@
             if suit_name != suit.name and suit_name != other_suit:
                 final_suit_cards = player.suit_cards[suit_name]
                 if final_suit_cards:
                     return log(inspect.stack(), final_suit_cards[-1])
     return None
 
 
-def surplus_card(player: Player) -> Union[Card, None]:
+def surplus_card(player: Player) -> Card | None:
     # Discard if more cards than the opposition
     for suit_name in SUITS:
         if player.unplayed_cards[suit_name]:
             card_count = len(player.unplayed_cards[suit_name])
             if card_count > len(player.total_unplayed_cards[suit_name]) - card_count:
                 return log(inspect.stack(), player.unplayed_cards[suit_name][-1])
     return None
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/first_seat.py` & `bfgcardplay-1.0.7/bfgcardplay/src/first_seat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ First seat card play."""
 
-from typing import List, Dict, Union, Tuple
 import random
 from termcolor import termcolor
 
 from bridgeobjects import SUITS, Card, Suit, CARD_NAMES
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player
 from .utilities import get_list_of_best_scores
 
 MODULE_COLOUR = 'red'
 
 
 class FirstSeat():
@@ -57,45 +56,45 @@
                     manager.set_suit_strategy(player.seat, player.trump_suit.name, '')
 
             suit = manager.suit_to_develop(player.seat)
             if suit:
                 if not player.unplayed_cards[suit]:
                     manager.set_suit_to_develop(player.seat, None)
 
-    def _deprecate_suits(self) -> List[Tuple[str, int]]:
+    def _deprecate_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on void."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         for suit in SUITS:
             if not self.player.suit_cards[suit]:
                 suit_scores[suit] -= self.VOID_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _partners_suit(self) -> List[Tuple[str, int]]:
+    def _partners_suit(self) -> list[tuple[str, int]]:
         """Assign score to suits based on it being suit partner led."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         partners_suit = self._get_partners_suit()
         if partners_suit and not partners_suit == self.player.trump_suit:
             suit_scores[partners_suit.name] += self.PARTNERS_SUIT_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _tenace_check(self) -> List[Tuple[str, int]]:
+    def _tenace_check(self) -> list[tuple[str, int]]:
         """Assign score to suits based on tenaces in dummy."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         dummy_tenaces = self.identify_dummy_tenaces()
         for suit in dummy_tenaces:
             if isinstance(suit, str):
                 if self.player.dummy_on_left:
                     # Lead through tenaces
                     suit_scores[suit] += self.TENACE_SCORE
                 elif self.player.dummy_on_right:
                     # Lead to tenaces
                     suit_scores[suit] -= self.TENACE_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _lead_through_strength(self) -> List[Tuple[str, int]]:
+    def _lead_through_strength(self) -> list[tuple[str, int]]:
         """Assign score to suits where you lead through or to strength."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
         if player.dummy_on_left:
             for suit, points in player.dummy_suit_strength.items():
                 if points >= 5:
                     suit_scores[suit] += self.STRENGTH_SCORE
@@ -106,15 +105,15 @@
                         suit_scores[suit] += self.STRENGTH_SCORE
                 else:
                     if suit != player.trump_suit.name:
                         if points <= 2:
                             suit_scores[suit] += self.STRENGTH_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _frozen_suits(self) -> List[Tuple[str, int]]:
+    def _frozen_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on frozen suits."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         frozen_suits = []
         for suit in SUITS:
             if self._frozen_suit(suit):
                 frozen_suits.append(suit)
         for suit in frozen_suits:
@@ -134,69 +133,69 @@
             for card in suit_cards:
                 if card.is_honour:
                     hand_honours += 1
         if dummy_honours == 1 and hand_honours == 1:
             return True
         return False
 
-    def _long_suits(self) -> List[Tuple[str, int]]:
+    def _long_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on length (long)."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         for suit in SUITS:
             cards = self.player.suit_cards[suit]
             number_cards = len(cards) - 4
             if number_cards > 0 and cards[0].value >= 12:
                 suit_scores[suit] = number_cards * self.LENGTH_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _short_suits(self) -> List[Tuple[str, int]]:
+    def _short_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on length (short)."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
         if player.trump_suit:
             if len(player.trump_cards) > 0:
                 for suit in SUITS:
                     number_cards = len(player.suit_cards[suit])
                     if 0 < number_cards < 3:
                         suit_scores[suit] = (2 - number_cards) * self.LENGTH_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _ruff_and_discard(self) -> List[Tuple[str, int]]:
+    def _ruff_and_discard(self) -> list[tuple[str, int]]:
         """Assign score to suits based on potential for ruff and discard."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         if len(self.player.dummys_suit_cards[self.player.trump_suit.name]) > 0:
             for suit in SUITS:
                 if len(self.player.dummys_suit_cards[suit]) == 0:
                     suit_scores[suit] -= self.RUFF_AND_DISCARD_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _get_partners_suit(self) -> Union[Suit, None]:
+    def _get_partners_suit(self) -> Suit | None:
         """Return partner's suit if this is 3rd hand on first lead."""
         trick_one = self.player.board.tricks[0]
         if trick_one.leader == self.player.partner_seat:
             opening_lead = trick_one.cards[0]
             if opening_lead.suit != self.player.trump_suit:
                 if opening_lead.value < 7 and self.player.suit_cards[opening_lead.suit.name]:
                     return opening_lead.suit
         return None
 
-    def identify_dummy_tenaces(self) -> List[Suit]:
+    def identify_dummy_tenaces(self) -> list[Suit]:
         """Return a list of suits with a tenace in dummy."""
         suits = []
         player = self.player
         for suit, tenace in player.dummy_suit_tenaces.items():
             if player.suit_cards[suit]:
                 if tenace and (player.trump_suit and not suit == player.trump_suit.name):
                     tenace_index = CARD_NAMES.index(tenace.name)
                     next_card_name = CARD_NAMES[tenace_index+1]
                     if Card(next_card_name) not in player.hand_cards.list:
                         suits.append(suit)
         return suits
 
-    def _best_suit(self, score_reasons: Dict[str, int]) -> Suit:
+    def _best_suit(self, score_reasons: dict[str, int]) -> Suit:
         """Return the best suit based on score."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
         for reason, suits in score_reasons.items():
             for suit in suits:
                 suit_scores[suit[0]] += suit[1]
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer.py` & `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # first_seat_declarer.py
 
 """ First seat card play for declarer."""
 
-from typing import List, Dict, Tuple
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, Suit
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player, Cards
 from .first_seat import FirstSeat
 
 MODULE_COLOUR = 'cyan'
 
 
 ALL_WINNERS = 5
@@ -133,15 +132,15 @@
         score_reasons['strength'] = self._suit_strength()
 
         # Select best suit
         best_suit = self._best_suit(score_reasons)
         # print(colored(f'{best_suit=} {score_reasons=}', 'red'))
         return best_suit
 
-    def _suits_to_develop(self, manager: object, controls: List[str]) -> List[str]:
+    def _suits_to_develop(self, manager: object, controls: list[str]) -> list[str]:
         """Return a list of suits to develop."""
         player = self.player
         suits_to_develop = []
         suit_to_develop = None
         for suit_name in SUITS:
             if not controls[suit_name]:
                 suits_to_develop.append(suit_name)
@@ -251,15 +250,15 @@
         for suit in winning_suits:
             suit_length = len(player.suit_cards[suit.name])
             if suit_length > max_length:
                 max_length = suit_length
                 long_suit = suit
         return long_suit
 
-    def _get_winning_suits(self, player: Player) -> List[Suit]:
+    def _get_winning_suits(self, player: Player) -> list[Suit]:
         """Return a list of winning suits."""
         winning_suits = []
         for suit_name, suit in SUITS.items():
             if suit != player.trump_suit:
                 if player.holds_all_winners_in_suit(suit):
                     winning_suits.append(suit)
         return winning_suits
@@ -301,30 +300,30 @@
             dummys_cards = player.unplayed_cards_by_suit(suit, player.dummy)
             suit_cards = declarers_cards + dummys_cards
 
             if not(Card('A', suit.name) in suit_cards or Card('K', suit.name) in suit_cards):
                 return False
         return True
 
-    def _long_suits(self) -> List[Tuple[str, int]]:
+    def _long_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on length (long)."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         length_score = self.LENGTH_SCORE
 
         for suit in SUITS:
             number_cards = len(player.our_cards[suit]) - len(player.opponents_cards[suit])
             if number_cards > 0:
                 if player.trump_suit:
                     if suit == player.trump_suit.name:
                         length_score = 0
                 suit_scores[suit] = number_cards * length_score
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    # def _frozen_suits(self) -> List[Tuple[str, int]]:
+    # def _frozen_suits(self) -> list[tuple[str, int]]:
     #     """Assign score to suits based on frozen suits."""
     #     player = self.player
     #     suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
     #     frozen_suits = []
     #     dummys_cards = player.board.hands[player.dummy].cards
     #     for suit, cards in player.get_cards_by_suit(dummys_cards).items():
     #         dummy_honours = 0
@@ -339,41 +338,41 @@
     #                     hand_honours += 1
     #         if dummy_honours ==1 and hand_honours == 1:
     #             frozen_suits.append(suit)
     #     for suit in frozen_suits:
     #         suit_scores[suit] -= self.FROZEN_SUIT_SCORE
     #     return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _all_winners_score(self) -> List[Tuple[str, int]]:
+    def _all_winners_score(self) -> list[tuple[str, int]]:
         """Assign score to a suit if all the cards are winners."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         for suit_name, suit in SUITS.items():
             if suit != player.trump_suit:
                 if player.holds_all_winners_in_suit(suit):
                     suit_scores[suit_name] = ALL_WINNERS
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _deprecate_trumps(self) -> List[Tuple[str, int]]:
+    def _deprecate_trumps(self) -> list[tuple[str, int]]:
         """Assign score to a suit if opponents have no trumps."""
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         suit_scores[self.player.trump_suit.name] = -1 * self.TRUMP_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _suit_strength(self) -> List[Tuple[str, int]]:
+    def _suit_strength(self) -> list[tuple[str, int]]:
         """Assign score to a suit by HCP."""
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         for suit_name in SUITS:
             cards = self.player.our_cards[suit_name]
             for card in cards:
                 if card.value >= 10:
                     suit_scores[suit_name] += card.value - 9
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _shortage_score(self, controls: Dict[str, int]) -> List[Tuple[str, int]]:
+    def _shortage_score(self, controls: dict[str, int]) -> list[tuple[str, int]]:
         """Assign score to a suit if we can create a shortage."""
         player = self.player
         manager = global_vars.manager
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         for suit_name, suit in SUITS.items():
             if suit != player.trump_suit:
                 if controls[suit_name] - len(player.partners_suit_cards[suit_name]) <= 1:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer_nt.py` & `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_nt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # first_seat_declarer_nt.py
 """ First seat card play for declarer in NT contracts."""
 
-from typing import List, Union
 from termcolor import cprint
 import random
 import inspect
 
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, Suit
 
-import bfgcardplay.source.declarer_play as declarer
-import bfgcardplay.source.global_variables as global_vars
-from .utilities import get_list_of_best_scores, get_suit_strength
+import bfgcardplay.src.declarer_play as declarer
+import bfgcardplay.src.global_variables as global_vars
+from .utilities import get_list_of_best_scores, get_suit_strength, play_to_unblock
 from .player import Player, Cards
 from .first_seat import FirstSeat
 from .declarer_play import card_combinations
 
-MODULE_COLOUR = 'cyan'
+MODULE_COLOUR = 'red'
 
 
 class FirstSeatDeclarerNT(FirstSeat):
     def __init__(self, player: Player):
         super().__init__(player)
 
     def selected_card(self) -> Card:
@@ -161,15 +160,15 @@
         suit = self._play_winner_no_entry()
         if suit:
             return suit
 
         # suit_to_develop has been defined
         suit = manager.suit_to_develop(player.seat)
         if suit and player.unplayed_cards[suit]:
-                return log(inspect.stack(), suit)
+            return log(inspect.stack(), suit)
 
         # Look for suit to develop
         suit = self._select_suit_to_develop()
         if suit:
             return suit
 
         # This crude logic stops the player cashing their winners early
@@ -205,15 +204,17 @@
 
     def _play_winner_no_entry(self):
         player = self.player
         dashboard = player.dashboard
         tricks_needed = dashboard.tricks_needed - player.declarers_tricks
         if tricks_needed <= dashboard.sure_tricks.count:
             for suit in SUITS:
-                opponents_length = len(player.total_unplayed_cards[suit]) - len(player.our_unplayed_cards[suit])
+                total_cards = len(player.total_unplayed_cards[suit])
+                our_cards = len(player.our_unplayed_cards[suit])
+                opponents_length = total_cards - our_cards
                 if opponents_length <= 2:
                     if player.unplayed_cards[suit] and not player.partners_unplayed_cards[suit]:
                         if player.is_winner_declarer(player.unplayed_cards[suit][0]):
                             return log(inspect.stack(), Suit(suit))
         return None
 
     def _select_suit_to_develop(self) -> Suit:
@@ -236,47 +237,45 @@
     def _select_best_suit(self) -> Suit:
         player = self.player
         suit_scores = {suit: 0 for suit in SUITS}
         for suit in SUITS:
             our_cards = Cards(player.our_unplayed_cards[suit])
             suit_scores[suit] += our_cards.value + len(player.our_unplayed_cards[suit])
         suits = get_list_of_best_scores(suit_scores)
-        if len(suits) == 1:
+        if len(suits) == 1 and len(player.unplayed_cards[suits[0]]) > 0:
             return log(inspect.stack(), Suit(suits[0]))
-        suit = Suit(random.choice(suits))
+        suit_choices = [suit for suit in SUITS if len(player.unplayed_cards[suit]) > 0]
+        suit = Suit(random.choice(suit_choices))
         return log(inspect.stack(), suit)
 
     def _find_suit_to_develop(self) -> Suit:
         player = self.player
         manager = global_vars.manager
         if not manager.suit_to_develop(player.seat):
             suit_to_develop = self._suit_to_develop()
             if suit_to_develop:
                 return log(inspect.stack(), suit_to_develop)
         return None
 
-    def _find_suits_with_extras(self) -> List[Suit]:
+    def _find_suits_with_extras(self) -> list[Suit]:
         dashboard = self.player.dashboard
         if dashboard.probable_tricks.count:
             return dashboard.probable_tricks.suits
         return dashboard.possible_tricks.suits
 
-
     def _select_suit_with_winners(self):
         """Return"""
         player = self.player
         manager = global_vars.manager
 
+        set_strategy_limit = 1
         if len(player.board.tricks) < 4:
             set_strategy_limit = 7
-        else:
-            set_strategy_limit = 1
 
         # Play
-
         winners = {suit: len(player.dashboard.winners[suit]) for suit in SUITS}
         best_suits = get_list_of_best_scores(winners)
         for suit in best_suits:
             if (player.dashboard.winners[suit] and
                     player.unplayed_cards[suit] and
                     len(player.our_cards[suit]) >= set_strategy_limit):
                 manager.set_suit_strategy(player.seat, suit, 'Play winners')
@@ -288,15 +287,15 @@
         player = self.player
         manager = global_vars.manager
         candidate_suits = {}
         if len(player.board.tricks) > 1:
             for suit in SUITS:
                 if (len(player.unplayed_cards[suit]) >= 4 or
                         (len(player.partners_unplayed_cards[suit]) >= 4 and
-                        len(player.unplayed_cards[suit]) > 0)):
+                         len(player.unplayed_cards[suit]) > 0)):
                     points = get_suit_strength(player.our_unplayed_cards[suit])
                     candidate_suits[suit] = len(player.our_unplayed_cards[suit]) + points[suit]
             if candidate_suits:
                 candidates = get_list_of_best_scores(candidate_suits)
                 suit = candidates[0]
                 manager.set_suit_to_develop(player.seat, Suit(suit))
                 for card in player.partners_unplayed_cards[suit]:
@@ -319,15 +318,15 @@
                 if player.unplayed_cards[suit]:
                     suits.append(suit)
 
         if len(suits) == 1:
             return log(inspect.stack(), Suit(suits[0]))
         return None
 
-    def _suit_to_develop(self) -> List[str]:
+    def _suit_to_develop(self) -> list[str]:
         """Return a list of suits to develop."""
         player = self.player
         if len(player.board.tricks) > 9:
             return None
         manager = global_vars.manager
         long_suits_to_develop = self._long_suits_to_develop()
         longest_strongest_suit = self._longest_strongest_suit(long_suits_to_develop)
@@ -355,19 +354,20 @@
         """Return a list of long suits to develop."""
         player = self.player
         long_suits_to_develop = []
         for suit_name in SUITS:
             declarers_suit_cards = player.declarers_suit_cards[suit_name]
             dummys_suit_cards = player.dummys_suit_cards[suit_name]
             total_cards = len(declarers_suit_cards) + len(dummys_suit_cards)
-            if (total_cards >= 6 and (len(declarers_suit_cards) >= 4 or len(dummys_suit_cards) >= 4)):
+            if (total_cards >= 6 and (len(declarers_suit_cards) >= 4
+                                      or len(dummys_suit_cards) >= 4)):
                 long_suits_to_develop.append(suit_name)
         return long_suits_to_develop
 
-    def _longest_strongest_suit(self, suits: List[str]) -> str:
+    def _longest_strongest_suit(self, suits: list[str]) -> str:
         """Return the longest and strongest suit from a list of suit_names."""
         player = self.player
         manager = global_vars.manager
         candidate_suits = {}
         for suit_name in suits:
             declarers_suit_cards = player.declarers_suit_cards[suit_name]
             dummys_suit_cards = player.dummys_suit_cards[suit_name]
@@ -395,15 +395,15 @@
         suits = []
         for suit in SUITS:
             if player.unplayed_cards[suit]:
                 suits.append(suit)
         suit = random.choice(suits)
         return suit
 
-    def _select_lead_card(self, suit: Suit) -> Union[Card, None]:
+    def _select_lead_card(self, suit: Suit) -> Card | None:
         """Return the selected lead card for declarer."""
         player = self.player
         manager = global_vars.manager
         cards = player.suit_cards[suit.name]
         if not cards:
             return None
 
@@ -413,16 +413,21 @@
             return log(inspect.stack(), card)
 
         # Play winning cards
         if (manager.suit_strategy(player.seat)[suit.name] == 'Play winners' or
                 player.holds_all_winners_in_suit(suit)):
             my_cards = player.unplayed_cards[suit.name]
             partners_cards = player.partners_unplayed_cards[suit.name]
+            card = play_to_unblock(my_cards, partners_cards)
+            if card:
+                return log(inspect.stack(), card)
+
             if (partners_cards and len(my_cards) > len(partners_cards) and
-                    player.is_winner_declarer(partners_cards[0])):
+                    player.is_winner_declarer(partners_cards[0]) and
+                    len(partners_cards) > 1):
                 return log(inspect.stack(), my_cards[-1])
             for card in cards[::-1]:
                 if player.opponents_unplayed_cards[suit.name]:
                     if player.is_winner_declarer(card):
                         return log(inspect.stack(), card)
                 else:
                     return log(inspect.stack(), card)
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/first_seat_declarer_suit.py` & `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_declarer_suit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # first_seat_declarer.py
 """ First seat card play for declarer."""
 
-from typing import List, Dict, Tuple
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, Suit
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .utilities import get_list_of_best_scores
 from .player import Player
 from .first_seat import FirstSeat
 from .declarer_play import card_combinations
 
 ALL_WINNERS = 5
 
@@ -150,15 +149,15 @@
             return suit
 
         # Select best suit
         score_reasons = self._get_score_reasons()
         best_suit = self._best_suit(score_reasons)
         return log(inspect.stack(), best_suit)
 
-    def _get_score_reasons(self) ->Dict[str, int]:
+    def _get_score_reasons(self) ->dict[str, int]:
         controls = self.player.get_controls()
         score_reasons = {
             'trumps': self._deprecate_trumps(),
             'shortage': self._shortage_score(controls),
             'void': self._deprecate_suits(),
             'all_winners': self._all_winners_score(),
             'frozen': self._frozen_suits(),
@@ -323,15 +322,15 @@
         winning_suits = self._get_winning_suit_list()
 
         long_suits = get_list_of_best_scores(winning_suits)
         if long_suits and player.unplayed_cards[long_suits[0]]:
             return log(inspect.stack(), Suit(long_suits[0]))
         return None
 
-    def _get_winning_suit_list(self) -> List[Suit]:
+    def _get_winning_suit_list(self) -> list[Suit]:
         """Return a list of winning suits."""
         player = self.player
         winning_suits = {}
         for suit_name, suit in SUITS.items():
             our_cards = player.our_unplayed_cards[suit.name]
             if suit != player.trump_suit and our_cards:
                 my_cards = player.unplayed_cards[suit_name]
@@ -343,15 +342,15 @@
                     if index < len(opponents_cards):
                         if card.value < opponents_cards[index].value:
                             break
                 else:
                     winning_suits[suit_name] = last_card
         return winning_suits
 
-    def _can_draw_trumps(self) -> Tuple[bool, bool]:
+    def _can_draw_trumps(self) -> tuple[bool, bool]:
         """Return True if declarer should draw trumps, and/or True to ruff in shorthand."""
         show_return = 0
         player = self.player
         if not player.opponents_unplayed_cards[player.trump_suit.name]:
             return return_and_print(False, 'can_draw_trumps z', show_return)
         if not player.trump_cards:
             return return_and_print(False, 'can_draw_trumps a', show_return)
@@ -453,56 +452,56 @@
                     if not player.dashboard.threats[suit]:
                         return False
                     # if not player.is_winner_declarer(player.unplayed_cards[suit][-1]):
                     #     print(colored(f'{suit} {player.unplayed_cards[suit]}', MODULE_COLOUR))
                     return True
         return False
 
-    def _long_suits(self) -> List[Tuple[str, int]]:
+    def _long_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on length (long)."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         length_score = self.LENGTH_SCORE
 
         for suit in SUITS:
             number_cards = len(player.our_cards[suit]) - len(player.opponents_cards[suit])
             if number_cards > 0:
                 if player.trump_suit:
                     if suit == player.trump_suit.name:
                         length_score = 0
                 suit_scores[suit] = number_cards * length_score
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _all_winners_score(self) -> List[Tuple[str, int]]:
+    def _all_winners_score(self) -> list[tuple[str, int]]:
         """Assign score to a suit if all the cards are winners."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         for suit_name, suit in SUITS.items():
             if suit != player.trump_suit:
                 if player.holds_all_winners_in_suit(suit):
                     suit_scores[suit_name] = ALL_WINNERS
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _deprecate_trumps(self) -> List[Tuple[str, int]]:
+    def _deprecate_trumps(self) -> list[tuple[str, int]]:
         """Assign score to a suit if opponents have no trumps."""
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         suit_scores[self.player.trump_suit.name] = -1 * self.TRUMP_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _suit_strength(self) -> List[Tuple[str, int]]:
+    def _suit_strength(self) -> list[tuple[str, int]]:
         """Assign score to a suit by HCP."""
         suit_scores = {suit_name: 0 for suit_name, suit in SUITS.items()}
         for suit_name in SUITS:
             cards = self.player.our_cards[suit_name]
             for card in cards:
                 if card.value >= 10:
                     suit_scores[suit_name] += card.value - 9
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _shortage_score(self, controls: Dict[str, int]) -> List[Tuple[str, int]]:
+    def _shortage_score(self, controls: dict[str, int]) -> list[tuple[str, int]]:
         """Assign score to a suit if we can create a shortage."""
         player = self.player
         manager = global_vars.manager
         my_trumps = player.unplayed_cards[player.trump_suit]
         partners_trumps = player.unplayed_cards[player.trump_suit]
 
         suit_scores = {suit_name: 0 for suit_name in SUITS}
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/first_seat_defender.py` & `bfgcardplay-1.0.7/bfgcardplay/src/first_seat_defender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """ First seat card play for defender."""
 
-from typing import List, Tuple, Dict
 from termcolor import cprint, colored
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, Suit, CARD_VALUES
 from .player import Player
 from .first_seat import FirstSeat
 from .defender_play import deduce_partner_void_in_trumps, dummy_is_short_trump_hand
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'blue'
 
 
 class FirstSeatDefender(FirstSeat):
     def __init__(self, player: Player):
         super().__init__(player)
@@ -105,23 +104,23 @@
             for suit in SUITS:
                 if suit != player.trump_suit and player.unplayed_cards[suit]:
                     if (len(player.dummys_unplayed_cards[suit]) == 1 and
                             player.is_winner_defender(player.unplayed_cards[suit][0])):
                         return log(inspect.stack(), Suit(suit))
         return None
 
-    def _get_deprecated_suits(self) -> List[Suit]:
+    def _get_deprecated_suits(self) -> list[Suit]:
         deprecated_suits = []
         dummy_tenaces = self.identify_dummy_tenaces()
         for suit in SUITS:
             if self.player.dummy_on_right and suit in dummy_tenaces:
                 deprecated_suits.append(suit)
         return deprecated_suits
 
-    def _get_tenace_suits(self, deprecated_suits) -> List[Suit]:
+    def _get_tenace_suits(self, deprecated_suits) -> list[Suit]:
         tenace_suits = []
         dummy_tenaces = self.identify_dummy_tenaces()
         for suit in SUITS:
             if suit not in deprecated_suits:
                 if self.player.dummy_on_left and suit in dummy_tenaces:
                     tenace_suits.append(Suit(suit))
         return tenace_suits
@@ -149,15 +148,16 @@
                                 return log(inspect.stack(), Suit(suit))
         return None
 
     def _select_liked_suit(self) -> Suit:
         player = self.player
         manager = global_vars.manager
         for suit in SUITS:
-            if player.dummys_unplayed_cards[suit] or not player.dummys_unplayed_cards[player.trump_suit]:
+            if (player.dummys_unplayed_cards[suit] or
+                    not player.dummys_unplayed_cards[player.trump_suit]):
                 if manager.like_dislike(player.partner_seat, suit) and player.unplayed_cards[suit]:
                     return log(inspect.stack(), Suit(suit))
                 if manager.like_dislike(player.seat, suit) and player.unplayed_cards[suit]:
                     return log(inspect.stack(), Suit(suit))
         return None
 
     def _dummy_out_of_trumps(self) -> Suit:
@@ -166,15 +166,15 @@
             for suit in SUITS:
                 if (len(player.total_unplayed_cards[suit]) == 1 and
                         player.total_unplayed_cards[suit][0] in player.unplayed_cards[suit] and
                         not player.dummys_suit_cards[player.trump_suit.name]):
                     return log(inspect.stack(), Suit(suit))
         return None
 
-    def _score_reasons(self) -> Dict[str, int]:
+    def _score_reasons(self) -> dict[str, int]:
         score_reasons = {}
 
         # Deprecate voids
         score_reasons['void'] = self._deprecate_suits()
 
         # Trumps
         score_reasons['trumps'] = self._trumps()
@@ -216,15 +216,14 @@
                     if player.dummys_unplayed_cards[suit]:
                         dummys_top_card = player.dummys_unplayed_cards[suit][0]
                         if (dummys_top_card.is_honour and
                                 dummys_top_card.value < player.total_unplayed_cards[suit][0].value):
                             return log(inspect.stack(), Suit(suit))
         return None
 
-
     def _partner_void_in_trumps(self) -> Suit:
         player = self.player
         manager = global_vars.manager
         if deduce_partner_void_in_trumps(player):
             manager.voids[player.partner_seat][player.trump_suit.name] = True
 
         partners_seat = player.partner_seat
@@ -236,15 +235,18 @@
                     manager.set_suit_strategy(player.seat, suit, 'ruff_in_void')
                     return log(inspect.stack(), Suit(suit))
         return None
 
     def _select_suit_for_nt_contract(self) -> Suit:
         """Return the trick lead suit for the defending a suit contract."""
         player = self.player
-        manager = global_vars.manager
+
+        # Return partner's suit
+        if len(player.unplayed_cards[player.board.tricks[0].suit]) > 0:
+            return log(inspect.stack(), player.board.tricks[0].suit)
 
         # Select suit after partner signal
         suit = self._suit_after_partner_signal()
         if suit:
             return suit
 
         suit = self._suit_to_develop()
@@ -267,27 +269,14 @@
         if suit:
             return suit
 
         score_reasons = self._score_reasons()
         best_suit = self._best_suit(score_reasons)
         return log(inspect.stack(), best_suit)
 
-    def _score_reasons(self):
-        score_reasons = {
-            'void': self._deprecate_suits(),
-            'partner': self._partners_suit(),
-            'sequence': self._sequences(),
-            'tenaces': self._tenace_check(),
-            'weakness': self._lead_through_strength(),
-            'frozen': self._frozen_suits(),
-            'long': self._long_suits(),
-            'short': self._short_suits(),
-        }
-        return score_reasons
-
     def _suit_after_partner_signal(self) -> Suit:
         player = self.player
         if len(player.board.tricks) == 2 and player.dummy_on_right:
             partners_lead = player.board.tricks[0].cards[0]
             if partners_lead.value >= CARD_VALUES['T'] or partners_lead.value < CARD_VALUES['6']:
                 if player.unplayed_cards[partners_lead.suit.name]:
                     return log(inspect.stack(), partners_lead.suit)
@@ -366,14 +355,19 @@
             if card.is_honour and card.value == cards[index+1].value + 1:
                 return log(inspect.stack(), card)
 
         # Top of doubleton
         if len(cards) == 2:
             return log(inspect.stack(), cards[0])
 
+        # Return winners
+        winners = player.dashboard.winners[suit.name]
+        if winners:
+            return log(inspect.stack(), winners[-1])
+
         # Return bottom card
         return log(inspect.stack(), cards[-1])
 
     def _sequences(self) -> Suit:
         """Return the score for sequences."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
@@ -399,28 +393,30 @@
         manager = global_vars.manager
         partners_voids = manager.voids[player.seat]
         for suit, void in partners_voids.items():
             if void:
                 suit_scores[suit] += self.PARTNERS_VOID
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _deprecate_suits(self) -> List[Tuple[str, int]]:
+    def _deprecate_suits(self) -> list[tuple[str, int]]:
         """Assign score to suits based on void."""
         player = self.player
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         for suit in SUITS:
             if not self.player.suit_cards[suit]:
                 suit_scores[suit] -= self.VOID_SCORE
             if player.trump_suit:
                 dummy_short_trumps = dummy_is_short_trump_hand(player)
                 if ((dummy_short_trumps and not player.dummys_suit_cards[suit])):
                     suit_scores[suit] -= self.RUFF_AND_DISCARD_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
-    def _trumps(self) -> List[Tuple[str, int]]:
+    def _trumps(self) -> list[tuple[str, int]]:
         """Assign score to suits based on void."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
         if player.trump_suit:
-            if len(player.unplayed_cards[player.trump_suit.name]) > len(player.dummys_suit_cards[player.trump_suit.name]):
+            my_cards = player.unplayed_cards[player.trump_suit.name]
+            dummys_cards = player.dummys_suit_cards[player.trump_suit.name]
+            if len(my_cards) > len(dummys_cards):
                 suit_scores[player.trump_suit.name] += self.TRUMP_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/fourth_seat_declarer.py` & `bfgcardplay-1.0.7/bfgcardplay/src/fourth_seat_defender.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,153 @@
-"""Fourth seat card play for declarer."""
+"""Fourth seat card play for defender."""
+
 import random
-from typing import List, Union
-from termcolor import colored
+
+from bridgeobjects.src.constants import CARD_VALUES
+from termcolor import cprint
 
 import inspect
 from ..logger import log
 
-from bridgeobjects import SUITS, Card, Suit, CARD_VALUES
+from bridgeobjects import SUITS, Card, Suit
 from bfgdealer import Trick
+import bfgcardplay.src.global_variables as global_vars
+
 from .player import Player
-from .utilities import get_list_of_best_scores
+from .utilities import (get_list_of_best_scores, get_suit_strength,
+                        trick_card_values)
 from .fourth_seat import FourthSeat
-import bfgcardplay.source.global_variables as global_vars
+from .defender_play import get_hilo_signal_card, signal_card, surplus_card, best_discard
 
 MODULE_COLOUR = 'cyan'
+PLAYER_INDEX = 3
 
 
-class FourthSeatDeclarer(FourthSeat):
+class FourthSeatDefender(FourthSeat):
     def __init__(self, player: Player):
         super().__init__(player)
         self.player = player
 
     def selected_card(self) -> Card:
         """Return the card if the third seat."""
         player = self.player
         trick = player.board.tricks[-1]
-        manager = global_vars.manager
 
         cards = player.cards_for_trick_suit(trick)
 
         # Void
         if not cards:
-            return self._select_card_if_void()
+            return self._select_card_if_void(player, trick)
 
         # Singleton
         if len(cards) == 1:
             return log(inspect.stack(), cards[0])
-        if manager.suit_strategy == '':
-            pass
 
         # play low if partner is winning trick
         if self._second_player_winning_trick(cards, trick, player.trump_suit):
             return log(inspect.stack(), cards[-1])
 
-        # When to duck - rule of 7
-        duck_trick = False
-        if not player.trump_suit:
-            if trick.suit == player.board.tricks[0].cards[0].suit:
-                duck_trick = self._duck_trick(player, trick, cards)
-                if duck_trick:
-                    return log(inspect.stack(), cards[-1])
-                else:
-                    for card in cards[::-1]:
-                        if self.can_win_trick(player, card):
-                            return log(inspect.stack(), card)
-
         # win trick if possible
         winning_card = self._winning_card(trick)
+        unplayed_cards = player.total_unplayed_cards[trick.suit.name]
         if winning_card:
-            return winning_card
+            value = winning_card.value
+            play_winner = False
+            while value > 1:
+                value -= 1
+                card = Card(CARD_VALUES[value], trick.suit.name)
+                if (card in unplayed_cards and
+                        card not in player.dummys_unplayed_cards[trick.suit.name]):
+                    play_winner = True
+                    break
+            if play_winner:
+                return log(inspect.stack(), winning_card)
+
+        # Play low if higher card is winner after trick played
+        # losing_trick = (trick.cards[0].value > trick.cards[1].value or
+        #                     trick.cards[2].value > trick.cards[1].value)
+        # if len(cards) == 2 and losing_trick:
+        #     winner = True
+        #     for card in unplayed_cards:
+        #         if card.value > cards[0].value:
+        #             winner = False
+        #     if winner:
+        #         return log(inspect.stack(), cards[1])
 
-        # play smallest card
-        return log(inspect.stack(), cards[-1])
+        # Signal even/odd
+        return get_hilo_signal_card(player, cards)
 
-    def _select_card_if_void(self) -> Card:
+    def _select_card_if_void(self, player: Player, trick: Trick) -> Card:
         """Return card if cannot follow suit."""
-        player = self.player
-        trick = player.board.tricks[-1]
         player.record_void(trick.suit)
+        manager = global_vars.manager
 
         # Trump if appropriate
         if player.trump_suit:
-            (value_0, value_1, value_2) = self._trick_card_values(trick, player.trump_suit)
+            values = trick_card_values(trick, player.trump_suit)
             if player.trump_cards:
-                if value_0 > value_1 or value_2 > value_1:
+                if values[0] > values[1] or values[2] > values[1]:
                     for card in player.trump_cards[::-1]:
-                        if card.value + 13 > value_0 and card.value + 13 > value_2:
+                        if card.value + 13 > values[0] and card.value + 13 > values[2]:
                             return log(inspect.stack(), card)
 
-        # Discard if winner in partner's hand
-        random_suits = [suit for suit in SUITS]
-        if player.trump_suit:
-            random_suits.remove(player.trump_suit.name)
-
-        # TODO do not discard an entry to partner's hand
-        # for suit in random_suits:
-
-        random.shuffle(random_suits)
-        for suit in random_suits:
-            my_cards = player.unplayed_cards[suit]
-            partners_cards = player.partners_unplayed_cards[suit]
-            if my_cards and partners_cards:
-                if len(my_cards) > 1:
-                    if player.is_winner_declarer(partners_cards[0]):
-                        return log(inspect.stack(), my_cards[-1])
-
-        # Find a card that is not an honour
-        for suit in random_suits:
-            if player.unplayed_cards[suit]:
-                if not player.unplayed_cards[suit][-1].is_honour:
-                    return log(inspect.stack(), player.unplayed_cards[suit][-1])
-
-        # Last resort - dump a low card
-        for suit in random_suits:
-            if player.unplayed_cards[suit]:
-                return log(inspect.stack(), player.unplayed_cards[suit][-1])
+        # Do not signal with winners
+        for suit in SUITS:
+            for card in player.unplayed_cards[suit]:
+                if not player.is_master_card(card):
+                    return log(inspect.stack(), card)
+
+        # Signal best suit
+        best_suit = self._best_suit()
+        card = signal_card(player, manager, best_suit)
+        if card:
+            if not player.is_master_card(card):
+                return log(inspect.stack(), card)
+
+        # Discard if more cards than the opposition
+        card = surplus_card(player)
+        if card:
+            return log(inspect.stack(), card)
 
-        # If all else fails play a trump
-        return log(inspect.stack(), player.trump_cards[-1])
+        # Best discard
+        return log(inspect.stack(), best_discard(player))
 
     def _best_suit(self) -> Suit:
         """Select suit for signal."""
         # TODO handle no points and equal suits
+        player = self.player
+        cards = player.hand_cards.list
+        suit_points = get_suit_strength(cards)
+        max_points = 0
         best_suit = self._strongest_suit()
         return best_suit
+        for suit in SUITS:
+            if suit != player.trump_suit.name:
+                hcp = suit_points[suit]
+                if hcp > max_points:
+                    max_points = hcp
+                    best_suit = suit
+        if not best_suit:
+            for suit in SUITS:
+                if suit != player.trump_suit.name:
+                    hcp = suit_points[suit]
+                    if hcp > max_points:
+                        max_points = hcp
+                        best_suit = suit
+        if not best_suit:
+            return player.trump_suit
+        return Suit(best_suit)
 
-    def _strongest_suit(self) -> Union[Suit, None]:
+    def _strongest_suit(self) -> Suit | None:
         """Return the strongest_suit."""
         player = self.player
         suits = {suit: 0 for suit in SUITS}
         for suit in SUITS:
             cards = player.unplayed_cards[suit]
             for card in cards:
                 suits[suit] += card.value
         if player.trump_suit:
             suits[player.trump_suit.name] = 0
         best_suits = get_list_of_best_scores(suits)
-        if not best_suits:
-            return player.trump_suit
+        # if not best_suits:
+        #     return player.trump_suit
         return Suit(random.choice(best_suits))
-
-    def _duck_trick(self, player: Player, trick: Trick, cards: List[Card]) -> bool:
-        """Return True if the player is to duck the trick."""
-        opponents_unplayed_cards = player.opponents_unplayed_cards[trick.suit.name]
-        if cards and opponents_unplayed_cards:
-            # partners_cards = player.partners_suit_cards[trick.suit.name]
-            # partner_can_win = False
-            # if partners_cards:
-            #     if  partners_cards[0].value > trick.cards[0].value:
-            #         partner_can_win = True
-            if (len(cards) == 2 and cards[0].value == CARD_VALUES['K'] and
-                    Card('A', trick.suit.name) in opponents_unplayed_cards):
-                return False
-            can_win_trick = (cards[0].value > opponents_unplayed_cards[0].value and
-                             cards[0].value > trick.cards[0].value and
-                             cards[0].value > trick.cards[2].value)
-            if self._rule_of_seven(player, trick) and can_win_trick:
-                return False
-        return True
-
-    @staticmethod
-    def _rule_of_seven(player: Player, trick: Trick) -> bool:
-        """Return True if rule of seven applies."""
-        our_cards = player.our_cards[trick.suit]
-        duck_count = 7 - len(our_cards) - len(player.board.tricks)
-        return duck_count < 0
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/manager.py` & `bfgcardplay-1.0.7/bfgcardplay/src/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """The manager supervises play and holds persistant data. It is created in global.py."""
-from typing import Union
 from termcolor import colored
 
 from bridgeobjects import SEATS, SUITS, RANKS, Suit
 
 MODULE_COLOUR = 'magenta'
 
 DECLARER_STRATEGY = {
@@ -86,15 +85,15 @@
         """Return 1 if the player likes the suit and -1 if not."""
         return self._like_dislike[seat][suit]
 
     def set_like_dislike(self, seat: str, suit: str, value: bool):
         """Set the like_dislike for a seat and suit."""
         self._like_dislike[seat][suit] = value
 
-    def _even_odd(self, seat: str, suit: str) -> Union[bool, None]:
+    def _even_odd(self, seat: str, suit: str) -> bool | None:
         """Return 1 if the player has an even number the suit and -1 if not."""
         return self._even_odd[seat][suit]
 
     def set_even_odd(self, seat: str, suit: str, value: int):
         """Set even/odd (0/1) for a seat and suit."""
         self._even_odd[seat][suit] = value
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/opening_lead.py` & `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Opening leads for Card Player."""
 
 from .opening_lead_card import opening_lead_card
 from .opening_lead_suit import opening_lead_suit
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'green'
 
 def opening_lead(board):
     """Return the proposed opening lead for the board."""
 
     manager = global_vars.manager
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/opening_lead_card.py` & `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/opening_lead_suit.py` & `bfgcardplay-1.0.7/bfgcardplay/src/opening_lead_suit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 from bridgeobjects import SUITS, Spades, Hearts, Diamonds, Clubs, SEATS, Denomination, Call
 
 from .card_player_components import SelectedSuit, Card
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 
 MODULE_COLOUR = 'cyan'
 
 
 def opening_lead_suit(board):
     """Return the opening lead from a list of cards given the contract."""
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/player.py` & `bfgcardplay-1.0.7/bfgcardplay/src/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Common functionality for cardplay."""
 
-# from types import List
 from termcolor import cprint
 
-from typing import List, Dict, Tuple, Union
-
 from bridgeobjects import Suit, Card, SEATS, SUITS, CARD_VALUES
 from bfgbidding import Hand
 from bfgdealer import Trick
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .data_classes import Cards
 from .dashboard import Dashboard
 from .data_classes import SuitCards
 from .utilities import get_list_of_best_scores, get_suit_strength
 
 global_vars.initialize()
 
@@ -52,29 +49,35 @@
         self.suit_cards = self.hand_cards.by_suit
         self.unplayed_cards = self.hand_cards.by_suit
 
         # self.longest_suit = self.hand_cards.longest_suit
         self.longest_suit = self._longest_suit()
 
         our_cards = Cards(board.hands[self.seat].cards + board.hands[self.partner_seat].cards)
-        our_unplayed_cards = Cards(board.hands[self.seat].unplayed_cards + board.hands[self.partner_seat].unplayed_cards)
-        self.our_cards: Dict[str, List[Card]] = our_cards.by_suit
-        self.our_unplayed_cards: Dict[str, List[Card]] = our_unplayed_cards.by_suit
+        my_unplayed_cards = board.hands[self.seat].unplayed_cards
+        partners_unplayed_cards = board.hands[self.partner_seat].unplayed_cards
+        our_unplayed_cards = Cards(my_unplayed_cards + partners_unplayed_cards)
+        self.our_cards: dict[str, list[Card]] = our_cards.by_suit
+        self.our_unplayed_cards: dict[str, list[Card]] = our_unplayed_cards.by_suit
 
         opponents_seats = (SEATS[(self.seat_index + 1) % 4], SEATS[(self.seat_index + 3) % 4])
-        opponents_cards = Cards(board.hands[opponents_seats[0]].cards + board.hands[opponents_seats[1]].cards)
+        opps_cards_0 = board.hands[opponents_seats[0]].cards
+        opps_cards_1 = board.hands[opponents_seats[1]].cards
+        opponents_cards = Cards(opps_cards_0 + opps_cards_1)
         opponents_unplayed_cards = Cards(board.hands[opponents_seats[0]].unplayed_cards +
                                          board.hands[opponents_seats[1]].unplayed_cards)
-        self.opponents_cards: Dict[str, List[Card]] = opponents_cards.by_suit
-        self.opponents_unplayed_cards: Dict[str, List[Card]] = opponents_unplayed_cards.by_suit
+        self.opponents_cards: dict[str, list[Card]] = opponents_cards.by_suit
+        self.opponents_unplayed_cards: dict[str, list[Card]] = opponents_unplayed_cards.by_suit
 
         self.seats_unplayed_cards = {seat: Cards(self.board.hands[seat].unplayed_cards).by_suit for seat in SEATS}
         self.seats_unplayed_cards = {}
+        self.highest_card = {}
         for seat in SEATS:
             self.seats_unplayed_cards[seat] = Cards(self.board.hands[seat].unplayed_cards).by_suit
+            self.highest_card[seat] = {}
 
         # Trumps
         if self.trump_suit:
             self.trump_cards = self.hand_cards.by_suit[self.trump_suit]
             self.opponents_trumps = opponents_unplayed_cards.by_suit[self.trump_suit]
         else:
             self.trump_cards = None
@@ -99,16 +102,16 @@
         self.total_unplayed_cards = self._total_unplayed_cards()
 
         # Declarer and Dummy
         # These card properties must be assigned in this order
         declarers_cards = Cards(board.hands[self.declarer].unplayed_cards)
         self.declarers_suit_cards = declarers_cards.by_suit
         dummys_cards = Cards(board.hands[self.dummy].unplayed_cards)
-        self.dummys_suit_cards: Dict[str, List[Card]] = dummys_cards.by_suit
-        self.dummys_unplayed_cards: Dict[str, List[Card]] = dummys_cards.by_suit
+        self.dummys_suit_cards: dict[str, list[Card]] = dummys_cards.by_suit
+        self.dummys_unplayed_cards: dict[str, list[Card]] = dummys_cards.by_suit
         self.dummy_suit_strength = get_suit_strength(dummys_cards.list)
         self.dummy_suit_tenaces = self._get_tenaces(self.dummys_suit_cards)
         # Short trump hands
         if self.trump_suit:
             declarers_trumps = self.declarers_suit_cards[self.trump_suit]
             dummys_trumps = self.dummys_suit_cards[self.trump_suit]
             if len(declarers_trumps) > len(dummys_trumps):
@@ -135,19 +138,19 @@
 
         # Information
         self.trick_number = len(board.tricks)
         self.declarers_target = self.board.contract.target_tricks
         (self.declarers_tricks, self.defenders_tricks) = self._get_trick_count()
         self.suit_rounds = self._get_suit_rounds()
 
-        if not self.is_defender:
-            self.dashboard = Dashboard(self)
+        # if not self.is_defender:
+        self.dashboard = Dashboard(self)
 
     @staticmethod
-    def cards_by_suit(hand: Hand) -> Dict[str, List[Card]]:
+    def cards_by_suit(hand: Hand) -> dict[str, list[Card]]:
         """Return a dict of unplayed cards by suit for the given hand."""
         cards = Cards(hand.unplayed_cards)
         return cards.by_suit
 
     @staticmethod
     def _get_partners_seat(seat: str) -> str:
         """Return partner's seat."""
@@ -163,43 +166,43 @@
         if trick.winner:
             leader = trick.winner
         leader_index = SEATS.index(leader)
         seat_index = (leader_index + len(trick.cards)) % 4
         seat = SEATS[seat_index]
         return seat
 
-    def cards_for_trick_suit(self, trick: Trick) -> List[Card]:
+    def cards_for_trick_suit(self, trick: Trick) -> list[Card]:
         """Return a list of cards in the trick suit."""
         return self.hand_cards.by_suit[trick.suit]
 
     def record_void(self, suit: Suit):
         """Add void to manager voids."""
         manager = global_vars.manager
         manager.voids[self.seat][suit.name] = True
 
     def _get_trump_suit(self) -> Suit:
         """Return the trump suit for the board (if any)."""
         if self.board.contract.is_nt:
             return None
         return self.board.contract.denomination
 
-    def get_strongest_suits(self, cards: List[Card]) -> List[Suit]:
+    def get_strongest_suits(self, cards: list[Card]) -> list[Suit]:
         """Return a list of suits that have the highest high card points."""
         suit_points = get_suit_strength(cards)
         strong_suits = get_list_of_best_scores(suit_points)
         return strong_suits
 
-    def _get_tenaces(self, cards: Dict[str, Card]) -> Dict[str, Card]:
+    def _get_tenaces(self, cards: dict[str, Card]) -> dict[str, Card]:
         """Return a dict of suit tenaces keyed on suit name."""
         suit_tenaces = {suit_name: None for suit_name, suit in SUITS.items()}
         for suit, cards in cards.items():
             suit_tenaces[suit] = self.get_suit_tenaces(cards)
         return suit_tenaces
 
-    def get_suit_tenaces(self, cards: List[Card]) -> Card:
+    def get_suit_tenaces(self, cards: list[Card]) -> Card:
         """Return the top card in a tenaces, or None."""
         if not cards:
             return None
 
         opponents_cards = self.opponents_unplayed_cards[cards[0].suit.name]
         suit = cards[0].suit_name
         for card in cards[:-2]:
@@ -207,46 +210,46 @@
                 value = card.value
                 missing_card = Card(CARD_VALUES[value-1], suit)
                 next_card = Card(CARD_VALUES[value-2], suit)
                 if missing_card in opponents_cards and next_card in cards:
                     return next_card
         return None
 
-    def _get_opponents_seats(self) -> Tuple[str, str]:
-        """Return a Tuple with right and left hand seats."""
+    def _get_opponents_seats(self) -> tuple[str, str]:
+        """Return a tuple with right and left hand seats."""
         seat_index = SEATS.index(self.seat)
         left_hand_seat_index = (seat_index + 1) % 4
         right_hand_seat_index = (seat_index + 3) % 4
-        return(SEATS[right_hand_seat_index], SEATS[left_hand_seat_index])
+        return (SEATS[right_hand_seat_index], SEATS[left_hand_seat_index])
 
     def card_has_been_played(self, card: Card) -> bool:
         """Return True if the card has already been played."""
         for seat in SEATS:
             hand = self.board.hands[seat]
             if card in hand.unplayed_cards:
                 return False
         return True
 
-    def get_unplayed_cards_by_suit(self, suit: Suit, seat: str) -> List[Card]:
+    def get_unplayed_cards_by_suit(self, suit: Suit, seat: str) -> list[Card]:
         """Return a list containing declarers and opponents unplayed cards in a suit."""
         hand = self.board.hands[seat]
         cards = hand.cards_by_suit[suit.name]
         unplayed_cards = [card for card in cards if card in hand.unplayed_cards]
         return unplayed_cards
 
-    def _total_unplayed_cards(self) -> Dict[str, List[Card]]:
+    def _total_unplayed_cards(self) -> dict[str, list[Card]]:
         """Return a dict containing all unplayed cards by suit."""
         unplayed_card_list = []
         for seat in SEATS:
             unplayed_card_list += self.hands[seat].unplayed_cards
             unplayed_cards = Cards(unplayed_card_list)
         return unplayed_cards.by_suit
 
     @staticmethod
-    def _sort_cards(cards: List[Card]) -> List[Card]:
+    def _sort_cards(cards: list[Card]) -> list[Card]:
         """Return a sorted list of cards."""
         return sorted(cards, reverse=True)
 
     def long_seat(self, suit: str) -> str:
         my_cards = self.unplayed_cards[suit]
         partners_cards = self.partners_unplayed_cards[suit]
         if len(my_cards) > len(partners_cards):
@@ -317,15 +320,15 @@
                         winners += 1
                     else:
                         break
                 else:
                     winners += 1
         return winners
 
-    def get_controls(self) -> Dict[str, int]:
+    def get_controls(self) -> dict[str, int]:
         """Return the current number of winners for declarer."""
         controls = {suit_name: 0 for suit_name in SUITS}
         for suit_name in SUITS:
             control_count = 0
             for card in self.our_unplayed_cards[suit_name]:
                 if self.opponents_unplayed_cards[suit_name]:
                     opponents_top_card_value = self.opponents_unplayed_cards[suit_name][0].value
@@ -363,16 +366,15 @@
         """Return True if card is a master."""
         unplayed_cards = self.total_unplayed_cards[card.suit]
         for unplayed_card in unplayed_cards:
             if unplayed_card.value > card.value:
                 return False
         return True
 
-
-    def _is_master(self, card: Card, other_masters: Dict[str, List[Card]]) -> bool:
+    def _is_master(self, card: Card, other_masters: dict[str, list[Card]]) -> bool:
         """Return True if card is a master."""
         # unplayed_cards = [unplayed_card for unplayed_card in self.unplayed_cards[card.suit.name]]
         unplayed_cards = self.total_unplayed_cards[card.suit]
         for master_card in other_masters[card.suit.name]:
             if master_card in unplayed_cards:
                 unplayed_cards.remove(master_card)
         for unplayed_card in unplayed_cards:
@@ -445,15 +447,15 @@
         entries = []
         for suit_name in SUITS:
             if suit_name != suit.name:
                 cards = self.get_entries(hand)[suit_name]
                 entries.extend(cards)
         return entries
 
-    def missing_honours(self, suit: Suit) -> List[Card]:
+    def missing_honours(self, suit: Suit) -> list[Card]:
         """Return a list of missing honours in the suit."""
         our_cards = self.our_unplayed_cards[suit]
         missing_honours = []
         for index, rank in enumerate('AKQJT'):
             card = Card(rank, suit.name)
             if card in self.total_unplayed_cards[suit]:
                 if card not in our_cards:
@@ -497,29 +499,22 @@
                         card = Card(CARD_VALUES[value], suit)
                         if card in cards:
                             return (higher_card, card)
                         if card in self.total_unplayed_cards[suit]:
                             return (None, None)
         return (None, None)
 
-    def card_value(self, card: Card) -> int:
-        """Return the card value adjusted for trumps."""
-        if self.trump_suit:
-            if card.suit == self.trump_suit:
-                return card.value + 13
-        return card.value
-
-    def touching_honours(self, cards: List[Card]) -> Union[Card, None]:
+    def touching_honours(self, cards: list[Card]) -> Card | None:
         """Return the top of touching honours if there is one or None otherwise."""
         for index, card in enumerate(cards[:-1]):
             if card.is_honour and card.value == cards[index+1].value + 1:
                 return card
         return None
 
-    def touching_honours_in_hand(self, hand: Hand, suit: str) -> Union[Card, None]:
+    def touching_honours_in_hand(self, hand: Hand, suit: str) -> Card | None:
         """Return the top of touching honours if there is one or None otherwise."""
         cards = Cards(hand.unplayed_cards).by_suit[suit]
         for index, card in enumerate(cards[:-1]):
             if card.is_honour and card.value == cards[index+1].value + 1:
                 return card
         return None
 
@@ -536,15 +531,15 @@
         for suit in long_suits:
             strength[suit] = get_suit_strength(self.unplayed_cards[suit])
         strong_suits = get_list_of_best_scores(lengths)
         if len(strong_suits) == 1:
             return Suit(strong_suits[0])
         return Suit(strong_suits[0])
 
-    def _get_suit_rounds(self) -> Dict[str, int]:
+    def _get_suit_rounds(self) -> dict[str, int]:
         """Return a dict of rounds played by suit."""
         rounds = {suit: 0 for suit in SUITS}
         for trick in self.board.tricks[:-1]:
             rounds[trick.suit.name] += 1
         return rounds
 
     def is_tenace(self, card_1: Card, card_2: Card, gap: int = 1) -> bool:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/second_seat.py` & `bfgcardplay-1.0.7/bfgcardplay/src/second_seat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Second seat card play."""
 
-from typing import List
 import inspect
 
 from bridgeobjects import SUITS, Card, Suit
 from bfgdealer import Trick
 from ..logger import log
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player
 from .utilities import other_suit_for_signals, get_suit_strength
 
 
 class SecondSeat():
     def __init__(self, player: Player):
         self.player = player
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/second_seat_declarer.py` & `bfgcardplay-1.0.7/bfgcardplay/src/second_seat_declarer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Second seat card play for declarer."""
 
-from bridgeobjects.source.constants import CARD_VALUES
+from bridgeobjects.src.constants import CARD_VALUES
 
-from typing import List, Union
-from termcolor import colored
+from termcolor import cprint
 
 import inspect
 
 from ..logger import log
 
 from bridgeobjects import Card, SUITS, Suit
 from bfgdealer import Trick
 from .player import Player
-from .utilities import get_list_of_best_scores, get_suit_strength
+from .utilities import get_list_of_best_scores, get_suit_strength, play_to_unblock
 from .second_seat import SecondSeat
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'green'
 
 
 class SecondSeatDeclarer(SecondSeat):
     def __init__(self, player: Player):
         super().__init__(player)
@@ -54,17 +53,18 @@
 
         # When to duck - rule of 7
         card = self._do_not_duck_if_appropriate(cards, trick)
         if card:
             return card
 
         # Cover honour if own touching honours
-        card = self._cover_honour(cards, trick)
-        if card:
-            return card
+        if trick.cards[0].is_honour:
+            card = self._cover_honour(cards, trick)
+            if card:
+                return card
 
         # Play card if it can beat intermediate lead
         card = self._win_over_intermediate_lead(cards, trick)
         if card:
             return card
 
         # Partner is void or only has pips
@@ -92,15 +92,15 @@
 
     def _can_duck_trick(self, cards, trick) -> bool:
         player = self.player
         if not player.trump_suit:
             return self._duck_trick(player, trick, cards)
         return False
 
-    def _duck_trick(self, player: Player, trick: Trick, cards: List[Card]) -> bool:
+    def _duck_trick(self, player: Player, trick: Trick, cards: list[Card]) -> bool:
         """Return True if the player is to duck the trick."""
         opponents_unplayed_cards = player.opponents_unplayed_cards[trick.suit.name]
         if cards and opponents_unplayed_cards:
             partners_cards = player.partners_suit_cards[trick.suit.name]
             partner_can_win = False
             if partners_cards:
                 if partners_cards[0].value > trick.cards[0].value:
@@ -108,15 +108,15 @@
             can_win_trick = (cards[0].value > opponents_unplayed_cards[0].value and
                              cards[0].value > trick.cards[0].value and
                              not partner_can_win)
             if self._rule_of_seven(player, trick) and can_win_trick:
                 return False
         return True
 
-    def _cover_honour(self, cards,trick) -> Card:
+    def _cover_honour(self, cards,  trick) -> Card:
         player = self.player
 
         # Cover honour if own touching honours
         touching_honours = player.touching_honours(player.our_unplayed_cards[trick.suit.name])
         my_unplayed_cards = len(player.unplayed_cards[trick.suit.name])
         partners_unplayed_cards = len(player.partners_unplayed_cards[trick.suit.name])
         if (trick.cards[0].value >= CARD_VALUES['T'] and cards[0].is_honour and
@@ -133,24 +133,24 @@
 
         if (len(cards) > 1 and
                 cards[0].value == cards[1].value + 1 and
                 CARD_VALUES['A'] > cards[1].value >= CARD_VALUES['T']):
             return log(inspect.stack(), cards[1])
         return None
 
-    def _win_over_intermediate_lead(self, cards,trick) -> Card:
+    def _win_over_intermediate_lead(self, cards, trick) -> Card:
         if trick.cards[0].value >= CARD_VALUES['9']:  # nine or above
             if len(cards) >= 2:
                 if cards[1].value >= CARD_VALUES['T']:
                     for card in cards[::-1]:
                         if card.value > trick.cards[0].value:
                             return log(inspect.stack(), card)
         return None
 
-    def _partner_weak(self, cards,trick) -> Card:
+    def _partner_weak(self, cards, trick) -> Card:
         player = self.player
         partner_void = True
         if player.partners_unplayed_cards[trick.suit.name]:
             partner_void = False
             partners_top_card = player.partners_unplayed_cards[trick.suit.name][0]
             partner_honour = partners_top_card.is_honour
 
@@ -204,15 +204,15 @@
 
         long_suits = get_list_of_best_scores(lengths)
         if player.unplayed_cards[long_suits[0]]:
             return log(inspect.stack(), player.unplayed_cards[long_suits[0]][-1])
 
         return log(inspect.stack(), player.unplayed_cards[player.trump_suit.name][-1])
 
-    def _trump_if_appropriate(self) -> Union[Suit, None]:
+    def _trump_if_appropriate(self) -> Suit | None:
         """Trump if appropriate."""
         player = self.player
         trick = player.board.tricks[-1]
         manager = global_vars.manager
         suit_name = trick.suit.name
 
         if player.trump_suit and player.unplayed_cards[player.trump_suit]:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/second_seat_defender.py` & `bfgcardplay-1.0.7/bfgcardplay/src/second_seat_defender.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from termcolor import colored
 
 import inspect
 
 from ..logger import log
 
 from bridgeobjects import Card, CARD_VALUES, SUITS, Suit, Trick
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player
 from .utilities import get_suit_strength
 from .second_seat import SecondSeat
 from .defender_play import get_hilo_signal_card, signal_card, surplus_card, best_discard
 from .data_classes import SuitCards
 
 MODULE_COLOUR = 'green'
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/suggested_card.py` & `bfgcardplay-1.0.7/bfgcardplay/src/suggested_card.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # suggested_card.py
 
 """Suggested card for Card Player."""
-from typing import Union
 from termcolor import cprint
 
 from bridgeobjects import Card, SEATS
 from bfgdealer import Board
 
 from .player import Player
 from .opening_lead_card import opening_lead_card
@@ -16,20 +15,20 @@
 from .second_seat_defender import SecondSeatDefender
 from .second_seat_declarer import SecondSeatDeclarer
 from .third_seat_defender import ThirdSeatDefender
 from .third_seat_declarer import ThirdSeatDeclarer
 from .fourth_seat_defender import FourthSeatDefender
 from .fourth_seat_declarer import FourthSeatDeclarer
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'blue'
 
 
-def next_card(board: Board) -> Union[Card, None]:
+def next_card(board: Board) -> Card | None:
     """Return the suggested card from the current status of the board."""
     unplayed_cards_in_board = _unplayed_cards(board)
 
     if unplayed_cards_in_board == 52:
         global_vars.initialize()
         return _opening_lead(board)
     if unplayed_cards_in_board == 0:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/third_seat.py` & `bfgcardplay-1.0.7/bfgcardplay/src/third_seat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 """ Third seat card play."""
 
-from typing import Tuple
-
 from bridgeobjects import Card, Denomination
 from bfgdealer import Trick
 
 from .player import Player
+from .utilities import trick_card_values
 
 
 class ThirdSeat():
     def __init__(self, player: Player):
         self.player = player
 
-    @staticmethod
-    def _trick_card_values(trick: Trick, trumps: Denomination) -> Tuple[int, int]:
-        """Return a tuple of card values."""
-        value_0 = trick.cards[0].value
-        if trick.cards[1].suit == trick.cards[0].suit:
-            value_1 = trick.cards[1].value
-        else:
-            value_1 = 0
-        if trumps:
-            if trick.cards[0].suit == trumps:
-                value_0 += 13
-            if trick.cards[1].suit == trumps:
-                value_1 = trick.cards[1].value + 13
-        return (value_0, value_1)
-
     def _ace_is_deprecated(self, trick: Trick, card: Card) -> bool:
         """Return True if the ace is not to be played."""
         player = self.player
         if card.value != 13:
             return False
 
         king = Card(f'K{card.suit.name}')
@@ -41,17 +25,17 @@
         if len(player.total_unplayed_cards[trick.suit]) < 9:
             return False
 
         return True
 
     def _trump_partners_card(self, player: Player, trick: Trick) -> bool:
         """Return True if third hand is to overtump partner's lead."""
-        (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
+        values = trick_card_values(trick, player.trump_suit)
         opponents_cards = player.opponents_unplayed_cards[trick.suit.name]
-        if value_1 > value_0 and trick.cards[0].suit != player.trump_suit:
+        if values[1] > values[0] and trick.cards[0].suit != player.trump_suit:
             return True
         for card in opponents_cards:
             if card.value > trick.cards[0].value:
                 return True
         return False
 
     # def _best_suit(self, player: Player) -> Suit:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/third_seat_declarer.py` & `bfgcardplay-1.0.7/bfgcardplay/src/third_seat_declarer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Third seat card play for declarer."""
-
-from typing import Union, Dict
 from termcolor import cprint
 
 from bridgeobjects import SUITS, Card, Suit
 from bfgdealer import Trick
 
 import inspect
 
 from ..logger import log
 
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 from .player import Player, SuitCards
 from .third_seat import ThirdSeat
 from .declarer_play import card_combinations
+from .utilities import trick_card_values
 
 MODULE_COLOUR = 'blue'
 
 
 class ThirdSeatDeclarer(ThirdSeat):
     def __init__(self, player: Player):
         super().__init__(player)
@@ -135,15 +134,14 @@
         if not player.is_winner_declarer(trick.cards[0], trick):
             for index, card in enumerate(cards[:-1]):
                 if card.value > trick.cards[1].value and card. value > cards[index+1].value + 1:
                     return log(inspect.stack(), card)
 
         return log(inspect.stack(), cards[-1])
 
-
     def _manager_win_trick(self, cards, suit) -> Card:
         player = self.player
         manager = global_vars.manager
         if manager.win_trick[player.seat]:
             manager.win_trick[player.seat] = False
             for card in cards[::-1]:
                 if card.value > player.opponents_unplayed_cards[suit.name][0].value:
@@ -162,15 +160,15 @@
 
     def _missing_king(self, cards, suit, trick) -> Card:
         player = self.player
         manager = global_vars.manager
         (ace, king, queen, jack) = SuitCards(suit.name).cards('A', 'J')
         missing_king = manager.missing_king[player.seat][suit.name]
         if missing_king:
-            if ace in cards and queen not in cards:
+            if ace in cards and queen not in cards and trick.cards[0] != queen:
                 return log(inspect.stack(), ace)
         if manager.suit_strategy(player.seat)[suit.name] == 'missing_king':
             if trick.cards[0] == queen or trick.cards[0] == jack:
                 return log(inspect.stack(), cards[-1])
         return None
 
     def _missing_queen(self, suit, trick) -> Card:
@@ -189,32 +187,31 @@
         dashboard = player.dashboard
         if dashboard.sure_tricks.count == 13 - player.trick_number:
             for card in cards[::-1]:
                 if player.is_winner_declarer(card, trick):
                     return log(inspect.stack(), card)
         return None
 
-
-    def _get_winning_card(self, trick: Trick) -> Union[Card, None]:
+    def _get_winning_card(self, trick: Trick) -> Card | None:
         """Return a card if it can win the trick."""
         player = self.player
         cards = player.cards_for_trick_suit(trick)
 
         # Trick cards
-        value_0, value_1 = player.card_value(trick.cards[0]), player.card_value(trick.cards[1])
+        values = trick_card_values(trick, player.trump_suit)
 
         # Look for tenace about a threat card and play lower card
         (higher_card, lower_card) = player.card_from_my_tenace()
         if (lower_card and
-                lower_card.value > value_0 and
-                lower_card.value > value_1):
+                lower_card.value > values[0] and
+                lower_card.value > values[1]):
             return log(inspect.stack(), lower_card)
 
         # Is this a suit to develop?
-        card = self._card_from_suit_to_develop(player, cards, trick, value_0)
+        card = self._card_from_suit_to_develop(player, cards, trick, values[0])
         if card:
             return card
 
         # If we hold all the winners, take the trick
         card = self._card_from_all_winners(cards, trick)
         if card:
             return card
@@ -265,39 +262,39 @@
             for card in cards[::-1]:
                 if player.is_winner_declarer(card, trick):
                     return log(inspect.stack(), card)
         return None
 
     def _deblock_suit(self, player, cards, trick) -> Card:
         if trick.cards[0].value < cards[0].value:
-            value_0, value_1 = player.card_value(trick.cards[0]), player.card_value(trick.cards[1])
-            is_winner = player.is_winner_declarer(trick.cards[0], trick) and value_0 > value_1
+            values = trick_card_values(trick, player.trump_suit)
+            is_winner = player.is_winner_declarer(trick.cards[0], trick) and values[0] > values[1]
             if is_winner and len(player.partners_unplayed_cards[trick.suit.name]) > 1:
                 return log(inspect.stack(), cards[-1])
 
             our_cards = player.our_unplayed_cards[trick.suit.name]
             partners_length = len(player.partners_unplayed_cards[trick.suit.name])
             my_length = len(player.unplayed_cards[trick.suit.name])
             if (player.is_winner_declarer(our_cards[0], trick) and
                     player.is_winner_declarer(our_cards[1], trick) and
                     my_length < partners_length):
                 return log(inspect.stack(), cards[0])
         return None
 
     def _overtake_partner(self, player, cards, trick) -> Card:
         if not player.is_winner_declarer(trick.cards[0], trick):
-            value_0, value_1 = player.card_value(trick.cards[0]), player.card_value(trick.cards[1])
+            values = trick_card_values(trick, player.trump_suit)
             for index, card in enumerate(cards[:-1]):
                 card_value = card.value
                 # trick card values already adjusted for trumps
                 if card.suit == player.trump_suit:
                     card_value += 13
 
-                if (card_value > value_0 + 1 and
-                        card_value > value_1 and
+                if (card_value > values[0] + 1 and
+                        card_value > values[1] and
                         card.value != cards[index+1].value + 1):
                     if not self._ace_is_deprecated(trick, card):
                         return log(inspect.stack(), card)
         return None
 
     @staticmethod
     def _cover_honour_with_honour(cards, trick) -> Card:
@@ -334,42 +331,42 @@
                 if (trick.cards[0].value > player.opponents_unplayed_cards[trick.suit][0].value and
                         trick.cards[0].value > trick.cards[1].value):
                     return log(inspect.stack(), cards[-1])
                 else:
                     return log(inspect.stack(), cards[0])
         return None
 
-    def _card_from_suit_to_develop(self, player, cards, trick, value_0) -> Card:
+    def _card_from_suit_to_develop(self, player, cards, trick, card_value) -> Card:
         manager = global_vars.manager
         if (manager.suit_to_develop(player.seat) == trick.suit or
                 manager.suit_strategy(player.seat)[trick.suit.name] == 'missing_queen'):
             opponents_cards = player.opponents_unplayed_cards[trick.suit.name]
 
             card = self._card_from_tenace_in_my_hand(cards)
             if card:
                 return card
             else:
-                card = self._card_can_win(cards, value_0, opponents_cards[0])
+                card = self._card_can_win(cards, card_value, opponents_cards[0])
                 if card:
                     return card
         return None
 
     def _card_from_tenace_in_my_hand(self, cards) -> Card:
         player = self.player
         tenace_in_my_hand = player.get_suit_tenaces(cards)
         if tenace_in_my_hand:
             for card in cards:
                 if card.value < tenace_in_my_hand.value:
                     return log(inspect.stack(), card)
         return None
 
     @staticmethod
-    def _card_can_win(cards, value_0, opps_card) -> Card:
+    def _card_can_win(cards, card_value, opps_card) -> Card:
         for card in cards[::-1]:
-            if card.value > value_0 + 1 and card.value > opps_card.value:
+            if card.value > card_value + 1 and card.value > opps_card.value:
                 return log(inspect.stack(), card)
         return None
 
     def _select_card_if_void(self, player: Player, trick: Trick) -> Card:
         """Return card if cannot follow suit."""
         player.record_void(trick.suit)
 
@@ -403,15 +400,15 @@
         # print(colored(f'{dashboard.probable_tricks.count=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.possible_tricks.count=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.sure_tricks.cards=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.probable_tricks.cards=}', MODULE_COLOUR))
         # print(colored(f'{dashboard.possible_promotions.cards=}', MODULE_COLOUR))
 
         # Find a loser
-        suit_length: Dict[str, int] = {}
+        suit_length: dict[str, int] = {}
         for suit_name, suit in suits.items():
             if player.suit_cards[suit_name]:
                 suit_length[suit_name] = len(player.suit_cards[suit_name])
                 our_cards = player.our_unplayed_cards[suit_name]
                 opponents_cards = player.opponents_unplayed_cards[suit_name]
                 # print(colored(f'{suit} {len(opponents_cards)}', MODULE_COLOUR))
                 if opponents_cards:
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/source/third_seat_defender.py` & `bfgcardplay-1.0.7/bfgcardplay/src/third_seat_defender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Third seat card play for defender."""
 
-from typing import Union
 from termcolor import cprint
 
 import inspect
 from ..logger import log
 
 from bridgeobjects import SUITS, Card, CARD_VALUES, Suit
 from bfgdealer import Trick
 from .player import Player
-from .utilities import other_suit_for_signals, get_suit_strength
+from .utilities import (other_suit_for_signals, get_suit_strength, get_seat,
+                        trick_card_values, card_values)
+
 from .third_seat import ThirdSeat
 from .defender_play import deduce_partner_void_in_trumps, get_hilo_signal_card
-import bfgcardplay.source.global_variables as global_vars
+import bfgcardplay.src.global_variables as global_vars
 
 MODULE_COLOUR = 'blue'
 
 MAXIMUM_TRICKS = 13
 TRUMP_VALUE_UPLIFT = 13
+PLAYER_INDEX = 2
 
 
 class ThirdSeatDefender(ThirdSeat):
     def __init__(self, player: Player):
         super().__init__(player)
 
     def selected_card(self) -> Card:
         """Return the card if the third seat."""
         player = self.player
-        manager = global_vars.manager
         trick = player.board.tricks[-1]
-
+        seat = get_seat(trick, PLAYER_INDEX)
 
         cards = player.cards_for_trick_suit(trick)
 
         # Void
         if not cards:
             return self._select_card_if_void(player, trick)
 
@@ -47,14 +48,15 @@
         card = self._winning_card()
         if card:
             return card
 
         # Play high
         card = self._play_high_card(cards, trick)
         if card:
+            player.highest_card[seat][card.suit.name] = card
             return card
 
         # Unblock suit
         card = self._unblock_suit(cards, trick)
         if card:
             return card
 
@@ -92,19 +94,19 @@
         suit_name = trick.suit.name
         if player.trick_number == 1:
             if trick.cards[0].is_honour:
                 manager.set_like_dislike(player.partner_seat, suit_name, True)
 
     def _play_high_card(self, cards, trick) -> Card:
         player = self.player
-        (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
-        if value_1 > value_0:
-            for card in cards[::-1]:
-                if card.value > value_1:
-                    return log(inspect.stack(), card)
+        values = trick_card_values(trick, player.trump_suit)
+        # if values[1] > values[0]:
+        #     for card in cards[::-1]:
+        if cards[0].value > values[1]:
+            return log(inspect.stack(), cards[0])
         return None
 
     def _unblock_suit(self, cards, trick) -> Card:
         player = self.player
         if player.trick_number == 1:
             if trick.cards[0].is_honour and len(cards) <= 2:
                 return log(inspect.stack(), cards[0])
@@ -153,54 +155,55 @@
                     if not card.is_honour:
                         if card.value >= CARD_VALUES['7']:
                             manager.set_like_dislike(player.seat, card.suit.name, 1)
                         return log(inspect.stack(), card)
                 manager.set_like_dislike(player.seat, cards[-1].suit.name, 0)
         return get_hilo_signal_card(player, cards)
 
-    def _winning_card(self) -> Union[Card, None]:
+    def _winning_card(self) -> Card | None:
         """Return the card if can win trick."""
         player = self.player
         trick = player.board.tricks[-1]
-        cards = player.cards_for_trick_suit(trick)
+        my_cards = player.cards_for_trick_suit(trick)
 
         # No cards in trick suit, look for trump winner
-        card = self._trump_if_void(cards, trick)
+        card = self._trump_if_void(my_cards, trick)
         if card:
             return card
 
         # Defeat contract if possible
-        card = self._defeat_contract(cards, trick)
+        card = self._defeat_contract(my_cards, trick)
         if card:
             return card
 
         # Play winner if long suit
-        card = self._winner_in_long_suit(cards, trick)
+        card = self._winner_in_long_suit(my_cards, trick)
         if card:
             return card
 
         # Look for winner
         card = self._look_for_winner(trick)
         if card:
             return card
 
-        card = self._select_card_based_on_position(cards, trick)
+        card = self._select_card_based_on_position(my_cards, trick)
         if card:
             return card
 
         return None
 
     def _trump_if_void(self, cards, trick) -> Card:
         if cards:
             return None
         player = self.player
-        (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
+        values = trick_card_values(trick, player.trump_suit)
         if player.trump and player.trump_cards:
             for card in player.trump_cards[::-1]:
-                if card.value + TRUMP_VALUE_UPLIFT > value_0 + 1 and card.value + TRUMP_VALUE_UPLIFT > value_1:
+                if (card.value + TRUMP_VALUE_UPLIFT > values[0] + 1 and
+                        card.value + TRUMP_VALUE_UPLIFT > values[1]):
                     return log(inspect.stack(), card)
         return None
 
     def _defeat_contract(self, cards, trick) -> Card:
         player = self.player
         if (player.is_winner_defender(cards[0], trick) and
                 not player.is_winner_defender(trick.cards[0], trick) and
@@ -220,53 +223,61 @@
         player = self.player
         if not player.is_winner_defender(trick.cards[0], trick):
             top_touching_honour = player.touching_honours_in_hand(player.hand, trick.suit.name)
             if top_touching_honour and top_touching_honour.value > trick.cards[1].value:
                 return log(inspect.stack(), top_touching_honour)
         return None
 
-    def _select_card_based_on_position(self, cards, trick) -> Card:
-        short_cards = [card for card in cards[:-1]]
-        for index, test_card in enumerate(short_cards[::-1]):
+    def _select_card_based_on_position(self, my_cards, trick) -> Card:
+        player = self.player
+        if not player.dummy_on_left:
+            return None
+
+        # Win trick if possible
+        my_values = card_values(my_cards)
+        for index, value in enumerate(my_values[::-1]):
+            if value > trick.cards[1].value:
+                return log(inspect.stack(), my_cards[::-1][index])
+
+        my_short_cards = [card for card in my_cards]
+        for index, test_card in enumerate(my_short_cards[::-1]):
             # If dummy on left and can win, do so
             card = self._dummy_on_left(test_card, trick)
             if card:
                 return card
 
-            card = self._dummy_tenace_not_dominated(cards, trick, test_card, index)
+            card = self._dummy_tenace_not_dominated(my_cards, trick, test_card, index)
             if card:
                 return card
         return None
 
     def _get_card_value(self, card) -> int:
         card_value = card.value
         # trick card values already adjusted for trumps
         if card.suit == self.player.trump_suit:
             card_value += TRUMP_VALUE_UPLIFT
         return card_value
 
     def _dummy_on_left(self, card, trick) -> Card:
         player = self.player
-        if not player.dummy_on_left:
-            return None
 
-        (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
         if player.dummys_unplayed_cards[trick.suit.name]:
-            if value_1 > value_0:
+            values = trick_card_values(trick, player.trump_suit)
+            if values[1] > values[0]:
                 card_value = self._get_card_value(card)
                 if card_value > player.dummys_unplayed_cards[trick.suit.name][0].value:
                     return log(inspect.stack(), card)
         return None
 
     def _dummy_tenace_not_dominated(self, cards, trick, card, index) -> Card:
         player = self.player
         card_value = self._get_card_value(card)
-        (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
-        if (card_value > value_0 + 3 and
-                card_value > value_1 and
+        values = trick_card_values(trick, player.trump_suit)
+        if (card_value > values[0] + 3 and
+                card_value > values[1] and
                 card.value != cards[index+1].value + 1):
             if (not self._seat_dominates_left_hand_dummy_tenace(card) and
                     not self._ace_is_deprecated(trick, card)):
                 return log(inspect.stack(), card)
         return None
 
     def _seat_dominates_left_hand_dummy_tenace(self, card: Card) -> bool:
@@ -280,26 +291,27 @@
         return False
 
     def _select_card_if_void(self, player: Player, trick: Trick) -> Card:
         """Return card if cannot follow suit."""
         player.record_void(trick.suit)
         # Trump if appropriate
         if player.trump_suit:
-            (value_0, value_1) = self._trick_card_values(trick, player.trump_suit)
+            values = trick_card_values(trick, player.trump_suit)
             if player.trump_cards:
                 unplayed_cards = player.total_unplayed_cards[trick.suit.name]
                 if unplayed_cards:
-                    if (value_1 > value_0 or
+                    if (values[1] > values[0] or
                             trick.cards[0].value < unplayed_cards[0].value):
                         return log(inspect.stack(), player.trump_cards[-1])
 
         # Signal suit preference first time it is led."""
-        signal_card = self._signal_on_first_lead(player, trick)
-        if signal_card:
-            return signal_card
+        if len(player.board.tricks) == 1:
+            signal_card = self._signal_on_first_lead(player, trick)
+            if signal_card:
+                return signal_card
 
         best_suit = self._best_suit(player)
         other_suit = other_suit_for_signals(best_suit)
         if other_suit != player.trump_suit:
             other_suit_cards = player.suit_cards[other_suit]
             if other_suit_cards and not other_suit_cards[-1].is_honour:
                 return log(inspect.stack(), other_suit_cards[-1])
@@ -330,15 +342,15 @@
         max_length = 0
         for suit in SUITS:
             if long_suit_cards[suit] > max_length:
                 max_length = long_suit_cards[suit]
                 long_suit = suit
         return log(inspect.stack(), player.suit_cards[long_suit][-1])
 
-    def _signal_on_first_lead(self, player: Player, trick: Trick) -> Union[Card, None]:
+    def _signal_on_first_lead(self, player: Player, trick: Trick) -> Card | None:
         """Return a card if it is first time that partner led it."""
         suits_already_signed = []
         if player.trump_suit:
             suits_already_signed.append(player.trump_suit)
         for board_trick in player.board.tricks:
             if board_trick.leader == player.partner_seat and board_trick != trick:
                 suits_already_signed.append(board_trick.start_suit)
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/test/test_opening_lead_card.py` & `bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bridgeobjects import Contract, Card
-from ..source.opening_lead_card import opening_lead_card
+from ..src.opening_lead_card import opening_lead_card
 
 SUIT_CONTRACT_TESTA = {
     '96532': ('3', '004'),
 }
 
 SUIT_CONTRACT_TEST = {
     # Based on Klinger's Basic Bridge p138-9
@@ -226,19 +226,19 @@
     'K872': ('2', '004'),
     'QJT2': ('Q', '020'),
     '86': ('8', '001'),
     '98642': ('4', '004'),
 }
 
 
-NT_CONTRACT_TESTA ={
+NT_CONTRACT_TESTA = {
     'AT95': ('T', '022'),
 }
 
-NT_CONTRACT_TEST ={
+NT_CONTRACT_TEST = {
     # Based on Klinger's Basic Bridge p138-9
     '95': ('9', '001'),
     '953': ('5', '005'),
     '96532': ('3', '004'),
 
     'T9': ('T', '001'),
     'T6': ('T', '001'),
@@ -445,25 +445,27 @@
     # 'xxx': ('x', 'xxx'),
     # 'xxx': ('x', 'xxx'),
     # 'xxx': ('x', 'xxx'),
     # 'xxx': ('x', 'xxx'),
 
 }
 
+
 def test_lead_suit_contract():
     """Test the lead card returned in a suit contract."""
     # Arbitrarily use spade suit and 'H' as the contract suit
     contract = Contract('4H')
     for holding, (lead_card, reason) in SUIT_CONTRACT_TEST.items():
         cards = [Card(card_name+'S') for card_name in holding]
         selected_card = opening_lead_card(cards, contract)
         assert selected_card == Card(lead_card+'S'), cards
         assert selected_card.selection_reason == reason, cards
 
+
 def test_lead_nt_contract():
     """Test the lead card returned in a NT contract."""
     contract = Contract('3NT')
     for holding, (lead_card, reason) in NT_CONTRACT_TEST.items():
         cards = [Card(card_name+'S') for card_name in holding]
         selected_card = opening_lead_card(cards, contract)
         assert selected_card == Card(lead_card+'S'), cards
-        assert selected_card.selection_reason == reason, cards
+        assert selected_card.selection_reason == reason, cards
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay/test/test_opening_lead_suit.py` & `bfgcardplay-1.0.7/bfgcardplay/tests/test_opening_lead_suit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 """Test opening lead cards."""
-from bridgeobjects import Hand, Auction, Contract, Call, Suit, Board
+from bridgeobjects import Hand, Auction, Contract, Suit, Board
+
+from ..src.opening_lead_suit import opening_lead_suit
 
-from ..source.opening_lead_suit import opening_lead_suit
 
 def _get_board(dealer, hand, bids):
     """Return a board based on parameters."""
     board = Board()
     board.dealer = dealer
     board.auction = Auction(bids, board.dealer)
     board.contract = Contract(auction=board.auction)
     board.hands[board.contract.leader] = hand
     return board
 
+
 def test_four_card_suit():
     """Test that a 4 card suit is selected against NT contract. Partner not bid."""
     hand = Hand('8642.754.A94.987')
     bids = ['1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '005'
 
+
 def test_best_four_card_suit():
     """Test that the 4 card long suit is selected against NT contract. Partner not bid."""
     hand = Hand('AJ83.754.AQ94.98')
     bids = ['P', '1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '006'
 
+
 def test_long_suit():
     """Test that the long suit is selected against NT contract. Partner not bid."""
     hand = Hand('A9832.75.AK94.98')
     bids = ['1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('E', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '003'
 
+
 def test_best_longest_suit():
     """Test that the best longest suit is selected against NT contract. Partner not bid."""
     hand = Hand('A9832.7.AK954.98')
     bids = ['1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('E', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '009'
 
+
 def test_klinger_3_B_1_i():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('752.87.AJT94.985')
     bids = ['P', '1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
@@ -69,389 +75,425 @@
     bids = ['P', '1D', 'P', '1NT', 'P', '3D', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '019'
 
+
 def test_klinger_3_B_ii_1_b():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('752.87.AJT94.985')
     bids = ['P', 'P', '1H', '1NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '020'
 
+
 def test_klinger_3_B_2_i():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('QJ982.Q4.JT32.98')
     bids = ['1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '001'
 
+
 def test_klinger_3_B_2_ii_a():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('QJ982.Q4.JT32.98')
     bids = ['1S', 'P', '2H', 'P', '2NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '019'
 
+
 def test_klinger_3_B_2_ii_b():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('QJ982.Q4.JT32.98')
     bids = ['1NT', 'P', '2C', 'P', '2H', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '019'
 
+
 def test_klinger_3_B_3_i():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('632.K9753.QT7.J8')
-    bids = ['P','1NT', 'P', '3NT', 'P', 'P', 'P']
+    bids = ['P', '1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '003'
 
+
 def test_klinger_3_B_3_ii_a():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('632.K9753.QT7.J8')
     bids = ['1NT', 'P', '3H', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '019'
 
+
 def test_klinger_3_B_3_ii_b():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('632.K9753.QT7.J8')
     bids = ['2NT', 'P', '3S', 'P', '4S', 'P', '4NT', 'P', '5H', 'P', '6NT', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '022'
 
+
 def test_klinger_3_B_4_i():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('QT982.J83.J732.4')
-    bids = ['P','1NT', 'P', '3NT', 'P', 'P', 'P']
+    bids = ['P', '1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '001'
 
+
 def test_klinger_3_B_4_ii_a():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('QT982.J83.J732.4')
     bids = ['P', '1S', 'P', '2D', 'P', '3D', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '019'
 
+
 # def test_klinger_3_B_4_ii_a(): # Too esoteric
     # """Klinger exercise. Better Card play p15."""
 #     hand = Hand('QT982.J83.J732.4')
 #     seat = 'W'
 #     dealer = 'W'
 #     auction = Auction(['P', '1C', 'P', '1NT', 'P', '2NT', 'P', '3NT', 'P', 'P', 'D', 'P', 'P', 'P'], dealer)
 #     suit = opening_lead_suit(hand, seat, dealer, auction)
 #     assert suit == Suit('C')
 #     assert suit.selection_reason == '019'
 
+
 def test_klinger_3_B_5_i():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('JT986.7.AQT.7432')
     bids = ['P', '1NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
 
-def test_klinger_3_B_5_i():
+
+def test_klinger_3_B_5_iA():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('JT986.7.AQT.7432')
     bids = ['P', '1D', '1H', '2D', 'P', '2H', 'P', '2NT', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '021'
 
+
 def test_klinger_3_B_5_ii():
     """Klinger exercise. Better Card play p15."""
     hand = Hand('JT986.7.AQT.7432')
     bids = ['P', '3C', 'P', '3NT', 'P', 'P', 'P']
     board = _get_board('W', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '021'
 
+
 def test_klinger_4_1_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AJ2.J7.9743.A852')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '014'
 
+
 def test_klinger_4_1_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AJ2.J7.9743.A852')
     dealer = 'S'
     bids = ['1S', 'P', '2D', 'P', '2S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '016'
 
+
 def test_klinger_4_1_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AJ2.J7.9743.A852')
     dealer = 'W'
     bids = ['P', '1NT', '2H', '4S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '020'
 
+
 def test_klinger_4_2_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.J843.K83.A964')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '023'
 
+
 def test_klinger_4_2_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.J843.K83.A964')
     dealer = 'S'
     bids = ['1S', 'P', '2C', 'P', '3C', 'P', '4S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('C')
     assert suit.selection_reason == '026'
 
+
 def test_klinger_4_2_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.J843.K83.A964')
     dealer = 'S'
     bids = ['1H', 'P', '2C', 'P', '2S', 'P', '3H', 'P', '4H', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '014'
 
+
 def test_klinger_4_3_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('83.9.KJ752.Q9843')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '008'
 
+
 # def test_klinger_4_3_ii_a():
     # """Klinger exercise. Better Card play p24."""
 #     hand = Hand('83.9.KJ752.Q9843')
 #     dealer = 'S'
 #     bids = ['1C', 'P', '1S', 'P', '2C', 'P', 'P', 'P']
 #     board = _get_board(dealer, hand, bids)
 #     suit = opening_lead_suit(board)
 
 #     assert suit == Suit('D')  # not sure of reason for D!!!
 #     assert suit.selection_reason == '026'
 
+
 def test_klinger_4_3_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('83.9.KJ752.Q9843')
     dealer = 'S'
     bids = ['1H', 'P', '2C', 'P', '3C', 'P', '4H', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('C')
     assert suit.selection_reason == '026'
 
+
 def test_klinger_4_4_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AQ8.832.QJ72.843')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '027'
 
+
 def test_klinger_4_4_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AQ8.832.QJ72.843')
     dealer = 'S'
     bids = ['1S', 'P', '1NT', 'P', '2H', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '028'
 
+
 def test_klinger_4_4_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('AQ8.832.QJ72.843')
     dealer = 'S'
     bids = ['1C', 'P', '1D', 'P', '1H', 'P', '2H', 'P', '3H', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '028'
 
+
 def test_klinger_4_5_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('KJ6.A975.2.KQ754')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('C')
     assert suit.selection_reason == '027'
 
+
 def test_klinger_4_5_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('KJ6.A975.2.KQ754')
     dealer = 'S'
     bids = ['1D', 'D', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '028'
 
+
 def test_klinger_4_5_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('KJ6.A975.2.KQ754')
     dealer = 'S'
     bids = ['3H', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('C')
     assert suit.selection_reason == '027'
 
+
 def test_klinger_4_6_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('98.AJ64.K763.873')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '028'
 
+
 def test_klinger_4_6_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('98.AJ64.K763.873')
     dealer = 'W'
     bids = ['P', '1C', 'P', '1S', 'P', '3C', 'P', '3S', '4S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '029'
 
+
 def test_klinger_4_6_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('98.AJ64.K763.873')
     dealer = 'S'
     bids = ['1S', 'P', '1NT', 'P', '2H', 'P', '2S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('S')
     assert suit.selection_reason == '028'
 
+
 def test_klinger_4_7_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('A8.7.K872.976432')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '008'
 
+
 def test_klinger_4_7_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('A8.7.K872.976432')
     dealer = 'S'
     bids = ['1S', 'P', '3S', 'P', '4NT', 'P', '5H', '6S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '030'
 
+
 def test_klinger_4_7_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('A8.7.K872.976432')
     dealer = 'S'
     bids = ['1S', 'P', '3D', 'P', '4D', 'P', '4NT', 'P', '5H', '6S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('D')
     assert suit.selection_reason == '030'
 
+
 def test_klinger_4_8_i():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.86.QJT7.98642')
     bids = ['1S', 'P', '3S', 'P', '4S', 'P', 'P', 'P']
     board = _get_board('S', hand, bids)
     suit = opening_lead_suit(board)
 
-
     assert suit == Suit('D')
     assert suit.selection_reason == '002'
 
+
 def test_klinger_4_8_ii_a():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.86.QJT7.98642')
     dealer = 'N'
     bids = ['1C', 'P', '2S', 'P', '3S', 'P', '4NT', 'P', '5H', 'D', '6S', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
 
     assert suit == Suit('H')
     assert suit.selection_reason == '031'
 
+
 def test_klinger_4_8_ii_b():
     """Klinger exercise. Better Card play p24."""
     hand = Hand('K2.86.QJT7.98642')
     dealer = 'N'
     bids = ['1C', 'P', '4NT', 'P', '5H', 'P', '6S', 'P', 'P', 'D', 'P', 'P', 'P']
     board = _get_board(dealer, hand, bids)
     suit = opening_lead_suit(board)
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.0.7/bfgcardplay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.5
+Version: 1.0.7
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.7 29 Jun 2023
+
+1. xxx
+
+------
+
+Version 1.0.7 29 Jun 2023
+
+1. xxx
+
+------
+
+Version 1.0.6 26 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.5 20 Jun 2023
 
 1. Fix bug in opening suit if void in suit
 
 ------
 
 Version 1.0.4 20 Jun 2023
```

### Comparing `bfgcardplay-1.0.5/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.0.7/bfgcardplay.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,39 +3,45 @@
 bfgcardplay/__init__.py
 bfgcardplay/_version.py
 bfgcardplay/logger.py
 bfgcardplay.egg-info/PKG-INFO
 bfgcardplay.egg-info/SOURCES.txt
 bfgcardplay.egg-info/dependency_links.txt
 bfgcardplay.egg-info/top_level.txt
-bfgcardplay/source/__init__.py
-bfgcardplay/source/card_player_components.py
-bfgcardplay/source/cards.py
-bfgcardplay/source/dashboard.py
-bfgcardplay/source/data_classes.py
-bfgcardplay/source/declarer_play.py
-bfgcardplay/source/defender_play.py
-bfgcardplay/source/first_seat.py
-bfgcardplay/source/first_seat_declarer.py
-bfgcardplay/source/first_seat_declarer_nt.py
-bfgcardplay/source/first_seat_declarer_suit.py
-bfgcardplay/source/first_seat_defender.py
-bfgcardplay/source/fourth_seat.py
-bfgcardplay/source/fourth_seat_declarer.py
-bfgcardplay/source/fourth_seat_defender.py
-bfgcardplay/source/global_variables.py
-bfgcardplay/source/manager.py
-bfgcardplay/source/opening_lead.py
-bfgcardplay/source/opening_lead_card.py
-bfgcardplay/source/opening_lead_suit.py
-bfgcardplay/source/player.py
-bfgcardplay/source/second_seat.py
-bfgcardplay/source/second_seat_declarer.py
-bfgcardplay/source/second_seat_defender.py
-bfgcardplay/source/suggested_card.py
-bfgcardplay/source/third_seat.py
-bfgcardplay/source/third_seat_declarer.py
-bfgcardplay/source/third_seat_defender.py
-bfgcardplay/source/utilities.py
-bfgcardplay/test/__init__.py
-bfgcardplay/test/test_opening_lead_card.py
-bfgcardplay/test/test_opening_lead_suit.py
+bfgcardplay/src/__init__.py
+bfgcardplay/src/card_player_components.py
+bfgcardplay/src/cards.py
+bfgcardplay/src/dashboard.py
+bfgcardplay/src/data_classes.py
+bfgcardplay/src/declarer_play.py
+bfgcardplay/src/defender_play.py
+bfgcardplay/src/first_seat.py
+bfgcardplay/src/first_seat_declarer.py
+bfgcardplay/src/first_seat_declarer_nt.py
+bfgcardplay/src/first_seat_declarer_suit.py
+bfgcardplay/src/first_seat_defender.py
+bfgcardplay/src/fourth_seat.py
+bfgcardplay/src/fourth_seat_declarer.py
+bfgcardplay/src/fourth_seat_defender.py
+bfgcardplay/src/global_variables.py
+bfgcardplay/src/manager.py
+bfgcardplay/src/opening_lead.py
+bfgcardplay/src/opening_lead_card.py
+bfgcardplay/src/opening_lead_suit.py
+bfgcardplay/src/player.py
+bfgcardplay/src/second_seat.py
+bfgcardplay/src/second_seat_declarer.py
+bfgcardplay/src/second_seat_defender.py
+bfgcardplay/src/suggested_card.py
+bfgcardplay/src/third_seat.py
+bfgcardplay/src/third_seat_declarer.py
+bfgcardplay/src/third_seat_defender.py
+bfgcardplay/src/utilities.py
+bfgcardplay/tests/__init__.py
+bfgcardplay/tests/test_first_seat_defender.py
+bfgcardplay/tests/test_fourth_seat_declarer.py
+bfgcardplay/tests/test_opening_lead_card.py
+bfgcardplay/tests/test_opening_lead_suit.py
+bfgcardplay/tests/test_player.py
+bfgcardplay/tests/test_third_seat_defender.py
+bfgcardplay/tests/test_utilities.py
+bfgcardplay/tests/utilities.py
```

### Comparing `bfgcardplay-1.0.5/setup.py` & `bfgcardplay-1.0.7/setup.py`

 * *Files identical despite different names*

