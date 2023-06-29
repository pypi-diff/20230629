# Comparing `tmp/tap-github-2.0.4.tar.gz` & `tmp/tap-github-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-github-2.0.4.tar", last modified: Tue May 16 10:47:24 2023, max compression
+gzip compressed data, was "tap-github-2.0.5.tar", last modified: Thu Jun 29 20:59:27 2023, max compression
```

## Comparing `tap-github-2.0.4.tar` & `tap-github-2.0.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.569047 tap-github-2.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-11 18:22:16.000000 tap-github-2.0.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-05-11 18:22:16.000000 tap-github-2.0.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-05-16 10:47:24.569047 tap-github-2.0.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4468 2023-05-11 18:22:16.000000 tap-github-2.0.4/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 10:47:24.569047 tap-github-2.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      895 2023-05-16 10:29:42.000000 tap-github-2.0.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.533047 tap-github-2.0.4/tap_github/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      956 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-05-16 10:29:42.000000 tap-github-2.0.4/tap_github/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2737 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.557047 tap-github-2.0.4/tap_github/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/assignees.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1468 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/collaborators.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2744 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/commit_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6843 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/commits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33251 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26740 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/issue_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/issue_labels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2819 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/issue_milestones.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6192 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/issues.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/pr_commits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2811 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/project_cards.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/project_columns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/projects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46825 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/pull_requests.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4696 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/releases.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3630 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/review_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1393 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/reviews.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.561047 tap-github-2.0.4/tap_github/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      381 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/shared/issue_permissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/shared/performed_via_github_app.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/shared/pull_permissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/shared/reactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/shared/user.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      348 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/stargazers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1571 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/team_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      336 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/team_memberships.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      894 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/schemas/teams.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30669 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10030 2023-05-11 18:22:16.000000 tap-github-2.0.4/tap_github/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.537047 tap-github-2.0.4/tap_github.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1797 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-16 10:47:24.000000 tap-github-2.0.4/tap_github.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:47:24.569047 tap-github-2.0.4/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5265 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2975 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10401 2023-05-11 18:27:12.000000 tap-github-2.0.4/tests/test_github_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9228 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_interrupted_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9163 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_interrupted_sync_add_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10788 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_interrupted_sync_remove_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2023-05-11 18:27:12.000000 tap-github-2.0.4/tests/test_github_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2000 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_parent_child_independednt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10993 2023-05-11 18:27:12.000000 tap-github-2.0.4/tests/test_github_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1016 2023-05-11 18:22:16.000000 tap-github-2.0.4/tests/test_github_sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.930698 tap-github-2.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-11 18:22:16.000000 tap-github-2.0.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-06-28 05:15:08.000000 tap-github-2.0.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-06-29 20:59:27.930698 tap-github-2.0.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4468 2023-06-28 05:15:08.000000 tap-github-2.0.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 20:59:27.930698 tap-github-2.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      895 2023-06-29 16:17:03.000000 tap-github-2.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.922699 tap-github-2.0.5/tap_github/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      956 2023-06-29 12:38:43.000000 tap-github-2.0.5/tap_github/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-06-29 12:38:52.000000 tap-github-2.0.5/tap_github/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2737 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.926699 tap-github-2.0.5/tap_github/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/assignees.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1468 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/collaborators.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2744 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/commit_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6843 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/commits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33251 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26740 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/issue_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/issue_labels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2819 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/issue_milestones.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6192 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/issues.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/pr_commits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2811 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/project_cards.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/project_columns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/projects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46825 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/pull_requests.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2023-06-29 16:17:03.000000 tap-github-2.0.5/tap_github/schemas/releases.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3630 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/review_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1393 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/reviews.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.926699 tap-github-2.0.5/tap_github/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      381 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/shared/issue_permissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/shared/performed_via_github_app.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/shared/pull_permissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/shared/reactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/shared/user.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      348 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/stargazers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1571 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/team_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      336 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/team_memberships.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      894 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/schemas/teams.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30669 2023-06-28 07:58:49.000000 tap-github-2.0.5/tap_github/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10030 2023-06-28 05:15:08.000000 tap-github-2.0.5/tap_github/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.922699 tap-github-2.0.5/tap_github.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1797 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-29 20:59:27.000000 tap-github-2.0.5/tap_github.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 20:59:27.930698 tap-github-2.0.5/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5265 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2975 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10401 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9228 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9163 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_interrupted_sync_add_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10788 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_interrupted_sync_remove_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2000 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_parent_child_independednt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10993 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1016 2023-06-28 05:15:08.000000 tap-github-2.0.5/tests/test_github_sync.py
```

### Comparing `tap-github-2.0.4/LICENSE` & `tap-github-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/README.md` & `tap-github-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/setup.py` & `tap-github-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-github',
-      version='2.0.4',
+      version='2.0.5',
       description='Singer.io tap for extracting data from the GitHub API',
       author='Stitch',
       url='http://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_github'],
       install_requires=[
           'singer-python==5.12.1',
```

### Comparing `tap-github-2.0.4/tap_github/__init__.py` & `tap-github-2.0.5/tap_github/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/client.py` & `tap-github-2.0.5/tap_github/client.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/discover.py` & `tap-github-2.0.5/tap_github/discover.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schema.py` & `tap-github-2.0.5/tap_github/schema.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/assignees.json` & `tap-github-2.0.5/tap_github/schemas/assignees.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/collaborators.json` & `tap-github-2.0.5/tap_github/schemas/collaborators.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/comments.json` & `tap-github-2.0.5/tap_github/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/commit_comments.json` & `tap-github-2.0.5/tap_github/schemas/commit_comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/commits.json` & `tap-github-2.0.5/tap_github/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/events.json` & `tap-github-2.0.5/tap_github/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/issue_events.json` & `tap-github-2.0.5/tap_github/schemas/issue_events.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/issue_labels.json` & `tap-github-2.0.5/tap_github/schemas/issue_labels.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/issue_milestones.json` & `tap-github-2.0.5/tap_github/schemas/issue_milestones.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/issues.json` & `tap-github-2.0.5/tap_github/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/pr_commits.json` & `tap-github-2.0.5/tap_github/schemas/pr_commits.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/project_cards.json` & `tap-github-2.0.5/tap_github/schemas/project_cards.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/project_columns.json` & `tap-github-2.0.5/tap_github/schemas/project_columns.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/projects.json` & `tap-github-2.0.5/tap_github/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/pull_requests.json` & `tap-github-2.0.5/tap_github/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/releases.json` & `tap-github-2.0.5/tap_github/schemas/releases.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998263888888889%*

 * *Differences: {"'properties'": "{'discussion_url': {delete: ['format']}}"}*

```diff
@@ -260,15 +260,14 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "discussion_url": {
-            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "draft": {
             "type": [
```

### Comparing `tap-github-2.0.4/tap_github/schemas/review_comments.json` & `tap-github-2.0.5/tap_github/schemas/review_comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/reviews.json` & `tap-github-2.0.5/tap_github/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/shared/performed_via_github_app.json` & `tap-github-2.0.5/tap_github/schemas/shared/performed_via_github_app.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/shared/reactions.json` & `tap-github-2.0.5/tap_github/schemas/shared/reactions.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/shared/user.json` & `tap-github-2.0.5/tap_github/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/team_members.json` & `tap-github-2.0.5/tap_github/schemas/team_members.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/schemas/teams.json` & `tap-github-2.0.5/tap_github/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/streams.py` & `tap-github-2.0.5/tap_github/streams.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github/sync.py` & `tap-github-2.0.5/tap_github/sync.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tap_github.egg-info/SOURCES.txt` & `tap-github-2.0.5/tap_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_all_fields.py` & `tap-github-2.0.5/tests/test_github_all_fields.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_automatic_fields.py` & `tap-github-2.0.5/tests/test_github_automatic_fields.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_bookmarks.py` & `tap-github-2.0.5/tests/test_github_bookmarks.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_discovery.py` & `tap-github-2.0.5/tests/test_github_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_interrupted_sync.py` & `tap-github-2.0.5/tests/test_github_interrupted_sync.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_interrupted_sync_add_stream.py` & `tap-github-2.0.5/tests/test_github_interrupted_sync_add_stream.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_interrupted_sync_remove_stream.py` & `tap-github-2.0.5/tests/test_github_interrupted_sync_remove_stream.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_pagination.py` & `tap-github-2.0.5/tests/test_github_pagination.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_parent_child_independednt.py` & `tap-github-2.0.5/tests/test_github_parent_child_independednt.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_start_date.py` & `tap-github-2.0.5/tests/test_github_start_date.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.4/tests/test_github_sync.py` & `tap-github-2.0.5/tests/test_github_sync.py`

 * *Files identical despite different names*

