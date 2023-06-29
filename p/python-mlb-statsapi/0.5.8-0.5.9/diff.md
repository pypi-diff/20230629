# Comparing `tmp/python-mlb-statsapi-0.5.8.tar.gz` & `tmp/python-mlb-statsapi-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mlb-statsapi-0.5.8.tar", last modified: Tue Mar  7 21:20:13 2023, max compression
+gzip compressed data, was "python-mlb-statsapi-0.5.9.tar", last modified: Tue Mar  7 21:38:02 2023, max compression
```

## Comparing `python-mlb-statsapi-0.5.8.tar` & `python-mlb-statsapi-0.5.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.732857 python-mlb-statsapi-0.5.8/mlbstatsapi/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74731 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_dataadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.732857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.732857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/attendance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/awards/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/awards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/awards/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/awards/awards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/data/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/divisions/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/divisions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/divisions/division.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/rounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/gamedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/boxscore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/linescore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/livedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.736857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/matchup/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/matchup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/matchup/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/matchup/matchup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/play.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playevent/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playevent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playevent/playevent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/playrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/playbyinning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/plays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/gamepace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/homerunderby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/leagues/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/leagues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/leagues/league.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/seasons/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/seasons/season.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/sports/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/sports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/sports/sport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.740857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/standings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/catching.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/fielding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/game.py
--rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/hitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    32030 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/pitching.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/running.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/streak.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-07 21:19:31.000000 python-mlb-statsapi-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-03-07 21:20:13.000000 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-07 21:20:13.000000 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:20:13.000000 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-07 21:20:13.000000 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-07 21:20:13.000000 python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 21:20:13.744857 python-mlb-statsapi-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74731 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_dataadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/awards/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/awards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/awards/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/awards/awards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/divisions/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/divisions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/divisions/division.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/rounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.131836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.135836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.135836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/boxscore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.135836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/linescore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/livedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/matchup/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/matchup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/matchup/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/matchup/matchup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/play.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playevent/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playevent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playevent/playevent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/playrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/playbyinning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/plays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/gamepace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/homerunderby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/leagues/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/leagues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/leagues/league.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/seasons/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/seasons/season.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.139836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/sports/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/sports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/sports/sport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/standings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/catching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/fielding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27660 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/hitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32030 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/pitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/streak.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-07 21:37:12.000000 python-mlb-statsapi-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-03-07 21:38:02.000000 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-07 21:38:02.000000 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:38:02.000000 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-07 21:38:02.000000 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-07 21:38:02.000000 python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 21:38:02.143836 python-mlb-statsapi-0.5.9/setup.cfg
```

### Comparing `python-mlb-statsapi-0.5.8/LICENSE` & `python-mlb-statsapi-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/PKG-INFO` & `python-mlb-statsapi-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mlb-statsapi
-Version: 0.5.8
+Version: 0.5.9
 Summary: mlbstatsapi python wrapper
 Author-email: Matthew Spah <spahmatthew@gmail.com>, Kristian Nilssen <krinilssen@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -65,34 +65,36 @@
 
 ### [Examples](#examples) | [Wiki](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki) | [API](https://statsapi.mlb.com/) 
 
 <div align="left">
 
 ## Installation
 ```python
-python3 -m pip install python-mlb-statsapi==0.5.7
+python3 -m pip install python-mlb-statsapi==0.5.9
 ```
 ## Usage
 ```python
 python3
 >>> import mlbstatsapi
 >>> mlb = mlbstatsapi.Mlb()
 >>> mlb.get_people_id("Ty France")
 [664034]
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
->>> mlb.get_player_stats(664034, stats=stats, groups=groups)
+>>> params = {'season': 2022}
+>>> mlb.get_player_stats(664034, stats, groups, **params)
 {'hitting': {'season': Stat, 'seasonadvanced': Stat }}
 
 >>> mlb.get_team_id("Oakland Athletics")
 [133]
 
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['pitching']
->>> mlb.get_team_stats(133, stats, groups)
+>>> params = {'season': 2022}
+>>> mlb.get_team_stats(133, stats, groups, **params)
 {'pitching': {'season': Stat, 'seasonadvanced': Stat }}
 ```
 
 
 ## Documentation
 
 ### [People, Person, Players, Coaches](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki/Data-Types:-People)
