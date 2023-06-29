# Comparing `tmp/mvt-2.2.6.tar.gz` & `tmp/mvt-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.2.6.tar", last modified: Tue Apr 25 10:26:51 2023, max compression
+gzip compressed data, was "mvt-2.3.0.tar", last modified: Thu Jun 29 15:10:48 2023, max compression
```

## Comparing `mvt-2.2.6.tar` & `mvt-2.3.0.tar`

### file list

```diff
@@ -1,190 +1,195 @@
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/
--rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2021-07-26 21:43:37.000000 mvt-2.2.6/LICENSE
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-25 10:26:51.083432 mvt-2.2.6/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2509 2022-06-17 08:45:47.000000 mvt-2.2.6/README.md
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    11066 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/android/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      973 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/cmd_check_adb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1083 2023-04-21 21:07:25.000000 mvt-2.2.6/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3798 2023-04-21 21:12:02.000000 mvt-2.2.6/mvt/android/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2589 2023-04-21 21:12:14.000000 mvt-2.2.6/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6077 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt/android/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/adb/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1271 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12263 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3211 2023-03-24 17:45:57.000000 mvt-2.2.6/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1772 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-03-24 17:25:12.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1975 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1633 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1329 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3080 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5130 2023-03-24 17:36:10.000000 mvt-2.2.6/mvt/android/modules/adb/files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2173 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1905 2023-03-01 21:33:36.000000 mvt-2.2.6/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    12138 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/adb/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2685 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1367 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3543 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5656 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/android/modules/adb/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3474 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      739 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1291 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2330 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2285 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3045 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3865 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3567 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2918 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2115 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2935 2023-03-01 21:41:19.000000 mvt-2.2.6/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2031 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/backup/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2175 2023-04-19 15:56:21.000000 mvt-2.2.6/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/modules/bugreport/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      646 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2396 2023-04-19 15:50:11.000000 mvt-2.2.6/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3202 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2911 2023-03-01 21:38:00.000000 mvt-2.2.6/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2687 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2146 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2315 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2341 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4205 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3772 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.071432 mvt-2.2.6/mvt/android/parsers/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      549 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/android/parsers/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7503 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/android/parsers/backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    15778 2023-03-01 21:38:01.000000 mvt-2.2.6/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      723 2023-03-29 12:05:03.000000 mvt-2.2.6/mvt/android/parsers/getprop.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-03-24 17:47:13.000000 mvt-2.2.6/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6436 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/command.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      799 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/help.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    20857 2023-04-07 13:06:52.000000 mvt-2.2.6/mvt/common/indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2132 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/logo.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8227 2023-04-13 07:25:51.000000 mvt-2.2.6/mvt/common/module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1242 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/options.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7797 2023-03-24 17:57:36.000000 mvt-2.2.6/mvt/common/updates.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5787 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/url.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6695 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/common/utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-04-25 10:18:47.000000 mvt-2.2.6/mvt/common/version.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1365 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/common/virustotal.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10628 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/ios/cli.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1189 2023-04-21 21:13:24.000000 mvt-2.2.6/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1170 2023-04-21 21:13:33.000000 mvt-2.2.6/mvt/ios/cmd_check_fs.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     8970 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/decrypt.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2450 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6222 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6614 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3829 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     7223 2023-04-07 10:26:00.000000 mvt-2.2.6/mvt/ios/modules/base.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.075432 mvt-2.2.6/mvt/ios/modules/fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      894 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4691 2023-04-12 08:16:00.000000 mvt-2.2.6/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2669 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2887 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3014 2023-04-11 19:15:22.000000 mvt-2.2.6/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1651 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3734 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3735 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2140 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1369 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1692 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1702 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1425 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/mvt/ios/modules/mixed/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1506 2023-04-11 18:44:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4984 2023-04-25 09:59:00.000000 mvt-2.2.6/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5072 2023-04-20 17:08:05.000000 mvt-2.2.6/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2349 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3354 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3185 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2148 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3215 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2906 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4377 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    14449 2023-04-07 10:26:00.000000 mvt-2.2.6/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5163 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1442 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2869 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6075 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5912 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5364 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5094 2023-04-12 10:39:42.000000 mvt-2.2.6/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4227 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6842 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4525 2023-04-07 12:42:40.000000 mvt-2.2.6/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6438 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     4597 2023-04-12 16:50:38.000000 mvt-2.2.6/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    10455 2023-02-21 19:11:24.000000 mvt-2.2.6/mvt/ios/modules/net_base.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)    14195 2023-04-07 20:22:15.000000 mvt-2.2.6/mvt/ios/versions.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.067432 mvt-2.2.6/mvt.egg-info/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     3040 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     6096 2023-04-25 10:26:51.000000 mvt-2.2.6/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/entry_points.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)      189 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/requires.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-04-25 10:26:50.000000 mvt-2.2.6/mvt.egg-info/top_level.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1638 2023-04-25 10:26:51.083432 mvt-2.2.6/setup.cfg
--rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-02-21 19:11:24.000000 mvt-2.2.6/setup.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/android/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2720 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_backup_module.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2061 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_backup_parser.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1585 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2372 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android/test_dumpsys_parser.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/android_androidqf/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:24.000000 mvt-2.2.6/tests/android_androidqf/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      629 2023-03-01 21:41:05.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      633 2023-03-01 21:39:38.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1353 2023-03-29 10:50:24.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      607 2023-03-01 21:41:53.000000 mvt-2.2.6/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-29 12:05:03.000000 mvt-2.2.6/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      670 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/android_androidqf/test_processes.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      618 2023-03-01 21:40:12.000000 mvt-2.2.6/tests/android_androidqf/test_settings.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      639 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.079432 mvt-2.2.6/tests/common/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/common/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1744 2023-04-07 12:35:45.000000 mvt-2.2.6/tests/common/test_indicators.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2290 2023-03-01 21:38:00.000000 mvt-2.2.6/tests/common/test_utils.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/conftest.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/tests/ios_backup/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      571 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1133 2023-04-11 19:12:42.000000 mvt-2.2.6/tests/ios_backup/test_calendar.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1125 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_datausage.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1008 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_manifest.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1010 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_sms.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1266 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_backup/test_tcc.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      688 2023-03-01 21:42:08.000000 mvt-2.2.6/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-04-25 10:26:51.083432 mvt-2.2.6/tests/ios_fs/
--rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/ios_fs/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1139 2023-04-11 19:15:26.000000 mvt-2.2.6/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      573 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_android_androidqf.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      587 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_android_bugreport.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      526 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_check_ios_backup.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      484 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/test_ios_versions.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)      928 2023-02-21 19:11:25.000000 mvt-2.2.6/tests/utils.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.301082 mvt-2.3.0/
+-rw-r--r--   0 donncha    (501) staff       (20)    17791 2022-06-22 15:39:11.000000 mvt-2.3.0/LICENSE
+-rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-06-29 15:10:48.301158 mvt-2.3.0/PKG-INFO
+-rw-r--r--   0 donncha    (501) staff       (20)     3711 2023-06-29 14:48:56.000000 mvt-2.3.0/README.md
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.272590 mvt-2.3.0/mvt/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.274896 mvt-2.3.0/mvt/android/
+-rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    11065 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cli.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1094 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3727 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2598 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6138 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.275045 mvt-2.3.0/mvt/android/modules/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/modules/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.278345 mvt-2.3.0/mvt/android/modules/adb/
+-rw-r--r--   0 donncha    (501) staff       (20)     1290 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    12370 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3274 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1798 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1779 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2779 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1992 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1635 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1757 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1353 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3269 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5185 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/files.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2190 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1820 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 donncha    (501) staff       (20)    12214 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2687 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1777 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3664 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5613 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3422 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.280354 mvt-2.3.0/mvt/android/modules/androidqf/
+-rw-r--r--   0 donncha    (501) staff       (20)      736 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1315 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2394 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2347 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3225 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3894 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3808 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2759 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3016 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2221 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2914 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.281067 mvt-2.3.0/mvt/android/modules/backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      238 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2069 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/backup/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2176 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.282866 mvt-2.3.0/mvt/android/modules/bugreport/
+-rw-r--r--   0 donncha    (501) staff       (20)      664 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2471 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2435 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3408 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2949 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2701 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2189 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2401 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2440 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4158 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4010 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.283493 mvt-2.3.0/mvt/android/parsers/
+-rw-r--r--   0 donncha    (501) staff       (20)      492 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7297 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)    16021 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/dumpsys.py
+-rw-r--r--   0 donncha    (501) staff       (20)      689 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/getprop.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.286051 mvt-2.3.0/mvt/common/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/common/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2598 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6294 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/command.py
+-rw-r--r--   0 donncha    (501) staff       (20)      799 2023-05-10 16:45:13.000000 mvt-2.3.0/mvt/common/help.py
+-rw-r--r--   0 donncha    (501) staff       (20)    22958 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/indicators.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2208 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/logo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     8455 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/module.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1258 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/options.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7545 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/updates.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5744 2023-06-29 12:27:56.000000 mvt-2.3.0/mvt/common/url.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6932 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/utils.py
+-rw-r--r--   0 donncha    (501) staff       (20)      215 2023-06-29 15:01:05.000000 mvt-2.3.0/mvt/common/version.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1358 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/virustotal.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.286903 mvt-2.3.0/mvt/ios/
+-rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    10651 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cli.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1200 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1181 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cmd_check_fs.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.287351 mvt-2.3.0/mvt/ios/data/
+-rw-r--r--   0 donncha    (501) staff       (20)     3550 2023-05-21 15:40:36.000000 mvt-2.3.0/mvt/ios/data/ios_models.json
+-rw-r--r--   0 donncha    (501) staff       (20)    15419 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/data/ios_versions.json
+-rw-r--r--   0 donncha    (501) staff       (20)     9049 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/decrypt.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.287792 mvt-2.3.0/mvt/ios/modules/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.288588 mvt-2.3.0/mvt/ios/modules/backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      439 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2601 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7211 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6914 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3838 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7146 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/base.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.290762 mvt-2.3.0/mvt/ios/modules/fs/
+-rw-r--r--   0 donncha    (501) staff       (20)      913 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4835 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2792 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3072 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2980 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1725 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3862 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3934 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2197 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1423 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1708 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1731 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1462 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.294201 mvt-2.3.0/mvt/ios/modules/mixed/
+-rw-r--r--   0 donncha    (501) staff       (20)     1512 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5579 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5143 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2488 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3406 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3213 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2381 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3266 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2957 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4352 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 donncha    (501) staff       (20)    14749 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5343 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1456 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2943 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6570 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5971 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5510 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5171 2023-06-29 15:09:26.000000 mvt-2.3.0/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4334 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7508 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4830 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6699 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4663 2023-06-29 08:51:11.000000 mvt-2.3.0/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 donncha    (501) staff       (20)    10973 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/net_base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1848 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/versions.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.273496 mvt-2.3.0/mvt.egg-info/
+-rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 donncha    (501) staff       (20)     6342 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 donncha    (501) staff       (20)        1 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 donncha    (501) staff       (20)       70 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 donncha    (501) staff       (20)      210 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/requires.txt
+-rw-r--r--   0 donncha    (501) staff       (20)       10 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/top_level.txt
+-rw-r--r--   0 donncha    (501) staff       (20)     1740 2023-06-29 15:10:48.301587 mvt-2.3.0/setup.cfg
+-rwxr-xr-x   0 donncha    (501) staff       (20)      231 2023-02-28 15:49:54.000000 mvt-2.3.0/setup.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.295811 mvt-2.3.0/tests/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.296479 mvt-2.3.0/tests/android/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/android/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2719 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_backup_module.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2168 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_backup_parser.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2304 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_dumpsys_parser.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298158 mvt-2.3.0/tests/android_androidqf/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/android_androidqf/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)      623 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 donncha    (501) staff       (20)      633 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 donncha    (501) staff       (20)      607 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1385 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)      692 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)      618 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)      661 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298444 mvt-2.3.0/tests/android_bugreport/
+-rw-r--r--   0 donncha    (501) staff       (20)        0 2023-05-10 16:45:13.000000 mvt-2.3.0/tests/android_bugreport/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1838 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_bugreport/test_bugreport.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298931 mvt-2.3.0/tests/common/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/common/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1743 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/common/test_indicators.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2291 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/common/test_utils.py
+-rw-r--r--   0 donncha    (501) staff       (20)      725 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/conftest.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.300552 mvt-2.3.0/tests/ios_backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/ios_backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)      570 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1132 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1124 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1257 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1009 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1265 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 donncha    (501) staff       (20)      690 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.300854 mvt-2.3.0/tests/ios_fs/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/ios_fs/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1160 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 donncha    (501) staff       (20)      572 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_android_androidqf.py
+-rw-r--r--   0 donncha    (501) staff       (20)      586 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_android_bugreport.py
+-rw-r--r--   0 donncha    (501) staff       (20)      525 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_ios_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)      483 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_ios_versions.py
+-rw-r--r--   0 donncha    (501) staff       (20)      928 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/utils.py
```

### Comparing `mvt-2.2.6/LICENSE` & `mvt-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/PKG-INFO` & `mvt-2.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: mvt
-Version: 2.2.6
-Summary: Mobile Verification Toolkit
-Home-page: https://github.com/mvt-project/mvt
-Author: Claudio Guarnieri
-Author-email: nex@nex.sx
-License: MVT v1.1
-Keywords: security,mobile,forensics,malware
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
      <img src="https://docs.mvt.re/en/latest/mvt.png" width="200" />
 </p>
 
 # Mobile Verification Toolkit
 
 [![](https://img.shields.io/pypi/v/mvt)](https://pypi.org/project/mvt/)
 [![Documentation Status](https://readthedocs.org/projects/mvt/badge/?version=latest)](https://docs.mvt.re/en/latest/?badge=latest)
 [![CI](https://github.com/mvt-project/mvt/actions/workflows/python-package.yml/badge.svg)](https://github.com/mvt-project/mvt/actions/workflows/python-package.yml)
 [![Downloads](https://pepy.tech/badge/mvt)](https://pepy.tech/project/mvt)
 
 Mobile Verification Toolkit (MVT) is a collection of utilities to simplify and automate the process of gathering forensic traces helpful to identify a potential compromise of Android and iOS devices.
 
-It has been developed and released by the [Amnesty International Security Lab](https://www.amnesty.org/en/tech/) in July 2021 in the context of the [Pegasus project](https://forbiddenstories.org/about-the-pegasus-project/) along with [a technical forensic methodology and forensic evidence](https://www.amnesty.org/en/latest/research/2021/07/forensic-methodology-report-how-to-catch-nso-groups-pegasus/).
+It has been developed and released by the [Amnesty International Security Lab](https://www.amnesty.org/en/tech/) in July 2021 in the context of the [Pegasus Project](https://forbiddenstories.org/about-the-pegasus-project/) along with [a technical forensic methodology](https://www.amnesty.org/en/latest/research/2021/07/forensic-methodology-report-how-to-catch-nso-groups-pegasus/). It continues to be maintained by Amnesty International and other contributors.
+
+> **Note**
+> MVT is a forensic research tool intended for technologists and investigators. It requires understanding digital forensics and using command-line tools. This is not intended for end-user self-assessment. If you are concerned with the security of your device please seek reputable expert assistance.
+>
+
+### Indicators of Compromise
+
+MVT supports using public [indicators of compromise (IOCs)](https://github.com/mvt-project/mvt-indicators) to scan mobile devices for potential traces of targeting or infection by known spyware campaigns. This includes IOCs published by [Amnesty International](https://github.com/AmnestyTech/investigations/) and other  research groups.
 
-*Warning*: MVT is a forensic research tool intended for technologists and investigators. Using it requires understanding the basics of forensic analysis and using command-line tools. This is not intended for end-user self-assessment. If you are concerned with the security of your device please seek expert assistance.
+> **Warning**
+> Public indicators of compromise are insufficient to determine that a device is "clean", and not targeted with a particular spyware tool. Reliance on public indicators alone can miss recent forensic traces and give a false sense of security.
+>
+> Reliable and comprehensive digital forensic support and triage requires access to non-public indicators, research and threat intelligence.
+>
+>Such support is available to civil society through [Amnesty International's Security Lab](https://www.amnesty.org/en/tech/) or through our forensic partnership with [Access Now’s Digital Security Helpline](https://www.accessnow.org/help/).
 
+More information about using indicators of compromise with MVT is available in the [documentation](https://docs.mvt.re/en/latest/iocs/).
 
 ## Installation
 
 MVT can be installed from sources or from [PyPi](https://pypi.org/project/mvt/) (you will need some dependencies, check the [documentation](https://docs.mvt.re/en/latest/install/)):
 
 ```
 pip3 install mvt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mvt-2.2.6/mvt/android/cli.py` & `mvt-2.3.0/mvt/android/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 
 import click
 
 from mvt.common.cmd_check_iocs import CmdCheckIOCS
-from mvt.common.help import (HELP_MSG_FAST, HELP_MSG_HASHES, HELP_MSG_IOC,
-                             HELP_MSG_LIST_MODULES, HELP_MSG_MODULE,
-                             HELP_MSG_OUTPUT, HELP_MSG_SERIAL,
-                             HELP_MSG_VERBOSE)
+from mvt.common.help import (
+    HELP_MSG_FAST,
+    HELP_MSG_HASHES,
+    HELP_MSG_IOC,
+    HELP_MSG_LIST_MODULES,
+    HELP_MSG_MODULE,
+    HELP_MSG_OUTPUT,
+    HELP_MSG_SERIAL,
+    HELP_MSG_VERBOSE,
+)
 from mvt.common.logo import logo
 from mvt.common.updates import IndicatorsUpdates
 from mvt.common.utils import init_logging, set_verbose_logging
 
 from .cmd_check_adb import CmdAndroidCheckADB
 from .cmd_check_androidqf import CmdAndroidCheckAndroidQF
 from .cmd_check_backup import CmdAndroidCheckBackup
@@ -24,47 +30,62 @@
 from .modules.adb import ADB_MODULES
 from .modules.adb.packages import Packages
 from .modules.backup import BACKUP_MODULES
 from .modules.bugreport import BUGREPORT_MODULES
 
 init_logging()
 log = logging.getLogger("mvt")
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-#==============================================================================
+# ==============================================================================
 # Main
-#==============================================================================
+# ==============================================================================
 @click.group(invoke_without_command=False)
 def cli():
     logo()
 
 
-#==============================================================================
+# ==============================================================================
 # Command: version
-#==============================================================================
+# ==============================================================================
 @cli.command("version", help="Show the currently installed version of MVT")
 def version():
     return
 
 
-#==============================================================================
+# ==============================================================================
 # Command: download-apks
-#==============================================================================
-@cli.command("download-apks", help="Download all or only non-system installed APKs",
-             context_settings=CONTEXT_SETTINGS)
+# ==============================================================================
+@cli.command(
+    "download-apks",
+    help="Download all or only non-system installed APKs",
+    context_settings=CONTEXT_SETTINGS,
+)
 @click.option("--serial", "-s", type=str, help=HELP_MSG_SERIAL)
-@click.option("--all-apks", "-a", is_flag=True,
-              help="Extract all packages installed on the phone, including system packages")
+@click.option(
+    "--all-apks",
+    "-a",
+    is_flag=True,
+    help="Extract all packages installed on the phone, including system packages",
+)
 @click.option("--virustotal", "-v", is_flag=True, help="Check packages on VirusTotal")
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help="Specify a path to a folder where you want to store the APKs")
-@click.option("--from-file", "-f", type=click.Path(exists=True),
-              help="Instead of acquiring from phone, load an existing packages.json file for "
-                   "lookups (mainly for debug purposes)")
+@click.option(
+    "--output",
+    "-o",
+    type=click.Path(exists=False),
+    help="Specify a path to a folder where you want to store the APKs",
+)
+@click.option(
+    "--from-file",
+    "-f",
+    type=click.Path(exists=True),
+    help="Instead of acquiring from phone, load an existing packages.json file for "
+    "lookups (mainly for debug purposes)",
+)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
 def download_apks(ctx, all_apks, virustotal, output, from_file, serial, verbose):
     set_verbose_logging(verbose)
     try:
         if from_file:
             download = DownloadAPKs.from_json(from_file)
@@ -95,154 +116,217 @@
             m = Packages()
             m.check_virustotal(packages_to_lookup)
     except KeyboardInterrupt:
         print("")
         ctx.exit(1)
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-adb
-#==============================================================================
-@cli.command("check-adb", help="Check an Android device over adb",
-             context_settings=CONTEXT_SETTINGS)
+# ==============================================================================
+@cli.command(
+    "check-adb",
+    help="Check an Android device over adb",
+    context_settings=CONTEXT_SETTINGS,
+)
 @click.option("--serial", "-s", type=str, help=HELP_MSG_SERIAL)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
 def check_adb(ctx, serial, iocs, output, fast, list_modules, module, verbose):
     set_verbose_logging(verbose)
-    cmd = CmdAndroidCheckADB(results_path=output, ioc_files=iocs,
-                             module_name=module, serial=serial, fast_mode=fast)
+    cmd = CmdAndroidCheckADB(
+        results_path=output,
+        ioc_files=iocs,
+        module_name=module,
+        serial=serial,
+        fast_mode=fast,
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking Android device over debug bridge")
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the Android device produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the Android device produced %d detections!",
+            cmd.detected_count,
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-bugreport
-#==============================================================================
-@cli.command("check-bugreport", help="Check an Android Bug Report",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+# ==============================================================================
+@cli.command(
+    "check-bugreport",
+    help="Check an Android Bug Report",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BUGREPORT_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_bugreport(ctx, iocs, output, list_modules, module, verbose, bugreport_path):
     set_verbose_logging(verbose)
-    # Always generate hashes as bug reports are small.
-    cmd = CmdAndroidCheckBugreport(target_path=bugreport_path,
-                                   results_path=output, ioc_files=iocs,
-                                   module_name=module, hashes=True)
+    # Always generate hashes as bug reports are small.
+    cmd = CmdAndroidCheckBugreport(
+        target_path=bugreport_path,
+        results_path=output,
+        ioc_files=iocs,
+        module_name=module,
+        hashes=True,
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking Android bug report at path: %s", bugreport_path)
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the Android bug report produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the Android bug report produced %d detections!",
+            cmd.detected_count,
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-backup
-#==============================================================================
-@cli.command("check-backup", help="Check an Android Backup",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+# ==============================================================================
+@cli.command(
+    "check-backup", help="Check an Android Backup", context_settings=CONTEXT_SETTINGS
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_backup(ctx, iocs, output, list_modules, verbose, backup_path):
     set_verbose_logging(verbose)
     # Always generate hashes as backups are generally small.
-    cmd = CmdAndroidCheckBackup(target_path=backup_path, results_path=output,
-                                ioc_files=iocs, hashes=True)
+    cmd = CmdAndroidCheckBackup(
+        target_path=backup_path, results_path=output, ioc_files=iocs, hashes=True
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking Android backup at path: %s", backup_path)
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the Android backup produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the Android backup produced %d detections!",
+            cmd.detected_count,
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-androidqf
-#==============================================================================
-@cli.command("check-androidqf", help="Check data collected with AndroidQF",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+# ==============================================================================
+@cli.command(
+    "check-androidqf",
+    help="Check data collected with AndroidQF",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("ANDROIDQF_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_androidqf(ctx, iocs, output, list_modules, module, hashes, verbose, androidqf_path):
+def check_androidqf(
+    ctx, iocs, output, list_modules, module, hashes, verbose, androidqf_path
+):
     set_verbose_logging(verbose)
-    cmd = CmdAndroidCheckAndroidQF(target_path=androidqf_path,
-                                   results_path=output, ioc_files=iocs,
-                                   module_name=module, hashes=hashes)
+    cmd = CmdAndroidCheckAndroidQF(
+        target_path=androidqf_path,
+        results_path=output,
+        ioc_files=iocs,
+        module_name=module,
+        hashes=hashes,
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking AndroidQF acquisition at path: %s", androidqf_path)
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the AndroidQF acquisition produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the AndroidQF acquisition produced %d detections!",
+            cmd.detected_count,
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-iocs
-#==============================================================================
-@cli.command("check-iocs", help="Compare stored JSON results to provided indicators",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
+# ==============================================================================
+@cli.command(
+    "check-iocs",
+    help="Compare stored JSON results to provided indicators",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.argument("FOLDER", type=click.Path(exists=True))
 @click.pass_context
 def check_iocs(ctx, iocs, list_modules, module, folder):
     cmd = CmdCheckIOCS(target_path=folder, ioc_files=iocs, module_name=module)
     cmd.modules = BACKUP_MODULES + ADB_MODULES + BUGREPORT_MODULES
@@ -250,15 +334,18 @@
     if list_modules:
         cmd.list_modules()
         return
 
     cmd.run()
 
 
-#==============================================================================
+# ==============================================================================
 # Command: download-iocs
-#==============================================================================
-@cli.command("download-iocs", help="Download public STIX2 indicators",
-             context_settings=CONTEXT_SETTINGS)
+# ==============================================================================
+@cli.command(
+    "download-iocs",
+    help="Download public STIX2 indicators",
+    context_settings=CONTEXT_SETTINGS,
+)
 def download_indicators():
     ioc_updates = IndicatorsUpdates()
     ioc_updates.update()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mvt-2.2.6/mvt/android/cmd_check_androidqf.py` & `mvt-2.3.0/mvt/android/cmd_check_androidqf.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 
 from .modules.androidqf import ANDROIDQF_MODULES
 
 log = logging.getLogger(__name__)
 
 
 class CmdAndroidCheckAndroidQF(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, hashes=hashes,
-                         log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            hashes=hashes,
+            log=log,
+        )
 
         self.name = "check-androidqf"
         self.modules = ANDROIDQF_MODULES
```

### Comparing `mvt-2.2.6/mvt/android/cmd_check_backup.py` & `mvt-2.3.0/mvt/android/cmd_check_backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,48 @@
 import tarfile
 from pathlib import Path
 from typing import List, Optional
 
 from rich.prompt import Prompt
 
 from mvt.android.modules.backup.base import BackupExtraction
-from mvt.android.parsers.backup import (AndroidBackupParsingError,
-                                        InvalidBackupPassword, parse_ab_header,
-                                        parse_backup_file)
+from mvt.android.parsers.backup import (
+    AndroidBackupParsingError,
+    InvalidBackupPassword,
+    parse_ab_header,
+    parse_backup_file,
+)
 from mvt.common.command import Command
 
 from .modules.backup import BACKUP_MODULES
 
 log = logging.getLogger(__name__)
 
 
 class CmdAndroidCheckBackup(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, hashes=hashes,
-                         log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            hashes=hashes,
+            log=log,
+        )
 
         self.name = "check-backup"
         self.modules = BACKUP_MODULES
 
         self.backup_type: str = ""
         self.backup_archive: Optional[tarfile.TarFile] = None
         self.backup_files: List[str] = []
@@ -81,20 +89,22 @@
                 self.backup_files.append(member.name)
 
         elif os.path.isdir(self.target_path):
             self.backup_type = "folder"
             self.target_path = Path(self.target_path).absolute().as_posix()
             for root, subdirs, subfiles in os.walk(os.path.abspath(self.target_path)):
                 for fname in subfiles:
-                    self.backup_files.append(os.path.relpath(os.path.join(root, fname),
-                                                             self.target_path))
+                    self.backup_files.append(
+                        os.path.relpath(os.path.join(root, fname), self.target_path)
+                    )
         else:
-            log.critical("Invalid backup path, path should be a folder or an "
-                         "Android Backup (.ab) file")
+            log.critical(
+                "Invalid backup path, path should be a folder or an "
+                "Android Backup (.ab) file"
+            )
             sys.exit(1)
 
     def module_init(self, module: BackupExtraction) -> None:  # type: ignore[override]
         if self.backup_type == "folder":
             module.from_folder(self.target_path, self.backup_files)
         else:
-            module.from_ab(self.target_path, self.backup_archive,
-                           self.backup_files)
+            module.from_ab(self.target_path, self.backup_archive, self.backup_files)
```

### Comparing `mvt-2.2.6/mvt/android/cmd_check_bugreport.py` & `mvt-2.3.0/mvt/android/cmd_check_bugreport.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,34 @@
 
 from .modules.bugreport import BUGREPORT_MODULES
 
 log = logging.getLogger(__name__)
 
 
 class CmdAndroidCheckBugreport(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, hashes=hashes,
-                         log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            hashes=hashes,
+            log=log,
+        )
 
         self.name = "check-bugreport"
         self.modules = BUGREPORT_MODULES
 
         self.bugreport_format: str = ""
         self.bugreport_archive: Optional[ZipFile] = None
         self.bugreport_files: List[str] = []
@@ -51,16 +56,17 @@
             for file_name in self.bugreport_archive.namelist():
                 self.bugreport_files.append(file_name)
         elif os.path.isdir(self.target_path):
             self.bugreport_format = "dir"
             parent_path = Path(self.target_path).absolute().as_posix()
             for root, _, subfiles in os.walk(os.path.abspath(self.target_path)):
                 for file_name in subfiles:
-                    file_path = os.path.relpath(os.path.join(root, file_name),
-                                                parent_path)
+                    file_path = os.path.relpath(
+                        os.path.join(root, file_name), parent_path
+                    )
                     self.bugreport_files.append(file_path)
 
     def module_init(self, module: BugReportModule) -> None:  # type: ignore[override]
         if self.bugreport_format == "zip":
             module.from_zip(self.bugreport_archive, self.bugreport_files)
         else:
             module.from_folder(self.target_path, self.bugreport_files)
```

### Comparing `mvt-2.2.6/mvt/android/cmd_download_apks.py` & `mvt-2.3.0/mvt/android/cmd_download_apks.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """DownloadAPKs is the main class operating the download of APKs
     from the device.
     """
 
     def __init__(
         self,
         results_path: Optional[str] = None,
-        all_apks: Optional[bool] = False,
+        all_apks: bool = False,
         packages: Optional[list] = None,
     ) -> None:
         """Initialize module.
         :param results_path: Path to the folder where data should be stored
         :param all_apks: Boolean indicating whether to download all packages
                          or filter known-goods
         :param packages: Provided list of packages, typically for JSON checks
@@ -62,35 +62,39 @@
         """
         log.info("Downloading %s ...", remote_path)
 
         file_name = ""
         if "==/" in remote_path:
             file_name = "_" + remote_path.split("==/")[1].replace(".apk", "")
 
-        local_path = os.path.join(self.results_path_apks,
-                                  f"{package_name}{file_name}.apk")
+        local_path = os.path.join(
+            self.results_path_apks, f"{package_name}{file_name}.apk"
+        )
         name_counter = 0
         while True:
             if not os.path.exists(local_path):
                 break
 
             name_counter += 1
-            local_path = os.path.join(self.results_path_apks,
-                                      f"{package_name}{file_name}_{name_counter}.apk")
+            local_path = os.path.join(
+                self.results_path_apks, f"{package_name}{file_name}_{name_counter}.apk"
+            )
 
         try:
             self._adb_download(remote_path, local_path)
         except InsufficientPrivileges:
-            log.error("Unable to pull package file from %s: insufficient privileges, "
-                      "it might be a system app", remote_path)
+            log.error(
+                "Unable to pull package file from %s: insufficient privileges, "
+                "it might be a system app",
+                remote_path,
+            )
             self._adb_reconnect()
             return None
         except Exception as exc:
-            log.exception("Failed to pull package file from %s: %s",
-                          remote_path, exc)
+            log.exception("Failed to pull package file from %s: %s", remote_path, exc)
             self._adb_reconnect()
             return None
 
         return local_path
 
     def get_packages(self) -> None:
         """Use the Packages adb module to retrieve the list of packages.
@@ -102,57 +106,66 @@
         m.log = self.log
         m.serial = self.serial
         m.run()
 
         self.packages = m.results
 
     def pull_packages(self) -> None:
-        """Download all files of all selected packages from the device.
-        """
-        log.info("Starting extraction of installed APKs at folder %s",
-                 self.results_path)
+        """Download all files of all selected packages from the device."""
+        log.info(
+            "Starting extraction of installed APKs at folder %s", self.results_path
+        )
 
         # If the user provided the flag --all-apks we select all packages.
         packages_selection = []
         if self.all_apks:
             log.info("Selected all %d available packages", len(self.packages))
             packages_selection = self.packages
         else:
             # Otherwise we loop through the packages and get only those that
             # are not marked as system.
             for package in self.packages:
                 if not package.get("system", False):
                     packages_selection.append(package)
 
-            log.info("Selected only %d packages which are not marked as \"system\"",
-                     len(packages_selection))
+            log.info(
+                'Selected only %d packages which are not marked as "system"',
+                len(packages_selection),
+            )
 
         if len(packages_selection) == 0:
             log.info("No packages were selected for download")
             return
 
         log.info("Downloading packages from device. This might take some time ...")
 
         self.results_path_apks = os.path.join(self.results_path, "apks")
         if not os.path.exists(self.results_path_apks):
             os.makedirs(self.results_path_apks, exist_ok=True)
 
-        for i in track(range(len(packages_selection)),
-                       description=f"Downloading {len(packages_selection)} packages..."):
+        for i in track(
+            range(len(packages_selection)),
+            description=f"Downloading {len(packages_selection)} packages...",
+        ):
             package = packages_selection[i]
 
-            log.info("[%d/%d] Package: %s", i, len(packages_selection),
-                     package["package_name"])
+            log.info(
+                "[%d/%d] Package: %s",
+                i,
+                len(packages_selection),
+                package["package_name"],
+            )
 
             # Sometimes the package path contains multiple lines for multiple
             # apks. We loop through each line and download each file.
             for package_file in package["files"]:
                 device_path = package_file["path"]
-                local_path = self.pull_package_file(package["package_name"],
-                                                    device_path)
+                local_path = self.pull_package_file(
+                    package["package_name"], device_path
+                )
                 if not local_path:
                     continue
 
                 package_file["local_path"] = local_path
 
         log.info("Download of selected packages completed")
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/__init__.py` & `mvt-2.3.0/mvt/android/modules/adb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,12 +19,28 @@
 from .processes import Processes
 from .root_binaries import RootBinaries
 from .selinux_status import SELinuxStatus
 from .settings import Settings
 from .sms import SMS
 from .whatsapp import Whatsapp
 
-ADB_MODULES = [ChromeHistory, SMS, Whatsapp, Processes, Getprop, Settings,
-               SELinuxStatus, DumpsysBatteryHistory, DumpsysBatteryDaily,
-               DumpsysReceivers, DumpsysActivities, DumpsysAccessibility,
-               DumpsysDBInfo, DumpsysFull, DumpsysAppOps, Packages, Logcat,
-               RootBinaries, Files]
+ADB_MODULES = [
+    ChromeHistory,
+    SMS,
+    Whatsapp,
+    Processes,
+    Getprop,
+    Settings,
+    SELinuxStatus,
+    DumpsysBatteryHistory,
+    DumpsysBatteryDaily,
+    DumpsysReceivers,
+    DumpsysActivities,
+    DumpsysAccessibility,
+    DumpsysDBInfo,
+    DumpsysFull,
+    DumpsysAppOps,
+    Packages,
+    Logcat,
+    RootBinaries,
+    Files,
+]
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/base.py` & `mvt-2.3.0/mvt/android/modules/adb/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,42 +12,54 @@
 import tempfile
 import time
 from typing import Callable, Optional
 
 from adb_shell.adb_device import AdbDeviceTcp, AdbDeviceUsb
 from adb_shell.auth.keygen import keygen, write_public_keyfile
 from adb_shell.auth.sign_pythonrsa import PythonRSASigner
-from adb_shell.exceptions import (AdbCommandFailureException, DeviceAuthError,
-                                  UsbDeviceNotFoundError, UsbReadFailedError)
+from adb_shell.exceptions import (
+    AdbCommandFailureException,
+    DeviceAuthError,
+    UsbDeviceNotFoundError,
+    UsbReadFailedError,
+)
 from rich.prompt import Prompt
 from usb1 import USBErrorAccess, USBErrorBusy
 
-from mvt.android.parsers.backup import (InvalidBackupPassword, parse_ab_header,
-                                        parse_backup_file)
+from mvt.android.parsers.backup import (
+    InvalidBackupPassword,
+    parse_ab_header,
+    parse_backup_file,
+)
 from mvt.common.module import InsufficientPrivileges, MVTModule
 
 ADB_KEY_PATH = os.path.expanduser("~/.android/adbkey")
 ADB_PUB_KEY_PATH = os.path.expanduser("~/.android/adbkey.pub")
 
 
 class AndroidExtraction(MVTModule):
     """This class provides a base for all Android extraction modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.device = None
         self.serial = None
 
     @staticmethod
     def _adb_check_keys() -> None:
         """Make sure Android adb keys exist."""
@@ -74,44 +86,57 @@
 
         # If no serial was specified or if the serial does not seem to be
         # a HOST:PORT definition, we use the USB transport.
         if not self.serial or ":" not in self.serial:
             try:
                 self.device = AdbDeviceUsb(serial=self.serial)
             except UsbDeviceNotFoundError:
-                self.log.critical("No device found. Make sure it is connected and unlocked.")
+                self.log.critical(
+                    "No device found. Make sure it is connected and unlocked."
+                )
                 sys.exit(-1)
         # Otherwise we try to use the TCP transport.
         else:
             addr = self.serial.split(":")
             if len(addr) < 2:
-                raise ValueError("TCP serial number must follow the format: `address:port`")
-
-            self.device = AdbDeviceTcp(addr[0], int(addr[1]),
-                                       default_transport_timeout_s=30.)
+                raise ValueError(
+                    "TCP serial number must follow the format: `address:port`"
+                )
+
+            self.device = AdbDeviceTcp(
+                addr[0], int(addr[1]), default_transport_timeout_s=30.0
+            )
 
         while True:
             try:
                 self.device.connect(rsa_keys=[signer], auth_timeout_s=5)
             except (USBErrorBusy, USBErrorAccess):
-                self.log.critical("Device is busy, maybe run `adb kill-server` and try again.")
+                self.log.critical(
+                    "Device is busy, maybe run `adb kill-server` and try again."
+                )
                 sys.exit(-1)
             except DeviceAuthError:
-                self.log.error("You need to authorize this computer on the Android device. "
-                               "Retrying in 5 seconds...")
+                self.log.error(
+                    "You need to authorize this computer on the Android device. "
+                    "Retrying in 5 seconds..."
+                )
                 time.sleep(5)
             except UsbReadFailedError:
-                self.log.error("Unable to connect to the device over USB. "
-                               "Try to unplug, plug the device and start again.")
+                self.log.error(
+                    "Unable to connect to the device over USB. "
+                    "Try to unplug, plug the device and start again."
+                )
                 sys.exit(-1)
             except OSError as exc:
                 if exc.errno == 113 and self.serial:
-                    self.log.critical("Unable to connect to the device %s: "
-                                      "did you specify the correct IP address?",
-                                      self.serial)
+                    self.log.critical(
+                        "Unable to connect to the device %s: "
+                        "did you specify the correct IP address?",
+                        self.serial,
+                    )
                     sys.exit(-1)
             else:
                 break
 
     def _adb_disconnect(self) -> None:
         """Close adb connection to the device."""
         self.device.close()
@@ -140,17 +165,19 @@
         """
         result = self._adb_command("command -v su && su -c true")
         return bool(result) and "Permission denied" not in result
 
     def _adb_root_or_die(self) -> None:
         """Check if we have a `su` binary, otherwise raise an Exception."""
         if not self._adb_check_if_root():
-            raise InsufficientPrivileges("This module is optionally available "
-                                         "in case the device is already rooted."
-                                         " Do NOT root your own device!")
+            raise InsufficientPrivileges(
+                "This module is optionally available "
+                "in case the device is already rooted."
+                " Do NOT root your own device!"
+            )
 
     def _adb_command_as_root(self, command):
         """Execute an adb shell command.
 
         :param command: Shell command to execute as root
         :returns: Output of command
 
@@ -173,73 +200,79 @@
         return bool(self._adb_command_as_root(f"[ ! -f {file} ] || echo 1"))
 
     def _adb_download(
         self,
         remote_path: str,
         local_path: str,
         progress_callback: Optional[Callable] = None,
-        retry_root: Optional[bool] = True
+        retry_root: Optional[bool] = True,
     ) -> None:
         """Download a file form the device.
 
         :param remote_path: Path to download from the device
         :param local_path: Path to where to locally store the copy of the file
         :param progress_callback: Callback for download progress bar
                                   (Default value = None)
         :param retry_root: Default value = True)
 
         """
         try:
             self.device.pull(remote_path, local_path, progress_callback)
         except AdbCommandFailureException as exc:
             if retry_root:
-                self._adb_download_root(remote_path, local_path,
-                                        progress_callback)
+                self._adb_download_root(remote_path, local_path, progress_callback)
             else:
-                raise Exception(f"Unable to download file {remote_path}: {exc}") from exc
+                raise Exception(
+                    f"Unable to download file {remote_path}: {exc}"
+                ) from exc
 
     def _adb_download_root(
         self,
         remote_path: str,
         local_path: str,
-        progress_callback: Optional[Callable] = None
+        progress_callback: Optional[Callable] = None,
     ) -> None:
         try:
             # Check if we have root, if not raise an Exception.
             self._adb_root_or_die()
 
             # We generate a random temporary filename.
-            allowed_chars = (string.ascii_uppercase
-                             + string.ascii_lowercase
-                             + string.digits)
-            tmp_filename = "tmp_" + ''.join(random.choices(allowed_chars, k=10))
+            allowed_chars = (
+                string.ascii_uppercase + string.ascii_lowercase + string.digits
+            )
+            tmp_filename = "tmp_" + "".join(random.choices(allowed_chars, k=10))
 
             # We create a temporary local file.
             new_remote_path = f"/sdcard/{tmp_filename}"
 
             # We copy the file from the data folder to /sdcard/.
             cp_output = self._adb_command_as_root(f"cp {remote_path} {new_remote_path}")
-            if cp_output.startswith("cp: ") and "No such file or directory" in cp_output:
+            if (
+                cp_output.startswith("cp: ")
+                and "No such file or directory" in cp_output
+            ):
                 raise Exception(f"Unable to process file {remote_path}: File not found")
             if cp_output.startswith("cp: ") and "Permission denied" in cp_output:
-                raise Exception(f"Unable to process file {remote_path}: Permission denied")
+                raise Exception(
+                    f"Unable to process file {remote_path}: Permission denied"
+                )
 
             # We download from /sdcard/ to the local temporary file.
             # If it doesn't work now, don't try again (retry_root=False)
-            self._adb_download(new_remote_path, local_path, progress_callback,
-                               retry_root=False)
+            self._adb_download(
+                new_remote_path, local_path, progress_callback, retry_root=False
+            )
 
             # Delete the copy on /sdcard/.
             self._adb_command(f"rm -rf {new_remote_path}")
 
         except AdbCommandFailureException as exc:
             raise Exception(f"Unable to download file {remote_path}: {exc}") from exc
 
-    def _adb_process_file(self, remote_path: str,
-                          process_routine: Callable) -> None:
+    def _adb_process_file(self, remote_path: str, process_routine: Callable) -> None:
         """Download a local copy of a file which is only accessible as root.
         This is a wrapper around process_routine.
 
         :param remote_path: Path of the file on the device to process
         :param process_routine: Function to be called on the local copy of the
                                 downloaded file
 
@@ -269,38 +302,40 @@
 
         # Delete the local copy.
         tmp.close()
         # Delete the copy on /sdcard/.
         self._adb_command(f"rm -f {new_remote_path}")
 
     def _generate_backup(self, package_name: str) -> bytes:
-        self.log.info("Please check phone and accept Android backup prompt. "
-                      "You may need to set a backup password. \a")
+        self.log.info(
+            "Please check phone and accept Android backup prompt. "
+            "You may need to set a backup password. \a"
+        )
 
         # TODO: Base64 encoding as temporary fix to avoid byte-mangling over
         #       the shell transport...
         cmd = f"/system/bin/bu backup -nocompress '{package_name}' | base64"
         backup_output_b64 = self._adb_command(cmd)
         backup_output = base64.b64decode(backup_output_b64)
         header = parse_ab_header(backup_output)
 
         if not header["backup"]:
-            self.log.error("Extracting SMS via Android backup failed. "
-                           "No valid backup data found.")
+            self.log.error(
+                "Extracting SMS via Android backup failed. "
+                "No valid backup data found."
+            )
             return None
 
         if header["encryption"] == "none":
             return parse_backup_file(backup_output, password=None)
 
         for _ in range(0, 3):
-            backup_password = Prompt.ask("Enter backup password",
-                                         password=True)
+            backup_password = Prompt.ask("Enter backup password", password=True)
             try:
-                decrypted_backup_tar = parse_backup_file(backup_output,
-                                                         backup_password)
+                decrypted_backup_tar = parse_backup_file(backup_output, backup_password)
                 return decrypted_backup_tar
             except InvalidBackupPassword:
                 self.log.error("You provided the wrong password! Please try again...")
 
         self.log.error("All attempts to decrypt backup with password failed!")
 
         return None
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/chrome_history.py` & `mvt-2.3.0/mvt/android/modules/adb/chrome_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,46 +4,50 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 import os
 import sqlite3
 from typing import Optional, Union
 
-from mvt.common.utils import (convert_chrometime_to_datetime,
-                              convert_datetime_to_iso)
+from mvt.common.utils import convert_chrometime_to_datetime, convert_datetime_to_iso
 
 from .base import AndroidExtraction
 
 CHROME_HISTORY_PATH = "data/data/com.android.chrome/app_chrome/Default/History"
 
 
 class ChromeHistory(AndroidExtraction):
     """This module extracts records from Android's Chrome browsing history."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.results = []
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "visit",
             "data": f"{record['id']} - {record['url']} (visit ID: {record['visit_id']}, "
-                    f"redirect source: {record['redirect_source']})"
+            f"redirect source: {record['redirect_source']})",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -55,46 +59,51 @@
 
         :param db_path: Path to the History database to process.
 
         """
         assert isinstance(self.results, list)  # assert results type for mypy
         conn = sqlite3.connect(db_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 urls.id,
                 urls.url,
                 visits.id,
                 visits.visit_time,
                 visits.from_visit
             FROM urls
             JOIN visits ON visits.url = urls.id
             ORDER BY visits.visit_time;
-        """)
+        """
+        )
 
         for item in cur:
-            self.results.append({
-                "id": item[0],
-                "url": item[1],
-                "visit_id": item[2],
-                "timestamp": item[3],
-                "isodate": convert_datetime_to_iso(
-                    convert_chrometime_to_datetime(item[3])),
-                "redirect_source": item[4],
-            })
+            self.results.append(
+                {
+                    "id": item[0],
+                    "url": item[1],
+                    "visit_id": item[2],
+                    "timestamp": item[3],
+                    "isodate": convert_datetime_to_iso(
+                        convert_chrometime_to_datetime(item[3])
+                    ),
+                    "redirect_source": item[4],
+                }
+            )
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d history items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d history items", len(self.results))
 
     def run(self) -> None:
         self._adb_connect()
 
         try:
-            self._adb_process_file(os.path.join("/", CHROME_HISTORY_PATH),
-                                   self._parse_db)
+            self._adb_process_file(
+                os.path.join("/", CHROME_HISTORY_PATH), self._parse_db
+            )
         except Exception as exc:
             self.log.error(exc)
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This module extracts stats on accessibility."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
@@ -42,12 +47,14 @@
         self._adb_connect()
         output = self._adb_command("dumpsys accessibility")
         self._adb_disconnect()
 
         self.results = parse_dumpsys_accessibility(output)
 
         for result in self.results:
-            self.log.info("Found installed accessibility service \"%s\"",
-                          result.get("service"))
-
-        self.log.info("Identified a total of %d accessibility services",
-                      len(self.results))
+            self.log.info(
+                'Found installed accessibility service "%s"', result.get("service")
+            )
+
+        self.log.info(
+            "Identified a total of %d accessibility services", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,57 +17,69 @@
     slug = "dumpsys_appops"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for perm in record["permissions"]:
             if "entries" not in perm:
                 continue
 
             for entry in perm["entries"]:
                 if "timestamp" in entry:
-                    records.append({
-                        "timestamp": entry["timestamp"],
-                        "module": self.__class__.__name__,
-                        "event": entry["access"],
-                        "data": f"{record['package_name']} access to "
-                                f"{perm['name']}: {entry['access']}",
-                    })
+                    records.append(
+                        {
+                            "timestamp": entry["timestamp"],
+                            "module": self.__class__.__name__,
+                            "event": entry["access"],
+                            "data": f"{record['package_name']} access to "
+                            f"{perm['name']}: {entry['access']}",
+                        }
+                    )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if self.indicators:
                 ioc = self.indicators.check_app_id(result.get("package_name"))
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             for perm in result["permissions"]:
-                if (perm["name"] == "REQUEST_INSTALL_PACKAGES"
-                        and perm["access"] == "allow"):
-                    self.log.info("Package %s with REQUEST_INSTALL_PACKAGES "
-                                  "permission", result["package_name"])
+                if (
+                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
+                    and perm["access"] == "allow"
+                ):
+                    self.log.info(
+                        "Package %s with REQUEST_INSTALL_PACKAGES " "permission",
+                        result["package_name"],
+                    )
 
     def run(self) -> None:
         self._adb_connect()
         output = self._adb_command("dumpsys appops")
         self._adb_disconnect()
 
         self.results = parse_dumpsys_appops(output)
 
-        self.log.info("Extracted a total of %d records from app-ops manager",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d records from app-ops manager", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,34 @@
     """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["from"],
             "module": self.__class__.__name__,
             "event": "battery_daily",
             "data": f"Recorded update of package {record['package_name']} "
-                    f"with vers {record['vers']}"
+            f"with vers {record['vers']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -50,9 +55,10 @@
     def run(self) -> None:
         self._adb_connect()
         output = self._adb_command("dumpsys batterystats --daily")
         self._adb_disconnect()
 
         self.results = parse_dumpsys_battery_daily(output)
 
-        self.log.info("Extracted %d records from battery daily stats",
-                      len(self.results))
+        self.log.info(
+            "Extracted %d records from battery daily stats", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This module extracts records from battery history events."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
@@ -41,9 +46,8 @@
     def run(self) -> None:
         self._adb_connect()
         output = self._adb_command("dumpsys batterystats --history")
         self._adb_disconnect()
 
         self.results = parse_dumpsys_battery_history(output)
 
-        self.log.info("Extracted %d records from battery history",
-                      len(self.results))
+        self.log.info("Extracted %d records from battery history", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,26 @@
     slug = "dumpsys_dbinfo"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             path = result.get("path", "")
@@ -45,9 +50,11 @@
     def run(self) -> None:
         self._adb_connect()
         output = self._adb_command("dumpsys dbinfo")
         self._adb_disconnect()
 
         self.results = parse_dumpsys_dbinfo(output)
 
-        self.log.info("Extracted a total of %d records from database information",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d records from database information",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_full.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,26 @@
     """This module extracts stats on battery consumption by processes."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
         self._adb_connect()
 
         output = self._adb_command("dumpsys")
         if self.results_path:
             output_path = os.path.join(self.results_path, "dumpsys.txt")
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.3.0/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,46 +21,61 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for intent, receivers in self.results.items():
             for receiver in receivers:
                 if intent == INTENT_NEW_OUTGOING_SMS:
-                    self.log.info("Found a receiver to intercept outgoing SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept outgoing SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_DATA_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming data SMS message: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming data SMS message: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_PHONE_STATE:
-                    self.log.info("Found a receiver monitoring "
-                                  "telephony state/incoming calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        "Found a receiver monitoring "
+                        'telephony state/incoming calls: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_NEW_OUTGOING_CALL:
-                    self.log.info("Found a receiver monitoring outgoing calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver monitoring outgoing calls: "%s"',
+                        receiver["receiver"],
+                    )
 
                 ioc = self.indicators.check_app_id(receiver["package_name"])
                 if ioc:
                     receiver["matched_indicator"] = ioc
                     self.detected.append({intent: receiver})
                     continue
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/files.py` & `mvt-2.3.0/mvt/android/modules/adb/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,26 @@
     """This module extracts the list of files on the device."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.full_find = False
 
     def serialize(self, record: dict) -> Union[dict, list, None]:
         if "modified_time" in record:
             return {
                 "timestamp": record["modified_time"],
                 "module": self.__class__.__name__,
@@ -49,67 +54,71 @@
             }
 
         return None
 
     def check_indicators(self) -> None:
         for result in self.results:
             if result.get("is_suid"):
-                self.log.warning("Found an SUID file in a non-standard directory \"%s\".",
-                                 result["path"])
+                self.log.warning(
+                    'Found an SUID file in a non-standard directory "%s".',
+                    result["path"],
+                )
 
             if self.indicators and self.indicators.check_file_path(result["path"]):
-                self.log.warning("Found a known suspicous file at path: \"%s\"",
-                                 result["path"])
+                self.log.warning(
+                    'Found a known suspicous file at path: "%s"', result["path"]
+                )
                 self.detected.append(result)
 
     def backup_file(self, file_path: str) -> None:
         if not self.results_path:
             return
 
         local_file_name = file_path.replace("/", "_").replace(" ", "-")
         local_files_folder = os.path.join(self.results_path, "files")
         if not os.path.exists(local_files_folder):
             os.mkdir(local_files_folder)
 
         local_file_path = os.path.join(local_files_folder, local_file_name)
 
         try:
-            self._adb_download(remote_path=file_path,
-                               local_path=local_file_path)
+            self._adb_download(remote_path=file_path, local_path=local_file_path)
         except Exception:
             pass
         else:
-            self.log.info("Downloaded file %s to local copy at %s",
-                          file_path, local_file_path)
+            self.log.info(
+                "Downloaded file %s to local copy at %s", file_path, local_file_path
+            )
 
     def find_files(self, folder: str) -> None:
         assert isinstance(self.results, list)
         if self.full_find:
             cmd = f"find '{folder}' -type f -printf '%T@ %m %s %u %g %p\n' 2> /dev/null"
             output = self._adb_command(cmd)
 
             for file_line in output.splitlines():
                 file_info = file_line.rstrip().split(" ", 5)
                 if len(file_line) < 6:
                     self.log.info("Skipping invalid file info - %s", file_line.rstrip())
                     continue
-                [unix_timestamp, mode, size,
-                 owner, group, full_path] = file_info
+                [unix_timestamp, mode, size, owner, group, full_path] = file_info
                 mod_time = convert_unix_to_iso(unix_timestamp)
 
-                self.results.append({
-                    "path": full_path,
-                    "modified_time": mod_time,
-                    "mode": mode,
-                    "is_suid": (int(mode, 8) & stat.S_ISUID) == 2048,
-                    "is_sgid": (int(mode, 8) & stat.S_ISGID) == 1024,
-                    "size": size,
-                    "owner": owner,
-                    "group": group,
-                })
+                self.results.append(
+                    {
+                        "path": full_path,
+                        "modified_time": mod_time,
+                        "mode": mode,
+                        "is_suid": (int(mode, 8) & stat.S_ISUID) == 2048,
+                        "is_sgid": (int(mode, 8) & stat.S_ISGID) == 1024,
+                        "size": size,
+                        "owner": owner,
+                        "group": group,
+                    }
+                )
         else:
             output = self._adb_command(f"find '{folder}' -type f 2> /dev/null")
             for file_line in output.splitlines():
                 self.results.append({"path": file_line.rstrip()})
 
     def run(self) -> None:
         self._adb_connect()
@@ -119,23 +128,23 @@
         if output or output.strip().splitlines():
             self.full_find = True
 
         for tmp_folder in ANDROID_TMP_FOLDERS:
             self.find_files(tmp_folder)
 
         for entry in self.results:
-            self.log.info("Found file in tmp folder at path %s",
-                          entry.get("path"))
+            self.log.info("Found file in tmp folder at path %s", entry.get("path"))
             self.backup_file(entry.get("path"))
 
         for media_folder in ANDROID_MEDIA_FOLDERS:
             self.find_files(media_folder)
 
-        self.log.info("Found %s files in primary Android tmp and media folders",
-                      len(self.results))
+        self.log.info(
+            "Found %s files in primary Android tmp and media folders", len(self.results)
+        )
 
         if self.fast_mode:
             self.log.info("Flag --fast was enabled: skipping full file listing")
         else:
             self.log.info("Processing full file listing. This may take a while...")
             self.find_files("/")
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/getprop.py` & `mvt-2.3.0/mvt/android/modules/adb/getprop.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,21 +16,26 @@
     """This module extracts device properties from getprop command."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {} if not results else results
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
@@ -48,14 +53,15 @@
         self.results = parse_getprop(output)
 
         # Alert if phone is outdated.
         for entry in self.results:
             if entry.get("name", "") != "ro.build.version.security_patch":
                 continue
             patch_date = datetime.strptime(entry["value"], "%Y-%m-%d")
-            if (datetime.now() - patch_date) > timedelta(days=6*30):
-                self.log.warning("This phone has not received security updates "
-                                 "for more than six months (last update: %s)",
-                                 entry["value"])
+            if (datetime.now() - patch_date) > timedelta(days=6 * 30):
+                self.log.warning(
+                    "This phone has not received security updates "
+                    "for more than six months (last update: %s)",
+                    entry["value"],
+                )
 
-        self.log.info("Extracted %d Android system properties",
-                      len(self.results))
+        self.log.info("Extracted %d Android system properties", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/logcat.py` & `mvt-2.3.0/mvt/android/modules/adb/logcat.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,41 +14,44 @@
     """This module extracts details on installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
         self._adb_connect()
 
         # Get the current logcat.
-        output = self._adb_command("logcat -d -b all \"*:V\"")
+        output = self._adb_command('logcat -d -b all "*:V"')
         # Get the locat prior to last reboot.
-        last_output = self._adb_command("logcat -L -b all \"*:V\"")
+        last_output = self._adb_command('logcat -L -b all "*:V"')
 
         if self.results_path:
-            logcat_path = os.path.join(self.results_path,
-                                       "logcat.txt")
+            logcat_path = os.path.join(self.results_path, "logcat.txt")
             with open(logcat_path, "w", encoding="utf-8") as handle:
                 handle.write(output)
 
-            self.log.info("Current logcat logs stored at %s",
-                          logcat_path)
+            self.log.info("Current logcat logs stored at %s", logcat_path)
 
-            logcat_last_path = os.path.join(self.results_path,
-                                            "logcat_last.txt")
+            logcat_last_path = os.path.join(self.results_path, "logcat_last.txt")
             with open(logcat_last_path, "w", encoding="utf-8") as handle:
                 handle.write(last_output)
 
-            self.log.info("Logcat logs prior to last reboot stored at %s",
-                          logcat_last_path)
+            self.log.info(
+                "Logcat logs prior to last reboot stored at %s", logcat_last_path
+            )
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/packages.py` & `mvt-2.3.0/mvt/android/modules/adb/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,67 +89,73 @@
     """This module extracts the list of installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
 
         timestamps = [
-            {
-                "event": "package_install",
-                "timestamp": record["timestamp"]
-            },
+            {"event": "package_install", "timestamp": record["timestamp"]},
             {
                 "event": "package_first_install",
-                "timestamp": record["first_install_time"]
-            },
-            {
-                "event": "package_last_update",
-                "timestamp": record["last_update_time"]
+                "timestamp": record["first_install_time"],
             },
+            {"event": "package_last_update", "timestamp": record["last_update_time"]},
         ]
 
         for timestamp in timestamps:
-            records.append({
-                "timestamp": timestamp["timestamp"],
-                "module": self.__class__.__name__,
-                "event": timestamp["event"],
-                "data": f"{record['package_name']} (system: {record['system']},"
-                        f" third party: {record['third_party']})",
-            })
+            records.append(
+                {
+                    "timestamp": timestamp["timestamp"],
+                    "module": self.__class__.__name__,
+                    "event": timestamp["event"],
+                    "data": f"{record['package_name']} (system: {record['system']},"
+                    f" third party: {record['third_party']})",
+                }
+            )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if result["package_name"] in ROOT_PACKAGES:
-                self.log.warning("Found an installed package related to "
-                                 "rooting/jailbreaking: \"%s\"",
-                                 result["package_name"])
+                self.log.warning(
+                    "Found an installed package related to "
+                    'rooting/jailbreaking: "%s"',
+                    result["package_name"],
+                )
                 self.detected.append(result)
                 continue
 
             if result["package_name"] in SECURITY_PACKAGES and result["disabled"]:
-                self.log.warning("Found a security package disabled: \"%s\"",
-                                 result["package_name"])
+                self.log.warning(
+                    'Found a security package disabled: "%s"', result["package_name"]
+                )
 
             if result["package_name"] in SYSTEM_UPDATE_PACKAGES and result["disabled"]:
-                self.log.warning("System OTA update package \"%s\" disabled on the phone",
-                                 result["package_name"])
+                self.log.warning(
+                    'System OTA update package "%s" disabled on the phone',
+                    result["package_name"],
+                )
 
             if not self.indicators:
                 continue
 
             ioc = self.indicators.check_app_id(result.get("package_name"))
             if ioc:
                 result["matched_indicator"] = ioc
@@ -235,30 +241,32 @@
         if not output:
             return []
 
         package_files = []
         for file_path in output.splitlines():
             file_path = file_path.strip()
 
-            md5 = self._adb_command(
-                f"md5sum {file_path}").split(" ", maxsplit=1)[0]
-            sha1 = self._adb_command(
-                f"sha1sum {file_path}").split(" ", maxsplit=1)[0]
-            sha256 = self._adb_command(
-                f"sha256sum {file_path}").split(" ", maxsplit=1)[0]
-            sha512 = self._adb_command(
-                f"sha512sum {file_path}").split(" ", maxsplit=1)[0]
-
-            package_files.append({
-                "path": file_path,
-                "md5": md5,
-                "sha1": sha1,
-                "sha256": sha256,
-                "sha512": sha512,
-            })
+            md5 = self._adb_command(f"md5sum {file_path}").split(" ", maxsplit=1)[0]
+            sha1 = self._adb_command(f"sha1sum {file_path}").split(" ", maxsplit=1)[0]
+            sha256 = self._adb_command(f"sha256sum {file_path}").split(" ", maxsplit=1)[
+                0
+            ]
+            sha512 = self._adb_command(f"sha512sum {file_path}").split(" ", maxsplit=1)[
+                0
+            ]
+
+            package_files.append(
+                {
+                    "path": file_path,
+                    "md5": md5,
+                    "sha1": sha1,
+                    "sha256": sha256,
+                    "sha512": sha512,
+                }
+            )
 
         return package_files
 
     def run(self) -> None:
         self._adb_connect()
 
         packages = self._adb_command("pm list packages -u -i -f")
@@ -286,16 +294,15 @@
                 "installer": installer,
                 "disabled": False,
                 "system": False,
                 "third_party": False,
                 "files": package_files,
             }
 
-            dumpsys_package = self._adb_command(
-                f"dumpsys package {package_name}")
+            dumpsys_package = self._adb_command(f"dumpsys package {package_name}")
             package_details = self.parse_package_for_details(dumpsys_package)
             new_package.update(package_details)
 
             self.results.append(new_package)
 
         cmds = [
             {"field": "disabled", "arg": "-d"},
@@ -320,29 +327,35 @@
 
             dangerous_permissions_count = 0
             for perm in result["requested_permissions"]:
                 if perm in DANGEROUS_PERMISSIONS:
                     dangerous_permissions_count += 1
 
             if dangerous_permissions_count >= DANGEROUS_PERMISSIONS_THRESHOLD:
-                self.log.info("Third-party package \"%s\" requested %d "
-                              "potentially dangerous permissions",
-                              result["package_name"],
-                              dangerous_permissions_count)
+                self.log.info(
+                    'Third-party package "%s" requested %d '
+                    "potentially dangerous permissions",
+                    result["package_name"],
+                    dangerous_permissions_count,
+                )
 
         packages_to_lookup = []
         for result in self.results:
             if result["system"]:
                 continue
 
             packages_to_lookup.append(result)
-            self.log.info("Found non-system package with name \"%s\" installed by \"%s\" on %s",
-                          result["package_name"], result["installer"],
-                          result["timestamp"])
+            self.log.info(
+                'Found non-system package with name "%s" installed by "%s" on %s',
+                result["package_name"],
+                result["installer"],
+                result["timestamp"],
+            )
 
         if not self.fast_mode:
             self.check_virustotal(packages_to_lookup)
 
-        self.log.info("Extracted at total of %d installed package names",
-                      len(self.results))
+        self.log.info(
+            "Extracted at total of %d installed package names", len(self.results)
+        )
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/processes.py` & `mvt-2.3.0/mvt/android/modules/adb/processes.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,26 @@
     """This module extracts details on running processes."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             proc_name = result.get("proc_name", "")
@@ -78,9 +83,8 @@
                 proc["pc"] = fields[6]
                 proc["name"] = fields[8]
 
             self.results.append(proc)
 
         self._adb_disconnect()
 
-        self.log.info("Extracted records on a total of %d processes",
-                      len(self.results))
+        self.log.info("Extracted records on a total of %d processes", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/root_binaries.py` & `mvt-2.3.0/mvt/android/modules/adb/root_binaries.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,26 @@
     """This module extracts the list of installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
         root_binaries = [
             "su",
             "busybox",
             "supersu",
             "Superuser.apk",
@@ -52,10 +57,10 @@
             if not output:
                 continue
 
             if "which: not found" in output:
                 continue
 
             self.detected.append(root_binary)
-            self.log.warning("Found root binary \"%s\"", root_binary)
+            self.log.warning('Found root binary "%s"', root_binary)
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/selinux_status.py` & `mvt-2.3.0/mvt/android/modules/adb/selinux_status.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,29 +15,34 @@
     slug = "selinux_status"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {} if not results else results
 
     def run(self) -> None:
         self._adb_connect()
         output = self._adb_command("getenforce")
         self._adb_disconnect()
 
         status = output.lower().strip()
         self.results["status"] = status
 
         if status == "enforcing":
             self.log.info("SELinux is being regularly enforced")
         else:
-            self.log.warning("SELinux status is \"%s\"!", status)
+            self.log.warning('SELinux status is "%s"!', status)
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/settings.py` & `mvt-2.3.0/mvt/android/modules/adb/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,45 +49,54 @@
         "key": "send_action_app_error",
         "safe_value": "1",
     },
     {
         "description": "enabled installation of non Google Play apps",
         "key": "install_non_market_apps",
         "safe_value": "0",
-    }
+    },
 ]
 
 
 class Settings(AndroidExtraction):
     """This module extracts Android system settings."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {} if not results else results
 
     def check_indicators(self) -> None:
         for _, settings in self.results.items():
             for key, value in settings.items():
                 for danger in ANDROID_DANGEROUS_SETTINGS:
                     # Check if one of the dangerous settings is using an unsafe
                     # value (different than the one specified).
                     if danger["key"] == key and danger["safe_value"] != value:
-                        self.log.warning("Found suspicious setting \"%s = %s\" (%s)",
-                                         key, value, danger["description"])
+                        self.log.warning(
+                            'Found suspicious setting "%s = %s" (%s)',
+                            key,
+                            value,
+                            danger["description"],
+                        )
                         break
 
     def run(self) -> None:
         self._adb_connect()
 
         for namespace in ["system", "secure", "global"]:
             out = self._adb_command(f"cmd settings list {namespace}")
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/sms.py` & `mvt-2.3.0/mvt/android/modules/adb/sms.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 import os
 import sqlite3
 from typing import Optional, Union
 
-from mvt.android.parsers.backup import (AndroidBackupParsingError,
-                                        parse_tar_for_sms)
+from mvt.android.parsers.backup import AndroidBackupParsingError, parse_tar_for_sms
 from mvt.common.module import InsufficientPrivileges
 from mvt.common.utils import check_for_links, convert_unix_to_iso
 
 from .base import AndroidExtraction
 
 SMS_BUGLE_PATH = "data/data/com.google.android.apps.messaging/databases/bugle_db"
 SMS_BUGLE_QUERY = """
@@ -46,31 +45,36 @@
     """This module extracts all SMS messages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.sms_db_type = 0
 
     def serialize(self, record: dict) -> Union[dict, list]:
         body = record["body"].replace("\n", "\\n")
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": f"sms_{record['direction']}",
-            "data": f"{record.get('address', 'unknown source')}: \"{body}\""
+            "data": f"{record.get('address', 'unknown source')}: \"{body}\"",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for message in self.results:
@@ -101,28 +105,27 @@
         names = [description[0] for description in cur.description]
 
         for item in cur:
             message = {}
             for index, value in enumerate(item):
                 message[names[index]] = value
 
-            message["direction"] = ("received" if message["incoming"] == 1 else "sent")
+            message["direction"] = "received" if message["incoming"] == 1 else "sent"
             message["isodate"] = convert_unix_to_iso(message["timestamp"])
 
             # Extract links in the message body
             links = check_for_links(message["body"])
             message["links"] = links
 
             self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d SMS messages",
-                      len(self.results))
+        self.log.info("Extracted a total of %d SMS messages", len(self.results))
 
     def _extract_sms_adb(self) -> None:
         """Use the Android backup command to extract SMS data from the native
         SMS app.
 
         It is crucial to use the under-documented "-nocompress" flag to disable
         the non-standard Java compression algorithm. This module only supports
@@ -131,38 +134,43 @@
         backup_tar = self._generate_backup("com.android.providers.telephony")
         if not backup_tar:
             return
 
         try:
             self.results = parse_tar_for_sms(backup_tar)
         except AndroidBackupParsingError:
-            self.log.info("Impossible to read SMS from the Android Backup, "
-                          "please extract the SMS and try extracting it with "
-                          "Android Backup Extractor")
+            self.log.info(
+                "Impossible to read SMS from the Android Backup, "
+                "please extract the SMS and try extracting it with "
+                "Android Backup Extractor"
+            )
             return
 
-        self.log.info("Extracted a total of %d SMS messages",
-                      len(self.results))
+        self.log.info("Extracted a total of %d SMS messages", len(self.results))
 
     def run(self) -> None:
         self._adb_connect()
 
         try:
             if self._adb_check_file_exists(os.path.join("/", SMS_BUGLE_PATH)):
                 self.sms_db_type = 1
-                self._adb_process_file(os.path.join("/", SMS_BUGLE_PATH),
-                                       self._parse_db)
+                self._adb_process_file(
+                    os.path.join("/", SMS_BUGLE_PATH), self._parse_db
+                )
             elif self._adb_check_file_exists(os.path.join("/", SMS_MMSSMS_PATH)):
                 self.sms_db_type = 2
-                self._adb_process_file(os.path.join("/", SMS_MMSSMS_PATH),
-                                       self._parse_db)
+                self._adb_process_file(
+                    os.path.join("/", SMS_MMSSMS_PATH), self._parse_db
+                )
 
             self._adb_disconnect()
             return
         except InsufficientPrivileges:
             pass
 
-        self.log.info("No SMS database found. Trying extraction of SMS data "
-                      "using Android backup feature.")
+        self.log.info(
+            "No SMS database found. Trying extraction of SMS data "
+            "using Android backup feature."
+        )
         self._extract_sms_adb()
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/adb/whatsapp.py` & `mvt-2.3.0/mvt/android/modules/adb/whatsapp.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,29 +20,34 @@
     """This module extracts all WhatsApp messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record["data"].replace("\n", "\\n")
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": f"whatsapp_msg_{record['direction']}",
-            "data": f"\"{text}\""
+            "data": f'"{text}"',
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for message in self.results:
@@ -57,51 +62,51 @@
         """Parse an Android msgstore.db WhatsApp database file.
 
         :param db_path: Path to the Android WhatsApp database file to process
 
         """
         conn = sqlite3.connect(db_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT * FROM messages;
-        """)
+        """
+        )
         names = [description[0] for description in cur.description]
 
         messages = []
         for item in cur:
             message = {}
             for index, value in enumerate(item):
                 message[names[index]] = value
 
             if not message["data"]:
                 continue
 
-            message["direction"] = ("send" if message["key_from_me"] == 1 else "received")
+            message["direction"] = "send" if message["key_from_me"] == 1 else "received"
             message["isodate"] = convert_unix_to_iso(message["timestamp"])
 
             # If we find links in the messages or if they are empty we add them
             # to the list.
-            if (check_for_links(message["data"])
-                    or message["data"].strip() == ""):
+            if check_for_links(message["data"]) or message["data"].strip() == "":
                 if message.get("thumb_image"):
-                    message["thumb_image"] = base64.b64encode(
-                        message["thumb_image"])
+                    message["thumb_image"] = base64.b64encode(message["thumb_image"])
 
                 messages.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d WhatsApp messages containing links",
-                      len(messages))
+        self.log.info(
+            "Extracted a total of %d WhatsApp messages containing links", len(messages)
+        )
         self.results = messages
 
     def run(self) -> None:
         self._adb_connect()
 
         try:
-            self._adb_process_file(os.path.join("/", WHATSAPP_PATH),
-                                                self._parse_db)
+            self._adb_process_file(os.path.join("/", WHATSAPP_PATH), self._parse_db)
         except Exception as exc:
             self.log.error(exc)
 
         self._adb_disconnect()
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/base.py` & `mvt-2.3.0/mvt/android/modules/androidqf/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This class provides a base for all Android Data analysis modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None
+        results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self._path = target_path
         self._files = []
 
         for root, dirs, files in os.walk(target_path):
             for name in files:
                 self._files.append(os.path.join(root, name))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.3.0/mvt/android/modules/bugreport/accessibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,65 +4,77 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
 from mvt.android.parsers import parse_dumpsys_accessibility
 
-from .base import AndroidQFModule
+from .base import BugReportModule
 
 
-class DumpsysAccessibility(AndroidQFModule):
-    """This module analyse dumpsys accessbility"""
+class Accessibility(BugReportModule):
+    """This module extracts stats on accessibility."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
+                continue
 
     def run(self) -> None:
-        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
-        if not dumpsys_file:
+        content = self._get_dumpstate_file()
+        if not content:
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
         in_accessibility = False
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.strip().startswith("DUMP OF SERVICE accessibility:"):
-                    in_accessibility = True
-                    continue
+        for line in content.decode(errors="ignore").splitlines():
+            if line.strip() == "DUMP OF SERVICE accessibility:":
+                in_accessibility = True
+                continue
+
+            if not in_accessibility:
+                continue
+
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
 
-                if not in_accessibility:
-                    continue
-
-                if line.strip().startswith("-------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
-                    break
-
-                lines.append(line.rstrip())
+            lines.append(line)
 
         self.results = parse_dumpsys_accessibility("\n".join(lines))
-
         for result in self.results:
-            self.log.info("Found installed accessibility service \"%s\"",
-                          result.get("service"))
-
-        self.log.info("Identified a total of %d accessibility services",
-                      len(self.results))
+            self.log.info(
+                'Found installed accessibility service "%s"', result.get("service")
+            )
+
+        self.log.info(
+            "Identified a total of %d accessibility services", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
@@ -52,15 +57,17 @@
                 if line.strip() == "DUMP OF SERVICE package:":
                     in_package = True
                     continue
 
                 if not in_package:
                     continue
 
-                if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+                if line.strip().startswith(
+                    "------------------------------------------------------------------------------"
+                ):  # pylint: disable=line-too-long
                     break
 
                 lines.append(line.rstrip())
 
         self.results = parse_dumpsys_activity_resolver_table("\n".join(lines))
 
         self.log.info("Extracted activities for %d intents", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,60 +8,70 @@
 
 from mvt.android.parsers import parse_dumpsys_appops
 
 from .base import AndroidQFModule
 
 
 class DumpsysAppops(AndroidQFModule):
-
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for perm in record["permissions"]:
             if "entries" not in perm:
                 continue
 
             for entry in perm["entries"]:
                 if "timestamp" in entry:
-                    records.append({
-                        "timestamp": entry["timestamp"],
-                        "module": self.__class__.__name__,
-                        "event": entry["access"],
-                        "data": f"{record['package_name']} access to "
-                                f"{perm['name']} : {entry['access']}",
-                    })
+                    records.append(
+                        {
+                            "timestamp": entry["timestamp"],
+                            "module": self.__class__.__name__,
+                            "event": entry["access"],
+                            "data": f"{record['package_name']} access to "
+                            f"{perm['name']} : {entry['access']}",
+                        }
+                    )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if self.indicators:
                 ioc = self.indicators.check_app_id(result.get("package_name"))
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             for perm in result["permissions"]:
-                if (perm["name"] == "REQUEST_INSTALL_PACKAGES"
-                        and perm["access"] == "allow"):
-                    self.log.info("Package %s with REQUEST_INSTALL_PACKAGES permission",
-                                  result["package_name"])
+                if (
+                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
+                    and perm["access"] == "allow"
+                ):
+                    self.log.info(
+                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
+                        result["package_name"],
+                    )
 
     def run(self) -> None:
         dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
         if not dumpsys_file:
             return
 
         lines = []
@@ -69,15 +79,16 @@
         with open(dumpsys_file[0]) as handle:
             for line in handle:
                 if line.startswith("DUMP OF SERVICE appops:"):
                     in_package = True
                     continue
 
                 if in_package:
-                    if line.startswith("-------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+                    if line.startswith(
+                        "-------------------------------------------------------------------------------"
+                    ):  # pylint: disable=line-too-long
                         break
 
                     lines.append(line.rstrip())
 
         self.results = parse_dumpsys_appops("\n".join(lines))
-        self.log.info("Identified %d applications in AppOps Manager",
-                      len(self.results))
+        self.log.info("Identified %d applications in AppOps Manager", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,58 +2,69 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Any, Dict, List, Optional, Union
 
-from mvt.android.modules.adb.packages import (DANGEROUS_PERMISSIONS,
-                                              DANGEROUS_PERMISSIONS_THRESHOLD,
-                                              ROOT_PACKAGES)
+from mvt.android.modules.adb.packages import (
+    DANGEROUS_PERMISSIONS,
+    DANGEROUS_PERMISSIONS_THRESHOLD,
+    ROOT_PACKAGES,
+)
 from mvt.android.parsers.dumpsys import parse_dumpsys_packages
 
 from .base import AndroidQFModule
 
 
 class DumpsysPackages(AndroidQFModule):
     """This module analyse dumpsys packages"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[List[Dict[str, Any]]] = None
+        results: Optional[List[Dict[str, Any]]] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         entries = []
         for entry in ["timestamp", "first_install_time", "last_update_time"]:
             if entry in record:
-                entries.append({
-                    "timestamp": record[entry],
-                    "module": self.__class__.__name__,
-                    "event": entry,
-                    "data": f"Package {record['package_name']} "
-                            f"({record['uid']})",
-                })
+                entries.append(
+                    {
+                        "timestamp": record[entry],
+                        "module": self.__class__.__name__,
+                        "event": entry,
+                        "data": f"Package {record['package_name']} "
+                        f"({record['uid']})",
+                    }
+                )
 
         return entries
 
     def check_indicators(self) -> None:
         for result in self.results:
             if result["package_name"] in ROOT_PACKAGES:
-                self.log.warning("Found an installed package related to "
-                                 "rooting/jailbreaking: \"%s\"",
-                                 result["package_name"])
+                self.log.warning(
+                    "Found an installed package related to "
+                    'rooting/jailbreaking: "%s"',
+                    result["package_name"],
+                )
                 self.detected.append(result)
                 continue
 
             if not self.indicators:
                 continue
 
             ioc = self.indicators.check_app_id(result.get("package_name", ""))
@@ -95,12 +106,14 @@
         for result in self.results:
             dangerous_permissions_count = 0
             for perm in result["permissions"]:
                 if perm["name"] in DANGEROUS_PERMISSIONS:
                     dangerous_permissions_count += 1
 
             if dangerous_permissions_count >= DANGEROUS_PERMISSIONS_THRESHOLD:
-                self.log.info("Found package \"%s\" requested %d potentially dangerous permissions",
-                              result["package_name"],
-                              dangerous_permissions_count)
+                self.log.info(
+                    'Found package "%s" requested %d potentially dangerous permissions',
+                    result["package_name"],
+                    dangerous_permissions_count,
+                )
 
         self.log.info("Extracted details on %d packages", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,61 +3,80 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Any, Dict, List, Optional, Union
 
 from mvt.android.modules.adb.dumpsys_receivers import (
-    INTENT_DATA_SMS_RECEIVED, INTENT_NEW_OUTGOING_CALL,
-    INTENT_NEW_OUTGOING_SMS, INTENT_PHONE_STATE, INTENT_SMS_RECEIVED)
+    INTENT_DATA_SMS_RECEIVED,
+    INTENT_NEW_OUTGOING_CALL,
+    INTENT_NEW_OUTGOING_SMS,
+    INTENT_PHONE_STATE,
+    INTENT_SMS_RECEIVED,
+)
 from mvt.android.parsers import parse_dumpsys_receiver_resolver_table
 
 from .base import AndroidQFModule
 
 
 class DumpsysReceivers(AndroidQFModule):
     """This module analyse dumpsys receivers"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Union[List[Any], Dict[str, Any], None] = None
+        results: Union[List[Any], Dict[str, Any], None] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for intent, receivers in self.results.items():
             for receiver in receivers:
                 if intent == INTENT_NEW_OUTGOING_SMS:
-                    self.log.info("Found a receiver to intercept outgoing SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept outgoing SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_DATA_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming data SMS message: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming data SMS message: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_PHONE_STATE:
-                    self.log.info("Found a receiver monitoring "
-                                  "telephony state/incoming calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        "Found a receiver monitoring "
+                        'telephony state/incoming calls: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_NEW_OUTGOING_CALL:
-                    self.log.info("Found a receiver monitoring outgoing calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver monitoring outgoing calls: "%s"',
+                        receiver["receiver"],
+                    )
 
                 ioc = self.indicators.check_app_id(receiver["package_name"])
                 if ioc:
                     receiver["matched_indicator"] = ioc
                     self.detected.append({intent: receiver})
 
     def run(self) -> None:
@@ -72,15 +91,17 @@
                 if line.strip() == "DUMP OF SERVICE package:":
                     in_receivers = True
                     continue
 
                 if not in_receivers:
                     continue
 
-                if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+                if line.strip().startswith(
+                    "------------------------------------------------------------------------------"
+                ):  # pylint: disable=line-too-long
                     break
 
                 lines.append(line.rstrip())
 
         self.results = parse_dumpsys_receiver_resolver_table("\n".join(lines))
 
         self.log.info("Extracted receivers for %d intents", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/getprop.py` & `mvt-2.3.0/mvt/android/modules/androidqf/getprop.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,33 +18,38 @@
     "ro.boot.serialno",
     "ro.build.version.sdk",
     "ro.build.version.security_patch",
     "ro.product.cpu.abi",
     "ro.product.locale",
     "ro.product.vendor.manufacturer",
     "ro.product.vendor.model",
-    "ro.product.vendor.name"
+    "ro.product.vendor.name",
 ]
 
 
 class Getprop(AndroidQFModule):
     """This module extracts data from get properties."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.results = []
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -64,13 +69,16 @@
 
         self.results = parse_getprop(data)
         for entry in self.results:
             if entry["name"] in INTERESTING_PROPERTIES:
                 self.log.info("%s: %s", entry["name"], entry["value"])
             if entry["name"] == "ro.build.version.security_patch":
                 last_patch = datetime.strptime(entry["value"], "%Y-%m-%d")
-                if (datetime.now() - last_patch) > timedelta(days=6*31):
-                    self.log.warning("This phone has not received security "
-                                     "updates for more than six months "
-                                     "(last update: %s)", entry["value"])
+                if (datetime.now() - last_patch) > timedelta(days=6 * 31):
+                    self.log.warning(
+                        "This phone has not received security "
+                        "updates for more than six months "
+                        "(last update: %s)",
+                        entry["value"],
+                    )
 
         self.log.info("Extracted a total of %d properties", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/processes.py` & `mvt-2.3.0/mvt/android/modules/androidqf/processes.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,26 @@
     """This module analyse running processes"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             proc_name = result.get("proc_name", "")
@@ -51,39 +56,41 @@
 
     def _parse_ps(self, data):
         for line in data.split("\n")[1:]:
             proc = line.split()
 
             # Sometimes WCHAN is empty.
             if len(proc) == 8:
-                proc = proc[:5] + [''] + proc[5:]
+                proc = proc[:5] + [""] + proc[5:]
 
             # Sometimes there is the security label.
             if proc[0].startswith("u:r"):
                 label = proc[0]
                 proc = proc[1:]
             else:
                 label = ""
 
             # Sometimes there is no WCHAN.
             if len(proc) < 9:
                 proc = proc[:5] + [""] + proc[5:]
 
-            self.results.append({
-                "user": proc[0],
-                "pid": int(proc[1]),
-                "ppid": int(proc[2]),
-                "virtual_memory_size": int(proc[3]),
-                "resident_set_size": int(proc[4]),
-                "wchan": proc[5],
-                "aprocress": proc[6],
-                "stat": proc[7],
-                "proc_name": proc[8].strip("[]"),
-                "label": label,
-            })
+            self.results.append(
+                {
+                    "user": proc[0],
+                    "pid": int(proc[1]),
+                    "ppid": int(proc[2]),
+                    "virtual_memory_size": int(proc[3]),
+                    "resident_set_size": int(proc[4]),
+                    "wchan": proc[5],
+                    "aprocress": proc[6],
+                    "stat": proc[7],
+                    "proc_name": proc[8].strip("[]"),
+                    "label": label,
+                }
+            )
 
     def run(self) -> None:
         ps_files = self._get_files_by_pattern("*/ps.txt")
         if not ps_files:
             return
 
         with open(ps_files[0]) as handle:
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/settings.py` & `mvt-2.3.0/mvt/android/modules/androidqf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,31 @@
     """This module analyse setting files"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.results = {}
 
     def run(self) -> None:
         for setting_file in self._get_files_by_pattern("*/settings_*.txt"):
-            namespace = setting_file[setting_file.rfind("_")+1:-4]
+            namespace = setting_file[setting_file.rfind("_") + 1 : -4]
 
             self.results[namespace] = {}
 
             with open(setting_file) as handle:
                 for line in handle:
                     line = line.strip()
                     try:
@@ -44,15 +49,19 @@
 
                     try:
                         self.results[namespace][key] = value
                     except IndexError:
                         continue
 
                     for danger in ANDROID_DANGEROUS_SETTINGS:
-                        if (danger["key"] == key
-                                and danger["safe_value"] != value):
-                            self.log.warning("Found suspicious setting \"%s = %s\" (%s)",
-                                             key, value, danger["description"])
+                        if danger["key"] == key and danger["safe_value"] != value:
+                            self.log.warning(
+                                'Found suspicious setting "%s = %s" (%s)',
+                                key,
+                                value,
+                                danger["description"],
+                            )
                             break
 
-        self.log.info("Identified %d settings",
-                      sum([len(val) for val in self.results.values()]))
+        self.log.info(
+            "Identified %d settings", sum([len(val) for val in self.results.values()])
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/androidqf/sms.py` & `mvt-2.3.0/mvt/android/modules/androidqf/sms.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,46 +3,55 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1
 
 import getpass
 import logging
 from typing import Optional
 
-from mvt.android.parsers.backup import (AndroidBackupParsingError,
-                                        InvalidBackupPassword, parse_ab_header,
-                                        parse_backup_file, parse_tar_for_sms)
+from mvt.android.parsers.backup import (
+    AndroidBackupParsingError,
+    InvalidBackupPassword,
+    parse_ab_header,
+    parse_backup_file,
+    parse_tar_for_sms,
+)
 
 from .base import AndroidQFModule
 
 
 class SMS(AndroidQFModule):
     """This module analyse SMS file in backup"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for message in self.results:
             if "body" not in message:
                 continue
 
-            if self.indicators.check_domains(message["links"]):
+            if self.indicators.check_domains(message.get("links", [])):
                 self.detected.append(message)
 
     def parse_backup(self, data):
         header = parse_ab_header(data)
         if not header["backup"]:
             self.log.critical("Invalid backup format, backup.ab was not analysed")
             return
@@ -52,34 +61,37 @@
             password = getpass.getpass(prompt="Backup Password: ", stream=None)
         try:
             tardata = parse_backup_file(data, password=password)
         except InvalidBackupPassword:
             self.log.critical("Invalid backup password")
             return
         except AndroidBackupParsingError:
-            self.log.critical("Impossible to parse this backup file, please use"
-                              " Android Backup Extractor instead")
+            self.log.critical(
+                "Impossible to parse this backup file, please use"
+                " Android Backup Extractor instead"
+            )
             return
 
         if not tardata:
             return
 
         try:
             self.results = parse_tar_for_sms(tardata)
         except AndroidBackupParsingError:
-            self.log.info("Impossible to read SMS from the Android Backup, "
-                          "please extract the SMS and try extracting it with "
-                          "Android Backup Extractor")
+            self.log.info(
+                "Impossible to read SMS from the Android Backup, "
+                "please extract the SMS and try extracting it with "
+                "Android Backup Extractor"
+            )
             return
 
     def run(self) -> None:
         files = self._get_files_by_pattern("*/backup.ab")
         if not files:
             self.log.info("No backup data found")
             return
 
         with open(files[0], "rb") as handle:
             data = handle.read()
 
         self.parse_backup(data)
-        self.log.info("Identified %d SMS in backup data",
-                      len(self.results))
+        self.log.info("Identified %d SMS in backup data", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/backup/base.py` & `mvt-2.3.0/mvt/android/modules/backup/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,41 @@
     """This class provides a base for all backup extractios modules"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.ab = None
         self.backup_path = None
         self.tar = None
         self.files = []
 
     def from_folder(self, backup_path: Optional[str], files: List[str]) -> None:
         """
         Get all the files and list them
         """
         self.backup_path = backup_path
         self.files = files
 
-    def from_ab(self, file_path: Optional[str], tar: Optional[TarFile], files: List[str]) -> None:
+    def from_ab(
+        self, file_path: Optional[str], tar: Optional[TarFile], files: List[str]
+    ) -> None:
         """
         Extract the files
         """
         self.ab = file_path
         self.tar = tar
         self.files = files
```

### Comparing `mvt-2.2.6/mvt/android/modules/backup/sms.py` & `mvt-2.3.0/mvt/android/modules/backup/sms.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 
 from mvt.android.modules.backup.base import BackupExtraction
 from mvt.android.parsers.backup import parse_sms_file
 from mvt.common.utils import check_for_links
 
 
 class SMS(BackupExtraction):
-
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.results = []
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for message in self.results:
@@ -51,9 +55,8 @@
 
         mms_path = "apps/com.android.providers.telephony/d_f/*_mms_backup"
         for file in self._get_files_by_pattern(mms_path):
             self.log.info("Processing MMS backup file at %s", file)
             data = self._get_file_content(file)
             self.results.extend(parse_sms_file(data))
 
-        self.log.info("Extracted a total of %d SMS & MMS messages",
-                      len(self.results))
+        self.log.info("Extracted a total of %d SMS & MMS messages", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.3.0/mvt/android/modules/bugreport/battery_daily.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional
+from typing import Optional, Union
 
-from mvt.android.parsers import parse_dumpsys_accessibility
+from mvt.android.parsers import parse_dumpsys_battery_daily
 
 from .base import BugReportModule
 
 
-class Accessibility(BugReportModule):
-    """This module extracts stats on accessibility."""
+class BatteryDaily(BugReportModule):
+    """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
+
+    def serialize(self, record: dict) -> Union[dict, list]:
+        return {
+            "timestamp": record["from"],
+            "module": self.__class__.__name__,
+            "event": "battery_daily",
+            "data": f"Recorded update of package {record['package_name']} "
+            f"with vers {record['vers']}",
+        }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
@@ -37,33 +51,40 @@
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
                 continue
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
-        in_accessibility = False
+        in_batterystats = False
+        in_daily = False
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE accessibility:":
-                in_accessibility = True
+            if line.strip() == "DUMP OF SERVICE batterystats:":
+                in_batterystats = True
                 continue
 
-            if not in_accessibility:
+            if not in_batterystats:
                 continue
 
-            if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+            if line.strip() == "Daily stats:":
+                lines.append(line)
+                in_daily = True
+                continue
+
+            if not in_daily:
+                continue
+
+            if line.strip() == "":
                 break
 
             lines.append(line)
 
-        self.results = parse_dumpsys_accessibility("\n".join(lines))
-        for result in self.results:
-            self.log.info("Found installed accessibility service \"%s\"",
-                          result.get("service"))
+        self.results = parse_dumpsys_battery_daily("\n".join(lines))
 
-        self.log.info("Identified a total of %d accessibility services",
-                      len(self.results))
+        self.log.info("Extracted a total of %d battery daily stats", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/activities.py` & `mvt-2.3.0/mvt/android/modules/bugreport/dbinfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,67 +2,80 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_activity_resolver_table
+from mvt.android.parsers import parse_dumpsys_dbinfo
 
 from .base import BugReportModule
 
 
-class Activities(BugReportModule):
-    """This module extracts details on receivers for risky activities."""
+class DBInfo(BugReportModule):
+    """This module extracts records from battery daily updates."""
+
+    slug = "dbinfo"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
-
-        self.results = results if results else {}
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
-        for intent, activities in self.results.items():
-            for activity in activities:
-                ioc = self.indicators.check_app_id(activity["package_name"])
+        for result in self.results:
+            path = result.get("path", "")
+            for part in path.split("/"):
+                ioc = self.indicators.check_app_id(part)
                 if ioc:
-                    activity["matched_indicator"] = ioc
-                    self.detected.append({intent: activity})
+                    result["matched_indicator"] = ioc
+                    self.detected.append(result)
                     continue
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
+        in_dbinfo = False
         lines = []
-        in_package = False
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE package:":
-                in_package = True
+            if line.strip() == "DUMP OF SERVICE dbinfo:":
+                in_dbinfo = True
                 continue
 
-            if not in_package:
+            if not in_dbinfo:
                 continue
 
-            if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
                 break
 
             lines.append(line)
 
-        self.results = parse_dumpsys_activity_resolver_table("\n".join(lines))
+        self.results = parse_dumpsys_dbinfo("\n".join(lines))
 
-        self.log.info("Extracted activities for %d intents", len(self.results))
+        self.log.info(
+            "Extracted a total of %d database connection pool records",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/appops.py` & `mvt-2.3.0/mvt/android/modules/bugreport/appops.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,74 +15,90 @@
     """This module extracts information on package from App-Ops Manager."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for perm in record["permissions"]:
             if "entries" not in perm:
                 continue
 
             for entry in perm["entries"]:
                 if "timestamp" in entry:
-                    records.append({
-                        "timestamp": entry["timestamp"],
-                        "module": self.__class__.__name__,
-                        "event": entry["access"],
-                        "data": f"{record['package_name']} access to "
-                                f"{perm['name']}: {entry['access']}",
-                    })
+                    records.append(
+                        {
+                            "timestamp": entry["timestamp"],
+                            "module": self.__class__.__name__,
+                            "event": entry["access"],
+                            "data": f"{record['package_name']} access to "
+                            f"{perm['name']}: {entry['access']}",
+                        }
+                    )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if self.indicators:
                 ioc = self.indicators.check_app_id(result.get("package_name"))
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             for perm in result["permissions"]:
-                if (perm["name"] == "REQUEST_INSTALL_PACKAGES"
-                        and perm["access"] == "allow"):
-                    self.log.info("Package %s with REQUEST_INSTALL_PACKAGES permission",
-                                  result["package_name"])
+                if (
+                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
+                    and perm["access"] == "allow"
+                ):
+                    self.log.info(
+                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
+                        result["package_name"],
+                    )
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
         in_appops = False
         for line in content.decode(errors="ignore").splitlines():
             if line.strip() == "DUMP OF SERVICE appops:":
                 in_appops = True
                 continue
 
             if not in_appops:
                 continue
 
-            if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
                 break
 
             lines.append(line)
 
         self.results = parse_dumpsys_appops("\n".join(lines))
 
-        self.log.info("Identified a total of %d packages in App-Ops Manager",
-                      len(self.results))
+        self.log.info(
+            "Identified a total of %d packages in App-Ops Manager", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/base.py` & `mvt-2.3.0/mvt/android/modules/bugreport/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,35 @@
     """This class provides a base for all Android Bug Report modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.zip_archive: Optional[ZipFile] = None
         self.extract_path: Optional[str] = None
         self.extract_files: List[str] = []
         self.zip_files: List[str] = []
 
-    def from_folder(self, extract_path: Optional[str], extract_files: List[str]) -> None:
+    def from_folder(
+        self, extract_path: Optional[str], extract_files: List[str]
+    ) -> None:
         self.extract_path = extract_path
         self.extract_files = extract_files
 
     def from_zip(self, zip_archive: Optional[ZipFile], zip_files: List[str]) -> None:
         self.zip_archive = zip_archive
         self.zip_files = zip_files
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,77 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional, Union
+from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_battery_daily
+from mvt.android.parsers import parse_dumpsys_accessibility
 
-from .base import BugReportModule
+from .base import AndroidQFModule
 
 
-class BatteryDaily(BugReportModule):
-    """This module extracts records from battery daily updates."""
+class DumpsysAccessibility(AndroidQFModule):
+    """This module analyse dumpsys accessbility"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
-
-    def serialize(self, record: dict) -> Union[dict, list]:
-        return {
-            "timestamp": record["from"],
-            "module": self.__class__.__name__,
-            "event": "battery_daily",
-            "data": f"Recorded update of package {record['package_name']} "
-                    f"with vers {record['vers']}"
-        }
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
-                continue
 
     def run(self) -> None:
-        content = self._get_dumpstate_file()
-        if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
+        if not dumpsys_file:
             return
 
         lines = []
-        in_batterystats = False
-        in_daily = False
-        for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE batterystats:":
-                in_batterystats = True
-                continue
+        in_accessibility = False
+        with open(dumpsys_file[0]) as handle:
+            for line in handle:
+                if line.strip().startswith("DUMP OF SERVICE accessibility:"):
+                    in_accessibility = True
+                    continue
+
+                if not in_accessibility:
+                    continue
+
+                if line.strip().startswith(
+                    "-------------------------------------------------------------------------------"
+                ):  # pylint: disable=line-too-long
+                    break
 
-            if not in_batterystats:
-                continue
+                lines.append(line.rstrip())
 
-            if line.strip() == "Daily stats:":
-                lines.append(line)
-                in_daily = True
-                continue
+        self.results = parse_dumpsys_accessibility("\n".join(lines))
 
-            if not in_daily:
-                continue
-
-            if line.strip() == "":
-                break
-
-            lines.append(line)
-
-        self.results = parse_dumpsys_battery_daily("\n".join(lines))
-
-        self.log.info("Extracted a total of %d battery daily stats",
-                      len(self.results))
+        for result in self.results:
+            self.log.info(
+                'Found installed accessibility service "%s"', result.get("service")
+            )
+
+        self.log.info(
+            "Identified a total of %d accessibility services", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.3.0/mvt/android/modules/bugreport/battery_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,26 @@
     """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
@@ -37,16 +42,18 @@
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
                 continue
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
         in_history = False
         for line in content.decode(errors="ignore").splitlines():
             if line.strip().startswith("Battery History "):
                 lines.append(line)
@@ -59,9 +66,10 @@
             if line.strip() == "":
                 break
 
             lines.append(line)
 
         self.results = parse_dumpsys_battery_history("\n".join(lines))
 
-        self.log.info("Extracted a total of %d battery history records",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d battery history records", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.3.0/mvt/ios/modules/mixed/contacts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
+import sqlite3
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_dbinfo
+from ..base import IOSExtraction
 
-from .base import BugReportModule
+CONTACTS_BACKUP_IDS = [
+    "31bb7ba8914766d4ba40d6dfb6113c8b614be442",
+]
+CONTACTS_ROOT_PATHS = [
+    "private/var/mobile/Library/AddressBook/AddressBook.sqlitedb",
+]
 
 
-class DBInfo(BugReportModule):
-    """This module extracts records from battery daily updates."""
-
-    slug = "dbinfo"
+class Contacts(IOSExtraction):
+    """This module extracts all contact details from the phone's address book."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
-
-    def check_indicators(self) -> None:
-        if not self.indicators:
-            return
-
-        for result in self.results:
-            path = result.get("path", "")
-            for part in path.split("/"):
-                ioc = self.indicators.check_app_id(part)
-                if ioc:
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
-                    continue
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
-        content = self._get_dumpstate_file()
-        if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
-            return
-
-        in_dbinfo = False
-        lines = []
-        for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE dbinfo:":
-                in_dbinfo = True
-                continue
-
-            if not in_dbinfo:
-                continue
-
-            if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
-                break
-
-            lines.append(line)
-
-        self.results = parse_dumpsys_dbinfo("\n".join(lines))
-
-        self.log.info("Extracted a total of %d database connection pool records",
-                      len(self.results))
+        self._find_ios_database(
+            backup_ids=CONTACTS_BACKUP_IDS, root_paths=CONTACTS_ROOT_PATHS
+        )
+        self.log.info("Found Contacts database at path: %s", self.file_path)
+
+        conn = sqlite3.connect(self.file_path)
+        cur = conn.cursor()
+        try:
+            cur.execute(
+                """
+                SELECT
+                    multi.value, person.first, person.middle, person.last,
+                    person.organization
+                FROM ABPerson person, ABMultiValue multi
+                WHERE person.rowid = multi.record_id and multi.value not null
+                ORDER by person.rowid ASC;
+            """
+            )
+        except sqlite3.OperationalError as e:
+            self.log.info("Error while reading the contact table: %s", e)
+            return None
+        names = [description[0] for description in cur.description]
+
+        for row in cur:
+            new_contact = {}
+            for index, value in enumerate(row):
+                new_contact[names[index]] = value
+
+            self.results.append(new_contact)
+
+        cur.close()
+        conn.close()
+
+        self.log.info(
+            "Extracted a total of %d contacts from the address book", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/getprop.py` & `mvt-2.3.0/mvt/android/modules/bugreport/getprop.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,52 +16,62 @@
     """This module extracts device properties from getprop command."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {} if not results else results
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
         in_getprop = False
+
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "------ SYSTEM PROPERTIES (getprop) ------":
+            if line.strip().startswith("------ SYSTEM PROPERTIES"):
                 in_getprop = True
                 continue
 
             if not in_getprop:
                 continue
 
             if line.strip() == "------":
                 break
 
             lines.append(line)
 
         self.results = parse_getprop("\n".join(lines))
 
         # Alert if phone is outdated.
-        security_patch = self.results.get("ro.build.version.security_patch", "")
-        if security_patch:
-            patch_date = datetime.strptime(security_patch, "%Y-%m-%d")
-            if (datetime.now() - patch_date) > timedelta(days=6*30):
-                self.log.warning("This phone has not received security updates "
-                                 "for more than six months (last update: %s)",
-                                 security_patch)
+        for entry in self.results:
+            if entry["name"] == "ro.build.version.security_patch":
+                security_patch = entry["value"]
+                patch_date = datetime.strptime(security_patch, "%Y-%m-%d")
+                if (datetime.now() - patch_date) > timedelta(days=6 * 30):
+                    self.log.warning(
+                        "This phone has not received security updates "
+                        "for more than six months (last update: %s)",
+                        security_patch,
+                    )
 
-        self.log.info("Extracted %d Android system properties",
-                      len(self.results))
+        self.log.info("Extracted %d Android system properties", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/packages.py` & `mvt-2.3.0/mvt/android/modules/bugreport/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,72 +2,77 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional, Union
 
-from mvt.android.modules.adb.packages import (DANGEROUS_PERMISSIONS,
-                                              DANGEROUS_PERMISSIONS_THRESHOLD,
-                                              ROOT_PACKAGES)
+from mvt.android.modules.adb.packages import (
+    DANGEROUS_PERMISSIONS,
+    DANGEROUS_PERMISSIONS_THRESHOLD,
+    ROOT_PACKAGES,
+)
 from mvt.android.parsers.dumpsys import parse_dumpsys_packages
 
 from .base import BugReportModule
 
 
 class Packages(BugReportModule):
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
 
         timestamps = [
-            {
-                "event": "package_install",
-                "timestamp": record["timestamp"]
-            },
+            {"event": "package_install", "timestamp": record["timestamp"]},
             {
                 "event": "package_first_install",
-                "timestamp": record["first_install_time"]
-            },
-            {
-                "event": "package_last_update",
-                "timestamp": record["last_update_time"]
+                "timestamp": record["first_install_time"],
             },
+            {"event": "package_last_update", "timestamp": record["last_update_time"]},
         ]
 
         for timestamp in timestamps:
-            records.append({
-                "timestamp": timestamp["timestamp"],
-                "module": self.__class__.__name__,
-                "event": timestamp["event"],
-                "data": f"Install or update of package {record['package_name']}",
-            })
+            records.append(
+                {
+                    "timestamp": timestamp["timestamp"],
+                    "module": self.__class__.__name__,
+                    "event": timestamp["event"],
+                    "data": f"Install or update of package {record['package_name']}",
+                }
+            )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if result["package_name"] in ROOT_PACKAGES:
-                self.log.warning("Found an installed package related to "
-                                 "rooting/jailbreaking: \"%s\"",
-                                 result["package_name"])
+                self.log.warning(
+                    "Found an installed package related to "
+                    'rooting/jailbreaking: "%s"',
+                    result["package_name"],
+                )
                 self.detected.append(result)
                 continue
 
             if not self.indicators:
                 continue
 
             ioc = self.indicators.check_app_id(result.get("package_name"))
@@ -75,16 +80,18 @@
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
                 continue
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         in_package = False
         in_packages_list = False
         lines = []
         for line in content.decode(errors="ignore").splitlines():
             if line.strip() == "DUMP OF SERVICE package:":
@@ -111,12 +118,14 @@
         for result in self.results:
             dangerous_permissions_count = 0
             for perm in result["permissions"]:
                 if perm["name"] in DANGEROUS_PERMISSIONS:
                     dangerous_permissions_count += 1
 
             if dangerous_permissions_count >= DANGEROUS_PERMISSIONS_THRESHOLD:
-                self.log.info("Found package \"%s\" requested %d potentially dangerous permissions",
-                              result["package_name"],
-                              dangerous_permissions_count)
+                self.log.info(
+                    'Found package "%s" requested %d potentially dangerous permissions',
+                    result["package_name"],
+                    dangerous_permissions_count,
+                )
 
         self.log.info("Extracted details on %d packages", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/modules/bugreport/receivers.py` & `mvt-2.3.0/mvt/android/modules/bugreport/receivers.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,71 +21,90 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for intent, receivers in self.results.items():
             for receiver in receivers:
                 if intent == INTENT_NEW_OUTGOING_SMS:
-                    self.log.info("Found a receiver to intercept outgoing SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept outgoing SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming SMS messages: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming SMS messages: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_DATA_SMS_RECEIVED:
-                    self.log.info("Found a receiver to intercept incoming data SMS message: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver to intercept incoming data SMS message: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_PHONE_STATE:
-                    self.log.info("Found a receiver monitoring "
-                                  "telephony state/incoming calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        "Found a receiver monitoring "
+                        'telephony state/incoming calls: "%s"',
+                        receiver["receiver"],
+                    )
                 elif intent == INTENT_NEW_OUTGOING_CALL:
-                    self.log.info("Found a receiver monitoring outgoing calls: \"%s\"",
-                                  receiver["receiver"])
+                    self.log.info(
+                        'Found a receiver monitoring outgoing calls: "%s"',
+                        receiver["receiver"],
+                    )
 
                 ioc = self.indicators.check_app_id(receiver["package_name"])
                 if ioc:
                     receiver["matched_indicator"] = ioc
                     self.detected.append({intent: receiver})
                     continue
 
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
-            self.log.error("Unable to find dumpstate file. "
-                           "Did you provide a valid bug report archive?")
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         in_receivers = False
         lines = []
         for line in content.decode(errors="ignore").splitlines():
             if line.strip() == "DUMP OF SERVICE package:":
                 in_receivers = True
                 continue
 
             if not in_receivers:
                 continue
 
-            if line.strip().startswith("------------------------------------------------------------------------------"):  # pylint: disable=line-too-long
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
                 break
 
             lines.append(line)
 
         self.results = parse_dumpsys_receiver_resolver_table("\n".join(lines))
 
         self.log.info("Extracted receivers for %d intents", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/android/parsers/backup.py` & `mvt-2.3.0/mvt/android/parsers/backup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,24 @@
 
 class InvalidBackupPassword(AndroidBackupParsingError):
     pass
 
 
 # TODO: Need to clean all the following code and conform it to the coding style.
 
+
 def to_utf8_bytes(input_bytes):
     output = []
     for byte in input_bytes:
-        if byte < ord(b'\x80'):
+        if byte < ord(b"\x80"):
             output.append(byte)
         else:
-            output.append(ord('\xef') | (byte >> 12))
-            output.append(ord('\xbc') | ((byte >> 6) & ord('\x3f')))
-            output.append(ord('\x80') | (byte & ord('\x3f')))
+            output.append(ord("\xef") | (byte >> 12))
+            output.append(ord("\xbc") | ((byte >> 6) & ord("\x3f")))
+            output.append(ord("\x80") | (byte & ord("\x3f")))
     return bytes(output)
 
 
 def parse_ab_header(data):
     """
     Parse the header of an Android Backup file
     Returns a dict {'backup': True, 'compression': False,
@@ -51,41 +52,46 @@
     """
     if data.startswith(b"ANDROID BACKUP"):
         [_, version, is_compressed, encryption, _] = data.split(b"\n", 4)
         return {
             "backup": True,
             "compression": (is_compressed == b"1"),
             "version": int(version),
-            "encryption": encryption.decode("utf-8")
+            "encryption": encryption.decode("utf-8"),
         }
 
-    return {
-        "backup": False,
-        "compression": None,
-        "version": None,
-        "encryption": None
-    }
+    return {"backup": False, "compression": None, "version": None, "encryption": None}
 
 
-def decrypt_master_key(password, user_salt, user_iv, pbkdf2_rounds,
-                       master_key_blob, format_version, checksum_salt):
+def decrypt_master_key(
+    password,
+    user_salt,
+    user_iv,
+    pbkdf2_rounds,
+    master_key_blob,
+    format_version,
+    checksum_salt,
+):
     """Generate AES key from user password uisng PBKDF2
 
     The backup master key is extracted from the master key blog after decryption.
     """
     # Derive key from password using PBKDF2.
-    kdf = PBKDF2HMAC(algorithm=hashes.SHA1(), length=32, salt=user_salt,
-                     iterations=pbkdf2_rounds)
+    kdf = PBKDF2HMAC(
+        algorithm=hashes.SHA1(), length=32, salt=user_salt, iterations=pbkdf2_rounds
+    )
     key = kdf.derive(password.encode("utf-8"))
 
     # Decrypt master key blob.
     cipher = Cipher(algorithms.AES(key), modes.CBC(user_iv))
     decryptor = cipher.decryptor()
     try:
-        decryted_master_key_blob = decryptor.update(master_key_blob) + decryptor.finalize()
+        decryted_master_key_blob = (
+            decryptor.update(master_key_blob) + decryptor.finalize()
+        )
 
         # Extract key and IV from decrypted blob.
         key_blob = io.BytesIO(decryted_master_key_blob)
         master_iv_length = ord(key_blob.read(1))
         master_iv = key_blob.read(master_iv_length)
 
         master_key_length = ord(key_blob.read(1))
@@ -99,53 +105,61 @@
     # Handle quirky encoding of master key bytes in Android original Java crypto code.
     if format_version > 1:
         hmac_mk = to_utf8_bytes(master_key)
     else:
         hmac_mk = master_key
 
     # Derive checksum to confirm successful backup decryption.
-    kdf = PBKDF2HMAC(algorithm=hashes.SHA1(), length=32, salt=checksum_salt,
-                     iterations=pbkdf2_rounds)
+    kdf = PBKDF2HMAC(
+        algorithm=hashes.SHA1(), length=32, salt=checksum_salt, iterations=pbkdf2_rounds
+    )
     calculated_checksum = kdf.derive(hmac_mk)
 
     if master_key_checksum != calculated_checksum:
         raise InvalidBackupPassword()
 
     return master_key, master_iv
 
 
-def decrypt_backup_data(encrypted_backup, password, encryption_algo,
-                        format_version):
+def decrypt_backup_data(encrypted_backup, password, encryption_algo, format_version):
     """
     Generate encryption keyffrom password and do decryption
 
     """
     if encryption_algo != b"AES-256":
         raise AndroidBackupNotImplemented("Encryption Algorithm not implemented")
 
     if password is None:
         raise InvalidBackupPassword()
 
-    [user_salt, checksum_salt, pbkdf2_rounds, user_iv,
-     master_key_blob, encrypted_data] = encrypted_backup.split(b"\n", 5)
+    [
+        user_salt,
+        checksum_salt,
+        pbkdf2_rounds,
+        user_iv,
+        master_key_blob,
+        encrypted_data,
+    ] = encrypted_backup.split(b"\n", 5)
 
     user_salt = bytes.fromhex(user_salt.decode("utf-8"))
     checksum_salt = bytes.fromhex(checksum_salt.decode("utf-8"))
     pbkdf2_rounds = int(pbkdf2_rounds)
     user_iv = bytes.fromhex(user_iv.decode("utf-8"))
     master_key_blob = bytes.fromhex(master_key_blob.decode("utf-8"))
 
     # Derive decryption master key from password.
-    master_key, master_iv = decrypt_master_key(password=password,
-                                               user_salt=user_salt,
-                                               user_iv=user_iv,
-                                               pbkdf2_rounds=pbkdf2_rounds,
-                                               master_key_blob=master_key_blob,
-                                               format_version=format_version,
-                                               checksum_salt=checksum_salt)
+    master_key, master_iv = decrypt_master_key(
+        password=password,
+        user_salt=user_salt,
+        user_iv=user_iv,
+        pbkdf2_rounds=pbkdf2_rounds,
+        master_key_blob=master_key_blob,
+        format_version=format_version,
+        checksum_salt=checksum_salt,
+    )
 
     # Decrypt and unpad backup data using derivied key.
     cipher = Cipher(algorithms.AES(master_key), modes.CBC(master_iv))
     decryptor = cipher.decryptor()
     decrypted_tar = decryptor.update(encrypted_data) + decryptor.finalize()
 
     unpadder = padding.PKCS7(128).unpadder()
@@ -156,46 +170,49 @@
     """
     Parse an ab file, returns a tar file
 
     """
     if not data.startswith(b"ANDROID BACKUP"):
         raise AndroidBackupParsingError("Invalid file header")
 
-    [_, version, is_compressed,
-     encryption_algo, tar_data] = data.split(b"\n", 4)
+    [_, version, is_compressed, encryption_algo, tar_data] = data.split(b"\n", 4)
 
     version = int(version)
     is_compressed = int(is_compressed)
 
     if encryption_algo != b"none":
-        tar_data = decrypt_backup_data(tar_data, password, encryption_algo,
-                                       format_version=version)
+        tar_data = decrypt_backup_data(
+            tar_data, password, encryption_algo, format_version=version
+        )
 
     if is_compressed:
         try:
             tar_data = zlib.decompress(tar_data)
         except zlib.error as exc:
-            raise AndroidBackupParsingError("Impossible to decompress the backup file") from exc
+            raise AndroidBackupParsingError(
+                "Impossible to decompress the backup file"
+            ) from exc
 
     return tar_data
 
 
 def parse_tar_for_sms(data):
     """
     Extract SMS from a tar backup archive
     Returns an array of SMS
     """
     dbytes = io.BytesIO(data)
 
     res = []
     with tarfile.open(fileobj=dbytes) as tar:
         for member in tar.getmembers():
-            if (member.name.startswith("apps/com.android.providers.telephony/d_f/")
-                    and (member.name.endswith("_sms_backup")
-                         or member.name.endswith("_mms_backup"))):
+            if member.name.startswith("apps/com.android.providers.telephony/d_f/") and (
+                member.name.endswith("_sms_backup")
+                or member.name.endswith("_mms_backup")
+            ):
                 dhandler = tar.extractfile(member)
                 res.extend(parse_sms_file(dhandler.read()))
 
     return res
 
 
 def parse_sms_file(data):
@@ -212,15 +229,15 @@
         if "mms_body" in entry:
             entry["body"] = entry["mms_body"]
             entry.pop("mms_body")
 
         message_links = check_for_links(entry["body"])
 
         entry["isodate"] = convert_unix_to_iso(int(entry["date"]) / 1000)
-        entry["direction"] = ("sent" if int(entry["date_sent"]) else "received")
+        entry["direction"] = "sent" if int(entry["date_sent"]) else "received"
 
         # Extract links from the body
         if message_links or entry["body"].strip() == "":
             entry["links"] = message_links
         res.append(entry)
 
     return res
```

### Comparing `mvt-2.2.6/mvt/android/parsers/dumpsys.py` & `mvt-2.3.0/mvt/android/parsers/dumpsys.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,20 @@
             continue
 
         if line.strip() == "}":
             break
 
         service = line.split(":")[1].strip()
 
-        results.append({
-            "package_name": service.split("/")[0],
-            "service": service,
-        })
+        results.append(
+            {
+                "package_name": service.split("/")[0],
+                "service": service,
+            }
+        )
 
     return results
 
 
 def parse_dumpsys_activity_resolver_table(output: str) -> Dict[str, Any]:
     results = {}
 
@@ -58,16 +60,15 @@
 
         # If we hit an empty line, the Non-Data Actions section should be
         # finished.
         if line.strip() == "":
             break
 
         # We detect the action name.
-        if (line.startswith(" " * 6) and not line.startswith(" " * 8)
-                and ":" in line):
+        if line.startswith(" " * 6) and not line.startswith(" " * 8) and ":" in line:
             intent = line.strip().replace(":", "")
             results[intent] = []
             continue
 
         # If we are not in an intent block yet, skip.
         if not intent:
             continue
@@ -80,18 +81,20 @@
             continue
 
         # If we got this far, we are processing receivers for the
         # activities we are interested in.
         activity = line.strip().split(" ")[1]
         package_name = activity.split("/")[0]
 
-        results[intent].append({
-            "package_name": package_name,
-            "activity": activity,
-        })
+        results[intent].append(
+            {
+                "package_name": package_name,
+                "activity": activity,
+            }
+        )
 
     return results
 
 
 def parse_dumpsys_battery_daily(output: str) -> list:
     results = []
     daily = None
@@ -115,27 +118,28 @@
 
         line = line.strip().replace("Update ", "")
         package_name, vers = line.split(" ", 1)
         vers_nr = vers.split("=", 1)[1]
 
         already_seen = False
         for update in daily_updates:
-            if (package_name == update["package_name"]
-                    and vers_nr == update["vers"]):
+            if package_name == update["package_name"] and vers_nr == update["vers"]:
                 already_seen = True
                 break
 
         if not already_seen:
-            daily_updates.append({
-                "action": "update",
-                "from": daily["from"],
-                "to": daily["to"],
-                "package_name": package_name,
-                "vers": vers_nr,
-            })
+            daily_updates.append(
+                {
+                    "action": "update",
+                    "from": daily["from"],
+                    "to": daily["to"],
+                    "package_name": package_name,
+                    "vers": vers_nr,
+                }
+            )
 
     if len(daily_updates) > 0:
         results.extend(daily_updates)
 
     return results
 
 
@@ -150,60 +154,68 @@
             break
 
         time_elapsed = line.strip().split(" ", 1)[0]
 
         event = ""
         if line.find("+job") > 0:
             event = "start_job"
-            uid = line[line.find("+job")+5:line.find(":")]
-            service = line[line.find(":")+1:].strip('"')
+            uid = line[line.find("+job") + 5 : line.find(":")]
+            service = line[line.find(":") + 1 :].strip('"')
             package_name = service.split("/")[0]
         elif line.find("-job") > 0:
             event = "end_job"
-            uid = line[line.find("-job")+5:line.find(":")]
-            service = line[line.find(":")+1:].strip('"')
+            uid = line[line.find("-job") + 5 : line.find(":")]
+            service = line[line.find(":") + 1 :].strip('"')
             package_name = service.split("/")[0]
         elif line.find("+running +wake_lock=") > 0:
-            uid = line[line.find("+running +wake_lock=")+21:line.find(":")]
+            uid = line[line.find("+running +wake_lock=") + 21 : line.find(":")]
             event = "wake"
-            service = line[line.find("*walarm*:")+9:].split(" ")[0].strip('"').strip()
+            service = (
+                line[line.find("*walarm*:") + 9 :].split(" ")[0].strip('"').strip()
+            )
             if service == "" or "/" not in service:
                 continue
 
             package_name = service.split("/")[0]
         elif (line.find("+top=") > 0) or (line.find("-top") > 0):
             if line.find("+top=") > 0:
                 event = "start_top"
                 top_pos = line.find("+top=")
             else:
                 event = "end_top"
                 top_pos = line.find("-top=")
-            colon_pos = top_pos+line[top_pos:].find(":")
-            uid = line[top_pos+5:colon_pos]
+            colon_pos = top_pos + line[top_pos:].find(":")
+            uid = line[top_pos + 5 : colon_pos]
             service = ""
-            package_name = line[colon_pos+1:].strip('"')
+            package_name = line[colon_pos + 1 :].strip('"')
         else:
             continue
 
-        results.append({
-            "time_elapsed": time_elapsed,
-            "event": event,
-            "uid": uid,
-            "package_name": package_name,
-            "service": service,
-        })
+        results.append(
+            {
+                "time_elapsed": time_elapsed,
+                "event": event,
+                "uid": uid,
+                "package_name": package_name,
+                "service": service,
+            }
+        )
 
     return results
 
 
 def parse_dumpsys_dbinfo(output: str) -> List[Dict[str, Any]]:
     results = []
 
-    rxp = re.compile(r'.*\[([0-9]{4}-[0-9]{2}-[0-9]{2} [0-9]{2}:[0-9]{2}:[0-9]{2}\.[0-9]{3})\].*\[Pid:\((\d+)\)\](\w+).*sql\=\"(.+?)\"')  # pylint: disable=line-too-long
-    rxp_no_pid = re.compile(r'.*\[([0-9]{4}-[0-9]{2}-[0-9]{2} [0-9]{2}:[0-9]{2}:[0-9]{2}\.[0-9]{3})\][ ]{1}(\w+).*sql\=\"(.+?)\"')  # pylint: disable=line-too-long
+    rxp = re.compile(
+        r".*\[([0-9]{4}-[0-9]{2}-[0-9]{2} [0-9]{2}:[0-9]{2}:[0-9]{2}\.[0-9]{3})\].*\[Pid:\((\d+)\)\](\w+).*sql\=\"(.+?)\""
+    )  # pylint: disable=line-too-long
+    rxp_no_pid = re.compile(
+        r".*\[([0-9]{4}-[0-9]{2}-[0-9]{2} [0-9]{2}:[0-9]{2}:[0-9]{2}\.[0-9]{3})\][ ]{1}(\w+).*sql\=\"(.+?)\""
+    )  # pylint: disable=line-too-long
 
     pool = None
     in_operations = False
     for line in output.splitlines():
         if line.startswith("Connection pool for "):
             pool = line.replace("Connection pool for ", "").rstrip(":")
 
@@ -225,29 +237,33 @@
         matches = rxp.findall(line)
         if not matches:
             matches = rxp_no_pid.findall(line)
             if not matches:
                 continue
 
             match = matches[0]
-            results.append({
-                "isodate": match[0],
-                "action": match[1],
-                "sql": match[2],
-                "path": pool,
-            })
+            results.append(
+                {
+                    "isodate": match[0],
+                    "action": match[1],
+                    "sql": match[2],
+                    "path": pool,
+                }
+            )
         else:
             match = matches[0]
-            results.append({
-                "isodate": match[0],
-                "pid": match[1],
-                "action": match[2],
-                "sql": match[3],
-                "path": pool,
-            })
+            results.append(
+                {
+                    "isodate": match[0],
+                    "pid": match[1],
+                    "action": match[2],
+                    "sql": match[3],
+                    "path": pool,
+                }
+            )
 
     return results
 
 
 def parse_dumpsys_receiver_resolver_table(output: str) -> Dict[str, Any]:
     results = {}
 
@@ -271,16 +287,15 @@
 
         # If we hit an empty line, the Non-Data Actions section should be
         # finished.
         if line.strip() == "":
             break
 
         # We detect the action name.
-        if (line.startswith(" " * 6) and not line.startswith(" " * 8)
-                and ":" in line):
+        if line.startswith(" " * 6) and not line.startswith(" " * 8) and ":" in line:
             intent = line.strip().replace(":", "")
             results[intent] = []
             continue
 
         # If we are not in an intent block yet, skip.
         if not intent:
             continue
@@ -293,18 +308,20 @@
             continue
 
         # If we got this far, we are processing receivers for the
         # activities we are interested in.
         receiver = line.strip().split(" ")[1]
         package_name = receiver.split("/")[0]
 
-        results[intent].append({
-            "package_name": package_name,
-            "receiver": receiver,
-        })
+        results[intent].append(
+            {
+                "package_name": package_name,
+                "receiver": receiver,
+            }
+        )
 
     return results
 
 
 def parse_dumpsys_appops(output: str) -> List[Dict[str, Any]]:
     results = []
     perm = {}
@@ -362,21 +379,23 @@
             # Permission entry like:
             # Reject: [fg-s]2021-05-19 22:02:52.054 (-314d1h25m2s33ms)
             if entry:
                 perm["entries"].append(entry)
                 entry = {}
 
             entry["access"] = line.split(":")[0].strip()
-            entry["type"] = line[line.find("[")+1:line.find("]")]
+            entry["type"] = line[line.find("[") + 1 : line.find("]")]
 
             try:
                 entry["timestamp"] = convert_datetime_to_iso(
                     datetime.strptime(
-                        line[line.find("]")+1:line.find("(")].strip(),
-                        "%Y-%m-%d %H:%M:%S.%f"))
+                        line[line.find("]") + 1 : line.find("(")].strip(),
+                        "%Y-%m-%d %H:%M:%S.%f",
+                    )
+                )
             except ValueError:
                 # Invalid date format
                 pass
 
         if line.strip() == "":
             break
 
@@ -414,47 +433,40 @@
             if line.startswith(" " * 4) and not line.startswith(" " * 6):
                 in_install_permissions = False
             else:
                 lineinfo = line.strip().split(":")
                 permission = lineinfo[0]
                 granted = None
                 if "granted=" in lineinfo[1]:
-                    granted = ("granted=true" in lineinfo[1])
+                    granted = "granted=true" in lineinfo[1]
 
-                details["permissions"].append({
-                    "name": permission,
-                    "granted": granted,
-                    "type": "install"
-                })
+                details["permissions"].append(
+                    {"name": permission, "granted": granted, "type": "install"}
+                )
 
         if in_runtime_permissions:
             if not line.startswith(" " * 8):
                 in_runtime_permissions = False
             else:
                 lineinfo = line.strip().split(":")
                 permission = lineinfo[0]
                 granted = None
                 if "granted=" in lineinfo[1]:
-                    granted = ("granted=true" in lineinfo[1])
+                    granted = "granted=true" in lineinfo[1]
 
-                details["permissions"].append({
-                    "name": permission,
-                    "granted": granted,
-                    "type": "runtime"
-                })
+                details["permissions"].append(
+                    {"name": permission, "granted": granted, "type": "runtime"}
+                )
 
         if in_declared_permissions:
             if not line.startswith(" " * 6):
                 in_declared_permissions = False
             else:
                 permission = line.strip().split(":")[0]
-                details["permissions"].append({
-                    "name": permission,
-                    "type": "declared"
-                })
+                details["permissions"].append({"name": permission, "type": "declared"})
         if in_requested_permissions:
             if not line.startswith(" " * 6):
                 in_requested_permissions = False
             else:
                 details["requested_permissions"].append(line.strip())
 
         if line.strip().startswith("userId="):
```

### Comparing `mvt-2.2.6/mvt/android/parsers/getprop.py` & `mvt-2.3.0/mvt/android/parsers/getprop.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,11 @@
         if line == "":
             continue
 
         matches = re.findall(rxp, line)
         if not matches or len(matches[0]) != 2:
             continue
 
-        entry = {
-            "name": matches[0][0],
-            "value": matches[0][1]
-        }
+        entry = {"name": matches[0][0], "value": matches[0][1]}
         results.append(entry)
 
     return results
```

### Comparing `mvt-2.2.6/mvt/common/cmd_check_iocs.py` & `mvt-2.3.0/mvt/common/cmd_check_iocs.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 import os
 from typing import Optional
 
 from mvt.common.command import Command
+from mvt.common.utils import exec_or_profile
 
 log = logging.getLogger(__name__)
 
 
 class CmdCheckIOCS(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            log=log,
+        )
 
         self.name = "check-iocs"
 
     def run(self) -> None:
         assert self.target_path is not None
         all_modules = []
         for entry in self.modules:
@@ -46,26 +52,31 @@
             for iocs_module in all_modules:
                 if self.module_name and iocs_module.__name__ != self.module_name:
                     continue
 
                 if iocs_module().get_slug() != name_only:
                     continue
 
-                log.info("Loading results from \"%s\" with module %s",
-                         file_name, iocs_module.__name__)
-
-                m = iocs_module.from_json(file_path,
-                                          log=logging.getLogger(iocs_module.__module__))
+                log.info(
+                    'Loading results from "%s" with module %s',
+                    file_name,
+                    iocs_module.__name__,
+                )
+
+                m = iocs_module.from_json(
+                    file_path, log=logging.getLogger(iocs_module.__module__)
+                )
                 if self.iocs.total_ioc_count > 0:
                     m.indicators = self.iocs
                     m.indicators.log = m.log
 
                 try:
-                    m.check_indicators()
+                    exec_or_profile("m.check_indicators()", globals(), locals())
                 except NotImplementedError:
                     continue
                 else:
                     total_detections += len(m.detected)
 
         if total_detections > 0:
-            log.warning("The check of the results produced %d detections!",
-                        total_detections)
+            log.warning(
+                "The check of the results produced %d detections!", total_detections
+            )
```

### Comparing `mvt-2.2.6/mvt/common/command.py` & `mvt-2.3.0/mvt/common/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 import os
 import sys
 from datetime import datetime
 from typing import Optional
 
 from mvt.common.indicators import Indicators
 from mvt.common.module import MVTModule, run_module, save_timeline
-from mvt.common.utils import (convert_datetime_to_iso,
-                              generate_hashes_from_path,
-                              get_sha256_from_file_path)
+from mvt.common.utils import (
+    convert_datetime_to_iso,
+    generate_hashes_from_path,
+    get_sha256_from_file_path,
+)
 from mvt.common.version import MVT_VERSION
 
 
 class Command:
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
     ) -> None:
         self.name = ""
         self.modules = []
 
         self.target_path = target_path
         self.results_path = results_path
@@ -58,43 +59,48 @@
         self.iocs.load_indicators_files(self.ioc_files)
 
     def _create_storage(self) -> None:
         if self.results_path and not os.path.exists(self.results_path):
             try:
                 os.makedirs(self.results_path)
             except Exception as exc:
-                self.log.critical("Unable to create output folder %s: %s",
-                                  self.results_path, exc)
+                self.log.critical(
+                    "Unable to create output folder %s: %s", self.results_path, exc
+                )
                 sys.exit(1)
 
     def _setup_logging(self):
         if not self.results_path:
             return
 
         logger = logging.getLogger("mvt")
-        file_handler = logging.FileHandler(os.path.join(self.results_path,
-                                                        "command.log"))
-        formatter = logging.Formatter("%(asctime)s - %(name)s - "
-                                      "%(levelname)s - %(message)s")
+        file_handler = logging.FileHandler(
+            os.path.join(self.results_path, "command.log")
+        )
+        formatter = logging.Formatter(
+            "%(asctime)s - %(name)s - " "%(levelname)s - %(message)s"
+        )
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
     def _store_timeline(self) -> None:
         if not self.results_path:
             return
 
         if len(self.timeline) > 0:
-            save_timeline(self.timeline,
-                          os.path.join(self.results_path, "timeline.csv"))
+            save_timeline(
+                self.timeline, os.path.join(self.results_path, "timeline.csv")
+            )
 
         if len(self.timeline_detected) > 0:
-            save_timeline(self.timeline_detected,
-                          os.path.join(self.results_path,
-                                       "timeline_detected.csv"))
+            save_timeline(
+                self.timeline_detected,
+                os.path.join(self.results_path, "timeline_detected.csv"),
+            )
 
     def _store_info(self) -> None:
         if not self.results_path:
             return
 
         target_path = None
         if self.target_path:
@@ -120,59 +126,59 @@
 
         info_path = os.path.join(self.results_path, "info.json")
         with open(info_path, "w+", encoding="utf-8") as handle:
             json.dump(info, handle, indent=4)
 
         if self.target_path and (os.environ.get("MVT_HASH_FILES") or self.hashes):
             info_hash = get_sha256_from_file_path(info_path)
-            self.log.info("Reference hash of the info.json file: \"%s\"", info_hash)
+            self.log.info('Reference hash of the info.json file: "%s"', info_hash)
 
     def generate_hashes(self) -> None:
         """
         Compute hashes for files in the target_path
         """
         if not self.target_path:
             return
 
         for file in generate_hashes_from_path(self.target_path, self.log):
             self.hash_values.append(file)
 
     def list_modules(self) -> None:
-        self.log.info("Following is the list of available %s modules:",
-                      self.name)
+        self.log.info("Following is the list of available %s modules:", self.name)
         for module in self.modules:
             self.log.info(" - %s", module.__name__)
 
     def init(self) -> None:
         raise NotImplementedError
 
     def module_init(self, module: MVTModule) -> None:
         raise NotImplementedError
 
     def finish(self) -> None:
         raise NotImplementedError
 
     def run(self) -> None:
-
         try:
             self.init()
         except NotImplementedError:
             pass
 
         for module in self.modules:
             if self.module_name and module.__name__ != self.module_name:
                 continue
 
-            # FIXME: do we need the logger here
+            # FIXME: do we need the logger here
             module_logger = logging.getLogger(module.__module__)
 
-            m = module(target_path=self.target_path,
-                       results_path=self.results_path,
-                       fast_mode=self.fast_mode,
-                       log=module_logger)
+            m = module(
+                target_path=self.target_path,
+                results_path=self.results_path,
+                fast_mode=self.fast_mode,
+                log=module_logger,
+            )
 
             if self.iocs.total_ioc_count:
                 m.indicators = self.iocs
                 m.indicators.log = m.log
 
             if self.serial:
                 m.serial = self.serial
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mvt-2.2.6/mvt/common/help.py` & `mvt-2.3.0/mvt/common/help.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/mvt/common/indicators.py` & `mvt-2.3.0/mvt/common/indicators.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import json
 import logging
 import os
 from typing import Any, Dict, Iterator, List, Optional, Union
+from functools import lru_cache
 
+import ahocorasick
 from appdirs import user_data_dir
 
 from .url import URL
 
 MVT_DATA_FOLDER = user_data_dir("mvt")
 MVT_INDICATORS_FOLDER = os.path.join(MVT_DATA_FOLDER, "indicators")
 
@@ -30,39 +32,39 @@
 
     def _load_downloaded_indicators(self) -> None:
         if not os.path.isdir(MVT_INDICATORS_FOLDER):
             return
 
         for ioc_file_name in os.listdir(MVT_INDICATORS_FOLDER):
             if ioc_file_name.lower().endswith(".stix2"):
-                self.parse_stix2(os.path.join(MVT_INDICATORS_FOLDER,
-                                              ioc_file_name))
+                self.parse_stix2(os.path.join(MVT_INDICATORS_FOLDER, ioc_file_name))
 
     def _check_stix2_env_variable(self) -> None:
         """
         Checks if a variable MVT_STIX2 contains path to a STIX files.
         """
         if "MVT_STIX2" not in os.environ:
             return
 
         paths = os.environ["MVT_STIX2"].split(":")
         for path in paths:
             if os.path.isfile(path):
                 self.parse_stix2(path)
             else:
-                self.log.error("Path specified with env MVT_STIX2 is not a valid file: %s",
-                               path)
+                self.log.error(
+                    "Path specified with env MVT_STIX2 is not a valid file: %s", path
+                )
 
     def _new_collection(
         self,
         cid: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
         file_name: Optional[str] = None,
-        file_path: Optional[str] = None
+        file_path: Optional[str] = None,
     ) -> dict:
         return {
             "id": cid,
             "name": name,
             "description": description,
             "stix2_file_name": file_name,
             "stix2_file_path": file_path,
@@ -74,80 +76,89 @@
             "files_sha256": [],
             "app_ids": [],
             "ios_profile_ids": [],
             "android_property_names": [],
             "count": 0,
         }
 
-    def _add_indicator(self, ioc: str, ioc_coll: dict,
-                       ioc_coll_list: list) -> None:
+    def _add_indicator(self, ioc: str, ioc_coll: dict, ioc_coll_list: list) -> None:
         ioc = ioc.strip("'")
         if ioc not in ioc_coll_list:
             ioc_coll_list.append(ioc)
             ioc_coll["count"] += 1
             self.total_ioc_count += 1
 
     def _process_indicator(self, indicator: dict, collection: dict) -> None:
         key, value = indicator.get("pattern", "").strip("[]").split("=")
 
         if key == "domain-name:value":
             # We force domain names to lower case.
-            self._add_indicator(ioc=value.lower(),
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["domains"])
+            self._add_indicator(
+                ioc=value.lower(),
+                ioc_coll=collection,
+                ioc_coll_list=collection["domains"],
+            )
         elif key == "process:name":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["processes"])
+            self._add_indicator(
+                ioc=value, ioc_coll=collection, ioc_coll_list=collection["processes"]
+            )
         elif key == "email-addr:value":
             # We force email addresses to lower case.
-            self._add_indicator(ioc=value.lower(),
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["emails"])
+            self._add_indicator(
+                ioc=value.lower(),
+                ioc_coll=collection,
+                ioc_coll_list=collection["emails"],
+            )
         elif key == "file:name":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["file_names"])
+            self._add_indicator(
+                ioc=value, ioc_coll=collection, ioc_coll_list=collection["file_names"]
+            )
         elif key == "file:path":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["file_paths"])
+            self._add_indicator(
+                ioc=value, ioc_coll=collection, ioc_coll_list=collection["file_paths"]
+            )
         elif key == "file:hashes.sha256":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["files_sha256"])
+            self._add_indicator(
+                ioc=value, ioc_coll=collection, ioc_coll_list=collection["files_sha256"]
+            )
         elif key == "app:id":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["app_ids"])
+            self._add_indicator(
+                ioc=value, ioc_coll=collection, ioc_coll_list=collection["app_ids"]
+            )
         elif key == "configuration-profile:id":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["ios_profile_ids"])
+            self._add_indicator(
+                ioc=value,
+                ioc_coll=collection,
+                ioc_coll_list=collection["ios_profile_ids"],
+            )
 
         elif key == "android-property:name":
-            self._add_indicator(ioc=value,
-                                ioc_coll=collection,
-                                ioc_coll_list=collection["android_property_names"])
+            self._add_indicator(
+                ioc=value,
+                ioc_coll=collection,
+                ioc_coll_list=collection["android_property_names"],
+            )
 
     def parse_stix2(self, file_path: str) -> None:
         """Extract indicators from a STIX2 file.
 
         :param file_path: Path to the STIX2 file to parse
         :type file_path: str
 
         """
         self.log.info("Parsing STIX2 indicators file at path %s", file_path)
 
         with open(file_path, "r", encoding="utf-8") as handle:
             try:
                 data = json.load(handle)
             except json.decoder.JSONDecodeError:
-                self.log.critical("Unable to parse STIX2 indicator file. "
-                                  "The file is corrupted or in the wrong format!")
+                self.log.critical(
+                    "Unable to parse STIX2 indicator file. "
+                    "The file is corrupted or in the wrong format!"
+                )
                 return
 
         malware = {}
         indicators = []
         relationships = []
         for entry in data.get("objects", []):
             entry_type = entry.get("type", "")
@@ -159,18 +170,21 @@
             elif entry_type == "indicator":
                 indicators.append(entry)
             elif entry_type == "relationship":
                 relationships.append(entry)
 
         collections = []
         for mal_id, mal_values in malware.items():
-            collection = self._new_collection(mal_id, mal_values.get("name"),
-                                              mal_values.get("description"),
-                                              os.path.basename(file_path),
-                                              file_path)
+            collection = self._new_collection(
+                mal_id,
+                mal_values.get("name"),
+                mal_values.get("description"),
+                os.path.basename(file_path),
+                file_path,
+            )
             collections.append(collection)
 
         # We loop through all indicators.
         for indicator in indicators:
             malware_id = None
 
             # We loop through all relationships and find the one pertinent to
@@ -188,128 +202,192 @@
             # got from the relationship.
             for collection in collections:
                 if collection["id"] == malware_id:
                     self._process_indicator(indicator, collection)
                     break
 
         for coll in collections:
-            self.log.info("Extracted %d indicators for collection with name \"%s\"",
-                          coll["count"], coll["name"])
+            self.log.info(
+                'Extracted %d indicators for collection with name "%s"',
+                coll["count"],
+                coll["name"],
+            )
 
         self.ioc_collections.extend(collections)
 
-    def load_indicators_files(self, files: list,
-                              load_default: Optional[bool] = True) -> None:
+    def load_indicators_files(
+        self, files: list, load_default: Optional[bool] = True
+    ) -> None:
         """
         Load a list of indicators files.
         """
         for file_path in files:
             if os.path.isfile(file_path):
                 self.parse_stix2(file_path)
             else:
-                self.log.warning("No indicators file exists at path %s",
-                                 file_path)
+                self.log.warning("No indicators file exists at path %s", file_path)
 
         # Load downloaded indicators and any indicators from env variable.
         if load_default:
             self._load_downloaded_indicators()
 
         self._check_stix2_env_variable()
-        self.log.info("Loaded a total of %d unique indicators",
-                      self.total_ioc_count)
+        self.log.info("Loaded a total of %d unique indicators", self.total_ioc_count)
 
     def get_iocs(self, ioc_type: str) -> Iterator[Dict[str, Any]]:
         for ioc_collection in self.ioc_collections:
             for ioc in ioc_collection.get(ioc_type, []):
                 yield {
                     "value": ioc,
                     "type": ioc_type,
                     "name": ioc_collection["name"],
                     "stix2_file_name": ioc_collection["stix2_file_name"],
                 }
 
+    @lru_cache()
+    def get_ioc_matcher(
+        self, ioc_type: Optional[str] = None, ioc_list: Optional[list] = None
+    ) -> ahocorasick.Automaton:
+        """
+        Build an Aho-Corasick automaton from a list of iocs (i.e indicators)
+        Returns an Aho-Corasick automaton
+
+        This data-structue and algorithim allows for fast matching of a large number
+        of match strings (i.e IOCs) against a large body of text. This will also
+        match strings containing the IOC, so it is important to confirm the
+        match is a valid IOC before using it.
+
+            for _, ioc in domains_automaton.iter(url.domain.lower()):
+                if ioc.value == url.domain.lower():
+                    print(ioc)
+
+        We use an LRU cache to avoid rebuilding the automaton every time we call a
+        function such as check_domain().
+        """
+        automaton = ahocorasick.Automaton()
+        if ioc_type:
+            iocs = self.get_iocs(ioc_type)
+        elif ioc_list:
+            iocs = ioc_list
+        else:
+            raise ValueError("Must provide either ioc_tyxpe or ioc_list")
+
+        for ioc in iocs:
+            automaton.add_word(ioc["value"], ioc)
+        automaton.make_automaton()
+        return automaton
+
+    @lru_cache()
     def check_domain(self, url: str) -> Union[dict, None]:
         """Check if a given URL matches any of the provided domain indicators.
 
         :param url: URL to match against domain indicators
         :type url: str
         :returns: Indicator details if matched, otherwise None
 
         """
         if not url:
             return None
         if not isinstance(url, str):
             return None
 
+        # Create an Aho-Corasick automaton from the list of domains
+        domain_matcher = self.get_ioc_matcher("domains")
+
         try:
             # First we use the provided URL.
             orig_url = URL(url)
 
             if orig_url.check_if_shortened():
                 # If it is, we try to retrieve the actual URL making an
                 # HTTP HEAD request.
                 unshortened = orig_url.unshorten()
 
-                self.log.debug("Found a shortened URL %s -> %s",
-                               url, unshortened)
+                self.log.debug("Found a shortened URL %s -> %s", url, unshortened)
                 if unshortened is None:
+                    self.log.warning("Unable to unshorten URL %s", url)
                     return None
 
                 # Now we check for any nested URL shorteners.
                 dest_url = URL(unshortened)
                 if dest_url.check_if_shortened():
-                    self.log.debug("Original URL %s appears to shorten another "
-                                   "shortened URL %s ... checking!",
-                                   orig_url.url, dest_url.url)
+                    self.log.debug(
+                        "Original URL %s appears to shorten another "
+                        "shortened URL %s ... checking!",
+                        orig_url.url,
+                        dest_url.url,
+                    )
                     return self.check_domain(dest_url.url)
 
                 final_url = dest_url
             else:
                 # If it's not shortened, we just use the original URL object.
                 final_url = orig_url
         except Exception:
             # If URL parsing failed, we just try to do a simple substring
             # match.
-            for ioc in self.get_iocs("domains"):
+            for idx, ioc in domain_matcher.iter(url):
                 if ioc["value"].lower() in url:
-                    self.log.warning("Maybe found a known suspicious domain %s "
-                                     "matching indicators from \"%s\"",
-                                     url, ioc["name"])
+                    self.log.warning(
+                        "Maybe found a known suspicious domain %s "
+                        'matching indicator "%s" from "%s"',
+                        url,
+                        ioc["value"],
+                        ioc["name"],
+                    )
                     return ioc
 
             # If nothing matched, we can quit here.
             return None
 
         # If all parsing worked, we start walking through available domain
         # indicators.
-        for ioc in self.get_iocs("domains"):
+        for idx, ioc in domain_matcher.iter(final_url.domain.lower()):
             # First we check the full domain.
             if final_url.domain.lower() == ioc["value"]:
                 if orig_url.is_shortened and orig_url.url != final_url.url:
-                    self.log.warning("Found a known suspicious domain %s "
-                                     "shortened as %s matching indicators from \"%s\"",
-                                     final_url.url, orig_url.url, ioc["name"])
+                    self.log.warning(
+                        "Found a known suspicious domain %s "
+                        'shortened as %s matching indicator "%s" from "%s"',
+                        final_url.url,
+                        orig_url.url,
+                        ioc["value"],
+                        ioc["name"],
+                    )
                 else:
-                    self.log.warning("Found a known suspicious domain %s "
-                                     "matching indicators from \"%s\"",
-                                     final_url.url, ioc["name"])
-
+                    self.log.warning(
+                        "Found a known suspicious domain %s "
+                        'matching indicator "%s" from "%s"',
+                        final_url.url,
+                        ioc["value"],
+                        ioc["name"],
+                    )
                 return ioc
 
-            # Then we just check the top level domain.
+        # Then we just check the top level domain.
+        for idx, ioc in domain_matcher.iter(final_url.top_level.lower()):
             if final_url.top_level.lower() == ioc["value"]:
                 if orig_url.is_shortened and orig_url.url != final_url.url:
-                    self.log.warning("Found a sub-domain with suspicious top "
-                                     "level %s shortened as %s matching "
-                                     "indicators from \"%s\"", final_url.url,
-                                     orig_url.url, ioc["name"])
+                    self.log.warning(
+                        "Found a sub-domain with suspicious top "
+                        "level %s shortened as %s matching "
+                        'indicator "%s" from "%s"',
+                        final_url.url,
+                        orig_url.url,
+                        ioc["value"],
+                        ioc["name"],
+                    )
                 else:
-                    self.log.warning("Found a sub-domain with a suspicious top "
-                                     "level %s matching indicators from \"%s\"",
-                                     final_url.url, ioc["name"])
+                    self.log.warning(
+                        "Found a sub-domain with a suspicious top "
+                        'level %s matching indicator "%s" from "%s"',
+                        final_url.url,
+                        ioc["value"],
+                        ioc["name"],
+                    )
 
                 return ioc
 
         return None
 
     def check_domains(self, urls: list) -> Union[dict, None]:
         """Check a list of URLs against the provided list of domain indicators.
@@ -340,24 +418,30 @@
         """
         if not process:
             return None
 
         proc_name = os.path.basename(process)
         for ioc in self.get_iocs("processes"):
             if proc_name == ioc["value"]:
-                self.log.warning("Found a known suspicious process name \"%s\" "
-                                 "matching indicators from \"%s\"",
-                                 process, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious process name "%s" '
+                    'matching indicators from "%s"',
+                    process,
+                    ioc["name"],
+                )
                 return ioc
 
             if len(proc_name) == 16:
                 if ioc["value"].startswith(proc_name):
-                    self.log.warning("Found a truncated known suspicious "
-                                     "process name \"%s\" matching indicators from \"%s\"",
-                                     process, ioc["name"])
+                    self.log.warning(
+                        "Found a truncated known suspicious "
+                        'process name "%s" matching indicators from "%s"',
+                        process,
+                        ioc["name"],
+                    )
                     return ioc
 
         return None
 
     def check_processes(self, processes: list) -> Union[dict, None]:
         """Check the provided list of processes against the list of
         process indicators.
@@ -386,17 +470,20 @@
 
         """
         if not email:
             return None
 
         for ioc in self.get_iocs("emails"):
             if email.lower() == ioc["value"].lower():
-                self.log.warning("Found a known suspicious email address \"%s\" "
-                                 "matching indicators from \"%s\"",
-                                 email, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious email address "%s" '
+                    'matching indicators from "%s"',
+                    email,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_file_name(self, file_name: str) -> Union[dict, None]:
         """Check the provided file name against the list of file indicators.
 
@@ -407,17 +494,20 @@
 
         """
         if not file_name:
             return None
 
         for ioc in self.get_iocs("file_names"):
             if ioc["value"] == file_name:
-                self.log.warning("Found a known suspicious file name \"%s\" "
-                                 "matching indicators from \"%s\"",
-                                 file_name, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious file name "%s" '
+                    'matching indicators from "%s"',
+                    file_name,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_file_path(self, file_path: str) -> Union[dict, None]:
         """Check the provided file path against the list of file indicators
         (both path and name).
@@ -435,17 +525,20 @@
         if ioc:
             return ioc
 
         for ioc in self.get_iocs("file_paths"):
             # Strip any trailing slash from indicator paths to match
             # directories.
             if file_path.startswith(ioc["value"].rstrip("/")):
-                self.log.warning("Found a known suspicious file path \"%s\" "
-                                 "matching indicators form \"%s\"",
-                                 file_path, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious file path "%s" '
+                    'matching indicators form "%s"',
+                    file_path,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_file_path_process(self, file_path: str) -> Optional[Dict[str, Any]]:
         """Check the provided file path contains a process name from the
         list of indicators
@@ -458,17 +551,20 @@
         """
         if not file_path:
             return None
 
         for ioc in self.get_iocs("processes"):
             parts = file_path.split("/")
             if ioc["value"] in parts:
-                self.log.warning("Found known suspicious process name mentioned in file at "
-                                  "path \"%s\" matching indicators from \"%s\"",
-                                  file_path, ioc["name"])
+                self.log.warning(
+                    "Found known suspicious process name mentioned in file at "
+                    'path "%s" matching indicators from "%s"',
+                    file_path,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_profile(self, profile_uuid: str) -> Union[dict, None]:
         """Check the provided configuration profile UUID against the list of
         indicators.
@@ -480,17 +576,20 @@
 
         """
         if not profile_uuid:
             return None
 
         for ioc in self.get_iocs("ios_profile_ids"):
             if profile_uuid in ioc["value"]:
-                self.log.warning("Found a known suspicious profile ID \"%s\" "
-                                 "matching indicators from \"%s\"",
-                                 profile_uuid, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious profile ID "%s" '
+                    'matching indicators from "%s"',
+                    profile_uuid,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_file_hash(self, file_hash: str) -> Union[dict, None]:
         """Check the provided SHA256 file hash against the list of indicators.
 
@@ -500,17 +599,20 @@
 
         """
         if not file_hash:
             return None
 
         for ioc in self.get_iocs("files_sha256"):
             if file_hash.lower() == ioc["value"].lower():
-                self.log.warning("Found a known suspicious file with hash \"%s\" "
-                                 "matching indicators from \"%s\"",
-                                 file_hash, ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious file with hash "%s" '
+                    'matching indicators from "%s"',
+                    file_hash,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_app_id(self, app_id: str) -> Union[dict, None]:
         """Check the provided app identifier (typically an Android package name)
         against the list of indicators.
@@ -521,17 +623,20 @@
 
         """
         if not app_id:
             return None
 
         for ioc in self.get_iocs("app_ids"):
             if app_id.lower() == ioc["value"].lower():
-                self.log.warning("Found a known suspicious app with ID \"%s\" "
-                                 "matching indicators from \"%s\"", app_id,
-                                 ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious app with ID "%s" '
+                    'matching indicators from "%s"',
+                    app_id,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
 
     def check_android_property_name(self, property_name: str) -> Optional[dict]:
         """Check the android property name against the list of indicators.
 
@@ -541,13 +646,16 @@
 
         """
         if property_name is None:
             return None
 
         for ioc in self.get_iocs("android_property_names"):
             if property_name.lower() == ioc["value"].lower():
-                self.log.warning("Found a known suspicious Android property \"%s\" "
-                                 "matching indicators from \"%s\"", property_name,
-                                 ioc["name"])
+                self.log.warning(
+                    'Found a known suspicious Android property "%s" '
+                    'matching indicators from "%s"',
+                    property_name,
+                    ioc["name"],
+                )
                 return ioc
 
         return None
```

### Comparing `mvt-2.2.6/mvt/common/logo.py` & `mvt-2.3.0/mvt/common/logo.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,44 +14,52 @@
     mvt_updates = MVTUpdates()
     try:
         latest_version = mvt_updates.check()
     except Exception:
         pass
     else:
         if latest_version:
-            rich_print(f"\t\t[bold]Version {latest_version} is available! "
-                       "Upgrade mvt with `pip3 install -U mvt`[/bold]")
+            rich_print(
+                f"\t\t[bold]Version {latest_version} is available! "
+                "Upgrade mvt with `pip3 install -U mvt`[/bold]"
+            )
 
     # Then we check for indicators files updates.
     ioc_updates = IndicatorsUpdates()
 
     # Before proceeding, we check if we have downloaded an indicators index.
     # If not, there's no point in proceeding with the updates check.
     if ioc_updates.get_latest_update() == 0:
-        rich_print("\t\t[bold]You have not yet downloaded any indicators, check "
-                   "the `download-iocs` command![/bold]")
+        rich_print(
+            "\t\t[bold]You have not yet downloaded any indicators, check "
+            "the `download-iocs` command![/bold]"
+        )
         return
 
     # We only perform this check at a fixed frequency, in order to not
     # overburden the user with too many lookups if the command is being run
     # multiple times.
     should_check, hours = ioc_updates.should_check()
     if not should_check:
-        rich_print(f"\t\tIndicators updates checked recently, next automatic check "
-                   f"in {int(hours)} hours")
+        rich_print(
+            f"\t\tIndicators updates checked recently, next automatic check "
+            f"in {int(hours)} hours"
+        )
         return
 
     try:
         ioc_to_update = ioc_updates.check()
     except Exception:
         pass
     else:
         if ioc_to_update:
-            rich_print("\t\t[bold]There are updates to your indicators files! "
-                       "Run the `download-iocs` command to update![/bold]")
+            rich_print(
+                "\t\t[bold]There are updates to your indicators files! "
+                "Run the `download-iocs` command to update![/bold]"
+            )
         else:
             rich_print("\t\tYour indicators files seem to be up to date.")
 
 
 def logo() -> None:
     rich_print("\n")
     rich_print("\t[bold]MVT[/bold] - Mobile Verification Toolkit")
```

### Comparing `mvt-2.2.6/mvt/common/module.py` & `mvt-2.3.0/mvt/common/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import logging
 import os
 import re
 from typing import Any, Dict, List, Optional, Union
 
 import simplejson as json
 
+from .utils import exec_or_profile
+
 
 class DatabaseNotFoundError(Exception):
     pass
 
 
 class DatabaseCorruptedError(Exception):
     pass
@@ -31,17 +33,17 @@
     slug: Optional[str] = None
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None
+        results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None,
     ) -> None:
         """Initialize module.
 
         :param file_path: Path to the module's database file, if there is any
         :type file_path: str
         :param target_path: Path to the target folder (backup or filesystem
                             dump)
@@ -66,16 +68,15 @@
         self.timeline_detected: List[Dict[str, str]] = []
 
     @classmethod
     def from_json(cls, json_path: str, log: logging.Logger):
         with open(json_path, "r", encoding="utf-8") as handle:
             results = json.load(handle)
             if log:
-                log.info("Loaded %d results from \"%s\"",
-                         len(results), json_path)
+                log.info('Loaded %d results from "%s"', len(results), json_path)
             return cls(results=results, log=log)
 
     def get_slug(self) -> str:
         """Use the module's class name to retrieve a slug"""
         if self.slug:
             return self.slug
 
@@ -95,28 +96,29 @@
         if not self.results_path:
             return
 
         name = self.get_slug()
 
         if self.results:
             results_file_name = f"{name}.json"
-            results_json_path = os.path.join(self.results_path,
-                                             results_file_name)
+            results_json_path = os.path.join(self.results_path, results_file_name)
             with open(results_json_path, "w", encoding="utf-8") as handle:
                 try:
                     json.dump(self.results, handle, indent=4, default=str)
                 except Exception as exc:
-                    self.log.error("Unable to store results of module %s to file %s: %s",
-                                   self.__class__.__name__, results_file_name,
-                                   exc)
+                    self.log.error(
+                        "Unable to store results of module %s to file %s: %s",
+                        self.__class__.__name__,
+                        results_file_name,
+                        exc,
+                    )
 
         if self.detected:
             detected_file_name = f"{name}_detected.json"
-            detected_json_path = os.path.join(self.results_path,
-                                              detected_file_name)
+            detected_json_path = os.path.join(self.results_path, detected_file_name)
             with open(detected_json_path, "w", encoding="utf-8") as handle:
                 json.dump(self.detected, handle, indent=4, default=str)
 
     def serialize(self, record: dict) -> Union[dict, list, None]:
         raise NotImplementedError
 
     @staticmethod
@@ -147,81 +149,105 @@
                 if isinstance(record, list):
                     self.timeline_detected.extend(record)
                 else:
                     self.timeline_detected.append(record)
 
         # De-duplicate timeline entries.
         self.timeline = self._deduplicate_timeline(self.timeline)
-        self.timeline_detected = self._deduplicate_timeline(
-            self.timeline_detected)
+        self.timeline_detected = self._deduplicate_timeline(self.timeline_detected)
 
     def run(self) -> None:
         """Run the main module procedure."""
         raise NotImplementedError
 
 
 def run_module(module: MVTModule) -> None:
     module.log.info("Running module %s...", module.__class__.__name__)
 
     try:
-        module.run()
+        exec_or_profile("module.run()", globals(), locals())
     except NotImplementedError:
-        module.log.exception("The run() procedure of module %s was not implemented yet!",
-                             module.__class__.__name__)
+        module.log.exception(
+            "The run() procedure of module %s was not implemented yet!",
+            module.__class__.__name__,
+        )
     except InsufficientPrivileges as exc:
-        module.log.info("Insufficient privileges for module %s: %s",
-                        module.__class__.__name__, exc)
+        module.log.info(
+            "Insufficient privileges for module %s: %s", module.__class__.__name__, exc
+        )
     except DatabaseNotFoundError as exc:
-        module.log.info("There might be no data to extract by module %s: %s",
-                        module.__class__.__name__, exc)
+        module.log.info(
+            "There might be no data to extract by module %s: %s",
+            module.__class__.__name__,
+            exc,
+        )
     except DatabaseCorruptedError as exc:
-        module.log.error("The %s module database seems to be corrupted: %s",
-                         module.__class__.__name__, exc)
+        module.log.error(
+            "The %s module database seems to be corrupted: %s",
+            module.__class__.__name__,
+            exc,
+        )
     except Exception as exc:
-        module.log.exception("Error in running extraction from module %s: %s",
-                             module.__class__.__name__, exc)
+        module.log.exception(
+            "Error in running extraction from module %s: %s",
+            module.__class__.__name__,
+            exc,
+        )
     else:
         try:
-            module.check_indicators()
+            exec_or_profile("module.check_indicators()", globals(), locals())
         except NotImplementedError:
-            module.log.info("The %s module does not support checking for indicators",
-                            module.__class__.__name__)
+            module.log.info(
+                "The %s module does not support checking for indicators",
+                module.__class__.__name__,
+            )
         except Exception as exc:
-            module.log.exception("Error when checking indicators from module %s: %s",
-                                 module.__class__.__name__, exc)
+            module.log.exception(
+                "Error when checking indicators from module %s: %s",
+                module.__class__.__name__,
+                exc,
+            )
 
         else:
             if module.indicators and not module.detected:
-                module.log.info("The %s module produced no detections!",
-                                module.__class__.__name__)
+                module.log.info(
+                    "The %s module produced no detections!", module.__class__.__name__
+                )
 
         try:
             module.to_timeline()
         except NotImplementedError:
             pass
         except Exception as exc:
-            module.log.exception("Error when serializing data from module %s: %s",
-                                 module.__class__.__name__, exc)
+            module.log.exception(
+                "Error when serializing data from module %s: %s",
+                module.__class__.__name__,
+                exc,
+            )
 
         module.save_to_json()
 
 
 def save_timeline(timeline: list, timeline_path: str) -> None:
     """Save the timeline in a csv file.
 
     :param timeline: List of records to order and store
     :param timeline_path: Path to the csv file to store the timeline to
 
     """
     with open(timeline_path, "a+", encoding="utf-8") as handle:
-        csvoutput = csv.writer(handle, delimiter=",", quotechar="\"",
-                               quoting=csv.QUOTE_ALL)
+        csvoutput = csv.writer(
+            handle, delimiter=",", quotechar='"', quoting=csv.QUOTE_ALL, escapechar="\\"
+        )
         csvoutput.writerow(["UTC Timestamp", "Plugin", "Event", "Description"])
 
-        for event in sorted(timeline, key=lambda x: x["timestamp"]
-                            if x["timestamp"] is not None else ""):
-            csvoutput.writerow([
-                event.get("timestamp"),
-                event.get("module"),
-                event.get("event"),
-                event.get("data"),
-            ])
+        for event in sorted(
+            timeline, key=lambda x: x["timestamp"] if x["timestamp"] is not None else ""
+        ):
+            csvoutput.writerow(
+                [
+                    event.get("timestamp"),
+                    event.get("module"),
+                    event.get("event"),
+                    event.get("data"),
+                ]
+            )
```

### Comparing `mvt-2.2.6/mvt/common/options.py` & `mvt-2.3.0/mvt/common/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     """This class extends click to support mutually exclusive options."""
 
     def __init__(self, *args, **kwargs):
         self.mutually_exclusive = set(kwargs.pop("mutually_exclusive", []))
         help_msg = kwargs.get("help", "")
         if self.mutually_exclusive:
             ex_str = ", ".join(self.mutually_exclusive)
-            kwargs["help"] = (f"{help_msg} NOTE: This argument is mutually exclusive with arguments"
-                              f"[{ex_str}].")
+            kwargs["help"] = (
+                f"{help_msg} NOTE: This argument is mutually exclusive with arguments"
+                f"[{ex_str}]."
+            )
 
         super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         if self.mutually_exclusive.intersection(opts) and self.name in opts:
             raise UsageError(
                 f"Illegal usage: `{self.name}` is mutually exclusive "
```

### Comparing `mvt-2.2.6/mvt/common/updates.py` & `mvt-2.3.0/mvt/common/updates.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,43 +18,43 @@
 log = logging.getLogger(__name__)
 
 # In hours.
 INDICATORS_CHECK_FREQUENCY = 12
 
 
 class MVTUpdates:
-
     def check(self) -> str:
         res = requests.get("https://pypi.org/pypi/mvt/json")
         data = res.json()
         latest_version = data.get("info", {}).get("version", "")
 
         if version.parse(latest_version) > version.parse(MVT_VERSION):
             return latest_version
 
         return ""
 
 
 class IndicatorsUpdates:
-
     def __init__(self) -> None:
         self.github_raw_url = "https://raw.githubusercontent.com/{}/{}/{}/{}"
 
         self.index_owner = "mvt-project"
         self.index_repo = "mvt-indicators"
         self.index_branch = "main"
         self.index_path = "indicators.yaml"
 
         if not os.path.exists(MVT_DATA_FOLDER):
             os.makedirs(MVT_DATA_FOLDER)
 
-        self.latest_update_path = os.path.join(MVT_DATA_FOLDER,
-                                               "latest_indicators_update")
-        self.latest_check_path = os.path.join(MVT_DATA_FOLDER,
-                                              "latest_indicators_check")
+        self.latest_update_path = os.path.join(
+            MVT_DATA_FOLDER, "latest_indicators_update"
+        )
+        self.latest_check_path = os.path.join(
+            MVT_DATA_FOLDER, "latest_indicators_check"
+        )
 
     def get_latest_check(self) -> int:
         if not os.path.exists(self.latest_check_path):
             return 0
 
         with open(self.latest_check_path, "r", encoding="utf-8") as handle:
             data = handle.read().strip()
@@ -81,29 +81,36 @@
 
     def set_latest_update(self) -> None:
         timestamp = int(datetime.utcnow().timestamp())
         with open(self.latest_update_path, "w", encoding="utf-8") as handle:
             handle.write(str(timestamp))
 
     def get_remote_index(self) -> Optional[dict]:
-        url = self.github_raw_url.format(self.index_owner, self.index_repo,
-                                         self.index_branch, self.index_path)
+        url = self.github_raw_url.format(
+            self.index_owner, self.index_repo, self.index_branch, self.index_path
+        )
         res = requests.get(url)
         if res.status_code != 200:
-            log.error("Failed to retrieve indicators index located at %s (error %d)",
-                      url, res.status_code)
+            log.error(
+                "Failed to retrieve indicators index located at %s (error %d)",
+                url,
+                res.status_code,
+            )
             return None
 
         return yaml.safe_load(res.content)
 
     def download_remote_ioc(self, ioc_url: str) -> Optional[str]:
         res = requests.get(ioc_url)
         if res.status_code != 200:
-            log.error("Failed to download indicators file from %s (error %d)",
-                      ioc_url, res.status_code)
+            log.error(
+                "Failed to download indicators file from %s (error %d)",
+                ioc_url,
+                res.status_code,
+            )
             return None
 
         clean_file_name = ioc_url.lstrip("https://").replace("/", "_")
         ioc_path = os.path.join(MVT_INDICATORS_FOLDER, clean_file_name)
 
         with open(ioc_path, "w", encoding="utf-8") as handle:
             handle.write(res.text)
@@ -131,50 +138,62 @@
                 path = github.get("path", "")
 
                 ioc_url = self.github_raw_url.format(owner, repo, branch, path)
             else:
                 ioc_url = ioc.get("download_url", "")
 
             if not ioc_url:
-                log.error("Could not find a way to download indicator file for %s",
-                          ioc.get("name"))
+                log.error(
+                    "Could not find a way to download indicator file for %s",
+                    ioc.get("name"),
+                )
                 continue
 
             ioc_local_path = self.download_remote_ioc(ioc_url)
             if not ioc_local_path:
                 continue
 
-            log.info("Downloaded indicators \"%s\" to %s",
-                     ioc.get("name"), ioc_local_path)
+            log.info(
+                'Downloaded indicators "%s" to %s', ioc.get("name"), ioc_local_path
+            )
 
         self.set_latest_update()
 
-    def _get_remote_file_latest_commit(self, owner: str, repo: str,
-                                       branch: str, path: str) -> int:
+    def _get_remote_file_latest_commit(
+        self, owner: str, repo: str, branch: str, path: str
+    ) -> int:
         # TODO: The branch is currently not taken into consideration.
         #       How do we specify which branch to look up to the API?
-        file_commit_url = f"https://api.github.com/repos/{owner}/{repo}/commits?path={path}"
+        file_commit_url = (
+            f"https://api.github.com/repos/{owner}/{repo}/commits?path={path}"
+        )
         res = requests.get(file_commit_url)
         if res.status_code != 200:
-            log.error("Failed to get details about file %s (error %d)",
-                      file_commit_url, res.status_code)
+            log.error(
+                "Failed to get details about file %s (error %d)",
+                file_commit_url,
+                res.status_code,
+            )
             return -1
 
         details = res.json()
         if len(details) == 0:
             return -1
 
         latest_commit = details[0]
-        latest_commit_date = latest_commit.get("commit", {}).get("author", {}).get("date", None)
+        latest_commit_date = (
+            latest_commit.get("commit", {}).get("author", {}).get("date", None)
+        )
         if not latest_commit_date:
-            log.error("Failed to retrieve date of latest update to indicators index file")
+            log.error(
+                "Failed to retrieve date of latest update to indicators index file"
+            )
             return -1
 
-        latest_commit_dt = datetime.strptime(latest_commit_date,
-                                             '%Y-%m-%dT%H:%M:%SZ')
+        latest_commit_dt = datetime.strptime(latest_commit_date, "%Y-%m-%dT%H:%M:%SZ")
         latest_commit_ts = int(latest_commit_dt.timestamp())
 
         return latest_commit_ts
 
     def should_check(self) -> Tuple[bool, int]:
         now = datetime.utcnow()
         latest_check_ts = self.get_latest_check()
@@ -188,18 +207,17 @@
 
         return False, int(INDICATORS_CHECK_FREQUENCY - diff_hours)
 
     def check(self) -> bool:
         self.set_latest_check()
 
         latest_update = self.get_latest_update()
-        latest_commit_ts = self._get_remote_file_latest_commit(self.index_owner,
-                                                               self.index_repo,
-                                                               self.index_branch,
-                                                               self.index_path)
+        latest_commit_ts = self._get_remote_file_latest_commit(
+            self.index_owner, self.index_repo, self.index_branch, self.index_path
+        )
 
         if latest_update < latest_commit_ts:
             return True
 
         index = self.get_remote_index()
         if not index:
             return False
@@ -210,15 +228,14 @@
 
             github = ioc.get("github", {})
             owner = github.get("owner", "")
             repo = github.get("repo", "")
             branch = github.get("branch", "main")
             path = github.get("path", "")
 
-            file_latest_commit_ts = self._get_remote_file_latest_commit(owner,
-                                                                        repo,
-                                                                        branch,
-                                                                        path)
+            file_latest_commit_ts = self._get_remote_file_latest_commit(
+                owner, repo, branch, path
+            )
             if latest_update < file_latest_commit_ts:
                 return True
 
         return False
```

### Comparing `mvt-2.2.6/mvt/common/url.py` & `mvt-2.3.0/mvt/common/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,14 @@
     "zi.pe",
     "zipmyurl.com",
     "zz.gd",
 ]
 
 
 class URL:
-
     def __init__(self, url: str) -> None:
         if isinstance(url, bytes):
             url = url.decode()
 
         self.url = url
         self.domain = self.get_domain()
         self.top_level = self.get_top_level()
@@ -269,30 +268,30 @@
 
         :param url: URL to parse
         :type url: str
         :returns: Domain name extracted from URL
         :rtype: str
 
         """
-        return get_tld(self.url,
-                       as_object=True,
-                       fix_protocol=True).parsed_url.netloc.lower().lstrip("www.")
+        return (
+            get_tld(self.url, as_object=True, fix_protocol=True)
+            .parsed_url.netloc.lower()
+            .lstrip("www.")
+        )
 
     def get_top_level(self) -> str:
         """Get only the top-level domain from a URL.
 
         :param url: URL to parse
         :type url: str
         :returns: Top-level domain name extracted from URL
         :rtype: str
 
         """
-        return get_tld(self.url,
-                       as_object=True,
-                       fix_protocol=True).fld.lower()
+        return get_tld(self.url, as_object=True, fix_protocol=True).fld.lower()
 
     def check_if_shortened(self) -> bool:
         """Check if the URL is among list of shortener services.
 
 
         :returns: True if the URL is shortened, otherwise False
```

### Comparing `mvt-2.2.6/mvt/common/utils.py` & `mvt-2.3.0/mvt/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #   https://license.mvt.re/1.1/
 
 import datetime
 import hashlib
 import logging
 import os
 import re
+import cProfile
 from typing import Any, Iterator, Union
 
 from rich.logging import RichHandler
 
 
 def convert_chrometime_to_datetime(timestamp: int) -> datetime.datetime:
     """Converts Chrome timestamp to a datetime.
@@ -38,15 +39,15 @@
     try:
         return date_time.strftime("%Y-%m-%d %H:%M:%S.%f")
     except Exception:
         return ""
 
 
 def convert_unix_to_utc_datetime(
-        timestamp: Union[int, float, str]
+    timestamp: Union[int, float, str]
 ) -> datetime.datetime:
     """Converts a unix epoch timestamp to UTC datetime.
 
     :param timestamp: Epoc timestamp to convert.
     :type timestamp: int
     :returns: datetime.
 
@@ -65,16 +66,15 @@
     """
     try:
         return convert_datetime_to_iso(convert_unix_to_utc_datetime(timestamp))
     except Exception:
         return ""
 
 
-def convert_mactime_to_datetime(timestamp: Union[int, float],
-                                from_2001: bool = True):
+def convert_mactime_to_datetime(timestamp: Union[int, float], from_2001: bool = True):
     """Converts Mac Standard Time to a datetime.
 
     :param timestamp: MacTime timestamp (either int or float).
     :type timestamp: int
     :param from_2001: bool: Whether to (Default value = True)
     :param from_2001: Default value = True)
     :returns: datetime.
@@ -107,16 +107,15 @@
     :param from_2001: bool: Whether to (Default value = True)
     :param from_2001: Default value = True)
     :returns: ISO timestamp string in YYYY-mm-dd HH:MM:SS.ms format.
     :rtype: str
 
     """
 
-    return convert_datetime_to_iso(
-        convert_mactime_to_datetime(timestamp, from_2001))
+    return convert_datetime_to_iso(convert_mactime_to_datetime(timestamp, from_2001))
 
 
 def check_for_links(text: str) -> list:
     """Checks if a given text contains HTTP links.
 
     :param text: Any provided text.
     :type text: str
@@ -181,26 +180,28 @@
     :params path: Path of the given folder or file
     :returns: generator of dict {"file_path", "hash"}
     """
     if os.path.isfile(path):
         hash_value = get_sha256_from_file_path(path)
         yield {"file_path": path, "sha256": hash_value}
     elif os.path.isdir(path):
-        for (root, _, files) in os.walk(path):
+        for root, _, files in os.walk(path):
             for file in files:
                 file_path = os.path.join(root, file)
                 try:
                     sha256 = get_sha256_from_file_path(file_path)
                 except FileNotFoundError:
-                    log.error("Failed to hash the file %s: might be a symlink",
-                              file_path)
+                    log.error(
+                        "Failed to hash the file %s: might be a symlink", file_path
+                    )
                     continue
                 except PermissionError:
-                    log.error("Failed to hash the file %s: permission denied",
-                              file_path)
+                    log.error(
+                        "Failed to hash the file %s: permission denied", file_path
+                    )
                     continue
 
                 yield {"file_path": file_path, "sha256": sha256}
 
 
 def init_logging(verbose: bool = False):
     """
@@ -221,7 +222,15 @@
 def set_verbose_logging(verbose: bool = False):
     log = logging.getLogger("mvt")
     handler = log.handlers[0]
     if verbose:
         handler.setLevel(logging.DEBUG)
     else:
         handler.setLevel(logging.INFO)
+
+
+def exec_or_profile(module, globals, locals):
+    """Hook for profiling MVT modules"""
+    if int(os.environ.get("MVT_PROFILE", False)):
+        cProfile.runctx(module, globals, locals)
+    else:
+        exec(module, globals, locals)
```

### Comparing `mvt-2.2.6/mvt/common/virustotal.py` & `mvt-2.3.0/mvt/common/virustotal.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,25 +19,28 @@
 
 class VTQuotaExceeded(Exception):
     pass
 
 
 def virustotal_lookup(file_hash: str):
     if MVT_VT_API_KEY not in os.environ:
-        raise VTNoKey("No VirusTotal API key provided: to use VirusTotal "
-                      "lookups please provide your API key with "
-                      "`export MVT_VT_API_KEY=<key>`")
+        raise VTNoKey(
+            "No VirusTotal API key provided: to use VirusTotal "
+            "lookups please provide your API key with "
+            "`export MVT_VT_API_KEY=<key>`"
+        )
 
     headers = {
         "User-Agent": "VirusTotal",
         "Content-Type": "application/json",
         "x-apikey": os.environ[MVT_VT_API_KEY],
     }
-    res = requests.get(f"https://www.virustotal.com/api/v3/files/{file_hash}",
-                       headers=headers)
+    res = requests.get(
+        f"https://www.virustotal.com/api/v3/files/{file_hash}", headers=headers
+    )
 
     if res.status_code == 200:
         report = res.json()
         return report["data"]
 
     if res.status_code == 404:
         log.info("Could not find results for file with hash %s", file_hash)
```

### Comparing `mvt-2.2.6/mvt/ios/cli.py` & `mvt-2.3.0/mvt/ios/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,94 +7,123 @@
 import logging
 import os
 
 import click
 from rich.prompt import Prompt
 
 from mvt.common.cmd_check_iocs import CmdCheckIOCS
-from mvt.common.help import (HELP_MSG_FAST, HELP_MSG_HASHES, HELP_MSG_IOC,
-                             HELP_MSG_LIST_MODULES, HELP_MSG_MODULE,
-                             HELP_MSG_OUTPUT, HELP_MSG_VERBOSE)
+from mvt.common.help import (
+    HELP_MSG_FAST,
+    HELP_MSG_HASHES,
+    HELP_MSG_IOC,
+    HELP_MSG_LIST_MODULES,
+    HELP_MSG_MODULE,
+    HELP_MSG_OUTPUT,
+    HELP_MSG_VERBOSE,
+)
 from mvt.common.logo import logo
 from mvt.common.options import MutuallyExclusiveOption
 from mvt.common.updates import IndicatorsUpdates
-from mvt.common.utils import (generate_hashes_from_path, init_logging,
-                              set_verbose_logging)
+from mvt.common.utils import (
+    generate_hashes_from_path,
+    init_logging,
+    set_verbose_logging,
+)
 
 from .cmd_check_backup import CmdIOSCheckBackup
 from .cmd_check_fs import CmdIOSCheckFS
 from .decrypt import DecryptBackup
 from .modules.backup import BACKUP_MODULES
 from .modules.fs import FS_MODULES
 from .modules.mixed import MIXED_MODULES
 
 init_logging()
 log = logging.getLogger("mvt")
 
 # Set this environment variable to a password if needed.
 MVT_IOS_BACKUP_PASSWORD = "MVT_IOS_BACKUP_PASSWORD"
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-#==============================================================================
+# ==============================================================================
 # Main
-#==============================================================================
+# ==============================================================================
 @click.group(invoke_without_command=False)
 def cli():
     logo()
 
 
-#==============================================================================
+# ==============================================================================
 # Command: version
-#==============================================================================
+# ==============================================================================
 @cli.command("version", help="Show the currently installed version of MVT")
 def version():
     return
 
 
-#==============================================================================
+# ==============================================================================
 # Command: decrypt-backup
-#==============================================================================
-@cli.command("decrypt-backup", help="Decrypt an encrypted iTunes backup",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--destination", "-d", required=True,
-              help="Path to the folder where to store the decrypted backup")
-@click.option("--password", "-p", cls=MutuallyExclusiveOption,
-              help="Password to use to decrypt the backup (or, set "
-                   f"{MVT_IOS_BACKUP_PASSWORD} environment variable)",
-              mutually_exclusive=["key_file"])
-@click.option("--key-file", "-k", cls=MutuallyExclusiveOption,
-              type=click.Path(exists=True),
-              help="File containing raw encryption key to use to decrypt "
-                   "the backup",
-              mutually_exclusive=["password"])
+# ==============================================================================
+@cli.command(
+    "decrypt-backup",
+    help="Decrypt an encrypted iTunes backup",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--destination",
+    "-d",
+    required=True,
+    help="Path to the folder where to store the decrypted backup",
+)
+@click.option(
+    "--password",
+    "-p",
+    cls=MutuallyExclusiveOption,
+    help="Password to use to decrypt the backup (or, set "
+    f"{MVT_IOS_BACKUP_PASSWORD} environment variable)",
+    mutually_exclusive=["key_file"],
+)
+@click.option(
+    "--key-file",
+    "-k",
+    cls=MutuallyExclusiveOption,
+    type=click.Path(exists=True),
+    help="File containing raw encryption key to use to decrypt " "the backup",
+    mutually_exclusive=["password"],
+)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
 def decrypt_backup(ctx, destination, password, key_file, hashes, backup_path):
     backup = DecryptBackup(backup_path, destination)
 
     if key_file:
         if MVT_IOS_BACKUP_PASSWORD in os.environ:
-            log.info("Ignoring %s environment variable, using --key-file"
-                     "'%s' instead", MVT_IOS_BACKUP_PASSWORD, key_file)
+            log.info(
+                "Ignoring %s environment variable, using --key-file" "'%s' instead",
+                MVT_IOS_BACKUP_PASSWORD,
+                key_file,
+            )
 
         backup.decrypt_with_key_file(key_file)
     elif password:
-        log.info("Your password may be visible in the process table because it "
-                 "was supplied on the command line!")
+        log.info(
+            "Your password may be visible in the process table because it "
+            "was supplied on the command line!"
+        )
 
         if MVT_IOS_BACKUP_PASSWORD in os.environ:
-            log.info("Ignoring %s environment variable, using --password"
-                     "argument instead", MVT_IOS_BACKUP_PASSWORD)
+            log.info(
+                "Ignoring %s environment variable, using --password" "argument instead",
+                MVT_IOS_BACKUP_PASSWORD,
+            )
 
         backup.decrypt_with_password(password)
     elif MVT_IOS_BACKUP_PASSWORD in os.environ:
-        log.info("Using password from %s environment variable",
-                  MVT_IOS_BACKUP_PASSWORD)
+        log.info("Using password from %s environment variable", MVT_IOS_BACKUP_PASSWORD)
         backup.decrypt_with_password(os.environ[MVT_IOS_BACKUP_PASSWORD])
     else:
         sekrit = Prompt.ask("Enter backup password", password=True)
         backup.decrypt_with_password(sekrit)
 
     if not backup.can_process():
         ctx.exit(1)
@@ -108,130 +137,182 @@
         for file in generate_hashes_from_path(destination, log):
             info["decrypted"].append(file)
         info_path = os.path.join(destination, "info.json")
         with open(info_path, "w+", encoding="utf-8") as handle:
             json.dump(info, handle, indent=4)
 
 
-#==============================================================================
+# ==============================================================================
 # Command: extract-key
-#==============================================================================
-@cli.command("extract-key", help="Extract decryption key from an iTunes backup",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--password", "-p",
-              help="Password to use to decrypt the backup (or, set "
-                   f"{MVT_IOS_BACKUP_PASSWORD} environment variable)")
-@click.option("--key-file", "-k",
-              help="Key file to be written (if unset, will print to STDOUT)",
-              required=False,
-              type=click.Path(exists=False, file_okay=True, dir_okay=False,
-                              writable=True))
+# ==============================================================================
+@cli.command(
+    "extract-key",
+    help="Extract decryption key from an iTunes backup",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--password",
+    "-p",
+    help="Password to use to decrypt the backup (or, set "
+    f"{MVT_IOS_BACKUP_PASSWORD} environment variable)",
+)
+@click.option(
+    "--key-file",
+    "-k",
+    help="Key file to be written (if unset, will print to STDOUT)",
+    required=False,
+    type=click.Path(exists=False, file_okay=True, dir_okay=False, writable=True),
+)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 def extract_key(password, key_file, backup_path):
     backup = DecryptBackup(backup_path)
 
     if password:
-        log.info("Your password may be visible in the process table because it "
-                 "was supplied on the command line!")
+        log.info(
+            "Your password may be visible in the process table because it "
+            "was supplied on the command line!"
+        )
 
         if MVT_IOS_BACKUP_PASSWORD in os.environ:
-            log.info("Ignoring %s environment variable, using --password "
-                     "argument instead", MVT_IOS_BACKUP_PASSWORD)
+            log.info(
+                "Ignoring %s environment variable, using --password "
+                "argument instead",
+                MVT_IOS_BACKUP_PASSWORD,
+            )
     elif MVT_IOS_BACKUP_PASSWORD in os.environ:
-        log.info("Using password from %s environment variable",
-                 MVT_IOS_BACKUP_PASSWORD)
+        log.info("Using password from %s environment variable", MVT_IOS_BACKUP_PASSWORD)
         password = os.environ[MVT_IOS_BACKUP_PASSWORD]
     else:
         password = Prompt.ask("Enter backup password", password=True)
 
     backup.decrypt_with_password(password)
     backup.get_key()
 
     if key_file:
         backup.write_key(key_file)
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-backup
-#==============================================================================
-@cli.command("check-backup", help="Extract artifacts from an iTunes backup",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+# ==============================================================================
+@cli.command(
+    "check-backup",
+    help="Extract artifacts from an iTunes backup",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_backup(ctx, iocs, output, fast, list_modules, module, hashes, verbose, backup_path):
+def check_backup(
+    ctx, iocs, output, fast, list_modules, module, hashes, verbose, backup_path
+):
     set_verbose_logging(verbose)
 
-    cmd = CmdIOSCheckBackup(target_path=backup_path, results_path=output,
-                            ioc_files=iocs, module_name=module, fast_mode=fast,
-                            hashes=hashes)
+    cmd = CmdIOSCheckBackup(
+        target_path=backup_path,
+        results_path=output,
+        ioc_files=iocs,
+        module_name=module,
+        fast_mode=fast,
+        hashes=hashes,
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking iTunes backup located at: %s", backup_path)
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the backup produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the backup produced %d detections!", cmd.detected_count
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-fs
-#==============================================================================
-@cli.command("check-fs", help="Extract artifacts from a full filesystem dump",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
-@click.option("--output", "-o", type=click.Path(exists=False),
-              help=HELP_MSG_OUTPUT)
+# ==============================================================================
+@cli.command(
+    "check-fs",
+    help="Extract artifacts from a full filesystem dump",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
+@click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("DUMP_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_fs(ctx, iocs, output, fast, list_modules, module, hashes, verbose, dump_path):
     set_verbose_logging(verbose)
-    cmd = CmdIOSCheckFS(target_path=dump_path, results_path=output,
-                        ioc_files=iocs, module_name=module, fast_mode=fast,
-                        hashes=hashes)
+    cmd = CmdIOSCheckFS(
+        target_path=dump_path,
+        results_path=output,
+        ioc_files=iocs,
+        module_name=module,
+        fast_mode=fast,
+        hashes=hashes,
+    )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking iOS filesystem located at: %s", dump_path)
 
     cmd.run()
 
     if cmd.detected_count > 0:
-        log.warning("The analysis of the iOS filesystem produced %d detections!",
-                    cmd.detected_count)
+        log.warning(
+            "The analysis of the iOS filesystem produced %d detections!",
+            cmd.detected_count,
+        )
 
 
-#==============================================================================
+# ==============================================================================
 # Command: check-iocs
-#==============================================================================
-@cli.command("check-iocs", help="Compare stored JSON results to provided indicators",
-             context_settings=CONTEXT_SETTINGS)
-@click.option("--iocs", "-i", type=click.Path(exists=True), multiple=True,
-              default=[], help=HELP_MSG_IOC)
+# ==============================================================================
+@cli.command(
+    "check-iocs",
+    help="Compare stored JSON results to provided indicators",
+    context_settings=CONTEXT_SETTINGS,
+)
+@click.option(
+    "--iocs",
+    "-i",
+    type=click.Path(exists=True),
+    multiple=True,
+    default=[],
+    help=HELP_MSG_IOC,
+)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.argument("FOLDER", type=click.Path(exists=True))
 @click.pass_context
 def check_iocs(ctx, iocs, list_modules, module, folder):
     cmd = CmdCheckIOCS(target_path=folder, ioc_files=iocs, module_name=module)
     cmd.modules = BACKUP_MODULES + FS_MODULES + MIXED_MODULES
@@ -239,15 +320,18 @@
     if list_modules:
         cmd.list_modules()
         return
 
     cmd.run()
 
 
-#==============================================================================
+# ==============================================================================
 # Command: download-iocs
-#==============================================================================
-@cli.command("download-iocs", help="Download public STIX2 indicators",
-             context_settings=CONTEXT_SETTINGS)
+# ==============================================================================
+@cli.command(
+    "download-iocs",
+    help="Download public STIX2 indicators",
+    context_settings=CONTEXT_SETTINGS,
+)
 def download_iocs():
     ioc_updates = IndicatorsUpdates()
     ioc_updates.update()
```

### Comparing `mvt-2.2.6/mvt/ios/cmd_check_backup.py` & `mvt-2.3.0/mvt/ios/cmd_check_backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 from .modules.backup import BACKUP_MODULES
 from .modules.mixed import MIXED_MODULES
 
 log = logging.getLogger(__name__)
 
 
 class CmdIOSCheckBackup(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, hashes=hashes,
-                         log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            hashes=hashes,
+            log=log,
+        )
 
         self.name = "check-backup"
         self.modules = BACKUP_MODULES + MIXED_MODULES
 
     def module_init(self, module):
         module.is_backup = True
```

### Comparing `mvt-2.2.6/mvt/ios/cmd_check_fs.py` & `mvt-2.3.0/mvt/ios/cmd_check_fs.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 from .modules.fs import FS_MODULES
 from .modules.mixed import MIXED_MODULES
 
 log = logging.getLogger(__name__)
 
 
 class CmdIOSCheckFS(Command):
-
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
-        hashes: Optional[bool] = False,
+        fast_mode: bool = False,
+        hashes: bool = False,
     ) -> None:
-        super().__init__(target_path=target_path, results_path=results_path,
-                         ioc_files=ioc_files, module_name=module_name,
-                         serial=serial, fast_mode=fast_mode, hashes=hashes,
-                         log=log)
+        super().__init__(
+            target_path=target_path,
+            results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
+            fast_mode=fast_mode,
+            hashes=hashes,
+            log=log,
+        )
 
         self.name = "check-fs"
         self.modules = FS_MODULES + MIXED_MODULES
 
     def module_init(self, module):
         module.is_fs_dump = True
```

### Comparing `mvt-2.2.6/mvt/ios/decrypt.py` & `mvt-2.3.0/mvt/ios/decrypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,21 +51,27 @@
             cur.execute("SELECT fileID FROM Files LIMIT 1;")
         except sqlite3.DatabaseError:
             return True
         else:
             log.critical("The backup does not seem encrypted!")
             return False
 
-    def _process_file(self, relative_path: str, domain: str, item,
-                      file_id: str, item_folder: str) -> None:
-        self._backup.getFileDecryptedCopy(manifestEntry=item,
-                                          targetName=file_id,
-                                          targetFolder=item_folder)
-        log.info("Decrypted file %s [%s] to %s/%s", relative_path, domain,
-                 item_folder, file_id)
+    def _process_file(
+        self, relative_path: str, domain: str, item, file_id: str, item_folder: str
+    ) -> None:
+        self._backup.getFileDecryptedCopy(
+            manifestEntry=item, targetName=file_id, targetFolder=item_folder
+        )
+        log.info(
+            "Decrypted file %s [%s] to %s/%s",
+            relative_path,
+            domain,
+            item_folder,
+            file_id,
+        )
 
     def process_backup(self) -> None:
         if not os.path.exists(self.dest_path):
             os.makedirs(self.dest_path)
 
         manifest_path = os.path.join(self.dest_path, "Manifest.db")
         # We extract a decrypted Manifest.db.
@@ -79,148 +85,175 @@
             try:
                 file_id = item["backupFile"]
                 relative_path = item["relativePath"]
                 domain = item["domain"]
 
                 # This may be a partial backup. Skip files from the manifest
                 # which do not exist locally.
-                source_file_path = os.path.join(self.backup_path, file_id[0:2],
-                                                file_id)
+                source_file_path = os.path.join(self.backup_path, file_id[0:2], file_id)
                 if not os.path.exists(source_file_path):
-                    log.debug("Skipping file %s. File not found in encrypted backup directory.",
-                              source_file_path)
+                    log.debug(
+                        "Skipping file %s. File not found in encrypted backup directory.",
+                        source_file_path,
+                    )
                     continue
 
                 item_folder = os.path.join(self.dest_path, file_id[0:2])
                 if not os.path.exists(item_folder):
                     os.makedirs(item_folder)
 
                 # iOSBackup getFileDecryptedCopy() claims to read a "file"
                 # parameter but the code actually is reading the "manifest" key.
                 # Add manifest plist to both keys to handle this.
                 item["manifest"] = item["file"]
 
-                pool.apply_async(self._process_file, args=(relative_path,
-                                                           domain, item,
-                                                           file_id,
-                                                           item_folder))
+                pool.apply_async(
+                    self._process_file,
+                    args=(relative_path, domain, item, file_id, item_folder),
+                )
             except Exception as exc:
                 log.error("Failed to decrypt file %s: %s", relative_path, exc)
 
         pool.close()
         pool.join()
 
         # Copying over the root plist files as well.
         for file_name in os.listdir(self.backup_path):
             if file_name.endswith(".plist"):
-                log.info("Copied plist file %s to %s",
-                         file_name, self.dest_path)
-                shutil.copy(os.path.join(self.backup_path, file_name),
-                            self.dest_path)
+                log.info("Copied plist file %s to %s", file_name, self.dest_path)
+                shutil.copy(os.path.join(self.backup_path, file_name), self.dest_path)
 
     def decrypt_with_password(self, password: str) -> None:
         """Decrypts an encrypted iOS backup.
 
         :param password: Password to use to decrypt the original backup
 
         """
-        log.info("Decrypting iOS backup at path %s with password",
-                 self.backup_path)
+        log.info("Decrypting iOS backup at path %s with password", self.backup_path)
 
         if not os.path.exists(os.path.join(self.backup_path, "Manifest.plist")):
-            possible = glob.glob(os.path.join(
-                self.backup_path, "*", "Manifest.plist"))
+            possible = glob.glob(os.path.join(self.backup_path, "*", "Manifest.plist"))
 
             if len(possible) == 1:
                 newpath = os.path.dirname(possible[0])
-                log.warning("No Manifest.plist in %s, using %s instead.",
-                            self.backup_path, newpath)
+                log.warning(
+                    "No Manifest.plist in %s, using %s instead.",
+                    self.backup_path,
+                    newpath,
+                )
                 self.backup_path = newpath
             elif len(possible) > 1:
-                log.critical("No Manifest.plist in %s, and %d Manifest.plist files in subdirs. "
-                             "Please choose one!",
-                             self.backup_path, len(possible))
+                log.critical(
+                    "No Manifest.plist in %s, and %d Manifest.plist files in subdirs. "
+                    "Please choose one!",
+                    self.backup_path,
+                    len(possible),
+                )
                 return
 
         # Before proceeding, we check whether the backup is indeed encrypted.
         if not self.is_encrypted(self.backup_path):
             return
 
         try:
-            self._backup = iOSbackup(udid=os.path.basename(self.backup_path),
-                                     cleartextpassword=password,
-                                     backuproot=os.path.dirname(self.backup_path))
+            self._backup = iOSbackup(
+                udid=os.path.basename(self.backup_path),
+                cleartextpassword=password,
+                backuproot=os.path.dirname(self.backup_path),
+            )
         except Exception as exc:
-            if (isinstance(exc, KeyError)
-                    and len(exc.args) > 0
-                    and exc.args[0] == b"KEY"):
+            if (
+                isinstance(exc, KeyError)
+                and len(exc.args) > 0
+                and exc.args[0] == b"KEY"
+            ):
                 log.critical("Failed to decrypt backup. Password is probably wrong.")
-            elif (isinstance(exc, FileNotFoundError)
-                    and os.path.basename(exc.filename) == "Manifest.plist"):
-                log.critical("Failed to find a valid backup at %s. "
-                             "Did you point to the right backup path?",
-                             self.backup_path)
+            elif (
+                isinstance(exc, FileNotFoundError)
+                and os.path.basename(exc.filename) == "Manifest.plist"
+            ):
+                log.critical(
+                    "Failed to find a valid backup at %s. "
+                    "Did you point to the right backup path?",
+                    self.backup_path,
+                )
             else:
                 log.exception(exc)
-                log.critical("Failed to decrypt backup. Did you provide the correct password? "
-                             "Did you point to the right backup path?")
+                log.critical(
+                    "Failed to decrypt backup. Did you provide the correct password? "
+                    "Did you point to the right backup path?"
+                )
 
     def decrypt_with_key_file(self, key_file: str) -> None:
         """Decrypts an encrypted iOS backup using a key file.
 
         :param key_file: File to read the key bytes to decrypt the backup
 
         """
-        log.info("Decrypting iOS backup at path %s with key file %s",
-                 self.backup_path, key_file)
+        log.info(
+            "Decrypting iOS backup at path %s with key file %s",
+            self.backup_path,
+            key_file,
+        )
 
         # Before proceeding, we check whether the backup is indeed encrypted.
         if not self.is_encrypted(self.backup_path):
             return
 
         with open(key_file, "rb") as handle:
             key_bytes = handle.read()
 
         # Key should be 64 hex encoded characters (32 raw bytes)
         if len(key_bytes) != 64:
-            log.critical("Invalid key from key file. Did you provide the correct key file?")
+            log.critical(
+                "Invalid key from key file. Did you provide the correct key file?"
+            )
             return
 
         try:
             key_bytes_raw = binascii.unhexlify(key_bytes)
-            self._backup = iOSbackup(udid=os.path.basename(self.backup_path),
-                                     derivedkey=key_bytes_raw,
-                                     backuproot=os.path.dirname(self.backup_path))
+            self._backup = iOSbackup(
+                udid=os.path.basename(self.backup_path),
+                derivedkey=key_bytes_raw,
+                backuproot=os.path.dirname(self.backup_path),
+            )
         except Exception as exc:
             log.exception(exc)
-            log.critical("Failed to decrypt backup. Did you provide the correct key file?")
+            log.critical(
+                "Failed to decrypt backup. Did you provide the correct key file?"
+            )
 
     def get_key(self) -> None:
         """Retrieve and prints the encryption key."""
         if not self._backup:
             return
 
         self._decryption_key = self._backup.getDecryptionKey()
-        log.info("Derived decryption key for backup at path %s is: \"%s\"",
-                 self.backup_path, self._decryption_key)
+        log.info(
+            'Derived decryption key for backup at path %s is: "%s"',
+            self.backup_path,
+            self._decryption_key,
+        )
 
     def write_key(self, key_path: str) -> None:
         """Save extracted key to file.
 
         :param key_path: Path to the file where to write the derived decryption
                          key.
 
         """
         if not self._decryption_key:
             return
 
         try:
-            with open(key_path, 'w', encoding="utf-8") as handle:
+            with open(key_path, "w", encoding="utf-8") as handle:
                 handle.write(self._decryption_key)
         except Exception as exc:
             log.exception(exc)
             log.critical("Failed to write key to file: %s", key_path)
             return
         else:
-            log.info("Wrote decryption key to file: %s. This file is "
-                     "equivalent to a plaintext password. Keep it safe!",
-                     key_path)
+            log.info(
+                "Wrote decryption key to file: %s. This file is "
+                "equivalent to a plaintext password. Keep it safe!",
+                key_path,
+            )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/backup/backup_info.py` & `mvt-2.3.0/mvt/ios/modules/backup/backup_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,39 +18,59 @@
     """This module extracts information about the device and the backup."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {}
 
     def run(self) -> None:
         info_path = os.path.join(self.target_path, "Info.plist")
         if not os.path.exists(info_path):
-            raise DatabaseNotFoundError("No Info.plist at backup path, unable to extract device "
-                                        "information")
+            raise DatabaseNotFoundError(
+                "No Info.plist at backup path, unable to extract device " "information"
+            )
 
         with open(info_path, "rb") as handle:
             info = plistlib.load(handle)
 
-        fields = ["Build Version", "Device Name", "Display Name",
-                  "GUID", "ICCID", "IMEI", "MEID", "Installed Applications",
-                  "Last Backup Date", "Phone Number", "Product Name",
-                  "Product Type", "Product Version", "Serial Number",
-                  "Target Identifier", "Target Type", "Unique Identifier",
-                  "iTunes Version"]
+        fields = [
+            "Build Version",
+            "Device Name",
+            "Display Name",
+            "GUID",
+            "ICCID",
+            "IMEI",
+            "MEID",
+            "Installed Applications",
+            "Last Backup Date",
+            "Phone Number",
+            "Product Name",
+            "Product Type",
+            "Product Version",
+            "Serial Number",
+            "Target Identifier",
+            "Target Type",
+            "Unique Identifier",
+            "iTunes Version",
+        ]
 
         for field in fields:
             value = info.get(field, None)
 
             if field == "Product Type" and value:
                 product_name = get_device_desc_from_id(value)
                 if product_name:
```

### Comparing `mvt-2.2.6/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.3.0/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,86 +9,99 @@
 from base64 import b64encode
 from typing import Optional, Union
 
 from mvt.common.utils import convert_datetime_to_iso
 
 from ..base import IOSExtraction
 
-CONF_PROFILES_DOMAIN = "SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles"
+CONF_PROFILES_DOMAIN = (
+    "SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles"
+)
 
 
 class ConfigurationProfiles(IOSExtraction):
     """This module extracts the full plist data from configuration profiles."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if not record["install_date"]:
             return {}
 
-        payload_name = record['plist'].get('PayloadDisplayName')
-        payload_description = record['plist'].get('PayloadDescription')
+        payload_name = record["plist"].get("PayloadDisplayName")
+        payload_description = record["plist"].get("PayloadDescription")
         return {
             "timestamp": record["install_date"],
             "module": self.__class__.__name__,
             "event": "configuration_profile_install",
             "data": f"{record['plist']['PayloadType']} installed: {record['plist']['PayloadUUID']} "
-                    f"- {payload_name}: {payload_description}"
+            f"- {payload_name}: {payload_description}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             if result["plist"].get("PayloadUUID"):
                 payload_content = result["plist"]["PayloadContent"][0]
 
                 # Alert on any known malicious configuration profiles in the
                 # indicator list.
                 ioc = self.indicators.check_profile(result["plist"]["PayloadUUID"])
                 if ioc:
-                    self.log.warning("Found a known malicious configuration "
-                                     "profile \"%s\" with UUID %s",
-                                     result['plist']['PayloadDisplayName'],
-                                     result['plist']['PayloadUUID'])
+                    self.log.warning(
+                        "Found a known malicious configuration "
+                        'profile "%s" with UUID %s',
+                        result["plist"]["PayloadDisplayName"],
+                        result["plist"]["PayloadUUID"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
                 # Highlight suspicious configuration profiles which may be used
                 # to hide notifications.
                 if payload_content["PayloadType"] in ["com.apple.notificationsettings"]:
-                    self.log.warning("Found a potentially suspicious configuration profile "
-                                     "\"%s\" with payload type %s",
-                                     result['plist']['PayloadDisplayName'],
-                                     payload_content['PayloadType'])
+                    self.log.warning(
+                        "Found a potentially suspicious configuration profile "
+                        '"%s" with payload type %s',
+                        result["plist"]["PayloadDisplayName"],
+                        payload_content["PayloadType"],
+                    )
                     self.detected.append(result)
                     continue
 
     def run(self) -> None:
         for conf_file in self._get_backup_files_from_manifest(
-                domain=CONF_PROFILES_DOMAIN):
+            domain=CONF_PROFILES_DOMAIN
+        ):
             conf_rel_path = conf_file["relative_path"]
 
             # Filter out all configuration files that are not configuration
             # profiles.
-            if not conf_rel_path or not os.path.basename(
-                    conf_rel_path).startswith("profile-"):
+            if not conf_rel_path or not os.path.basename(conf_rel_path).startswith(
+                "profile-"
+            ):
                 continue
 
             conf_file_path = self._get_backup_file_from_id(conf_file["file_id"])
             if not conf_file_path:
                 continue
 
             with open(conf_file_path, "rb") as handle:
@@ -96,41 +109,79 @@
                     conf_plist = plistlib.load(handle)
                 except Exception:
                     conf_plist = {}
 
             # TODO: Tidy up the following code hell.
 
             if "SignerCerts" in conf_plist:
-                conf_plist["SignerCerts"] = [b64encode(x) for x in conf_plist["SignerCerts"]]
+                conf_plist["SignerCerts"] = [
+                    b64encode(x) for x in conf_plist["SignerCerts"]
+                ]
 
             if "OTAProfileStub" in conf_plist:
                 if "SignerCerts" in conf_plist["OTAProfileStub"]:
-                    conf_plist["OTAProfileStub"]["SignerCerts"] = [b64encode(x) for x in conf_plist["OTAProfileStub"]["SignerCerts"]]
+                    conf_plist["OTAProfileStub"]["SignerCerts"] = [
+                        b64encode(x)
+                        for x in conf_plist["OTAProfileStub"]["SignerCerts"]
+                    ]
 
                 if "PayloadContent" in conf_plist["OTAProfileStub"]:
-                    if "EnrollmentIdentityPersistentID" in conf_plist["OTAProfileStub"]["PayloadContent"]:
-                        conf_plist["OTAProfileStub"]["PayloadContent"]["EnrollmentIdentityPersistentID"] = b64encode(conf_plist["OTAProfileStub"]["PayloadContent"]["EnrollmentIdentityPersistentID"])
+                    if (
+                        "EnrollmentIdentityPersistentID"
+                        in conf_plist["OTAProfileStub"]["PayloadContent"]
+                    ):
+                        conf_plist["OTAProfileStub"]["PayloadContent"][
+                            "EnrollmentIdentityPersistentID"
+                        ] = b64encode(
+                            conf_plist["OTAProfileStub"]["PayloadContent"][
+                                "EnrollmentIdentityPersistentID"
+                            ]
+                        )
 
             if "PushTokenDataSentToServerKey" in conf_plist:
-                conf_plist["PushTokenDataSentToServerKey"] = b64encode(conf_plist["PushTokenDataSentToServerKey"])
+                conf_plist["PushTokenDataSentToServerKey"] = b64encode(
+                    conf_plist["PushTokenDataSentToServerKey"]
+                )
 
             if "LastPushTokenHash" in conf_plist:
-                conf_plist["LastPushTokenHash"] = b64encode(conf_plist["LastPushTokenHash"])
+                conf_plist["LastPushTokenHash"] = b64encode(
+                    conf_plist["LastPushTokenHash"]
+                )
 
             if "PayloadContent" in conf_plist:
                 for content_entry in range(len(conf_plist["PayloadContent"])):
                     if "PERSISTENT_REF" in conf_plist["PayloadContent"][content_entry]:
-                        conf_plist["PayloadContent"][content_entry]["PERSISTENT_REF"] = b64encode(conf_plist["PayloadContent"][content_entry]["PERSISTENT_REF"])
-
-                    if "IdentityPersistentRef" in conf_plist["PayloadContent"][content_entry]:
-                        conf_plist["PayloadContent"][content_entry]["IdentityPersistentRef"] = b64encode(conf_plist["PayloadContent"][content_entry]["IdentityPersistentRef"])
-
-            self.results.append({
-                "file_id": conf_file["file_id"],
-                "relative_path": conf_file["relative_path"],
-                "domain": conf_file["domain"],
-                "plist": conf_plist,
-                "install_date": convert_datetime_to_iso(conf_plist.get("InstallDate")),
-            })
-
-        self.log.info("Extracted details about %d configuration profiles",
-                      len(self.results))
+                        conf_plist["PayloadContent"][content_entry][
+                            "PERSISTENT_REF"
+                        ] = b64encode(
+                            conf_plist["PayloadContent"][content_entry][
+                                "PERSISTENT_REF"
+                            ]
+                        )
+
+                    if (
+                        "IdentityPersistentRef"
+                        in conf_plist["PayloadContent"][content_entry]
+                    ):
+                        conf_plist["PayloadContent"][content_entry][
+                            "IdentityPersistentRef"
+                        ] = b64encode(
+                            conf_plist["PayloadContent"][content_entry][
+                                "IdentityPersistentRef"
+                            ]
+                        )
+
+            self.results.append(
+                {
+                    "file_id": conf_file["file_id"],
+                    "relative_path": conf_file["relative_path"],
+                    "domain": conf_file["domain"],
+                    "plist": conf_plist,
+                    "install_date": convert_datetime_to_iso(
+                        conf_plist.get("InstallDate")
+                    ),
+                }
+            )
+
+        self.log.info(
+            "Extracted details about %d configuration profiles", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/backup/manifest.py` & `mvt-2.3.0/mvt/ios/modules/backup/manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,36 @@
     """This module extracts information from a backup Manifest.db file."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def _get_key(self, dictionary, key):
         """Unserialized plist objects can have keys which are str or byte types
         This is a helper to try fetch a key as both a byte or string type.
 
         :param dictionary:
         :param key:
 
         """
-        return (dictionary.get(key.encode("utf-8"), None)
-                or dictionary.get(key, None))
+        return dictionary.get(key.encode("utf-8"), None) or dictionary.get(key, None)
 
     @staticmethod
     def _convert_timestamp(timestamp_or_unix_time_int):
         """Older iOS versions stored the manifest times as unix timestamps.
 
         :param timestamp_or_unix_time_int:
 
@@ -58,41 +62,49 @@
         return convert_unix_to_iso(timestamp_or_unix_time_int)
 
     def serialize(self, record: dict) -> []:
         records = []
         if "modified" not in record or "status_changed" not in record:
             return records
 
-        for timestamp in set([record["created"], record["modified"],
-                             record["status_changed"]]):
+        for timestamp in set(
+            [record["created"], record["modified"], record["status_changed"]]
+        ):
             macb = ""
             macb += "M" if timestamp == record["modified"] else "-"
             macb += "-"
             macb += "C" if timestamp == record["status_changed"] else "-"
             macb += "B" if timestamp == record["created"] else "-"
 
-            records.append({
-                "timestamp": timestamp,
-                "module": self.__class__.__name__,
-                "event": macb,
-                "data": f"{record['relative_path']} - {record['domain']}"
-            })
+            records.append(
+                {
+                    "timestamp": timestamp,
+                    "module": self.__class__.__name__,
+                    "event": macb,
+                    "data": f"{record['relative_path']} - {record['domain']}",
+                }
+            )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if not result.get("relative_path"):
                 continue
 
             if result["domain"]:
-                if (os.path.basename(result["relative_path"]) == "com.apple.CrashReporter.plist"
-                        and result["domain"] == "RootDomain"):
-                    self.log.warning("Found a potentially suspicious "
-                                     "\"com.apple.CrashReporter.plist\" file created in RootDomain")
+                if (
+                    os.path.basename(result["relative_path"])
+                    == "com.apple.CrashReporter.plist"
+                    and result["domain"] == "RootDomain"
+                ):
+                    self.log.warning(
+                        "Found a potentially suspicious "
+                        '"com.apple.CrashReporter.plist" file created in RootDomain'
+                    )
                     self.detected.append(result)
                     continue
 
             if not self.indicators:
                 continue
 
             if self.indicators.check_file_path("/" + result["relative_path"]):
@@ -105,26 +117,29 @@
                 try:
                     URL(part)
                 except Exception:
                     continue
 
                 ioc = self.indicators.check_domain(part)
                 if ioc:
-                    self.log.warning("Found mention of domain \"%s\" in a backup file with "
-                                     "path: %s", ioc["value"], rel_path)
+                    self.log.warning(
+                        'Found mention of domain "%s" in a backup file with '
+                        "path: %s",
+                        ioc["value"],
+                        rel_path,
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
 
     def run(self) -> None:
         manifest_db_path = os.path.join(self.target_path, "Manifest.db")
         if not os.path.isfile(manifest_db_path):
             raise DatabaseNotFoundError("unable to find backup's Manifest.db")
 
-        self.log.info("Found Manifest.db database at path: %s",
-                      manifest_db_path)
+        self.log.info("Found Manifest.db database at path: %s", manifest_db_path)
 
         conn = sqlite3.connect(manifest_db_path)
         cur = conn.cursor()
 
         cur.execute("SELECT * FROM Files;")
         names = [description[0] for description in cur.description]
 
@@ -144,31 +159,37 @@
             if file_data["file"]:
                 try:
                     file_plist = plistlib.load(io.BytesIO(file_data["file"]))
                     file_metadata = self._get_key(file_plist, "$objects")[1]
 
                     birth = self._get_key(file_metadata, "Birth")
                     last_modified = self._get_key(file_metadata, "LastModified")
-                    last_status_change = self._get_key(file_metadata,
-                                                       "LastStatusChange")
-
-                    cleaned_metadata.update({
-                        "created": self._convert_timestamp(birth),
-                        "modified": self._convert_timestamp(last_modified),
-                        "status_changed": self._convert_timestamp(last_status_change),
-                        "mode": oct(self._get_key(file_metadata, "Mode")),
-                        "owner": self._get_key(file_metadata, "UserID"),
-                        "size": self._get_key(file_metadata, "Size"),
-                    })
+                    last_status_change = self._get_key(
+                        file_metadata, "LastStatusChange"
+                    )
+
+                    cleaned_metadata.update(
+                        {
+                            "created": self._convert_timestamp(birth),
+                            "modified": self._convert_timestamp(last_modified),
+                            "status_changed": self._convert_timestamp(
+                                last_status_change
+                            ),
+                            "mode": oct(self._get_key(file_metadata, "Mode")),
+                            "owner": self._get_key(file_metadata, "UserID"),
+                            "size": self._get_key(file_metadata, "Size"),
+                        }
+                    )
                 except Exception:
-                    self.log.exception("Error reading manifest file metadata for file with ID %s "
-                                       "and relative path %s",
-                                       file_data["fileID"],
-                                       file_data["relativePath"])
+                    self.log.exception(
+                        "Error reading manifest file metadata for file with ID %s "
+                        "and relative path %s",
+                        file_data["fileID"],
+                        file_data["relativePath"],
+                    )
 
             self.results.append(cleaned_metadata)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d file metadata items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d file metadata items", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/backup/profile_events.py` & `mvt-2.3.0/mvt/ios/modules/backup/profile_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,35 +17,41 @@
 
 class ProfileEvents(IOSExtraction):
     """This module extracts events related to the installation of configuration
     profiles.
 
 
     """
+
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record.get("timestamp"),
             "module": self.__class__.__name__,
             "event": "profile_operation",
             "data": f"Process {record.get('process')} started operation "
-                    f"{record.get('operation')} of profile "
-                    f"{record.get('profile_id')}"
+            f"{record.get('operation')} of profile "
+            f"{record.get('profile_id')}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -88,25 +94,28 @@
 
             results.append(result)
 
         return results
 
     def run(self) -> None:
         for events_file in self._get_backup_files_from_manifest(
-                relative_path=CONF_PROFILES_EVENTS_RELPATH):
-            events_file_path = self._get_backup_file_from_id(
-                events_file["file_id"])
+            relative_path=CONF_PROFILES_EVENTS_RELPATH
+        ):
+            events_file_path = self._get_backup_file_from_id(events_file["file_id"])
             if not events_file_path:
                 continue
 
-            self.log.info("Found MCProfileEvents.plist file at %s",
-                          events_file_path)
+            self.log.info("Found MCProfileEvents.plist file at %s", events_file_path)
 
             with open(events_file_path, "rb") as handle:
                 self.results.extend(self.parse_profile_events(handle.read()))
 
         for result in self.results:
-            self.log.info("On %s process \"%s\" started operation \"%s\" of profile \"%s\"",
-                          result.get("timestamp"), result.get("process"),
-                          result.get("operation"), result.get("profile_id"))
+            self.log.info(
+                'On %s process "%s" started operation "%s" of profile "%s"',
+                result.get("timestamp"),
+                result.get("process"),
+                result.get("operation"),
+                result.get("profile_id"),
+            )
 
         self.log.info("Extracted %d profile events", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/base.py` & `mvt-2.3.0/mvt/ios/modules/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,45 @@
 import logging
 import os
 import shutil
 import sqlite3
 import subprocess
 from typing import Iterator, Optional, Union
 
-from mvt.common.module import (DatabaseCorruptedError, DatabaseNotFoundError,
-                               MVTModule)
+from mvt.common.module import DatabaseCorruptedError, DatabaseNotFoundError, MVTModule
 
 
 class IOSExtraction(MVTModule):
     """This class provides a base for all iOS filesystem/backup extraction
     modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.is_backup = False
         self.is_fs_dump = False
 
-    def _recover_sqlite_db_if_needed(self, file_path: str,
-                                     forced: Optional[bool] = False) -> None:
+    def _recover_sqlite_db_if_needed(
+        self, file_path: str, forced: bool = False
+    ) -> None:
         """Tries to recover a malformed database by running a .clone command.
 
         :param file_path: Path to the malformed database file.
 
         """
         # TODO: Find a better solution.
         if not forced:
@@ -55,38 +60,43 @@
                     recover = True
             finally:
                 conn.close()
 
             if not recover:
                 return
 
-        self.log.info("Database at path %s is malformed. Trying to recover...",
-                      file_path)
+        self.log.info(
+            "Database at path %s is malformed. Trying to recover...", file_path
+        )
 
         if not shutil.which("sqlite3"):
-            raise DatabaseCorruptedError("failed to recover without sqlite3 binary: please install "
-                                         "sqlite3!")
+            raise DatabaseCorruptedError(
+                "failed to recover without sqlite3 binary: please install " "sqlite3!"
+            )
         if '"' in file_path:
-            raise DatabaseCorruptedError(f"database at path '{file_path}' is corrupted. unable to "
-                                         "recover because it has a quotation mark (\") in its name")
+            raise DatabaseCorruptedError(
+                f"database at path '{file_path}' is corrupted. unable to "
+                'recover because it has a quotation mark (") in its name'
+            )
 
         bak_path = f"{file_path}.bak"
         shutil.move(file_path, bak_path)
 
-        ret = subprocess.call(["sqlite3", bak_path, f".clone \"{file_path}\""],
-                              stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        ret = subprocess.call(
+            ["sqlite3", bak_path, f'.clone "{file_path}"'],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
         if ret != 0:
             raise DatabaseCorruptedError("failed to recover database")
 
         self.log.info("Database at path %s recovered successfully!", file_path)
 
     def _get_backup_files_from_manifest(
-        self,
-        relative_path: Optional[str] = None,
-        domain: Optional[str] = None
+        self, relative_path: Optional[str] = None, domain: Optional[str] = None
     ) -> Iterator[dict]:
         """Locate files from Manifest.db.
 
         :param relative_path: Relative path to use as filter from Manifest.db.
                               (Default value = None)
         :param domain: Domain to use as filter from Manifest.db.
                        (Default value = None)
@@ -98,24 +108,27 @@
 
         base_sql = "SELECT fileID, domain, relativePath FROM Files WHERE "
 
         try:
             conn = sqlite3.connect(manifest_db_path)
             cur = conn.cursor()
             if relative_path and domain:
-                cur.execute(f"{base_sql} relativePath = ? AND domain = ?;",
-                            (relative_path, domain))
+                cur.execute(
+                    f"{base_sql} relativePath = ? AND domain = ?;",
+                    (relative_path, domain),
+                )
             else:
                 if relative_path:
                     if "*" in relative_path:
-                        cur.execute(f"{base_sql} relativePath LIKE ?;",
-                                    (relative_path.replace("*", "%"),))
+                        cur.execute(
+                            f"{base_sql} relativePath LIKE ?;",
+                            (relative_path.replace("*", "%"),),
+                        )
                     else:
-                        cur.execute(f"{base_sql} relativePath = ?;",
-                                    (relative_path,))
+                        cur.execute(f"{base_sql} relativePath = ?;", (relative_path,))
                 elif domain:
                     cur.execute(f"{base_sql} domain = ?;", (domain,))
         except Exception as exc:
             raise DatabaseCorruptedError(f"failed to query Manifest.db: {exc}") from exc
 
         for row in cur:
             yield {
@@ -129,25 +142,22 @@
         if os.path.exists(file_path):
             return file_path
 
         return None
 
     def _get_fs_files_from_patterns(self, root_paths: list) -> Iterator[str]:
         for root_path in root_paths:
-            for found_path in glob.glob(os.path.join(self.target_path,
-                                                     root_path)):
+            for found_path in glob.glob(os.path.join(self.target_path, root_path)):
                 if not os.path.exists(found_path):
                     continue
 
                 yield found_path
 
     def _find_ios_database(
-        self,
-        backup_ids: Optional[list] = None,
-        root_paths: Optional[list] = None
+        self, backup_ids: Optional[list] = None, root_paths: Optional[list] = None
     ) -> None:
         """Try to locate a module's database file from either an iTunes
         backup or a full filesystem dump. This is intended only for
         modules that expect to work with a single SQLite database.
         If a module requires to process multiple databases or files,
         you should use the helper functions above.
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/__init__.py` & `mvt-2.3.0/mvt/ios/modules/fs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,20 @@
 from .safari_favicon import SafariFavicon
 from .shutdownlog import ShutdownLog
 from .version_history import IOSVersionHistory
 from .webkit_indexeddb import WebkitIndexedDB
 from .webkit_localstorage import WebkitLocalStorage
 from .webkit_safariviewservice import WebkitSafariViewService
 
-FS_MODULES = [CacheFiles, Filesystem, Netusage, Analytics, AnalyticsIOSVersions,
-              SafariFavicon, ShutdownLog, IOSVersionHistory, WebkitIndexedDB,
-              WebkitLocalStorage, WebkitSafariViewService]
+FS_MODULES = [
+    CacheFiles,
+    Filesystem,
+    Netusage,
+    Analytics,
+    AnalyticsIOSVersions,
+    SafariFavicon,
+    ShutdownLog,
+    IOSVersionHistory,
+    WebkitIndexedDB,
+    WebkitLocalStorage,
+    WebkitSafariViewService,
+]
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/analytics.py` & `mvt-2.3.0/mvt/ios/modules/fs/analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,26 @@
     private/var/Keychains/Analytics/*.db files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": record["artifact"],
             "data": f"{record}",
@@ -50,66 +55,76 @@
         for result in self.results:
             for value in result.values():
                 if not isinstance(value, str):
                     continue
 
                 ioc = self.indicators.check_process(value)
                 if ioc:
-                    self.log.warning("Found mention of a malicious process \"%s\" in %s file at %s",
-                                     value, result["artifact"],
-                                     result["isodate"])
+                    self.log.warning(
+                        'Found mention of a malicious process "%s" in %s file at %s',
+                        value,
+                        result["artifact"],
+                        result["isodate"],
+                    )
                     new_result = copy.copy(result)
                     new_result["matched_indicator"] = ioc
                     self.detected.append(new_result)
                     continue
 
                 ioc = self.indicators.check_domain(value)
                 if ioc:
-                    self.log.warning("Found mention of a malicious domain \"%s\" in %s file at %s",
-                                     value, result["artifact"],
-                                     result["isodate"])
+                    self.log.warning(
+                        'Found mention of a malicious domain "%s" in %s file at %s',
+                        value,
+                        result["artifact"],
+                        result["isodate"],
+                    )
                     new_result = copy.copy(result)
                     new_result["matched_indicator"] = ioc
                     self.detected.append(new_result)
 
     def _extract_analytics_data(self):
         artifact = self.file_path.split("/")[-1]
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
 
         try:
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     timestamp,
                     data
                 FROM hard_failures
                 UNION
                 SELECT
                     timestamp,
                     data
                 FROM soft_failures
                 UNION
                 SELECT
                     timestamp,
                     data
                 FROM all_events;
-            """)
+            """
+            )
         except sqlite3.OperationalError:
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     timestamp,
                     data
                 FROM hard_failures
                 UNION
                 SELECT
                     timestamp,
                     data
                 FROM soft_failures;
-            """)
+            """
+            )
 
         for row in cur:
             if row[0] and row[1]:
                 isodate = convert_mactime_to_iso(row[0], False)
                 data = plistlib.loads(row[1])
                 data["isodate"] = isodate
             elif row[0]:
@@ -127,18 +142,18 @@
 
         cur.close()
         conn.close()
 
     def process_analytics_dbs(self):
         for file_path in self._get_fs_files_from_patterns(ANALYTICS_DB_PATH):
             self.file_path = file_path
-            self.log.info("Found Analytics database file at path: %s",
-                          file_path)
+            self.log.info("Found Analytics database file at path: %s", file_path)
             self._extract_analytics_data()
 
     def run(self) -> None:
         self.process_analytics_dbs()
 
-        self.log.info("Extracted %d records from analytics databases",
-                      len(self.results))
+        self.log.info(
+            "Extracted %d records from analytics databases", len(self.results)
+        )
 
         self.results = sorted(self.results, key=lambda entry: entry["isodate"])
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.3.0/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,21 +19,26 @@
     files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "analytics_ios_version",
             "data": f"Seen iOS version {record['version']} ({record['build']})",
@@ -64,17 +69,23 @@
 
             if result_dt < cur_dt:
                 builds[build] = isodate
 
         for build, isodate in builds.items():
             version = find_version_by_build(build)
 
-            self.results.append({
-                "isodate": isodate,
-                "build": build,
-                "version": version,
-            })
+            self.results.append(
+                {
+                    "isodate": isodate,
+                    "build": build,
+                    "version": version,
+                }
+            )
 
         self.results = sorted(self.results, key=lambda entry: entry["isodate"])
         for result in self.results:
-            self.log.info("iOS version %s (%s) first appeared on %s",
-                          result["version"], result["build"], result["isodate"])
+            self.log.info(
+                "iOS version %s (%s) first appeared on %s",
+                result["version"],
+                result["build"],
+                result["isodate"],
+            )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/cache_files.py` & `mvt-2.3.0/mvt/ios/modules/fs/cache_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,52 +8,60 @@
 import sqlite3
 from typing import Optional, Union
 
 from ..base import IOSExtraction
 
 
 class CacheFiles(IOSExtraction):
-
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for item in self.results[record]:
-            records.append({
-                "timestamp": item["isodate"],
-                "module": self.__class__.__name__,
-                "event": "cache_response",
-                "data": f"{record} recorded visit to URL {item['url']}"
-            })
+            records.append(
+                {
+                    "timestamp": item["isodate"],
+                    "module": self.__class__.__name__,
+                    "event": "cache_response",
+                    "data": f"{record} recorded visit to URL {item['url']}",
+                }
+            )
 
         return records
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         self.detected = {}
         for key, values in self.results.items():
             for value in values:
                 ioc = self.indicators.check_domain(value["url"])
                 if ioc:
                     value["matched_indicator"] = ioc
                     if key not in self.detected:
-                        self.detected[key] = [value, ]
+                        self.detected[key] = [
+                            value,
+                        ]
                     else:
                         self.detected[key].append(value)
 
     def _process_cache_file(self, file_path):
         self.log.info("Processing cache file at path: %s", file_path)
 
         conn = sqlite3.connect(file_path)
@@ -65,22 +73,24 @@
             return
 
         key_name = os.path.relpath(file_path, self.target_path)
         if key_name not in self.results:
             self.results[key_name] = []
 
         for row in cur:
-            self.results[key_name].append({
-                "entry_id": row[0],
-                "version": row[1],
-                "hash_value": row[2],
-                "storage_policy": row[3],
-                "url": row[4],
-                "isodate": row[5],
-            })
+            self.results[key_name].append(
+                {
+                    "entry_id": row[0],
+                    "version": row[1],
+                    "hash_value": row[2],
+                    "storage_policy": row[3],
+                    "url": row[4],
+                    "isodate": row[5],
+                }
+            )
 
     def run(self) -> None:
         self.results = {}
         for root, _, files in os.walk(self.target_path):
             for file_name in files:
                 if file_name != "Cache.db":
                     continue
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/filesystem.py` & `mvt-2.3.0/mvt/ios/modules/fs/filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,26 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["modified"],
             "module": self.__class__.__name__,
             "event": "entry_modified",
             "data": record["path"],
@@ -63,27 +68,25 @@
     def run(self) -> None:
         for root, dirs, files in os.walk(self.target_path):
             for dir_name in dirs:
                 try:
                     dir_path = os.path.join(root, dir_name)
                     result = {
                         "path": os.path.relpath(dir_path, self.target_path),
-                        "modified": convert_unix_to_iso(
-                            os.stat(dir_path).st_mtime),
+                        "modified": convert_unix_to_iso(os.stat(dir_path).st_mtime),
                     }
                 except Exception:
                     continue
                 else:
                     self.results.append(result)
 
             for file_name in files:
                 try:
                     file_path = os.path.join(root, file_name)
                     result = {
                         "path": os.path.relpath(file_path, self.target_path),
-                        "modified": convert_unix_to_iso(
-                            os.stat(file_path).st_mtime),
+                        "modified": convert_unix_to_iso(os.stat(file_path).st_mtime),
                     }
                 except Exception:
                     continue
                 else:
                     self.results.append(result)
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.3.0/mvt/ios/modules/fs/net_netusage.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sqlite3
 from typing import Optional
 
 from ..net_base import NetBase
 
 NETUSAGE_ROOT_PATHS = [
     "private/var/networkd/netusage.sqlite",
-    "private/var/networkd/db/netusage.sqlite"
+    "private/var/networkd/db/netusage.sqlite",
 ]
 
 
 class Netusage(NetBase):
     """This class extracts data from netusage.sqlite and attempts to identify
     any suspicious processes if running on a full filesystem dump.
 
@@ -23,27 +23,35 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
         for netusage_path in self._get_fs_files_from_patterns(NETUSAGE_ROOT_PATHS):
             self.file_path = netusage_path
             self.log.info("Found NetUsage database at path: %s", self.file_path)
             try:
                 self._extract_net_data()
             except sqlite3.OperationalError as exc:
-                self.log.info("Skipping this NetUsage database because "
-                              "it seems empty or malformed: %s", exc)
+                self.log.info(
+                    "Skipping this NetUsage database because "
+                    "it seems empty or malformed: %s",
+                    exc,
+                )
                 continue
 
         self._find_suspicious_processes()
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.3.0/mvt/ios/modules/fs/safari_favicon.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,34 @@
     """This module extracts all Safari favicon records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "safari_favicon",
             "data": f"Safari favicon from {record['url']} with icon URL "
-                    f"{record['icon_url']} ({record['type']})",
+            f"{record['icon_url']} ({record['type']})",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -56,59 +61,65 @@
                 self.detected.append(result)
 
     def _process_favicon_db(self, file_path):
         conn = sqlite3.connect(file_path)
 
         # Fetch valid icon cache.
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 page_url.url,
                 icon_info.url,
                 icon_info.timestamp
             FROM page_url
             JOIN icon_info ON page_url.uuid = icon_info.uuid
             ORDER BY icon_info.timestamp;
-        """)
+        """
+        )
 
         for row in cur:
-            self.results.append({
-                "url": row[0],
-                "icon_url": row[1],
-                "timestamp": row[2],
-                "isodate": convert_mactime_to_iso(row[2]),
-                "type": "valid",
-                "safari_favicon_db_path": file_path,
-            })
+            self.results.append(
+                {
+                    "url": row[0],
+                    "icon_url": row[1],
+                    "timestamp": row[2],
+                    "isodate": convert_mactime_to_iso(row[2]),
+                    "type": "valid",
+                    "safari_favicon_db_path": file_path,
+                }
+            )
 
         # Fetch icons from the rejected icons table.
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 page_url,
                 icon_url,
                 timestamp
             FROM rejected_resources ORDER BY timestamp;
-        """)
+        """
+        )
 
         for row in cur:
-            self.results.append({
-                "url": row[0],
-                "icon_url": row[1],
-                "timestamp": row[2],
-                "isodate": convert_mactime_to_iso(row[2]),
-                "type": "rejected",
-                "safari_favicon_db_path": file_path,
-            })
+            self.results.append(
+                {
+                    "url": row[0],
+                    "icon_url": row[1],
+                    "timestamp": row[2],
+                    "isodate": convert_mactime_to_iso(row[2]),
+                    "type": "rejected",
+                    "safari_favicon_db_path": file_path,
+                }
+            )
 
         cur.close()
         conn.close()
 
     def run(self) -> None:
         for file_path in self._get_fs_files_from_patterns(SAFARI_FAVICON_ROOT_PATHS):
-            self.log.info("Found Safari favicon cache database at path: %s",
-                          file_path)
+            self.log.info("Found Safari favicon cache database at path: %s", file_path)
             self._process_favicon_db(file_path)
 
-        self.log.info("Extracted a total of %d favicon records",
-                      len(self.results))
+        self.log.info("Extracted a total of %d favicon records", len(self.results))
 
         self.results = sorted(self.results, key=lambda x: x["isodate"])
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.3.0/mvt/ios/modules/fs/shutdownlog.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,29 +19,34 @@
     """This module extracts processes information from the shutdown log file."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "shutdown",
             "data": f"Client {record['client']} with PID {record['pid']} "
-                     "was running when the device was shut down",
+            "was running when the device was shut down",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -50,48 +55,55 @@
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
                 continue
 
             for ioc in self.indicators.get_iocs("processes"):
                 parts = result["client"].split("/")
                 if ioc in parts:
-                    self.log.warning("Found mention of a known malicious process \"%s\" in "
-                                     "shutdown.log", ioc)
+                    self.log.warning(
+                        'Found mention of a known malicious process "%s" in '
+                        "shutdown.log",
+                        ioc,
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
     def process_shutdownlog(self, content):
         current_processes = []
         for line in content.split("\n"):
             line = line.strip()
 
             if line.startswith("remaining client pid:"):
-                current_processes.append({
-                    "pid": line[line.find("pid: ")+5:line.find(" (")],
-                    "client": line[line.find("(")+1:line.find(")")],
-                })
+                current_processes.append(
+                    {
+                        "pid": line[line.find("pid: ") + 5 : line.find(" (")],
+                        "client": line[line.find("(") + 1 : line.find(")")],
+                    }
+                )
             elif line.startswith("SIGTERM: "):
                 try:
-                    mac_timestamp = int(line[line.find("[")+1:line.find("]")])
+                    mac_timestamp = int(line[line.find("[") + 1 : line.find("]")])
                 except ValueError:
                     try:
                         start = line.find(" @") + 2
-                        mac_timestamp = int(line[start:start+10])
+                        mac_timestamp = int(line[start : start + 10])
                     except Exception:
                         mac_timestamp = 0
 
                 isodate = convert_mactime_to_iso(mac_timestamp, from_2001=False)
 
                 for current_process in current_processes:
-                    self.results.append({
-                        "isodate": isodate,
-                        "pid": current_process["pid"],
-                        "client": current_process["client"],
-                    })
+                    self.results.append(
+                        {
+                            "isodate": isodate,
+                            "pid": current_process["pid"],
+                            "client": current_process["client"],
+                        }
+                    )
 
                 current_processes = []
 
         self.results = sorted(self.results, key=lambda entry: entry["isodate"])
 
     def run(self) -> None:
         self._find_ios_database(root_paths=SHUTDOWN_LOG_PATH)
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/version_history.py` & `mvt-2.3.0/mvt/ios/modules/fs/version_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,37 +21,45 @@
     """This module extracts iOS update history from Analytics Journal log files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "ios_version",
             "data": f"Recorded iOS version {record['os_version']}",
         }
 
     def run(self) -> None:
         for found_path in self._get_fs_files_from_patterns(IOS_ANALYTICS_JOURNAL_PATHS):
             with open(found_path, "r", encoding="utf-8") as analytics_log:
                 log_line = json.loads(analytics_log.readline().strip())
 
-                timestamp = datetime.datetime.strptime(log_line["timestamp"],
-                                                       "%Y-%m-%d %H:%M:%S.%f %z")
+                timestamp = datetime.datetime.strptime(
+                    log_line["timestamp"], "%Y-%m-%d %H:%M:%S.%f %z"
+                )
                 timestamp_utc = timestamp.astimezone(datetime.timezone.utc)
-                self.results.append({
-                    "isodate": convert_datetime_to_iso(timestamp_utc),
-                    "os_version": log_line["os_version"],
-                })
+                self.results.append(
+                    {
+                        "isodate": convert_datetime_to_iso(timestamp_utc),
+                        "os_version": log_line["os_version"],
+                    }
+                )
 
         self.results = sorted(self.results, key=lambda entry: entry["isodate"])
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.3.0/mvt/ios/modules/fs/webkit_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,12 +31,14 @@
                 if not name.startswith("http"):
                     continue
 
                 name = name.replace("http_", "http://")
                 name = name.replace("https_", "https://")
                 url = name.split("_")[0]
 
-                self.results.append({
-                    "folder": key,
-                    "url": url,
-                    "isodate": convert_unix_to_iso(os.stat(found_path).st_mtime),
-                })
+                self.results.append(
+                    {
+                        "folder": key,
+                        "url": url,
+                        "isodate": convert_unix_to_iso(os.stat(found_path).st_mtime),
+                    }
+                )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.3.0/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,28 +23,34 @@
     slug = "webkit_indexeddb"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "webkit_indexeddb",
             "data": f"IndexedDB folder {record['folder']} containing "
-                    f"file for URL {record['url']}",
+            f"file for URL {record['url']}",
         }
 
     def run(self) -> None:
         self._process_webkit_folder(WEBKIT_INDEXEDDB_ROOT_PATHS)
-        self.log.info("Extracted a total of %d WebKit IndexedDB records",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d WebKit IndexedDB records", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.3.0/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,28 +21,35 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "webkit_local_storage",
             "data": f"WebKit Local Storage folder {record['folder']} "
-                    f"containing file for URL {record['url']}",
+            f"containing file for URL {record['url']}",
         }
 
     def run(self) -> None:
         self._process_webkit_folder(WEBKIT_LOCALSTORAGE_ROOT_PATHS)
-        self.log.info("Extracted a total of %d records from WebKit Local Storages",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d records from WebKit Local Storages",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.3.0/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,26 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
         self._process_webkit_folder(WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS)
-        self.log.info("Extracted a total of %d records from WebKit SafariViewService WebsiteData",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d records from WebKit SafariViewService WebsiteData",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/__init__.py` & `mvt-2.3.0/mvt/ios/modules/mixed/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,13 +22,31 @@
 from .sms import SMS
 from .sms_attachments import SMSAttachments
 from .tcc import TCC
 from .webkit_resource_load_statistics import WebkitResourceLoadStatistics
 from .webkit_session_resource_log import WebkitSessionResourceLog
 from .whatsapp import Whatsapp
 
-MIXED_MODULES = [Calls, ChromeFavicon, ChromeHistory, Contacts, FirefoxFavicon,
-                 FirefoxHistory, IDStatusCache, InteractionC, LocationdClients,
-                 OSAnalyticsADDaily, Datausage, SafariBrowserState, SafariHistory,
-                 TCC, SMS, SMSAttachments, WebkitResourceLoadStatistics,
-                 WebkitSessionResourceLog, Whatsapp, Shortcuts, Applications,
-                 Calendar]
+MIXED_MODULES = [
+    Calls,
+    ChromeFavicon,
+    ChromeHistory,
+    Contacts,
+    FirefoxFavicon,
+    FirefoxHistory,
+    IDStatusCache,
+    InteractionC,
+    LocationdClients,
+    OSAnalyticsADDaily,
+    Datausage,
+    SafariBrowserState,
+    SafariHistory,
+    TCC,
+    SMS,
+    SMSAttachments,
+    WebkitResourceLoadStatistics,
+    WebkitSessionResourceLog,
+    Whatsapp,
+    Shortcuts,
+    Applications,
+    Calendar,
+]
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/applications.py` & `mvt-2.3.0/mvt/ios/modules/mixed/applications.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,66 +17,95 @@
 APPLICATIONS_DB_PATH = [
     "private/var/containers/Bundle/Application/*/iTunesMetadata.plist"
 ]
 
 
 class Applications(IOSExtraction):
     """Extract information from accounts installed on the phone."""
+
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if "isodate" in record:
             return {
                 "timestamp": record["isodate"],
                 "module": self.__class__.__name__,
                 "event": "app_installed",
-                "data": f"App {record.get('name', '')} version {record.get('bundleShortVersionString', '')} from {record.get('artistName', '')} installed from {record.get('sourceApp', '')}"
+                "data": f"App {record.get('name', '')} version {record.get('bundleShortVersionString', '')} from {record.get('artistName', '')} installed from {record.get('sourceApp', '')}",
             }
         return []
 
     def check_indicators(self) -> None:
         for result in self.results:
             if self.indicators:
+                if "softwareVersionBundleId" not in result:
+                    self.log.warning(
+                        "Suspicious application identified without softwareVersionBundleId"
+                    )
+                    self.detected.append(result)
+                    continue
+
                 ioc = self.indicators.check_process(result["softwareVersionBundleId"])
                 if ioc:
-                    self.log.warning("Malicious application %s identified", result["softwareVersionBundleId"])
+                    self.log.warning(
+                        "Malicious application %s identified",
+                        result["softwareVersionBundleId"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
                 ioc = self.indicators.check_app_id(result["softwareVersionBundleId"])
                 if ioc:
-                    self.log.warning("Malicious application %s identified", result["softwareVersionBundleId"])
+                    self.log.warning(
+                        "Malicious application %s identified",
+                        result["softwareVersionBundleId"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
-            if result.get("sourceApp", "com.apple.AppStore") not in ["com.apple.AppStore", "com.apple.dmd", "dmd"]:
-                self.log.warning("Suspicious app not installed from the App Store or MDM: %s", result["softwareVersionBundleId"])
+            if result.get("sourceApp", "com.apple.AppStore") not in [
+                "com.apple.AppStore",
+                "com.apple.dmd",
+                "dmd",
+            ]:
+                self.log.warning(
+                    "Suspicious app not installed from the App Store or MDM: %s",
+                    result["softwareVersionBundleId"],
+                )
                 self.detected.append(result)
 
     def _parse_itunes_timestamp(self, entry: Dict[str, Any]) -> None:
         """
         Parse the iTunes metadata info
         """
-        if entry.get("com.apple.iTunesStore.downloadInfo", {}).get("purchaseDate", None):
+        if entry.get("com.apple.iTunesStore.downloadInfo", {}).get(
+            "purchaseDate", None
+        ):
             timestamp = datetime.strptime(
                 entry["com.apple.iTunesStore.downloadInfo"]["purchaseDate"],
-                "%Y-%m-%dT%H:%M:%SZ")
+                "%Y-%m-%dT%H:%M:%SZ",
+            )
             timestamp_utc = timestamp.astimezone(timezone.utc)
             entry["isodate"] = convert_datetime_to_iso(timestamp_utc)
 
     def _parse_itunes_metadata(self, plist_path: str) -> None:
         """
         Parse iTunesMetadata.plist file from an application in fs dump
         """
@@ -115,9 +144,8 @@
             if not os.path.isfile(plist_path):
                 raise DatabaseNotFoundError("Impossible to find Info.plist file")
             self._parse_info_plist(plist_path)
         elif self.is_fs_dump:
             for file_path in self._get_fs_files_from_patterns(APPLICATIONS_DB_PATH):
                 self._parse_itunes_metadata(file_path)
 
-        self.log.info("Extracted a total of %d applications",
-                      len(self.results))
+        self.log.info("Extracted a total of %d applications", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/calendar.py` & `mvt-2.3.0/mvt/ios/modules/mixed/calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,79 +10,87 @@
 from mvt.common.utils import convert_mactime_to_iso
 
 from ..base import IOSExtraction
 
 CALENDAR_BACKUP_IDS = [
     "2041457d5fe04d39d0ab481178355df6781e6858",
 ]
-CALENDAR_ROOT_PATHS = [
-    "private/var/mobile/Library/Calendar/Calendar.sqlitedb"
-]
+CALENDAR_ROOT_PATHS = ["private/var/mobile/Library/Calendar/Calendar.sqlitedb"]
 
 
 class Calendar(IOSExtraction):
     """This module extracts all calendar entries."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
         self.timestamps = [
             "start_date",
             "end_date",
             "last_modified",
             "creation_date",
-            "participant_last_modified"
+            "participant_last_modified",
         ]
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for timestamp in self.timestamps:
             if timestamp not in record or not record[timestamp]:
                 continue
 
-            records.append({
-                "timestamp": record[timestamp],
-                "module": self.__class__.__name__,
-                "event": timestamp,
-                "data": f"Calendar event {record['summary']} ({record['description']}) "
-                        f"(invitation by {record['participant_email']})"
-            })
+            records.append(
+                {
+                    "timestamp": record[timestamp],
+                    "module": self.__class__.__name__,
+                    "event": timestamp,
+                    "data": f"Calendar event {record['summary']} ({record['description']}) "
+                    f"(invitation by {record['participant_email']})",
+                }
+            )
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if result["participant_email"] and self.indicators:
                 ioc = self.indicators.check_email(result["participant_email"])
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
-            # Custom check for Quadream exploit
+            # Custom check for Quadream exploit
             if result["summary"] == "Meeting" and result["description"] == "Notes":
-                self.log.warning("Potential Quadream exploit event identified: %s", result["uuid"])
+                self.log.warning(
+                    "Potential Quadream exploit event identified: %s", result["uuid"]
+                )
                 self.detected.append(result)
 
     def _parse_calendar_db(self):
         """
         Parse the calendar database
         """
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
 
-        cur.execute("""
+        cur.execute(
+            """
         SELECT
             CalendarItem.ROWID as "id",
             CalendarItem.summary as "summary",
             CalendarItem.description as "description",
             CalendarItem.start_date as "start_date",
             CalendarItem.end_date as "end_date",
             CalendarItem.all_day as "all_day",
@@ -101,15 +109,16 @@
             Participant.UUID as "participant_uuid",
             Participant.email as "participant_email",
             Participant.phone_number as "participant_phone",
             Participant.comment as "participant_comment",
             Participant.last_modified as "participant_last_modified"
         FROM CalendarItem
             LEFT JOIN Participant ON Participant.ROWID = CalendarItem.organizer_id;
-        """)
+        """
+        )
 
         names = [description[0] for description in cur.description]
         for item in cur:
             entry = {}
             for index, value in enumerate(item):
                 if names[index] in self.timestamps:
                     if value is None or isinstance(value, str):
@@ -121,16 +130,15 @@
 
             self.results.append(entry)
 
         cur.close()
         conn.close()
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=CALENDAR_BACKUP_IDS,
-                                root_paths=CALENDAR_ROOT_PATHS)
-        self.log.info("Found calendar database at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=CALENDAR_BACKUP_IDS, root_paths=CALENDAR_ROOT_PATHS
+        )
+        self.log.info("Found calendar database at path: %s", self.file_path)
 
         self._parse_calendar_db()
 
-        self.log.info("Extracted a total of %d calendar items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d calendar items", len(self.results))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/calls.py` & `mvt-2.3.0/mvt/ios/modules/mixed/calls.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,59 +10,74 @@
 from mvt.common.utils import convert_mactime_to_iso
 
 from ..base import IOSExtraction
 
 CALLS_BACKUP_IDS = [
     "5a4935c78a5255723f707230a451d79c540d2741",
 ]
-CALLS_ROOT_PATHS = [
-    "private/var/mobile/Library/CallHistoryDB/CallHistory.storedata"
-]
+CALLS_ROOT_PATHS = ["private/var/mobile/Library/CallHistoryDB/CallHistory.storedata"]
 
 
 class Calls(IOSExtraction):
     """This module extracts phone calls details"""
 
-    def __init__(self, file_path: str = None, target_path: str = None,
-                 results_path: str = None, fast_mode: bool = False,
-                 log: logging.Logger = logging.getLogger(__name__),
-                 results: list = []) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+    def __init__(
+        self,
+        file_path: str = None,
+        target_path: str = None,
+        results_path: str = None,
+        fast_mode: bool = False,
+        log: logging.Logger = logging.getLogger(__name__),
+        results: list = [],
+    ) -> None:
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "call",
             "data": f"From {record['number']} using {record['provider']} "
-                    f"during {record['duration']} seconds"
+            f"during {record['duration']} seconds",
         }
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=CALLS_BACKUP_IDS,
-                                root_paths=CALLS_ROOT_PATHS)
+        self._find_ios_database(
+            backup_ids=CALLS_BACKUP_IDS, root_paths=CALLS_ROOT_PATHS
+        )
         self.log.info("Found Calls database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 ZDATE, ZDURATION, ZLOCATION, ZADDRESS, ZSERVICE_PROVIDER
             FROM ZCALLRECORD;
-        """)
+        """
+        )
         # names = [description[0] for description in cur.description]
 
         for row in cur:
-            self.results.append({
-                "isodate": convert_mactime_to_iso(row[0]),
-                "duration": row[1],
-                "location": row[2],
-                "number": row[3].decode("utf-8") if row[3] and row[3] is bytes else row[3],
-                "provider": row[4]
-            })
+            self.results.append(
+                {
+                    "isodate": convert_mactime_to_iso(row[0]),
+                    "duration": row[1],
+                    "location": row[2],
+                    "number": row[3].decode("utf-8")
+                    if row[3] and row[3] is bytes
+                    else row[3],
+                    "provider": row[4],
+                }
+            )
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d calls", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.3.0/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import sqlite3
 from typing import Optional, Union
 
-from mvt.common.utils import (convert_chrometime_to_datetime,
-                              convert_datetime_to_iso)
+from mvt.common.utils import convert_chrometime_to_datetime, convert_datetime_to_iso
 
 from ..base import IOSExtraction
 
-CHROME_FAVICON_BACKUP_IDS = [
-    "55680ab883d0fdcffd94f959b1632e5fbbb18c5b"
-]
+CHROME_FAVICON_BACKUP_IDS = ["55680ab883d0fdcffd94f959b1632e5fbbb18c5b"]
 # TODO: Confirm Chrome database path.
 CHROME_FAVICON_ROOT_PATHS = [
     "private/var/mobile/Containers/Data/Application/*/Library/Application Support/Google/Chrome/Default/Favicons",
 ]
 
 
 class ChromeFavicon(IOSExtraction):
     """This module extracts all Chrome favicon records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "new_favicon",
-            "data": f"{record['icon_url']} from {record['url']}"
+            "data": f"{record['icon_url']} from {record['url']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -55,44 +57,49 @@
                 ioc = self.indicators.check_domain(result["icon_url"])
 
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=CHROME_FAVICON_BACKUP_IDS,
-                                root_paths=CHROME_FAVICON_ROOT_PATHS)
-        self.log.info("Found Chrome favicon cache database at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=CHROME_FAVICON_BACKUP_IDS, root_paths=CHROME_FAVICON_ROOT_PATHS
+        )
+        self.log.info("Found Chrome favicon cache database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
 
         # Fetch icon cache
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 icon_mapping.page_url,
                 favicons.url,
                 favicon_bitmaps.last_updated,
                 favicon_bitmaps.last_requested
             FROM icon_mapping
             JOIN favicon_bitmaps ON icon_mapping.icon_id = favicon_bitmaps.icon_id
             JOIN favicons ON icon_mapping.icon_id = favicons.id
             ORDER BY icon_mapping.id;
-        """)
+        """
+        )
 
         records = []
         for row in cur:
             last_timestamp = int(row[2]) or int(row[3])
-            records.append({
-                "url": row[0],
-                "icon_url": row[1],
-                "timestamp": last_timestamp,
-                "isodate": convert_datetime_to_iso(
-                    convert_chrometime_to_datetime(last_timestamp)),
-            })
+            records.append(
+                {
+                    "url": row[0],
+                    "icon_url": row[1],
+                    "timestamp": last_timestamp,
+                    "isodate": convert_datetime_to_iso(
+                        convert_chrometime_to_datetime(last_timestamp)
+                    ),
+                }
+            )
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d favicon records", len(records))
         self.results = sorted(records, key=lambda row: row["isodate"])
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.3.0/mvt/ios/modules/mixed/chrome_history.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import sqlite3
 from typing import Optional, Union
 
-from mvt.common.utils import (convert_chrometime_to_datetime,
-                              convert_datetime_to_iso)
+from mvt.common.utils import convert_chrometime_to_datetime, convert_datetime_to_iso
 
 from ..base import IOSExtraction
 
 CHROME_HISTORY_BACKUP_IDS = [
     "faf971ce92c3ac508c018dce1bef2a8b8e9838f1",
 ]
 # TODO: Confirm Chrome database path.
@@ -25,71 +24,80 @@
     """This module extracts all Chome visits."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "visit",
             "data": f"{record['id']} - {record['url']} "
-                    f"(visit ID: {record['visit_id']}, "
-                    f"redirect source: {record['redirect_source']})"
+            f"(visit ID: {record['visit_id']}, "
+            f"redirect source: {record['redirect_source']})",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_domain(result["url"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=CHROME_HISTORY_BACKUP_IDS,
-                                root_paths=CHROME_HISTORY_ROOT_PATHS)
-        self.log.info("Found Chrome history database at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=CHROME_HISTORY_BACKUP_IDS, root_paths=CHROME_HISTORY_ROOT_PATHS
+        )
+        self.log.info("Found Chrome history database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 urls.id,
                 urls.url,
                 visits.id,
                 visits.visit_time,
                 visits.from_visit
             FROM urls
             JOIN visits ON visits.url = urls.id
             ORDER BY visits.visit_time;
-        """)
+        """
+        )
 
         for item in cur:
-            self.results.append({
-                "id": item[0],
-                "url": item[1],
-                "visit_id": item[2],
-                "timestamp": item[3],
-                "isodate": convert_datetime_to_iso(
-                    convert_chrometime_to_datetime(item[3])),
-                "redirect_source": item[4],
-            })
+            self.results.append(
+                {
+                    "id": item[0],
+                    "url": item[1],
+                    "visit_id": item[2],
+                    "timestamp": item[3],
+                    "isodate": convert_datetime_to_iso(
+                        convert_chrometime_to_datetime(item[3])
+                    ),
+                    "redirect_source": item[4],
+                }
+            )
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d history items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.3.0/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,29 +23,34 @@
     """This module extracts all Firefox favicon"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "firefox_history",
             "data": f"Firefox favicon {record['url']} "
-                    f"when visiting {record['history_url']}",
+            f"when visiting {record['history_url']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -54,46 +59,49 @@
                 ioc = self.indicators.check_domain(result.get("history_url", ""))
 
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=FIREFOX_HISTORY_BACKUP_IDS,
-                                root_paths=FIREFOX_HISTORY_ROOT_PATHS)
-        self.log.info("Found Firefox favicon database at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=FIREFOX_HISTORY_BACKUP_IDS, root_paths=FIREFOX_HISTORY_ROOT_PATHS
+        )
+        self.log.info("Found Firefox favicon database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 favicons.id,
                 favicons.url,
                 favicons.width,
                 favicons.height,
                 favicons.type,
                 favicons.date,
                 history.id,
                 history.url
             FROM favicons
             INNER JOIN favicon_sites ON favicon_sites.faviconID = favicons.id
             INNER JOIN history ON favicon_sites.siteID = history.id;
-        """)
+        """
+        )
 
         for item in cur:
-            self.results.append({
-                "id": item[0],
-                "url": item[1],
-                "width": item[2],
-                "height": item[3],
-                "type": item[4],
-                "isodate": convert_unix_to_iso(item[5]),
-                "history_id": item[6],
-                "history_url": item[7]
-            })
+            self.results.append(
+                {
+                    "id": item[0],
+                    "url": item[1],
+                    "width": item[2],
+                    "height": item[3],
+                    "type": item[4],
+                    "isodate": convert_unix_to_iso(item[5]),
+                    "history_id": item[6],
+                    "history_url": item[7],
+                }
+            )
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d history items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.3.0/mvt/ios/modules/mixed/firefox_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,21 +27,26 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "firefox_history",
             "data": f"Firefox visit with ID {record['id']} to URL: {record['url']}",
@@ -54,41 +59,44 @@
         for result in self.results:
             ioc = self.indicators.check_domain(result["url"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=FIREFOX_HISTORY_BACKUP_IDS,
-                                root_paths=FIREFOX_HISTORY_ROOT_PATHS)
-        self.log.info("Found Firefox history database at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=FIREFOX_HISTORY_BACKUP_IDS, root_paths=FIREFOX_HISTORY_ROOT_PATHS
+        )
+        self.log.info("Found Firefox history database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 visits.id,
                 visits.date/1000000,
                 history.url,
                 history.title,
                 visits.is_local,
                 visits.type
             FROM visits, history
             WHERE visits.siteID = history.id;
-        """)
+        """
+        )
 
         for row in cur:
-            self.results.append({
-                "id": row[0],
-                "isodate": convert_unix_to_iso(row[1]),
-                "url": row[2],
-                "title": row[3],
-                "i1000000s_local": row[4],
-                "type": row[5]
-            })
+            self.results.append(
+                {
+                    "id": row[0],
+                    "isodate": convert_unix_to_iso(row[1]),
+                    "url": row[2],
+                    "title": row[3],
+                    "i1000000s_local": row[4],
+                    "type": row[5],
+                }
+            )
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d history items",
-                      len(self.results))
+        self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.3.0/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,34 @@
     """Extracts Apple Authentication information from idstatuscache.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "lookup",
             "data": f"Lookup of {record['user']} within {record['package']} "
-                    f"(Status {record['idstatus']})"
+            f"(Status {record['idstatus']})",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -56,16 +61,18 @@
                 ioc = self.indicators.check_email(email)
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             if "\\x00\\x00" in result.get("user", ""):
-                self.log.warning("Found an ID Status Cache entry with suspicious patterns: %s",
-                                 result.get("user"))
+                self.log.warning(
+                    "Found an ID Status Cache entry with suspicious patterns: %s",
+                    result.get("user"),
+                )
                 self.detected.append(result)
 
     def _extract_idstatuscache_entries(self, file_path):
         with open(file_path, "rb") as handle:
             file_plist = plistlib.load(handle)
 
         id_status_cache_entries = []
@@ -76,39 +83,40 @@
             for entry in file_plist[app]:
                 try:
                     lookup_date = file_plist[app][entry]["LookupDate"]
                     id_status = file_plist[app][entry]["IDStatus"]
                 except KeyError:
                     continue
 
-                id_status_cache_entries.append({
-                    "package": app,
-                    "user": entry.replace("\x00", "\\x00"),
-                    "isodate": convert_mactime_to_iso(lookup_date),
-                    "idstatus": id_status,
-                })
-
-        entry_counter = collections.Counter([entry["user"]
-                                                for entry in
-                                                    id_status_cache_entries])
+                id_status_cache_entries.append(
+                    {
+                        "package": app,
+                        "user": entry.replace("\x00", "\\x00"),
+                        "isodate": convert_mactime_to_iso(lookup_date),
+                        "idstatus": id_status,
+                    }
+                )
+
+        entry_counter = collections.Counter(
+            [entry["user"] for entry in id_status_cache_entries]
+        )
         for entry in id_status_cache_entries:
             # Add total count of occurrences to the status cache entry.
             entry["occurrences"] = entry_counter[entry["user"]]
             self.results.append(entry)
 
     def run(self) -> None:
-
         if self.is_backup:
             self._find_ios_database(backup_ids=IDSTATUSCACHE_BACKUP_IDS)
-            self.log.info("Found IDStatusCache plist at path: %s",
-                          self.file_path)
+            self.log.info("Found IDStatusCache plist at path: %s", self.file_path)
             self._extract_idstatuscache_entries(self.file_path)
         elif self.is_fs_dump:
             for idstatuscache_path in self._get_fs_files_from_patterns(
-                    IDSTATUSCACHE_ROOT_PATHS):
+                IDSTATUSCACHE_ROOT_PATHS
+            ):
                 self.file_path = idstatuscache_path
-                self.log.info("Found IDStatusCache plist at path: %s",
-                              self.file_path)
+                self.log.info("Found IDStatusCache plist at path: %s", self.file_path)
                 self._extract_idstatuscache_entries(self.file_path)
 
-        self.log.info("Extracted a total of %d ID Status Cache entries",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d ID Status Cache entries", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.3.0/mvt/ios/modules/mixed/interactionc.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,33 +205,38 @@
             ZINTERACTIONS.ZLOCATIONUUID AS "location_uuid",
             ZINTERACTIONS.Z_PK AS "table_id"
     FROM
         ZINTERACTIONS
         LEFT JOIN
             ZCONTACTS
             ON ZINTERACTIONS.ZSENDER = ZCONTACTS.Z_PK
-    """
+    """,
 ]
 
 
 class InteractionC(IOSExtraction):
     """This module extracts data from InteractionC db."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.timestamps = [
             "start_date",
             "end_date",
             "interactions_creation_date",
             "contacts_creation_date",
             "first_incoming_recipient_date",
@@ -250,45 +255,54 @@
             if timestamp not in record or not record[timestamp]:
                 continue
 
             # Check if the timestamp was already processed.
             if record[timestamp] in processed:
                 continue
 
-            records.append({
-                "timestamp": record[timestamp],
-                "module": self.__class__.__name__,
-                "event": timestamp,
-                "data": f"[{record['bundle_id']}] {record['account']} - "
-                        f"from {record['sender_display_name']} ({record['sender_identifier']}) "
-                        f"to {record.get('recipient_display_name', '')} ({record.get('recipient_identifier', '')}):"
-                        f" {record.get('content', '')}"
-            })
+            records.append(
+                {
+                    "timestamp": record[timestamp],
+                    "module": self.__class__.__name__,
+                    "event": timestamp,
+                    "data": f"[{record['bundle_id']}] {record['account']} - "
+                    f"from {record['sender_display_name']} ({record['sender_identifier']}) "
+                    f"to {record.get('recipient_display_name', '')} ({record.get('recipient_identifier', '')}):"
+                    f" {record.get('content', '')}",
+                }
+            )
             processed.append(record[timestamp])
 
         return records
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=INTERACTIONC_BACKUP_IDS,
-                                root_paths=INTERACTIONC_ROOT_PATHS)
+        self._find_ios_database(
+            backup_ids=INTERACTIONC_BACKUP_IDS, root_paths=INTERACTIONC_ROOT_PATHS
+        )
         self.log.info("Found InteractionC database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
 
         try:
             cur.execute(QUERIES[0])
         except sqlite3.OperationalError:
             try:
                 cur.execute(QUERIES[1])
             except sqlite3.OperationalError:
                 try:
                     cur.execute(QUERIES[2])
                 except sqlite3.OperationalError:
-                    cur.execute(QUERIES[3])
+                    try:
+                        cur.execute(QUERIES[3])
+                    except sqlite3.OperationalError as e:
+                        self.log.info(
+                            "Error while reading the InteractionC table: %s", e
+                        )
+                        return None
 
         names = [description[0] for description in cur.description]
         for item in cur:
             entry = {}
             for index, value in enumerate(item):
                 if names[index] in self.timestamps:
                     if value is None or isinstance(value, str):
@@ -299,9 +313,8 @@
                     entry[names[index]] = value
 
             self.results.append(entry)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d InteractionC events",
-                      len(self.results))
+        self.log.info("Extracted a total of %d InteractionC events", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/locationd.py` & `mvt-2.3.0/mvt/ios/modules/mixed/locationd.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,33 +12,38 @@
 from ..base import IOSExtraction
 
 LOCATIOND_BACKUP_IDS = [
     "a690d7769cce8904ca2b67320b107c8fe5f79412",
 ]
 LOCATIOND_ROOT_PATHS = [
     "private/var/mobile/Library/Caches/locationd/clients.plist",
-    "private/var/root/Library/Caches/locationd/clients.plist"
+    "private/var/root/Library/Caches/locationd/clients.plist",
 ]
 
 
 class LocationdClients(IOSExtraction):
     """Extract information from apps who used geolocation."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.timestamps = [
             "ConsumptionPeriodBegin",
             "ReceivingLocationInformationTimeStopped",
             "VisitTimeStopped",
             "LocationTimeStopped",
             "BackgroundLocationTimeStopped",
@@ -48,89 +53,100 @@
             "BeaconRegionTimeStopped",
         ]
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for timestamp in self.timestamps:
             if timestamp in record.keys():
-                records.append({
-                    "timestamp": record[timestamp],
-                    "module": self.__class__.__name__,
-                    "event": timestamp,
-                    "data": f"{timestamp} from {record['package']}"
-                })
+                records.append(
+                    {
+                        "timestamp": record[timestamp],
+                        "module": self.__class__.__name__,
+                        "event": timestamp,
+                        "data": f"{timestamp} from {record['package']}",
+                    }
+                )
 
         return records
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             parts = result["package"].split("/")
-            proc_name = parts[len(parts)-1]
+            proc_name = parts[len(parts) - 1]
 
             ioc = self.indicators.check_process(proc_name)
             if ioc:
-                self.log.warning("Found a suspicious process name in LocationD entry %s",
-                                 result["package"])
+                self.log.warning(
+                    "Found a suspicious process name in LocationD entry %s",
+                    result["package"],
+                )
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
                 continue
 
             if "BundlePath" in result:
                 ioc = self.indicators.check_file_path(result["BundlePath"])
                 if ioc:
-                    self.log.warning("Found a suspicious file path in Location D: %s",
-                                     result["BundlePath"])
+                    self.log.warning(
+                        "Found a suspicious file path in Location D: %s",
+                        result["BundlePath"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             if "Executable" in result:
                 ioc = self.indicators.check_file_path(result["Executable"])
                 if ioc:
-                    self.log.warning("Found a suspicious file path in Location D: %s",
-                                     result["Executable"])
+                    self.log.warning(
+                        "Found a suspicious file path in Location D: %s",
+                        result["Executable"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
             if "Registered" in result:
                 ioc = self.indicators.check_file_path(result["Registered"])
                 if ioc:
-                    self.log.warning("Found a suspicious file path in Location D: %s",
-                                     result["Registered"])
+                    self.log.warning(
+                        "Found a suspicious file path in Location D: %s",
+                        result["Registered"],
+                    )
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
     def _extract_locationd_entries(self, file_path):
         with open(file_path, "rb") as handle:
             file_plist = plistlib.load(handle)
 
         for key, _ in file_plist.items():
             result = file_plist[key]
             result["package"] = key
             for timestamp in self.timestamps:
                 if timestamp in result.keys():
-                    result[timestamp] = convert_mactime_to_iso(
-                        result[timestamp])
+                    result[timestamp] = convert_mactime_to_iso(result[timestamp])
 
             self.results.append(result)
 
     def run(self) -> None:
         if self.is_backup:
             self._find_ios_database(backup_ids=LOCATIOND_BACKUP_IDS)
-            self.log.info("Found Locationd Clients plist at path: %s",
-                          self.file_path)
+            self.log.info("Found Locationd Clients plist at path: %s", self.file_path)
             self._extract_locationd_entries(self.file_path)
         elif self.is_fs_dump:
             for locationd_path in self._get_fs_files_from_patterns(
-                    LOCATIOND_ROOT_PATHS):
+                LOCATIOND_ROOT_PATHS
+            ):
                 self.file_path = locationd_path
-                self.log.info("Found Locationd Clients plist at path: %s",
-                              self.file_path)
+                self.log.info(
+                    "Found Locationd Clients plist at path: %s", self.file_path
+                )
                 self._extract_locationd_entries(self.file_path)
 
-        self.log.info("Extracted a total of %d Locationd Clients entries",
-                      len(self.results))
+        self.log.info(
+            "Extracted a total of %d Locationd Clients entries", len(self.results)
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.3.0/mvt/ios/modules/mixed/net_datausage.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,28 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=DATAUSAGE_BACKUP_IDS,
-                                root_paths=DATAUSAGE_ROOT_PATHS)
+        self._find_ios_database(
+            backup_ids=DATAUSAGE_BACKUP_IDS, root_paths=DATAUSAGE_ROOT_PATHS
+        )
         self.log.info("Found DataUsage database at path: %s", self.file_path)
 
         self._extract_net_data()
         self._find_suspicious_processes()
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.3.0/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,57 +24,69 @@
     from com.apple.osanalytics.addaily.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["ts"],
             "module": self.__class__.__name__,
             "event": "osanalytics_addaily",
             "data": f"{record['package']} WIFI IN: {record['wifi_in']}, "
-                    f"WIFI OUT: {record['wifi_out']} - "
-                    f"WWAN IN: {record['wwan_in']}, "
-                    f"WWAN OUT: {record['wwan_out']}",
+            f"WIFI OUT: {record['wifi_out']} - "
+            f"WWAN IN: {record['wwan_in']}, "
+            f"WWAN OUT: {record['wwan_out']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_process(result["package"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=OSANALYTICS_ADDAILY_BACKUP_IDS,
-                                root_paths=OSANALYTICS_ADDAILY_ROOT_PATHS)
-        self.log.info("Found com.apple.osanalytics.addaily plist at path: %s",
-                      self.file_path)
+        self._find_ios_database(
+            backup_ids=OSANALYTICS_ADDAILY_BACKUP_IDS,
+            root_paths=OSANALYTICS_ADDAILY_ROOT_PATHS,
+        )
+        self.log.info(
+            "Found com.apple.osanalytics.addaily plist at path: %s", self.file_path
+        )
 
         with open(self.file_path, "rb") as handle:
             file_plist = plistlib.load(handle)
 
         for app, values in file_plist.get("netUsageBaseline", {}).items():
-            self.results.append({
-                "package": app,
-                "ts": convert_datetime_to_iso(values[0]),
-                "wifi_in": values[1],
-                "wifi_out": values[2],
-                "wwan_in": values[3],
-                "wwan_out": values[4],
-            })
-
-        self.log.info("Extracted a total of %d com.apple.osanalytics.addaily entries",
-                      len(self.results))
+            self.results.append(
+                {
+                    "package": app,
+                    "ts": convert_datetime_to_iso(values[0]),
+                    "wifi_in": values[1],
+                    "wifi_out": values[2],
+                    "wwan_in": values[3],
+                    "wwan_out": values[4],
+                }
+            )
+
+        self.log.info(
+            "Extracted a total of %d com.apple.osanalytics.addaily entries",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.3.0/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,30 +25,35 @@
     """This module extracts all Safari browser state records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self._session_history_count = 0
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["last_viewed_timestamp"],
             "module": self.__class__.__name__,
             "event": "tab",
-            "data": f"{record['tab_title']} - {record['tab_url']}"
+            "data": f"{record['tab_title']} - {record['tab_url']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -71,33 +76,37 @@
 
     def _process_browser_state_db(self, db_path):
         self._recover_sqlite_db_if_needed(db_path)
         conn = sqlite3.connect(db_path)
 
         cur = conn.cursor()
         try:
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     tabs.title,
                     tabs.url,
                     tabs.user_visible_url,
                     tabs.last_viewed_time,
                     tab_sessions.session_data
                 FROM tabs
                 JOIN tab_sessions ON tabs.uuid = tab_sessions.tab_uuid
                 ORDER BY tabs.last_viewed_time;
-            """)
+            """
+            )
         except sqlite3.OperationalError:
             # Old version iOS <12 likely
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     title, url, user_visible_url, last_viewed_time, session_data
                 FROM tabs
                 ORDER BY last_viewed_time;
-            """)
+            """
+            )
 
         for row in cur:
             session_entries = []
 
             if row[4]:
                 # Skip a 4 byte header before the plist content.
                 session_plist = row[4][4:]
@@ -106,52 +115,72 @@
                     session_data = plistlib.load(io.BytesIO(session_plist))
                     session_data = keys_bytes_to_string(session_data)
                 except plistlib.InvalidFileException:
                     pass
 
                 if "SessionHistoryEntries" in session_data.get("SessionHistory", {}):
                     for session_entry in session_data["SessionHistory"].get(
-                            "SessionHistoryEntries"):
+                        "SessionHistoryEntries"
+                    ):
                         self._session_history_count += 1
 
                         data_length = 0
                         if "SessionHistoryEntryData" in session_entry:
-                            data_length = len(session_entry.get("SessionHistoryEntryData"))
-
-                        session_entries.append({
-                            "entry_title": session_entry.get("SessionHistoryEntryOriginalURL"),
-                            "entry_url": session_entry.get("SessionHistoryEntryURL"),
-                            "data_length": data_length,
-                        })
-
-            self.results.append({
-                "tab_title": row[0],
-                "tab_url": row[1],
-                "tab_visible_url": row[2],
-                "last_viewed_timestamp": convert_mactime_to_iso(row[3]),
-                "session_data": session_entries,
-                "safari_browser_state_db": os.path.relpath(db_path,
-                                                           self.target_path),
-            })
+                            data_length = len(
+                                session_entry.get("SessionHistoryEntryData")
+                            )
+
+                        session_entries.append(
+                            {
+                                "entry_title": session_entry.get(
+                                    "SessionHistoryEntryOriginalURL"
+                                ),
+                                "entry_url": session_entry.get(
+                                    "SessionHistoryEntryURL"
+                                ),
+                                "data_length": data_length,
+                            }
+                        )
+
+            self.results.append(
+                {
+                    "tab_title": row[0],
+                    "tab_url": row[1],
+                    "tab_visible_url": row[2],
+                    "last_viewed_timestamp": convert_mactime_to_iso(row[3]),
+                    "session_data": session_entries,
+                    "safari_browser_state_db": os.path.relpath(
+                        db_path, self.target_path
+                    ),
+                }
+            )
 
     def run(self) -> None:
         if self.is_backup:
             for backup_file in self._get_backup_files_from_manifest(
-                    relative_path=SAFARI_BROWSER_STATE_BACKUP_RELPATH):
+                relative_path=SAFARI_BROWSER_STATE_BACKUP_RELPATH
+            ):
                 browserstate_path = self._get_backup_file_from_id(
-                    backup_file["file_id"])
+                    backup_file["file_id"]
+                )
 
                 if not browserstate_path:
                     continue
 
-                self.log.info("Found Safari browser state database at path: %s",
-                              browserstate_path)
+                self.log.info(
+                    "Found Safari browser state database at path: %s", browserstate_path
+                )
                 self._process_browser_state_db(browserstate_path)
         elif self.is_fs_dump:
             for browserstate_path in self._get_fs_files_from_patterns(
-                    SAFARI_BROWSER_STATE_ROOT_PATHS):
-                self.log.info("Found Safari browser state database at path: %s",
-                              browserstate_path)
+                SAFARI_BROWSER_STATE_ROOT_PATHS
+            ):
+                self.log.info(
+                    "Found Safari browser state database at path: %s", browserstate_path
+                )
                 self._process_browser_state_db(browserstate_path)
 
-        self.log.info("Extracted a total of %d tab records and %d session history entries",
-                      len(self.results), self._session_history_count)
+        self.log.info(
+            "Extracted a total of %d tab records and %d session history entries",
+            len(self.results),
+            self._session_history_count,
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.3.0/mvt/ios/modules/mixed/safari_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 import logging
 import os
 import sqlite3
 from typing import Optional, Union
 
 from mvt.common.url import URL
-from mvt.common.utils import (convert_mactime_to_datetime,
-                              convert_mactime_to_iso)
+from mvt.common.utils import convert_mactime_to_datetime, convert_mactime_to_iso
 
 from ..base import IOSExtraction
 
 SAFARI_HISTORY_BACKUP_RELPATH = "Library/Safari/History.db"
 SAFARI_HISTORY_ROOT_PATHS = [
     "private/var/mobile/Library/Safari/History.db",
     "private/var/mobile/Containers/Data/Application/*/Library/Safari/History.db",
@@ -29,29 +28,34 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "safari_history",
             "data": f"Safari visit to {record['url']} (ID: {record['id']}, "
-                    f"Visit ID: {record['visit_id']})",
+            f"Visit ID: {record['visit_id']})",
         }
 
     def _find_injections(self):
         for result in self.results:
             # We presume injections only happen on HTTP visits.
             if not result["url"].lower().startswith("http://"):
                 continue
@@ -76,25 +80,30 @@
                     redirect_domain = ""
 
                 # If the redirect destination is the same domain as the origin,
                 # it's most likely an HTTPS upgrade.
                 if origin_domain == redirect_domain:
                     continue
 
-                self.log.info("Found HTTP redirect to different domain: \"%s\" -> \"%s\"",
-                              origin_domain, redirect_domain)
+                self.log.info(
+                    'Found HTTP redirect to different domain: "%s" -> "%s"',
+                    origin_domain,
+                    redirect_domain,
+                )
 
                 redirect_time = convert_mactime_to_datetime(redirect["timestamp"])
                 origin_time = convert_mactime_to_datetime(result["timestamp"])
                 elapsed_time = redirect_time - origin_time
                 elapsed_ms = elapsed_time.microseconds / 1000
 
                 if elapsed_time.seconds == 0:
-                    self.log.warning("Redirect took less than a second! (%d milliseconds)",
-                                     elapsed_ms)
+                    self.log.warning(
+                        "Redirect took less than a second! (%d milliseconds)",
+                        elapsed_ms,
+                    )
 
     def check_indicators(self) -> None:
         self._find_injections()
 
         if not self.indicators:
             return
 
@@ -104,59 +113,62 @@
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def _process_history_db(self, history_path):
         self._recover_sqlite_db_if_needed(history_path)
         conn = sqlite3.connect(history_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 history_items.id,
                 history_items.url,
                 history_visits.id,
                 history_visits.visit_time,
                 history_visits.redirect_source,
                 history_visits.redirect_destination
             FROM history_items
             JOIN history_visits ON history_visits.history_item = history_items.id
             ORDER BY history_visits.visit_time;
-        """)
+        """
+        )
 
         for row in cur:
-            self.results.append({
-                "id": row[0],
-                "url": row[1],
-                "visit_id": row[2],
-                "timestamp": row[3],
-                "isodate": convert_mactime_to_iso(row[3]),
-                "redirect_source": row[4],
-                "redirect_destination": row[5],
-                "safari_history_db": os.path.relpath(history_path,
-                                                     self.target_path),
-            })
+            self.results.append(
+                {
+                    "id": row[0],
+                    "url": row[1],
+                    "visit_id": row[2],
+                    "timestamp": row[3],
+                    "isodate": convert_mactime_to_iso(row[3]),
+                    "redirect_source": row[4],
+                    "redirect_destination": row[5],
+                    "safari_history_db": os.path.relpath(
+                        history_path, self.target_path
+                    ),
+                }
+            )
 
         cur.close()
         conn.close()
 
     def run(self) -> None:
         if self.is_backup:
             for history_file in self._get_backup_files_from_manifest(
-                    relative_path=SAFARI_HISTORY_BACKUP_RELPATH):
-                history_path = self._get_backup_file_from_id(
-                    history_file["file_id"])
+                relative_path=SAFARI_HISTORY_BACKUP_RELPATH
+            ):
+                history_path = self._get_backup_file_from_id(history_file["file_id"])
 
                 if not history_path:
                     continue
 
-                self.log.info("Found Safari history database at path: %s",
-                              history_path)
+                self.log.info("Found Safari history database at path: %s", history_path)
 
                 self._process_history_db(history_path)
         elif self.is_fs_dump:
             for history_path in self._get_fs_files_from_patterns(
-                    SAFARI_HISTORY_ROOT_PATHS):
-                self.log.info("Found Safari history database at path: %s",
-                              history_path)
+                SAFARI_HISTORY_ROOT_PATHS
+            ):
+                self.log.info("Found Safari history database at path: %s", history_path)
                 self._process_history_db(history_path)
 
-        self.log.info("Extracted a total of %d history records",
-                      len(self.results))
+        self.log.info("Extracted a total of %d history records", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.3.0/mvt/ios/modules/mixed/shortcuts.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,91 +26,101 @@
     """This module extracts all info about SMS/iMessage attachments."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         found_urls = ""
         if record["action_urls"]:
             found_urls = f"- URLs in actions: {', '.join(record['action_urls'])}"
 
         desc = ""
         if record["description"]:
             desc = record["description"].decode("utf-8", errors="ignore")
 
-        return [{
-            "timestamp": record["isodate"],
-            "module": self.__class__.__name__,
-            "event": "shortcut_created",
-            "data": f"iOS Shortcut '{record['shortcut_name'].decode('utf-8')}': {desc} {found_urls}"
-        }, {
-            "timestamp": record["modified_date"],
-            "module": self.__class__.__name__,
-            "event": "shortcut_modified",
-            "data": f"iOS Shortcut '{record['shortcut_name'].decode('utf-8')}': {desc} {found_urls}"
-        }]
+        return [
+            {
+                "timestamp": record["isodate"],
+                "module": self.__class__.__name__,
+                "event": "shortcut_created",
+                "data": f"iOS Shortcut '{record['shortcut_name'].decode('utf-8')}': {desc} {found_urls}",
+            },
+            {
+                "timestamp": record["modified_date"],
+                "module": self.__class__.__name__,
+                "event": "shortcut_modified",
+                "data": f"iOS Shortcut '{record['shortcut_name'].decode('utf-8')}': {desc} {found_urls}",
+            },
+        ]
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_domains(result["action_urls"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=SHORTCUT_BACKUP_IDS,
-                                root_paths=SHORTCUT_ROOT_PATHS)
+        self._find_ios_database(
+            backup_ids=SHORTCUT_BACKUP_IDS, root_paths=SHORTCUT_ROOT_PATHS
+        )
         self.log.info("Found Shortcuts database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         conn.text_factory = bytes
         cur = conn.cursor()
         try:
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     ZSHORTCUT.Z_PK as "shortcut_id",
                     ZSHORTCUT.ZNAME as "shortcut_name",
                     ZSHORTCUT.ZCREATIONDATE as "created_date",
                     ZSHORTCUT.ZMODIFICATIONDATE as "modified_date",
                     ZSHORTCUT.ZACTIONSDESCRIPTION as "description",
                     ZSHORTCUTACTIONS.ZDATA as "action_data"
                 FROM ZSHORTCUT
                 LEFT JOIN ZSHORTCUTACTIONS ON ZSHORTCUTACTIONS.ZSHORTCUT == ZSHORTCUT.Z_PK;
-            """)
+            """
+            )
         except sqlite3.OperationalError:
-            # Table ZSHORTCUT does not exist
+            # Table ZSHORTCUT does not exist
             self.log.info("Invalid shortcut database format, skipping...")
             cur.close()
             conn.close()
             return
 
         names = [description[0] for description in cur.description]
 
         for item in cur:
             shortcut = {}
             # We store the value of each column under the proper key.
             for index, value in enumerate(item):
                 shortcut[names[index]] = value
 
             try:
-                action_data = plistlib.load(io.BytesIO(
-                    shortcut.pop("action_data", [])))
+                action_data = plistlib.load(io.BytesIO(shortcut.pop("action_data", [])))
                 actions = []
                 for action_entry in action_data:
                     action = {}
                     action["identifier"] = action_entry["WFWorkflowActionIdentifier"]
                     action["parameters"] = action_entry["WFWorkflowActionParameters"]
 
                     # URLs might be in multiple fields, do a simple regex search
@@ -118,22 +128,25 @@
                     extracted_urls = check_for_links(str(action["parameters"]))
 
                     # Remove quoting characters that may have been captured by the
                     # regex.
                     action["urls"] = [url.rstrip("',") for url in extracted_urls]
                     actions.append(action)
                 shortcut["parsed_actions"] = len(actions)
-                shortcut["action_urls"] = list(itertools.chain(
-                    *[action["urls"] for action in actions]))
+                shortcut["action_urls"] = list(
+                    itertools.chain(*[action["urls"] for action in actions])
+                )
             except plistlib.InvalidFileException:
                 self.log.debug("Shortcut without action data")
                 shortcut["action_urls"] = None
                 shortcut["parsed_actions"] = 0
 
             shortcut["isodate"] = convert_mactime_to_iso(shortcut.pop("created_date"))
-            shortcut["modified_date"] = convert_mactime_to_iso(shortcut["modified_date"])
+            shortcut["modified_date"] = convert_mactime_to_iso(
+                shortcut["modified_date"]
+            )
             self.results.append(shortcut)
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d Shortcuts", len(self.results))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/sms.py` & `mvt-2.3.0/mvt/ios/modules/mixed/sms.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,30 +24,35 @@
     """This module extracts all SMS messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record["text"].replace("\n", "\\n")
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "sms_received",
             "data": f"{record['service']}: {record['guid']} \"{text}\" "
-                    f"from {record['phone_number']} ({record['account']})"
+            f"from {record['phone_number']} ({record['account']})",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
@@ -57,79 +62,86 @@
                 message_links = check_for_links(result.get("text", ""))
             ioc = self.indicators.check_domains(message_links)
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=SMS_BACKUP_IDS,
-                                root_paths=SMS_ROOT_PATHS)
+        self._find_ios_database(backup_ids=SMS_BACKUP_IDS, root_paths=SMS_ROOT_PATHS)
         self.log.info("Found SMS database at path: %s", self.file_path)
 
         try:
             conn = sqlite3.connect(self.file_path)
             cur = conn.cursor()
-            cur.execute("""
+            cur.execute(
+                """
                 SELECT
                     message.*,
                     handle.id as "phone_number"
                 FROM message, handle
                 WHERE handle.rowid = message.handle_id;
-            """)
+            """
+            )
             # Force the query early to catch database issues
             items = list(cur)
         except sqlite3.DatabaseError as exc:
             conn.close()
             if "database disk image is malformed" in str(exc):
                 self._recover_sqlite_db_if_needed(self.file_path, forced=True)
                 conn = sqlite3.connect(self.file_path)
                 cur = conn.cursor()
-                cur.execute("""
+                cur.execute(
+                    """
                     SELECT
                         message.*,
                         handle.id as "phone_number"
                     FROM message, handle
                     WHERE handle.rowid = message.handle_id;
-                """)
+                """
+                )
                 items = list(cur)
             else:
                 raise exc
         names = [description[0] for description in cur.description]
 
         for item in items:
             message = {}
             for index, value in enumerate(item):
                 # We base64 escape some of the attributes that could contain
                 # binary data.
-                if (names[index] == "attributedBody"
-                        or names[index] == "payload_data"
-                        or names[index] == "message_summary_info") and value:
+                if (
+                    names[index] == "attributedBody"
+                    or names[index] == "payload_data"
+                    or names[index] == "message_summary_info"
+                ) and value:
                     value = b64encode(value).decode()
 
                 # We store the value of each column under the proper key.
                 message[names[index]] = value
 
             # We convert Mac's ridiculous timestamp format.
             message["isodate"] = convert_mactime_to_iso(message["date"])
-            message["direction"] = ("sent" if message.get("is_from_me", 0) == 1
-                                        else "received")
+            message["direction"] = (
+                "sent" if message.get("is_from_me", 0) == 1 else "received"
+            )
 
             # Sometimes "text" is None instead of empty string.
             if not message.get("text", None):
                 message["text"] = ""
 
             alert = "ALERT: State-sponsored attackers may be targeting your iPhone"
             if message.get("text", "").startswith(alert):
-                self.log.warning("Apple warning about state-sponsored attack received on the %s",
-                                 message["isodate"])
+                self.log.warning(
+                    "Apple warning about state-sponsored attack received on the %s",
+                    message["isodate"],
+                )
             else:
                 # Extract links from the SMS message.
                 message_links = check_for_links(message.get("text", ""))
                 message["links"] = message_links
 
             self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d SMS messages",
-                      len(self.results))
+        self.log.info("Extracted a total of %d SMS messages", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.3.0/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,83 +24,99 @@
     """This module extracts all info about SMS/iMessage attachments."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "sms_attachment",
             "data": f"{record['service']}: Attachment "
-                    f"'{record['transfer_name']}' {record['direction']} "
-                    f"from {record['phone_number']} "
-                    f"with {record['total_bytes']} bytes "
-                    f"(is_sticker: {record['is_sticker']}, "
-                    f"has_user_info: {record['has_user_info']})"
+            f"'{record['transfer_name']}' {record['direction']} "
+            f"from {record['phone_number']} "
+            f"with {record['total_bytes']} bytes "
+            f"(is_sticker: {record['is_sticker']}, "
+            f"has_user_info: {record['has_user_info']})",
         }
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=SMS_BACKUP_IDS,
-                                root_paths=SMS_ROOT_PATHS)
+        self._find_ios_database(backup_ids=SMS_BACKUP_IDS, root_paths=SMS_ROOT_PATHS)
         self.log.info("Found SMS database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 attachment.ROWID as "attachment_id",
                 attachment.*,
                 message.service as "service",
                 handle.id as "phone_number"
             FROM attachment
             LEFT JOIN message_attachment_join ON
                 message_attachment_join.attachment_id = attachment.ROWID
             LEFT JOIN message ON
                 message.ROWID = message_attachment_join.message_id
             LEFT JOIN handle ON handle.ROWID = message.handle_id;
-        """)
+        """
+        )
         names = [description[0] for description in cur.description]
 
         for item in cur:
             attachment = {}
             for index, value in enumerate(item):
-                if (names[index] in ["user_info", "sticker_user_info",
-                                     "attribution_info",
-                                     "ck_server_change_token_blob",
-                                     "sr_ck_server_change_token_blob"]) and value:
+                if (
+                    names[index]
+                    in [
+                        "user_info",
+                        "sticker_user_info",
+                        "attribution_info",
+                        "ck_server_change_token_blob",
+                        "sr_ck_server_change_token_blob",
+                    ]
+                ) and value:
                     value = b64encode(value).decode()
                 attachment[names[index]] = value
 
-            attachment["isodate"] = convert_mactime_to_iso(
-                attachment["created_date"])
-            attachment["start_date"] = convert_mactime_to_iso(
-                attachment["start_date"])
-            attachment["direction"] = ("sent" if attachment["is_outgoing"] == 1 else "received")
+            attachment["isodate"] = convert_mactime_to_iso(attachment["created_date"])
+            attachment["start_date"] = convert_mactime_to_iso(attachment["start_date"])
+            attachment["direction"] = (
+                "sent" if attachment["is_outgoing"] == 1 else "received"
+            )
             attachment["has_user_info"] = attachment["user_info"] is not None
             attachment["service"] = attachment["service"] or "Unknown"
             attachment["filename"] = attachment["filename"] or "NULL"
 
-            if (attachment["filename"].startswith("/var/tmp/")
-                    and attachment["filename"].endswith("-1")
-                    and attachment["direction"] == "received"):
-                self.log.warning("Suspicious iMessage attachment %s on %s",
-                                 attachment['filename'], attachment['isodate'])
+            if (
+                attachment["filename"].startswith("/var/tmp/")
+                and attachment["filename"].endswith("-1")
+                and attachment["direction"] == "received"
+            ):
+                self.log.warning(
+                    "Suspicious iMessage attachment %s on %s",
+                    attachment["filename"],
+                    attachment["isodate"],
+                )
                 self.detected.append(attachment)
 
             self.results.append(attachment)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d SMS attachments",
-                      len(self.results))
+        self.log.info("Extracted a total of %d SMS attachments", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/tcc.py` & `mvt-2.3.0/mvt/ios/modules/mixed/tcc.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 TCC_BACKUP_IDS = [
     "64d0019cb3d46bfc8cce545a8ba54b93e7ea9347",
 ]
 TCC_ROOT_PATHS = [
     "private/var/mobile/Library/TCC/TCC.db",
 ]
 
-AUTH_VALUE_OLD = {
-    0: "denied",
-    1: "allowed"
-}
+AUTH_VALUE_OLD = {0: "denied", 1: "allowed"}
 AUTH_VALUES = {
     0: "denied",
     1: "unknown",
     2: "allowed",
     3: "limited",
 }
 AUTH_REASONS = {
@@ -48,36 +45,45 @@
     """This module extracts records from the TCC.db SQLite database."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if "last_modified" in record:
             if "allowed_value" in record:
-                msg = (f"Access to {record['service']} by {record['client']} "
-                       f"{record['allowed_value']}")
+                msg = (
+                    f"Access to {record['service']} by {record['client']} "
+                    f"{record['allowed_value']}"
+                )
             else:
-                msg = (f"Access to {record['service']} by {record['client']} "
-                       f"{record['auth_value']}")
+                msg = (
+                    f"Access to {record['service']} by {record['client']} "
+                    f"{record['auth_value']}"
+                )
 
             return {
                 "timestamp": record["last_modified"],
                 "module": self.__class__.__name__,
                 "event": "AccessRequest",
-                "data": msg
+                "data": msg,
             }
 
         return {}
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
@@ -89,105 +95,130 @@
                 self.detected.append(result)
 
     def process_db(self, file_path):
         conn = sqlite3.connect(file_path)
         cur = conn.cursor()
         db_version = "v3"
         try:
-            cur.execute("""SELECT
+            cur.execute(
+                """SELECT
                 service, client, client_type, auth_value,
                 auth_reason, last_modified
-            FROM access;""")
+            FROM access;"""
+            )
         except sqlite3.OperationalError:
             # v2 version
             try:
-                cur.execute("""SELECT
+                cur.execute(
+                    """SELECT
                     service, client, client_type, allowed,
                     prompt_count, last_modified
-                    FROM access;""")
+                    FROM access;"""
+                )
                 db_version = "v2"
             except sqlite3.OperationalError:
-                cur.execute("""SELECT
+                cur.execute(
+                    """SELECT
                     service, client, client_type, allowed,
                     prompt_count
-                    FROM access;""")
+                    FROM access;"""
+                )
                 db_version = "v1"
 
         for row in cur:
             service = row[0]
             client = row[1]
             client_type = row[2]
-            client_type_desc = ("bundle_id" if client_type == 0
-                                    else "absolute_path")
+            client_type_desc = "bundle_id" if client_type == 0 else "absolute_path"
             if db_version == "v3":
                 auth_value = row[3]
                 auth_value_desc = AUTH_VALUES.get(auth_value, "")
                 auth_reason = row[4]
                 auth_reason_desc = AUTH_REASONS.get(auth_reason, "unknown")
                 last_modified = convert_unix_to_iso(row[5])
 
                 if service in ["kTCCServiceMicrophone", "kTCCServiceCamera"]:
-                    device = "microphone" if service == "kTCCServiceMicrophone" else "camera"
-                    self.log.info("Found client \"%s\" with access %s to %s on %s by %s",
-                                  client, auth_value_desc, device,
-                                  last_modified, auth_reason_desc)
-
-                self.results.append({
-                    "service": service,
-                    "client": client,
-                    "client_type": client_type_desc,
-                    "auth_value": auth_value_desc,
-                    "auth_reason_desc": auth_reason_desc,
-                    "last_modified": last_modified,
-                })
+                    device = (
+                        "microphone" if service == "kTCCServiceMicrophone" else "camera"
+                    )
+                    self.log.info(
+                        'Found client "%s" with access %s to %s on %s by %s',
+                        client,
+                        auth_value_desc,
+                        device,
+                        last_modified,
+                        auth_reason_desc,
+                    )
+
+                self.results.append(
+                    {
+                        "service": service,
+                        "client": client,
+                        "client_type": client_type_desc,
+                        "auth_value": auth_value_desc,
+                        "auth_reason_desc": auth_reason_desc,
+                        "last_modified": last_modified,
+                    }
+                )
             else:
                 allowed_value = row[3]
                 allowed_desc = AUTH_VALUE_OLD.get(allowed_value, "")
                 prompt_count = row[4]
 
                 if db_version == "v2":
                     last_modified = convert_unix_to_iso(row[5])
                     if service in ["kTCCServiceMicrophone", "kTCCServiceCamera"]:
                         device = "camera"
                         if service == "kTCCServiceMicrophone":
                             device = "microphone"
 
-                        self.log.info("Found client \"%s\" with access %s to %s at %s",
-                                      client, allowed_desc, device,
-                                      last_modified)
-
-                    self.results.append({
-                        "service": service,
-                        "client": client,
-                        "client_type": client_type_desc,
-                        "allowed_value": allowed_desc,
-                        "prompt_count": prompt_count,
-                        "last_modified": last_modified
-                    })
+                        self.log.info(
+                            'Found client "%s" with access %s to %s at %s',
+                            client,
+                            allowed_desc,
+                            device,
+                            last_modified,
+                        )
+
+                    self.results.append(
+                        {
+                            "service": service,
+                            "client": client,
+                            "client_type": client_type_desc,
+                            "allowed_value": allowed_desc,
+                            "prompt_count": prompt_count,
+                            "last_modified": last_modified,
+                        }
+                    )
                 else:
                     if service in ["kTCCServiceMicrophone", "kTCCServiceCamera"]:
                         device = "camera"
                         if service == "kTCCServiceMicrophone":
                             device = "microphone"
 
-                        self.log.info("Found client \"%s\" with access %s to %s",
-                                      client, allowed_desc, device)
-
-                    self.results.append({
-                        "service": service,
-                        "client": client,
-                        "client_type": client_type_desc,
-                        "allowed_value": allowed_desc,
-                        "prompt_count": prompt_count
-                    })
+                        self.log.info(
+                            'Found client "%s" with access %s to %s',
+                            client,
+                            allowed_desc,
+                            device,
+                        )
+
+                    self.results.append(
+                        {
+                            "service": service,
+                            "client": client,
+                            "client_type": client_type_desc,
+                            "allowed_value": allowed_desc,
+                            "prompt_count": prompt_count,
+                        }
+                    )
 
         cur.close()
         conn.close()
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=TCC_BACKUP_IDS,
-                                root_paths=TCC_ROOT_PATHS)
+        self._find_ios_database(backup_ids=TCC_BACKUP_IDS, root_paths=TCC_ROOT_PATHS)
         self.log.info("Found TCC database at path: %s", self.file_path)
 
         self.process_db(self.file_path)
 
         self.log.info("Extracted a total of %d TCC items", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.3.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,92 +24,112 @@
     observations.db."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = [] if not results else results
 
     def serialize(self, record: dict) -> Union[dict, list]:
         msg = f"Webkit resource loaded from {record['registrable_domain']}"
         if record["domain"] != "":
             msg += f" by app in domain {record['domain']}"
         return {
             "timestamp": record["last_seen_isodate"],
             "module": self.__class__.__name__,
             "event": "visit",
-            "data": msg
+            "data": msg,
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         self.detected = {}
         for result in self.results:
             ioc = self.indicators.check_domain(result["registrable_domain"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def _process_observations_db(self, db_path: str, domain: str, path: str) -> None:
-        self.log.info("Found WebKit ResourceLoadStatistics observations.db file at path %s",
-                      db_path)
+        self.log.info(
+            "Found WebKit ResourceLoadStatistics observations.db file at path %s",
+            db_path,
+        )
 
         self._recover_sqlite_db_if_needed(db_path)
 
         conn = sqlite3.connect(db_path)
         cur = conn.cursor()
 
         try:
-            # FIXME: table contains extra fields with timestamp here
-            cur.execute("""
+            # FIXME: table contains extra fields with timestamp here
+            cur.execute(
+                """
                 SELECT
                     domainID,
                     registrableDomain,
                     lastSeen,
                     hadUserInteraction
                 from ObservedDomains;
-            """)
+            """
+            )
         except sqlite3.OperationalError:
             return
 
         for row in cur:
-            self.results.append({
-                "domain_id": row[0],
-                "registrable_domain": row[1],
-                "last_seen": row[2],
-                "had_user_interaction": bool(row[3]),
-                "last_seen_isodate": convert_unix_to_iso(row[2]),
-                "domain": domain,
-                "path": path
-            })
+            self.results.append(
+                {
+                    "domain_id": row[0],
+                    "registrable_domain": row[1],
+                    "last_seen": row[2],
+                    "had_user_interaction": bool(row[3]),
+                    "last_seen_isodate": convert_unix_to_iso(row[2]),
+                    "domain": domain,
+                    "path": path,
+                }
+            )
 
         if len(self.results) > 0:
-            self.log.info("Extracted a total of %d records from %s",
-                          len(self.results), db_path)
+            self.log.info(
+                "Extracted a total of %d records from %s", len(self.results), db_path
+            )
 
     def run(self) -> None:
         if self.is_backup:
             try:
                 for backup_file in self._get_backup_files_from_manifest(
-                        relative_path=WEBKIT_RESOURCELOADSTATICS_BACKUP_RELPATH):
+                    relative_path=WEBKIT_RESOURCELOADSTATICS_BACKUP_RELPATH
+                ):
                     db_path = self._get_backup_file_from_id(backup_file["file_id"])
 
                     if db_path:
-                        self._process_observations_db(db_path=db_path, domain=backup_file['domain'], path=WEBKIT_RESOURCELOADSTATICS_BACKUP_RELPATH)
+                        self._process_observations_db(
+                            db_path=db_path,
+                            domain=backup_file["domain"],
+                            path=WEBKIT_RESOURCELOADSTATICS_BACKUP_RELPATH,
+                        )
             except Exception as exc:
                 self.log.info("Unable to find WebKit observations.db: %s", exc)
         elif self.is_fs_dump:
             for db_path in self._get_fs_files_from_patterns(
-                    WEBKIT_RESOURCELOADSTATICS_ROOT_PATHS):
+                WEBKIT_RESOURCELOADSTATICS_ROOT_PATHS
+            ):
                 db_rel_path = os.path.relpath(db_path, self.target_path)
-                self._process_observations_db(db_path=db_path, domain="", path=db_rel_path)
+                self._process_observations_db(
+                    db_path=db_path, domain="", path=db_rel_path
+                )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.3.0/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,26 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
         self.results = {} if not results else results
 
     @staticmethod
     def _extract_domains(entries):
         if not entries:
             return []
@@ -64,96 +69,110 @@
         if not self.indicators:
             return
 
         for _, entries in self.results.items():
             for entry in entries:
                 source_domains = self._extract_domains(entry["redirect_source"])
                 destination_domains = self._extract_domains(
-                    entry["redirect_destination"])
+                    entry["redirect_destination"]
+                )
 
                 # TODO: Currently not used.
                 # subframe_origins = self._extract_domains(
                 #    entry["subframe_under_origin"])
                 # subresource_domains = self._extract_domains(
                 #    entry["subresource_under_origin"])
 
                 all_origins = set(
-                    [entry["origin"]]
-                    + source_domains
-                    + destination_domains
+                    [entry["origin"]] + source_domains + destination_domains
                 )
 
                 ioc = self.indicators.check_domains(all_origins)
                 if ioc:
                     entry["matched_indicator"] = ioc
                     self.detected.append(entry)
 
                     redirect_path = ""
                     if len(source_domains) > 0:
                         redirect_path += "SOURCE: "
                         for idx, item in enumerate(source_domains):
-                            source_domains[idx] = f"\"{item}\""
+                            source_domains[idx] = f'"{item}"'
 
                         redirect_path += ", ".join(source_domains)
                         redirect_path += " -> "
 
                     redirect_path += f"ORIGIN: \"{entry['origin']}\""
 
                     if len(destination_domains) > 0:
                         redirect_path += " -> "
                         redirect_path += "DESTINATION: "
                         for idx, item in enumerate(destination_domains):
-                            destination_domains[idx] = f"\"{item}\""
+                            destination_domains[idx] = f'"{item}"'
 
                         redirect_path += ", ".join(destination_domains)
 
-                    self.log.warning("Found HTTP redirect between suspicious domains: %s",
-                                     redirect_path)
+                    self.log.warning(
+                        "Found HTTP redirect between suspicious domains: %s",
+                        redirect_path,
+                    )
 
     def _extract_browsing_stats(self, log_path):
         items = []
 
         with open(log_path, "rb") as handle:
             file_plist = plistlib.load(handle)
 
         if "browsingStatistics" not in file_plist:
             return items
 
         browsing_stats = file_plist["browsingStatistics"]
 
         for item in browsing_stats:
-            items.append({
-                "origin": item.get("PrevalentResourceOrigin", ""),
-                "redirect_source": item.get("topFrameUniqueRedirectsFrom", ""),
-                "redirect_destination": item.get("topFrameUniqueRedirectsTo", ""),
-                "subframe_under_origin": item.get("subframeUnderTopFrameOrigins", ""),
-                "subresource_under_origin": item.get("subresourceUnderTopFrameOrigins", ""),
-                "user_interaction": item.get("hadUserInteraction"),
-                "most_recent_interaction": convert_datetime_to_iso(
-                    item["mostRecentUserInteraction"]),
-                "last_seen": convert_datetime_to_iso(item["lastSeen"]),
-            })
+            items.append(
+                {
+                    "origin": item.get("PrevalentResourceOrigin", ""),
+                    "redirect_source": item.get("topFrameUniqueRedirectsFrom", ""),
+                    "redirect_destination": item.get("topFrameUniqueRedirectsTo", ""),
+                    "subframe_under_origin": item.get(
+                        "subframeUnderTopFrameOrigins", ""
+                    ),
+                    "subresource_under_origin": item.get(
+                        "subresourceUnderTopFrameOrigins", ""
+                    ),
+                    "user_interaction": item.get("hadUserInteraction"),
+                    "most_recent_interaction": convert_datetime_to_iso(
+                        item["mostRecentUserInteraction"]
+                    ),
+                    "last_seen": convert_datetime_to_iso(item["lastSeen"]),
+                }
+            )
 
         return items
 
     def run(self) -> None:
         if self.is_backup:
             for log_file in self._get_backup_files_from_manifest(
-                    relative_path=WEBKIT_SESSION_RESOURCE_LOG_BACKUP_RELPATH):
+                relative_path=WEBKIT_SESSION_RESOURCE_LOG_BACKUP_RELPATH
+            ):
                 log_path = self._get_backup_file_from_id(log_file["file_id"])
 
                 if not log_path:
                     continue
 
-                self.log.info("Found Safari browsing session resource log at path: %s",
-                              log_path)
+                self.log.info(
+                    "Found Safari browsing session resource log at path: %s", log_path
+                )
                 self.results[log_path] = self._extract_browsing_stats(log_path)
         elif self.is_fs_dump:
             for log_path in self._get_fs_files_from_patterns(
-                    WEBKIT_SESSION_RESOURCE_LOG_ROOT_PATHS):
-                self.log.info("Found Safari browsing session resource log at path: %s",
-                              log_path)
+                WEBKIT_SESSION_RESOURCE_LOG_ROOT_PATHS
+            ):
+                self.log.info(
+                    "Found Safari browsing session resource log at path: %s", log_path
+                )
                 key = os.path.relpath(log_path, self.target_path)
                 self.results[key] = self._extract_browsing_stats(log_path)
 
-        self.log.info("Extracted records from %d Safari browsing session resource logs",
-                      len(self.results))
+        self.log.info(
+            "Extracted records from %d Safari browsing session resource logs",
+            len(self.results),
+        )
```

### Comparing `mvt-2.2.6/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.3.0/mvt/ios/modules/mixed/whatsapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,102 +23,114 @@
     """This module extracts all WhatsApp messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record.get("ZTEXT", "").replace("\n", "\\n")
         links_text = ""
         if record.get("links"):
             links_text = " - Embedded links: " + ", ".join(record["links"])
 
         return {
             "timestamp": record.get("isodate"),
             "module": self.__class__.__name__,
             "event": "message",
-            "data": f"\'{text}\' from {record.get('ZFROMJID', 'Unknown')}{links_text}",
+            "data": f"'{text}' from {record.get('ZFROMJID', 'Unknown')}{links_text}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_domains(result.get("links", []))
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
-        self._find_ios_database(backup_ids=WHATSAPP_BACKUP_IDS,
-                                root_paths=WHATSAPP_ROOT_PATHS)
+        self._find_ios_database(
+            backup_ids=WHATSAPP_BACKUP_IDS, root_paths=WHATSAPP_ROOT_PATHS
+        )
         self.log.info("Found WhatsApp database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
 
         # Query all messages and join tables which can contain media attachments
         # and links.
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 ZWAMESSAGE.*,
                 ZWAMEDIAITEM.ZAUTHORNAME,
                 ZWAMEDIAITEM.ZMEDIAURL,
                 ZWAMESSAGEDATAITEM.ZCONTENT1,
                 ZWAMESSAGEDATAITEM.ZCONTENT2,
                 ZWAMESSAGEDATAITEM.ZMATCHEDTEXT,
                 ZWAMESSAGEDATAITEM.ZSUMMARY,
                 ZWAMESSAGEDATAITEM.ZTITLE
             FROM ZWAMESSAGE
             LEFT JOIN ZWAMEDIAITEM ON ZWAMEDIAITEM.ZMESSAGE = ZWAMESSAGE.Z_PK
             LEFT JOIN ZWAMESSAGEDATAITEM ON
                 ZWAMESSAGEDATAITEM.ZMESSAGE = ZWAMESSAGE.Z_PK;
-        """)
+        """
+        )
         names = [description[0] for description in cur.description]
 
         for message_row in cur:
             message = {}
             for index, value in enumerate(message_row):
                 message[names[index]] = value
 
-            message["isodate"] = convert_mactime_to_iso(
-                message.get("ZMESSAGEDATE"))
+            message["isodate"] = convert_mactime_to_iso(message.get("ZMESSAGEDATE"))
             message["ZTEXT"] = message["ZTEXT"] if message["ZTEXT"] else ""
 
             # Extract links from the WhatsApp message. URLs can be stored in
             # multiple fields/columns.
             # Check each of them!
             message_links = []
-            fields_with_links = ["ZTEXT", "ZMATCHEDTEXT", "ZMEDIAURL",
-                                 "ZCONTENT1", "ZCONTENT2"]
+            fields_with_links = [
+                "ZTEXT",
+                "ZMATCHEDTEXT",
+                "ZMEDIAURL",
+                "ZCONTENT1",
+                "ZCONTENT2",
+            ]
             for field in fields_with_links:
                 if message.get(field):
-                    message_links.extend(check_for_links(
-                        message.get(field, "")))
+                    message_links.extend(check_for_links(message.get(field, "")))
 
             # Remove WhatsApp internal media URLs.
             filtered_links = []
             for link in message_links:
-                if not (link.startswith("https://mmg-fna.whatsapp.net/")
-                        or link.startswith("https://mmg.whatsapp.net/")):
+                if not (
+                    link.startswith("https://mmg-fna.whatsapp.net/")
+                    or link.startswith("https://mmg.whatsapp.net/")
+                ):
                     filtered_links.append(link)
 
             # Add all the links found to the record
             if filtered_links or (message.get("ZTEXT") or "").strip() == "":
                 message["links"] = list(set(filtered_links))
             self.results.append(message)
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted a total of %d WhatsApp messages",
-                      len(self.results))
+        self.log.info("Extracted a total of %d WhatsApp messages", len(self.results))
```

### Comparing `mvt-2.2.6/mvt/ios/modules/net_base.py` & `mvt-2.3.0/mvt/ios/modules/net_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,32 @@
     modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: Optional[bool] = False,
+        fast_mode: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None
+        results: Optional[list] = None,
     ) -> None:
-        super().__init__(file_path=file_path, target_path=target_path,
-                         results_path=results_path, fast_mode=fast_mode,
-                         log=log, results=results)
+        super().__init__(
+            file_path=file_path,
+            target_path=target_path,
+            results_path=results_path,
+            fast_mode=fast_mode,
+            log=log,
+            results=results,
+        )
 
     def _extract_net_data(self):
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
-        cur.execute("""
+        cur.execute(
+            """
             SELECT
                 ZPROCESS.ZFIRSTTIMESTAMP,
                 ZPROCESS.ZTIMESTAMP,
                 ZPROCESS.ZPROCNAME,
                 ZPROCESS.ZBUNDLENAME,
                 ZPROCESS.Z_PK,
                 ZLIVEUSAGE.ZWIFIIN,
@@ -51,15 +57,16 @@
             FROM ZLIVEUSAGE
             LEFT JOIN ZPROCESS ON ZLIVEUSAGE.ZHASPROCESS = ZPROCESS.Z_PK
             UNION
             SELECT ZFIRSTTIMESTAMP, ZTIMESTAMP, ZPROCNAME, ZBUNDLENAME, Z_PK,
                    NULL, NULL, NULL, NULL, NULL, NULL, NULL
             FROM ZPROCESS WHERE Z_PK NOT IN
                 (SELECT ZHASPROCESS FROM ZLIVEUSAGE);
-        """)
+        """
+        )
 
         for row in cur:
             # ZPROCESS records can be missing after the JOIN.
             # Handle NULL timestamps.
             if row[0] and row[1]:
                 first_isodate = convert_mactime_to_iso(row[0])
                 isodate = convert_mactime_to_iso(row[1])
@@ -68,84 +75,97 @@
                 isodate = row[1]
 
             if row[11]:
                 live_timestamp = convert_mactime_to_iso(row[11])
             else:
                 live_timestamp = ""
 
-            self.results.append({
-                "first_isodate": first_isodate,
-                "isodate": isodate,
-                "proc_name": row[2],
-                "bundle_id": row[3],
-                "proc_id": row[4],
-                "wifi_in": row[5],
-                "wifi_out": row[6],
-                "wwan_in": row[7],
-                "wwan_out": row[8],
-                "live_id": row[9],
-                "live_proc_id": row[10],
-                "live_isodate": live_timestamp if row[10] else first_isodate,
-            })
+            self.results.append(
+                {
+                    "first_isodate": first_isodate,
+                    "isodate": isodate,
+                    "proc_name": row[2],
+                    "bundle_id": row[3],
+                    "proc_id": row[4],
+                    "wifi_in": row[5],
+                    "wifi_out": row[6],
+                    "wwan_in": row[7],
+                    "wwan_out": row[8],
+                    "live_id": row[9],
+                    "live_proc_id": row[10],
+                    "live_isodate": live_timestamp if row[10] else first_isodate,
+                }
+            )
 
         cur.close()
         conn.close()
 
-        self.log.info("Extracted information on %d processes",
-                      len(self.results))
+        self.log.info("Extracted information on %d processes", len(self.results))
 
     def serialize(self, record: dict) -> Union[dict, list]:
-        record_data = (f"{record['proc_name']} (Bundle ID: {record['bundle_id']},"
-                       f" ID: {record['proc_id']})")
-        record_data_usage = (record_data + " "
-                             f"WIFI IN: {record['wifi_in']}, "
-                             f"WIFI OUT: {record['wifi_out']} - "
-                             f"WWAN IN: {record['wwan_in']}, "
-                             f"WWAN OUT: {record['wwan_out']}")
-
-        records = [{
-            "timestamp": record["live_isodate"],
-            "module": self.__class__.__name__,
-            "event": "live_usage",
-            "data": record_data_usage,
-        }]
+        record_data = (
+            f"{record['proc_name']} (Bundle ID: {record['bundle_id']},"
+            f" ID: {record['proc_id']})"
+        )
+        record_data_usage = (
+            record_data + " "
+            f"WIFI IN: {record['wifi_in']}, "
+            f"WIFI OUT: {record['wifi_out']} - "
+            f"WWAN IN: {record['wwan_in']}, "
+            f"WWAN OUT: {record['wwan_out']}"
+        )
+
+        records = [
+            {
+                "timestamp": record["live_isodate"],
+                "module": self.__class__.__name__,
+                "event": "live_usage",
+                "data": record_data_usage,
+            }
+        ]
 
         # Only included first_usage and current_usage records when a
         # ZPROCESS entry exists.
-        if ("MANIPULATED" not in record["proc_name"]
-                and "MISSING" not in record["proc_name"]
-                and record["live_proc_id"] is not None):
-            records.extend([
-                {
-                    "timestamp": record["first_isodate"],
-                    "module": self.__class__.__name__,
-                    "event": "first_usage",
-                    "data": record_data,
-                },
-                {
-                    "timestamp": record["isodate"],
-                    "module": self.__class__.__name__,
-                    "event": "current_usage",
-                    "data": record_data,
-                }
-            ])
+        if (
+            "MANIPULATED" not in record["proc_name"]
+            and "MISSING" not in record["proc_name"]
+            and record["live_proc_id"] is not None
+        ):
+            records.extend(
+                [
+                    {
+                        "timestamp": record["first_isodate"],
+                        "module": self.__class__.__name__,
+                        "event": "first_usage",
+                        "data": record_data,
+                    },
+                    {
+                        "timestamp": record["isodate"],
+                        "module": self.__class__.__name__,
+                        "event": "current_usage",
+                        "data": record_data,
+                    },
+                ]
+            )
 
         return records
 
     def _find_suspicious_processes(self):
         if not self.is_fs_dump:
             return
 
         if not self.results:
             return
 
         # If we are instructed to run fast, we skip this.
         if self.fast_mode:
-            self.log.info("Flag --fast was enabled: skipping extended "
-                          "search for suspicious processes")
+            self.log.info(
+                "Flag --fast was enabled: skipping extended "
+                "search for suspicious processes"
+            )
             return
 
         self.log.info("Extended search for suspicious processes ...")
 
         files = []
         for posix_path in Path(self.target_path).rglob("*"):
             try:
@@ -154,77 +174,94 @@
             except PermissionError:
                 continue
 
             files.append([posix_path.name, str(posix_path)])
 
         for proc in self.results:
             if not proc["bundle_id"]:
-                self.log.debug("Found process with no Bundle ID with name: %s",
-                               proc["proc_name"])
+                self.log.debug(
+                    "Found process with no Bundle ID with name: %s", proc["proc_name"]
+                )
 
                 binary_path = None
                 for file in files:
                     if proc["proc_name"] == file[0]:
                         binary_path = file[1]
                         break
 
                 if binary_path:
                     self.log.debug("Located at %s", binary_path)
                 else:
-                    msg = ("Could not find the binary associated with the "
-                           f"process with name {proc['proc_name']}")
+                    msg = (
+                        "Could not find the binary associated with the "
+                        f"process with name {proc['proc_name']}"
+                    )
                     if not proc["proc_name"]:
-                        msg = ("Found process entry with empty 'proc_name': "
-                               f"{proc['live_proc_id']} at {proc['live_isodate']}")
+                        msg = (
+                            "Found process entry with empty 'proc_name': "
+                            f"{proc['live_proc_id']} at {proc['live_isodate']}"
+                        )
                     elif len(proc["proc_name"]) == 16:
-                        msg += (" (However, the process name might have "
-                                "been truncated in the database)")
+                        msg += (
+                            " (However, the process name might have "
+                            "been truncated in the database)"
+                        )
 
                     self.log.warning(msg)
             if not proc["live_proc_id"]:
-                self.log.info("Found process entry in ZPROCESS but not in ZLIVEUSAGE: %s at %s",
-                              proc['proc_name'], proc['live_isodate'])
+                self.log.info(
+                    "Found process entry in ZPROCESS but not in ZLIVEUSAGE: %s at %s",
+                    proc["proc_name"],
+                    proc["live_isodate"],
+                )
 
     def check_manipulated(self):
         """Check for missing or manipulate DB entries"""
         # Don't show duplicates for each missing process.
         missing_process_cache = set()
-        for result in sorted(
-                self.results, key=operator.itemgetter("live_isodate")):
+        for result in sorted(self.results, key=operator.itemgetter("live_isodate")):
             if result["proc_id"]:
                 continue
 
             # Avoid duplicate warnings for same process.
             if result["live_proc_id"] not in missing_process_cache:
                 missing_process_cache.add(result["live_proc_id"])
-                self.log.warning("Found manipulated process entry %s. Entry on %s",
-                                 result["live_proc_id"], result["live_isodate"])
+                self.log.warning(
+                    "Found manipulated process entry %s. Entry on %s",
+                    result["live_proc_id"],
+                    result["live_isodate"],
+                )
 
             # Set manipulated proc timestamp so it appears in timeline.
             result["first_isodate"] = result["isodate"] = result["live_isodate"]
             result["proc_name"] = "MANIPULATED [process record deleted]"
             self.detected.append(result)
 
     def find_deleted(self):
         """Identify process which may have been deleted from the DataUsage
         database."""
-        results_by_proc = {proc["proc_id"]: proc for proc in self.results if proc["proc_id"]}
+        results_by_proc = {
+            proc["proc_id"]: proc for proc in self.results if proc["proc_id"]
+        }
         all_proc_id = sorted(results_by_proc.keys())
 
         # Fix issue #108
         if not all_proc_id:
             return
 
         missing_procs, last_proc_id = {}, None
         for proc_id in range(min(all_proc_id), max(all_proc_id)):
             if proc_id not in all_proc_id:
                 previous_proc = results_by_proc[last_proc_id]
-                self.log.info("Missing process %d. Previous process at \"%s\" (%s)",
-                              proc_id, previous_proc["first_isodate"],
-                              previous_proc["proc_name"])
+                self.log.info(
+                    'Missing process %d. Previous process at "%s" (%s)',
+                    proc_id,
+                    previous_proc["first_isodate"],
+                    previous_proc["proc_name"],
+                )
 
                 missing_procs[proc_id] = {
                     "proc_id": proc_id,
                     "prev_proc_id": last_proc_id,
                     "prev_proc_name": previous_proc["proc_name"],
                     "prev_proc_bundle": previous_proc["bundle_id"],
                     "prev_proc_first": previous_proc["first_isodate"],
@@ -232,23 +269,24 @@
             else:
                 last_proc_id = proc_id
 
         # Add a placeholder entry for the missing processes.
         for proc_id, proc in missing_procs.items():
             # Set default DataUsage keys.
             result = {key: None for key in self.results[0].keys()}
-            result["first_isodate"] = result["isodate"] = result["live_isodate"] = proc["prev_proc_first"]
+            result["first_isodate"] = result["isodate"] = result["live_isodate"] = proc[
+                "prev_proc_first"
+            ]
             result["proc_name"] = f"MISSING [follows {proc['prev_proc_name']}]"
             result["proc_id"] = result["live_proc_id"] = proc["proc_id"]
             result["bundle_id"] = None
 
             self.results.append(result)
 
-        self.results = sorted(self.results,
-                              key=operator.itemgetter("first_isodate"))
+        self.results = sorted(self.results, key=operator.itemgetter("first_isodate"))
 
     def check_indicators(self) -> None:
         # Check for manipulated process records.
         # TODO: Catching KeyError for live_isodate for retro-compatibility.
         #       This is not very good.
         try:
             self.check_manipulated()
```

### Comparing `mvt-2.2.6/mvt.egg-info/SOURCES.txt` & `mvt-2.3.0/mvt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 ./mvt/common/virustotal.py
 ./mvt/ios/__init__.py
 ./mvt/ios/cli.py
 ./mvt/ios/cmd_check_backup.py
 ./mvt/ios/cmd_check_fs.py
 ./mvt/ios/decrypt.py
 ./mvt/ios/versions.py
+./mvt/ios/data/ios_models.json
+./mvt/ios/data/ios_versions.json
 ./mvt/ios/modules/__init__.py
 ./mvt/ios/modules/base.py
 ./mvt/ios/modules/net_base.py
 ./mvt/ios/modules/backup/__init__.py
 ./mvt/ios/modules/backup/backup_info.py
 ./mvt/ios/modules/backup/configuration_profiles.py
 ./mvt/ios/modules/backup/manifest.py
@@ -136,32 +138,37 @@
 ./tests/test_check_android_bugreport.py
 ./tests/test_check_ios_backup.py
 ./tests/test_ios_versions.py
 ./tests/utils.py
 ./tests/android/__init__.py
 ./tests/android/test_backup_module.py
 ./tests/android/test_backup_parser.py
-./tests/android/test_bugreport.py
 ./tests/android/test_dumpsys_parser.py
 ./tests/android_androidqf/__init__.py
 ./tests/android_androidqf/test_dumpsysaccessbility.py
 ./tests/android_androidqf/test_dumpsysappops.py
 ./tests/android_androidqf/test_dumpsyspackages.py
 ./tests/android_androidqf/test_dumpsysreceivers.py
 ./tests/android_androidqf/test_getprop.py
 ./tests/android_androidqf/test_processes.py
 ./tests/android_androidqf/test_settings.py
 ./tests/android_androidqf/test_sms.py
+./tests/android_bugreport/__init__.py
+./tests/android_bugreport/test_bugreport.py
 ./tests/common/__init__.py
 ./tests/common/test_indicators.py
 ./tests/common/test_utils.py
 ./tests/ios_backup/__init__.py
 ./tests/ios_backup/test_backup_info.py
 ./tests/ios_backup/test_calendar.py
 ./tests/ios_backup/test_datausage.py
 ./tests/ios_backup/test_manifest.py
 ./tests/ios_backup/test_safari_browserstate.py
 ./tests/ios_backup/test_sms.py
 ./tests/ios_backup/test_tcc.py
 ./tests/ios_backup/test_webkit_resource_load_statistics.py
 ./tests/ios_fs/__init__.py
-./tests/ios_fs/test_filesystem.py
+./tests/ios_fs/test_filesystem.py
+tests/test_check_android_androidqf.py
+tests/test_check_android_bugreport.py
+tests/test_check_ios_backup.py
+tests/test_ios_versions.py
```

### Comparing `mvt-2.2.6/setup.cfg` & `mvt-2.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -29,33 +29,38 @@
 	packaging >=21.3
 	appdirs >=1.4.4
 	iOSbackup >=0.9.923
 	adb-shell >=0.4.3
 	libusb1 >=3.0.0
 	cryptography >=38.0.1
 	pyyaml >=6.0
+	pyahocorasick >= 2.0.0
 
 [options.packages.find]
 where = ./
 
 [options.entry_points]
 console_scripts = 
 	mvt-ios = mvt.ios:cli
 	mvt-android = mvt.android:cli
 
+[options.package_data]
+mvt = ios/data/*.json
+
 [flake8]
 max-complexity = 10
 max-line-length = 1000
 ignore = 
 	C901,
 	E265,
 	F401,
 	E127,
 	W503,
-	E226
+	E226,
+	E203
 
 [pylint]
 score = no
 reports = no
 output-format = colorized
 max-locals = 25
 max-args = 10
@@ -75,11 +80,14 @@
 	missing-module-docstring,
 	missing-class-docstring,
 	missing-function-docstring,
 
 [mypy]
 ignore_missing_imports = True
 
+[isort]
+profile = black
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mvt-2.2.6/tests/android/test_backup_module.py` & `mvt-2.3.0/tests/android/test_backup_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from mvt.android.parsers.backup import parse_backup_file
 from mvt.common.module import run_module
 
 from ..utils import get_android_backup_folder
 
 
 class TestBackupModule:
-
     def test_module_folder(self):
         backup_path = get_android_backup_folder()
         mod = SMS(target_path=backup_path)
         files = []
         for root, subdirs, subfiles in os.walk(os.path.abspath(backup_path)):
             for fname in subfiles:
                 files.append(os.path.relpath(os.path.join(root, fname), backup_path))
```

### Comparing `mvt-2.2.6/tests/android/test_backup_parser.py` & `mvt-2.3.0/tests/android/test_backup_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,53 +7,61 @@
 
 from mvt.android.parsers.backup import parse_backup_file, parse_tar_for_sms
 
 from ..utils import get_artifact
 
 
 class TestBackupParsing:
-
     def test_parsing_noencryption(self):
         file = get_artifact("android_backup/backup.ab")
         with open(file, "rb") as f:
             data = f.read()
         ddata = parse_backup_file(data)
 
         m = hashlib.sha256()
         m.update(ddata)
-        assert m.hexdigest() == "ce1ac5009fea5187a9f546b51e1446ba450243ae91d31dc779233ec0937b5d18"
+        assert (
+            m.hexdigest()
+            == "ce1ac5009fea5187a9f546b51e1446ba450243ae91d31dc779233ec0937b5d18"
+        )
         sms = parse_tar_for_sms(ddata)
         assert isinstance(sms, list)
         assert len(sms) == 2
         assert len(sms[0]["links"]) == 1
         assert sms[0]["links"][0] == "http://google.com"
 
     def test_parsing_encryption(self):
         file = get_artifact("android_backup/backup2.ab")
         with open(file, "rb") as f:
             data = f.read()
         ddata = parse_backup_file(data, password="123456")
 
         m = hashlib.sha256()
         m.update(ddata)
-        assert m.hexdigest() == "f365ace1effbc4902c6aeba241ca61544f8a96ad456c1861808ea87b7dd03896"
+        assert (
+            m.hexdigest()
+            == "f365ace1effbc4902c6aeba241ca61544f8a96ad456c1861808ea87b7dd03896"
+        )
         sms = parse_tar_for_sms(ddata)
         assert isinstance(sms, list)
         assert len(sms) == 1
         assert len(sms[0]["links"]) == 1
         assert sms[0]["links"][0] == "https://google.com/"
 
     def test_parsing_compression(self):
         file = get_artifact("android_backup/backup3.ab")
         with open(file, "rb") as f:
             data = f.read()
         ddata = parse_backup_file(data)
 
         m = hashlib.sha256()
         m.update(ddata)
-        assert m.hexdigest() == "33e73df2ede9798dcb3a85c06200ee41c8f52dd2f2e50ffafcceb0407bc13e3a"
+        assert (
+            m.hexdigest()
+            == "33e73df2ede9798dcb3a85c06200ee41c8f52dd2f2e50ffafcceb0407bc13e3a"
+        )
         sms = parse_tar_for_sms(ddata)
         print(sms)
         assert isinstance(sms, list)
         assert len(sms) == 1
         assert len(sms[0]["links"]) == 1
         assert sms[0]["links"][0] == "https://google.com/"
```

### Comparing `mvt-2.2.6/tests/android/test_bugreport.py` & `mvt-2.3.0/tests/android_bugreport/test_bugreport.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,40 +3,49 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import os
 from pathlib import Path
 
 from mvt.android.modules.bugreport.appops import Appops
+from mvt.android.modules.bugreport.getprop import Getprop
 from mvt.android.modules.bugreport.packages import Packages
 from mvt.common.module import run_module
 
 from ..utils import get_artifact_folder
 
 
 class TestBugreportAnalysis:
-
     def launch_bug_report_module(self, module):
         fpath = os.path.join(get_artifact_folder(), "android_data/bugreport/")
         m = module(target_path=fpath)
         folder_files = []
         parent_path = Path(fpath).absolute().as_posix()
         for root, subdirs, subfiles in os.walk(os.path.abspath(fpath)):
             for file_name in subfiles:
-                folder_files.append(os.path.relpath(os.path.join(root, file_name), parent_path))
+                folder_files.append(
+                    os.path.relpath(os.path.join(root, file_name), parent_path)
+                )
         m.from_folder(fpath, folder_files)
         run_module(m)
         return m
 
     def test_appops_module(self):
         m = self.launch_bug_report_module(Appops)
         assert len(m.results) == 12
         assert len(m.timeline) == 16
         assert len(m.detected) == 0
 
     def test_packages_module(self):
         m = self.launch_bug_report_module(Packages)
         assert len(m.results) == 2
-        assert m.results[0]["package_name"] == "com.samsung.android.provider.filterprovider"
+        assert (
+            m.results[0]["package_name"]
+            == "com.samsung.android.provider.filterprovider"
+        )
         assert m.results[1]["package_name"] == "com.instagram.android"
         assert len(m.results[0]["permissions"]) == 4
         assert len(m.results[1]["permissions"]) == 32
+
+    def test_getprop_module(self):
+        m = self.launch_bug_report_module(Getprop)
+        assert len(m.results) == 0
```

### Comparing `mvt-2.2.6/tests/android/test_dumpsys_parser.py` & `mvt-2.3.0/tests/android/test_dumpsys_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
-from mvt.android.parsers.dumpsys import (parse_dumpsys_appops,
-                                         parse_dumpsys_battery_history,
-                                         parse_dumpsys_packages)
+from mvt.android.parsers.dumpsys import (
+    parse_dumpsys_appops,
+    parse_dumpsys_battery_history,
+    parse_dumpsys_packages,
+)
 
 from ..utils import get_artifact
 
 
 class TestDumpsysParsing:
-
     def test_appops_parsing(self):
         file = get_artifact("android_data/dumpsys_appops.txt")
         with open(file) as f:
             data = f.read()
 
         res = parse_dumpsys_appops(data)
```

### Comparing `mvt-2.2.6/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.3.0/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
-from mvt.android.modules.androidqf.dumpsys_accessibility import \
-    DumpsysAccessibility
+from mvt.android.modules.androidqf.dumpsys_accessibility import DumpsysAccessibility
 from mvt.common.module import run_module
 
 from ..utils import get_android_androidqf
 
 
 class TestDumpsysAccessibilityModule:
     def test_parsing(self):
```

### Comparing `mvt-2.2.6/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.3.0/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.3.0/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     def test_parsing(self):
         data_path = get_android_androidqf()
         m = DumpsysPackages(target_path=data_path)
         run_module(m)
         assert len(m.results) == 2
         assert len(m.detected) == 0
         assert len(m.timeline) == 6
-        assert m.results[0]["package_name"] == "com.samsung.android.provider.filterprovider"
+        assert (
+            m.results[0]["package_name"]
+            == "com.samsung.android.provider.filterprovider"
+        )
 
     def test_detection_pkgname(self, indicator_file):
         data_path = get_android_androidqf()
         m = DumpsysPackages(target_path=data_path)
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         ind.ioc_collections[0]["app_ids"].append("com.sec.android.app.DataCreate")
```

### Comparing `mvt-2.2.6/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.3.0/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/tests/android_androidqf/test_getprop.py` & `mvt-2.3.0/tests/android_androidqf/test_getprop.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 from mvt.common.indicators import Indicators
 from mvt.common.module import run_module
 
 from ..utils import get_artifact_folder
 
 
 class TestAndroidqfGetpropAnalysis:
-
     def test_androidqf_getprop(self):
-        m = Getprop(target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging)
+        m = Getprop(
+            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
+        )
         run_module(m)
         assert len(m.results) == 10
         assert m.results[0]["name"] == "dalvik.vm.appimageformat"
         assert m.results[0]["value"] == "lz4"
         assert len(m.timeline) == 0
         assert len(m.detected) == 0
 
     def test_androidqf_getprop_detection(self, indicator_file):
-        m = Getprop(target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging)
+        m = Getprop(
+            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
+        )
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         ind.ioc_collections[0]["android_property_names"].append("dalvik.vm.heapmaxfree")
         m.indicators = ind
         run_module(m)
         assert len(m.results) == 10
         assert len(m.detected) == 1
```

### Comparing `mvt-2.2.6/tests/android_androidqf/test_processes.py` & `mvt-2.3.0/tests/android_androidqf/test_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 from mvt.common.module import run_module
 
 from ..utils import get_artifact_folder
 
 
 class TestAndroidqfProcessesAnalysis:
     def test_androidqf_processes(self):
-        m = Processes(target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging)
+        m = Processes(
+            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
+        )
         run_module(m)
         assert len(m.results) == 15
         assert len(m.timeline) == 0
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/android_androidqf/test_settings.py` & `mvt-2.3.0/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/tests/android_androidqf/test_sms.py` & `mvt-2.3.0/tests/android_androidqf/test_sms.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 from mvt.common.module import run_module
 
 from ..utils import get_artifact_folder
 
 
 class TestAndroidqfSMSAnalysis:
     def test_androidqf_sms(self):
-        m = SMS(target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging)
+        m = SMS(
+            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
+        )
         run_module(m)
         assert len(m.results) == 2
         assert len(m.timeline) == 0
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/common/test_indicators.py` & `mvt-2.3.0/tests/common/test_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import os
 
 from mvt.common.indicators import Indicators
 
 
 class TestIndicators:
-
     def test_parse_stix2(self, indicator_file):
         ind = Indicators(log=logging)
         ind.load_indicators_files([indicator_file], load_default=False)
         assert ind.ioc_collections[0]["count"] == 5
         assert len(ind.ioc_collections[0]["domains"]) == 1
         assert len(ind.ioc_collections[0]["emails"]) == 1
         assert len(ind.ioc_collections[0]["file_names"]) == 1
```

### Comparing `mvt-2.2.6/tests/common/test_utils.py` & `mvt-2.3.0/tests/common/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 # Copyright (c) 2021-2022 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import os
 
-from mvt.common.utils import (convert_datetime_to_iso, convert_mactime_to_iso,
-                              convert_unix_to_iso,
-                              convert_unix_to_utc_datetime,
-                              generate_hashes_from_path,
-                              get_sha256_from_file_path)
+from mvt.common.utils import (
+    convert_datetime_to_iso,
+    convert_mactime_to_iso,
+    convert_unix_to_iso,
+    convert_unix_to_utc_datetime,
+    generate_hashes_from_path,
+    get_sha256_from_file_path,
+)
 
 from ..utils import get_artifact_folder
 
 TEST_DATE_EPOCH = 1626566400
 TEST_DATE_ISO = "2021-07-18 00:00:00.000000"
 TEST_DATE_MAC = TEST_DATE_EPOCH - 978307200
 
 
 class TestDateConversions:
-
     def test_convert_unix_to_iso(self):
         assert convert_unix_to_iso(TEST_DATE_EPOCH) == TEST_DATE_ISO
 
     def test_convert_mactime_to_iso(self):
         assert convert_mactime_to_iso(TEST_DATE_MAC) == TEST_DATE_ISO
 
     def test_convert_unix_to_utc_datetime(self):
@@ -35,23 +37,30 @@
 
     def test_convert_datetime_to_iso(self):
         converted = convert_unix_to_utc_datetime(TEST_DATE_EPOCH)
         assert convert_datetime_to_iso(converted) == TEST_DATE_ISO
 
 
 class TestHashes:
-
     def test_hash_from_file(self):
         path = os.path.join(get_artifact_folder(), "androidqf", "backup.ab")
         sha256 = get_sha256_from_file_path(path)
-        assert sha256 == "f0e32fe8a7fd5ac0e2de19636d123c0072e979396986139ba2bc49ec385dc325"
+        assert (
+            sha256 == "f0e32fe8a7fd5ac0e2de19636d123c0072e979396986139ba2bc49ec385dc325"
+        )
 
     def test_hash_from_folder(self):
         path = os.path.join(get_artifact_folder(), "androidqf")
         hashes = list(generate_hashes_from_path(path, logging))
         assert len(hashes) == 5
         # Sort the files to have reliable order for tests.
         hashes = sorted(hashes, key=lambda x: x["file_path"])
         assert hashes[0]["file_path"] == os.path.join(path, "backup.ab")
-        assert hashes[0]["sha256"] == "f0e32fe8a7fd5ac0e2de19636d123c0072e979396986139ba2bc49ec385dc325"
+        assert (
+            hashes[0]["sha256"]
+            == "f0e32fe8a7fd5ac0e2de19636d123c0072e979396986139ba2bc49ec385dc325"
+        )
         assert hashes[1]["file_path"] == os.path.join(path, "dumpsys.txt")
-        assert hashes[1]["sha256"] == "bac858001784657a43c7cfa771fd1fc4a49428eb6b7c458a1ebf2fdeef78dd86"
+        assert (
+            hashes[1]["sha256"]
+            == "bac858001784657a43c7cfa771fd1fc4a49428eb6b7c458a1ebf2fdeef78dd86"
+        )
```

### Comparing `mvt-2.2.6/tests/conftest.py` & `mvt-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.2.6/tests/ios_backup/test_backup_info.py` & `mvt-2.3.0/tests/ios_backup/test_backup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,12 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.backup.backup_info import BackupInfo
 
 from ..utils import get_ios_backup_folder
 
 
 class TestBackupInfoModule:
-
     def test_manifest(self):
         m = BackupInfo(target_path=get_ios_backup_folder())
         run_module(m)
         assert m.results["Build Version"] == "18C66"
         assert m.results["IMEI"] == "42"
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_calendar.py` & `mvt-2.3.0/tests/ios_backup/test_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.mixed.calendar import Calendar
 
 from ..utils import get_ios_backup_folder
 
 
 class TestCalendarModule:
-
     def test_calendar(self):
         m = Calendar(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 1
         assert len(m.timeline) == 4
         assert len(m.detected) == 0
         assert m.results[0]["summary"] == "Super interesting meeting"
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_datausage.py` & `mvt-2.3.0/tests/ios_backup/test_datausage.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.mixed.net_datausage import Datausage
 
 from ..utils import get_ios_backup_folder
 
 
 class TestDatausageModule:
-
     def test_datausage(self):
         m = Datausage(target_path=get_ios_backup_folder())
         run_module(m)
         assert m.results[0]["isodate"][0:19] == "2019-08-27 15:08:09"
         assert len(m.results) == 42
         assert len(m.timeline) == 60
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_manifest.py` & `mvt-2.3.0/tests/ios_backup/test_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.backup.manifest import Manifest
 
 from ..utils import get_ios_backup_folder
 
 
 class TestManifestModule:
-
     def test_manifest(self):
         m = Manifest(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 3721
         assert len(m.timeline) == 5881
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.3.0/tests/ios_backup/test_safari_browserstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.mixed.safari_browserstate import SafariBrowserState
 
 from ..utils import get_ios_backup_folder
 
 
 class TestSafariBrowserStateModule:
-
     def test_parsing(self):
         m = SafariBrowserState(target_path=get_ios_backup_folder())
         m.is_backup = True
         run_module(m)
         assert len(m.results) == 1
         assert len(m.timeline) == 1
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_sms.py` & `mvt-2.3.0/tests/ios_backup/test_sms.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.mixed.sms import SMS
 
 from ..utils import get_ios_backup_folder
 
 
 class TestSMSModule:
-
     def test_sms(self):
         m = SMS(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 1
         assert len(m.timeline) == 1
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_tcc.py` & `mvt-2.3.0/tests/ios_backup/test_tcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.mixed.tcc import TCC
 
 from ..utils import get_ios_backup_folder
 
 
 class TestTCCtModule:
-
     def test_tcc(self):
         m = TCC(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 11
         assert len(m.timeline) == 11
         assert len(m.detected) == 0
         assert m.results[0]["service"] == "kTCCServiceUbiquity"
```

### Comparing `mvt-2.2.6/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.3.0/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 from mvt.common.module import run_module
-from mvt.ios.modules.mixed.webkit_resource_load_statistics import \
-    WebkitResourceLoadStatistics
+from mvt.ios.modules.mixed.webkit_resource_load_statistics import (
+    WebkitResourceLoadStatistics,
+)
 
 from ..utils import get_ios_backup_folder
 
 
 class TestWebkitResourceLoadStatisticsModule:
-
     def test_webkit(self):
         m = WebkitResourceLoadStatistics(target_path=get_ios_backup_folder())
         m.is_backup = True
         run_module(m)
         assert len(m.results) == 2
         assert len(m.timeline) == 2
         assert len(m.detected) == 0
```

### Comparing `mvt-2.2.6/tests/ios_fs/test_filesystem.py` & `mvt-2.3.0/tests/ios_fs/test_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 from mvt.common.module import run_module
 from mvt.ios.modules.fs.filesystem import Filesystem
 
 from ..utils import get_ios_backup_folder
 
 
 class TestFilesystem:
-
     def test_filesystem(self):
         m = Filesystem(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 14
         assert len(m.timeline) == 14
         assert len(m.detected) == 0
 
     def test_detection(self, indicator_file):
         m = Filesystem(target_path=get_ios_backup_folder())
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         # Adds a filename that exist in the folder
-        ind.ioc_collections[0]["processes"].append("64d0019cb3d46bfc8cce545a8ba54b93e7ea9347")
+        ind.ioc_collections[0]["processes"].append(
+            "64d0019cb3d46bfc8cce545a8ba54b93e7ea9347"
+        )
         m.indicators = ind
         run_module(m)
         assert len(m.results) == 14
         assert len(m.timeline) == 14
         assert len(m.detected) == 1
```

### Comparing `mvt-2.2.6/tests/test_check_android_androidqf.py` & `mvt-2.3.0/tests/test_check_android_androidqf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 
 from mvt.android.cli import check_androidqf
 
 from .utils import get_artifact_folder
 
 
 class TestCheckAndroidqfCommand:
-
     def test_check(self):
         runner = CliRunner()
         path = os.path.join(get_artifact_folder(), "androidqf")
         result = runner.invoke(check_androidqf, [path])
         assert result.exit_code == 0
```

### Comparing `mvt-2.2.6/tests/test_check_android_bugreport.py` & `mvt-2.3.0/tests/test_check_android_bugreport.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 
 from mvt.android.cli import check_bugreport
 
 from .utils import get_artifact_folder
 
 
 class TestCheckBugreportCommand:
-
     def test_check(self):
         runner = CliRunner()
         path = os.path.join(get_artifact_folder(), "android_data/bugreport/")
         result = runner.invoke(check_bugreport, [path])
         assert result.exit_code == 0
```

### Comparing `mvt-2.2.6/tests/test_check_ios_backup.py` & `mvt-2.3.0/tests/test_check_ios_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,12 @@
 
 from mvt.ios.cli import check_backup
 
 from .utils import get_ios_backup_folder
 
 
 class TestCheckBackupCommand:
-
     def test_check(self):
         runner = CliRunner()
         path = get_ios_backup_folder()
         result = runner.invoke(check_backup, [path])
         assert result.exit_code == 0
```

### Comparing `mvt-2.2.6/tests/utils.py` & `mvt-2.3.0/tests/utils.py`

 * *Files identical despite different names*