@@ -158,18 +160,20 @@
 #### Player Stats
 Get the Id(s) of the players you want stats for and set stat types and groups.
 ```python
 >>> mlb = mlbstatsapi.Mlb()
 >>> player_id = mlb.get_people_id("Ty France")[0]
 >>> stats = ['season', 'career']
 >>> groups = ['hitting', 'pitching']
+>>> params = {'season': 2022}
+
 ```
 Use player.id and stat types and groups to return a stats dictionary
 ```python
->>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups )
+>>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups, **params)
 >>> season_hitting_stat = stat_dict['hitting']['season']
 >>> career_pitching_stat = stat_dict['pitching']['career']
 ```
 Print season hitting stats
 ```python
 >>> for split in season_hitting_stat.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -210,18 +214,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Use team.id and the stat types and groups to return season hitting stats
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 Print season and seasonadvanced stats
 ```python
 >>> for split in season_hitting.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -249,18 +255,20 @@
 ```python
 >>> player_id = mlb.get_people_id('Ty France')[0]
 ```
 Set the stat type and group
 ```python
 >>> stats = ['expectedStatistics']
 >>> group = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Get Stats
 ```python
->>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group)
+>>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group, **params)
 >>> expectedstats = stats['hitting']['expectedstatistics']
 >>> for split in expectedstats.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...         print(k, v)
 avg .259
 slg .394
 woba .317
@@ -272,19 +280,19 @@
 >>> ty_france_id = mlb.get_people_id('Ty France')[0]
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set stat type, stat groups, and params
 ```python
 >>> stats = ['vsPlayer']
 >>> group = ['hitting']
->>> params = {'opposingPlayerId': shohei_ohtani_id}
+>>> params = {'opposingPlayerId': shohei_ohtani_id, 'season': 2022}
 ```
 Get stats
 ```python
->>> stats = mlb.get_player_stats(ty_france_id, stats=self.stats, groups=self.group, **self.params)
+>>> stats = mlb.get_player_stats(ty_france_id, stats=stats, groups=group, **params)
 >>> vs_player_total = stats['hitting']['vsplayertotal']
 >>> for split in vs_player_total.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...             print(k, v)
 gamesplayed 4
 groundouts 3
 airouts 4
@@ -312,20 +320,21 @@
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set the stat types and groups
 ```python
 >>> stats = ['hotColdZones']
 >>> hitting_group = ['hitting']
 >>> pitching_group = ['pitching']
+>>> params = {'season': 2022}
 ```
 The stat groups pitching and hitting both return hotColdZones for a pitcher and hitter. hotColdZones are not assigned to a
 stat group because of issues related to the REST API. So hotColdZones will be assigned to the stat key in stats return dict.
 ```python
->>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=type, groups=hitting_group)
->>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=type, groups=pitching_group)
+>>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=stats, groups=hitting_group, **params)
+>>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=stats, groups=pitching_group, **params)
 ```
 hotColdZones returns a list of the HotColdZones
 ```python
 >>> ty_france_hotcoldzones = hitting_hotcoldzones['stats']['hotcoldzones']
 >>> shohei_ohtani_hotcoldzones = pitching_hotcoldzones['stats']['hotcoldzones']
 ```
 Loop through hotColdZone objects for Ty France
@@ -372,18 +381,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Pass season to get_team_stats()
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, season=2018)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 season should be 2018
 ```python
 >>> for split in season_hitting.splits:
 ...     print('Season: ', split.season)
```

### Comparing `python-mlb-statsapi-0.5.8/README.md` & `python-mlb-statsapi-0.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,34 +31,36 @@
 
 ### [Examples](#examples) | [Wiki](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki) | [API](https://statsapi.mlb.com/) 
 
 <div align="left">
 
 ## Installation
 ```python
-python3 -m pip install python-mlb-statsapi==0.5.7
+python3 -m pip install python-mlb-statsapi==0.5.9
 ```
 ## Usage
 ```python
 python3
 >>> import mlbstatsapi
 >>> mlb = mlbstatsapi.Mlb()
 >>> mlb.get_people_id("Ty France")
 [664034]
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
->>> mlb.get_player_stats(664034, stats=stats, groups=groups)
+>>> params = {'season': 2022}
+>>> mlb.get_player_stats(664034, stats, groups, **params)
 {'hitting': {'season': Stat, 'seasonadvanced': Stat }}
 
 >>> mlb.get_team_id("Oakland Athletics")
 [133]
 
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['pitching']
->>> mlb.get_team_stats(133, stats, groups)
+>>> params = {'season': 2022}
+>>> mlb.get_team_stats(133, stats, groups, **params)
 {'pitching': {'season': Stat, 'seasonadvanced': Stat }}
 ```
 
 
 ## Documentation
 
 ### [People, Person, Players, Coaches](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki/Data-Types:-People)
@@ -124,18 +126,20 @@
 #### Player Stats
 Get the Id(s) of the players you want stats for and set stat types and groups.
 ```python
 >>> mlb = mlbstatsapi.Mlb()
 >>> player_id = mlb.get_people_id("Ty France")[0]
 >>> stats = ['season', 'career']
 >>> groups = ['hitting', 'pitching']
+>>> params = {'season': 2022}
+
 ```
 Use player.id and stat types and groups to return a stats dictionary
 ```python
->>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups )
+>>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups, **params)
 >>> season_hitting_stat = stat_dict['hitting']['season']
 >>> career_pitching_stat = stat_dict['pitching']['career']
 ```
 Print season hitting stats
 ```python
 >>> for split in season_hitting_stat.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -176,18 +180,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Use team.id and the stat types and groups to return season hitting stats
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 Print season and seasonadvanced stats
 ```python
 >>> for split in season_hitting.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -215,18 +221,20 @@
 ```python
 >>> player_id = mlb.get_people_id('Ty France')[0]
 ```
 Set the stat type and group
 ```python
 >>> stats = ['expectedStatistics']
 >>> group = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Get Stats
 ```python
->>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group)
+>>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group, **params)
 >>> expectedstats = stats['hitting']['expectedstatistics']
 >>> for split in expectedstats.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...         print(k, v)
 avg .259
 slg .394
 woba .317
@@ -238,19 +246,19 @@
 >>> ty_france_id = mlb.get_people_id('Ty France')[0]
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set stat type, stat groups, and params
 ```python
 >>> stats = ['vsPlayer']
 >>> group = ['hitting']
->>> params = {'opposingPlayerId': shohei_ohtani_id}
+>>> params = {'opposingPlayerId': shohei_ohtani_id, 'season': 2022}
 ```
 Get stats
 ```python
->>> stats = mlb.get_player_stats(ty_france_id, stats=self.stats, groups=self.group, **self.params)
+>>> stats = mlb.get_player_stats(ty_france_id, stats=stats, groups=group, **params)
 >>> vs_player_total = stats['hitting']['vsplayertotal']
 >>> for split in vs_player_total.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...             print(k, v)
 gamesplayed 4
 groundouts 3
 airouts 4
@@ -278,20 +286,21 @@
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set the stat types and groups
 ```python
 >>> stats = ['hotColdZones']
 >>> hitting_group = ['hitting']
 >>> pitching_group = ['pitching']
+>>> params = {'season': 2022}
 ```
 The stat groups pitching and hitting both return hotColdZones for a pitcher and hitter. hotColdZones are not assigned to a
 stat group because of issues related to the REST API. So hotColdZones will be assigned to the stat key in stats return dict.
 ```python
->>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=type, groups=hitting_group)
->>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=type, groups=pitching_group)
+>>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=stats, groups=hitting_group, **params)
+>>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=stats, groups=pitching_group, **params)
 ```
 hotColdZones returns a list of the HotColdZones
 ```python
 >>> ty_france_hotcoldzones = hitting_hotcoldzones['stats']['hotcoldzones']
 >>> shohei_ohtani_hotcoldzones = pitching_hotcoldzones['stats']['hotcoldzones']
 ```
 Loop through hotColdZone objects for Ty France
@@ -338,18 +347,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Pass season to get_team_stats()
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, season=2018)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 season should be 2018
 ```python
 >>> for split in season_hitting.splits:
 ...     print('Season: ', split.season)
```

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_api.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_api.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_dataadapter.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_dataadapter.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/mlb_module.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/mlb_module.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/attendance.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/attendance.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/attendances/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/attendances/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/awards/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/awards/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/data/data.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/data/data.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/divisions/division.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/divisions/division.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/drafts/rounds.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/drafts/rounds.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/game.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/game.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/gamedata/gamedata.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/gamedata/gamedata.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/boxscore/boxscore.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/boxscore/boxscore.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/linescore/linescore.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/linescore/linescore.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/livedata.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/livedata.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/matchup/matchup.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/matchup/matchup.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/play.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/play.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playevent/playevent.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playevent/playevent.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/play/playrunner/playrunner.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/play/playrunner/playrunner.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/playbyinning/playbyinning.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/playbyinning/playbyinning.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/game/livedata/plays/plays.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/game/livedata/plays/plays.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/gamepace/gamepace.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/gamepace/gamepace.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/homerunderby/homerunderby.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/homerunderby/homerunderby.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/leagues/league.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/leagues/league.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/people/people.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/people/people.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/schedules/schedule.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/schedules/schedule.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/seasons/season.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/seasons/season.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/sports/sport.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/sports/sport.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/standings/standings.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/standings/standings.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/__init__.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/catching.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/catching.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/fielding.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/fielding.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/game.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/game.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/hitting.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/hitting.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/pitching.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/pitching.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/running.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/running.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/stats/stats.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/stats/stats.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/teams/team.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/teams/team.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/attributes.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/attributes.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/mlbstatsapi/models/venues/venue.py` & `python-mlb-statsapi-0.5.9/mlbstatsapi/models/venues/venue.py`

 * *Files identical despite different names*

### Comparing `python-mlb-statsapi-0.5.8/pyproject.toml` & `python-mlb-statsapi-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-mlb-statsapi"
-version = "0.5.8"
+version = "0.5.9"
 
 authors = [
   { name="Matthew Spah", email="spahmatthew@gmail.com" },
   { name="Kristian Nilssen", email="krinilssen@gmail.com" },
 ]
 description = "mlbstatsapi python wrapper"
 readme = "README.md"
```

### Comparing `python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/PKG-INFO` & `python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mlb-statsapi
-Version: 0.5.8
+Version: 0.5.9
 Summary: mlbstatsapi python wrapper
 Author-email: Matthew Spah <spahmatthew@gmail.com>, Kristian Nilssen <krinilssen@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -65,34 +65,36 @@
 
 ### [Examples](#examples) | [Wiki](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki) | [API](https://statsapi.mlb.com/) 
 
 <div align="left">
 
 ## Installation
 ```python
-python3 -m pip install python-mlb-statsapi==0.5.7
+python3 -m pip install python-mlb-statsapi==0.5.9
 ```
 ## Usage
 ```python
 python3
 >>> import mlbstatsapi
 >>> mlb = mlbstatsapi.Mlb()
 >>> mlb.get_people_id("Ty France")
 [664034]
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
->>> mlb.get_player_stats(664034, stats=stats, groups=groups)
+>>> params = {'season': 2022}
+>>> mlb.get_player_stats(664034, stats, groups, **params)
 {'hitting': {'season': Stat, 'seasonadvanced': Stat }}
 
 >>> mlb.get_team_id("Oakland Athletics")
 [133]
 
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['pitching']
->>> mlb.get_team_stats(133, stats, groups)
+>>> params = {'season': 2022}
+>>> mlb.get_team_stats(133, stats, groups, **params)
 {'pitching': {'season': Stat, 'seasonadvanced': Stat }}
 ```
 
 
 ## Documentation
 
 ### [People, Person, Players, Coaches](https://github.com/zero-sum-seattle/python-mlb-statsapi/wiki/Data-Types:-People)
@@ -158,18 +160,20 @@
 #### Player Stats
 Get the Id(s) of the players you want stats for and set stat types and groups.
 ```python
 >>> mlb = mlbstatsapi.Mlb()
 >>> player_id = mlb.get_people_id("Ty France")[0]
 >>> stats = ['season', 'career']
 >>> groups = ['hitting', 'pitching']
+>>> params = {'season': 2022}
+
 ```
 Use player.id and stat types and groups to return a stats dictionary
 ```python
->>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups )
+>>> stat_dict = mlb.get_player_stats(player_id, stats=stats, groups=groups, **params)
 >>> season_hitting_stat = stat_dict['hitting']['season']
 >>> career_pitching_stat = stat_dict['pitching']['career']
 ```
 Print season hitting stats
 ```python
 >>> for split in season_hitting_stat.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -210,18 +214,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Use team.id and the stat types and groups to return season hitting stats
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 Print season and seasonadvanced stats
 ```python
 >>> for split in season_hitting.splits:
 ...     for k, v in split.stat.__dict__.items():
@@ -249,18 +255,20 @@
 ```python
 >>> player_id = mlb.get_people_id('Ty France')[0]
 ```
 Set the stat type and group
 ```python
 >>> stats = ['expectedStatistics']
 >>> group = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Get Stats
 ```python
->>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group)
+>>> stats = mlb.get_player_stats(player_id, stats=stats, groups=group, **params)
 >>> expectedstats = stats['hitting']['expectedstatistics']
 >>> for split in expectedstats.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...         print(k, v)
 avg .259
 slg .394
 woba .317
@@ -272,19 +280,19 @@
 >>> ty_france_id = mlb.get_people_id('Ty France')[0]
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set stat type, stat groups, and params
 ```python
 >>> stats = ['vsPlayer']
 >>> group = ['hitting']
->>> params = {'opposingPlayerId': shohei_ohtani_id}
+>>> params = {'opposingPlayerId': shohei_ohtani_id, 'season': 2022}
 ```
 Get stats
 ```python
->>> stats = mlb.get_player_stats(ty_france_id, stats=self.stats, groups=self.group, **self.params)
+>>> stats = mlb.get_player_stats(ty_france_id, stats=stats, groups=group, **params)
 >>> vs_player_total = stats['hitting']['vsplayertotal']
 >>> for split in vs_player_total.splits:
 ...     for k, v in split.stat.__dict__.items():
 ...             print(k, v)
 gamesplayed 4
 groundouts 3
 airouts 4
@@ -312,20 +320,21 @@
 >>> shohei_ohtani_id = mlb.get_people_id('Shohei Ohtani')[0]
 ```
 Set the stat types and groups
 ```python
 >>> stats = ['hotColdZones']
 >>> hitting_group = ['hitting']
 >>> pitching_group = ['pitching']
+>>> params = {'season': 2022}
 ```
 The stat groups pitching and hitting both return hotColdZones for a pitcher and hitter. hotColdZones are not assigned to a
 stat group because of issues related to the REST API. So hotColdZones will be assigned to the stat key in stats return dict.
 ```python
->>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=type, groups=hitting_group)
->>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=type, groups=pitching_group)
+>>> hitting_hotcoldzones = mlb.get_player_stats(ty_france_id stats=stats, groups=hitting_group, **params)
+>>> pitching_hotcoldzones = mlb.get_player_stats(shohei_ohtani_id, stats=stats, groups=pitching_group, **params)
 ```
 hotColdZones returns a list of the HotColdZones
 ```python
 >>> ty_france_hotcoldzones = hitting_hotcoldzones['stats']['hotcoldzones']
 >>> shohei_ohtani_hotcoldzones = pitching_hotcoldzones['stats']['hotcoldzones']
 ```
 Loop through hotColdZone objects for Ty France
@@ -372,18 +381,20 @@
 >>> mlb = mlbstatsapi.Mlb()
 >>> team_id = mlb.get_team_id('Seattle Mariners')[0]
 ```
 Set the stat types and groups.
 ```python
 >>> stats = ['season', 'seasonAdvanced']
 >>> groups = ['hitting']
+>>> params = {'season': 2022}
+
 ```
 Pass season to get_team_stats()
 ```python
-stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, season=2018)
+stats = mlb.get_team_stats(team_id, stats=stats, groups=groups, **params)
 season_hitting = stats['hitting']['season']
 advanced_hitting = stats['hitting']['seasonadvanced']
 ```
 season should be 2018
 ```python
 >>> for split in season_hitting.splits:
 ...     print('Season: ', split.season)
```

### Comparing `python-mlb-statsapi-0.5.8/python_mlb_statsapi.egg-info/SOURCES.txt` & `python-mlb-statsapi-0.5.9/python_mlb_statsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

