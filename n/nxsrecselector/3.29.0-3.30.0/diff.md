# Comparing `tmp/nxsrecselector-3.29.0.tar.gz` & `tmp/nxsrecselector-3.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.29.0.tar", last modified: Wed Jun  7 08:19:18 2023, max compression
+gzip compressed data, was "nxsrecselector-3.30.0.tar", last modified: Thu Jun 29 12:49:32 2023, max compression
```

## Comparing `nxsrecselector-3.29.0.tar` & `nxsrecselector-3.30.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.29.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.29.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.29.0/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7058 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4303 2023-06-07 07:08:17.000000 nxsrecselector-3.29.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.29.0/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.29.0/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 07:18:20.000000 nxsrecselector-3.29.0/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.29.0/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 07:18:50.000000 nxsrecselector-3.29.0/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    75512 2023-06-07 07:18:35.000000 nxsrecselector-3.29.0/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.29.0/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-07 07:15:39.000000 nxsrecselector-3.29.0/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.29.0/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    44983 2023-06-02 09:06:46.000000 nxsrecselector-3.29.0/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.29.0/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.29.0/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7058 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.29.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.30.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.30.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.30.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7068 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.30.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.048490 nxsrecselector-3.30.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.30.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.30.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 08:45:59.000000 nxsrecselector-3.30.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.30.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 08:45:59.000000 nxsrecselector-3.30.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    75699 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59493 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.30.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45630 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.30.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.30.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7068 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-29 12:49:32.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.30.0/setup.py
```

### Comparing `nxsrecselector-3.29.0/COPYRIGHT` & `nxsrecselector-3.30.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/NXSRecSelector` & `nxsrecselector-3.30.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/PKG-INFO` & `nxsrecselector-3.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.29.0
+Version: 3.30.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -62,29 +62,29 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
+        Debian bookworm, bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally, install module
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.29.0/README.rst` & `nxsrecselector-3.30.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -54,29 +54,29 @@
 .. code-block:: console
 
 	  $ python setup.py install
 
 Debian packages
 ^^^^^^^^^^^^^^^
 
-Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
+Debian bookworm, bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
 	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
 
 and then download the corresponding source list
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
 
 Finally, install module
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.29.0/man/NXSRecSelector.1` & `nxsrecselector-3.30.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/man/nxsrecconfig.1` & `nxsrecselector-3.30.0/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.30.0/nxsrecconfig/CheckerThread.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Converter.py` & `nxsrecselector-3.30.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Describer.py` & `nxsrecselector-3.30.0/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.30.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.30.0/nxsrecconfig/MacroServerPools.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.30.0/nxsrecconfig/NXSConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                          defaultzone, defaultmntgrp, syncsnapshot,
                          writepoolmotorpositions)
         self.set_state(tango.DevState.ON)
         self.__stg.poolBlacklist = self.PoolBlacklist or []
         self.__stg.timerFilters = self.TimerFilters or [
             "*dgg*", "*/timer/*", "*/ctctrl0*"]
         self.__stg.masterTimerFirst = bool(self.MasterTimerFirst)
+        self.__stg.masterTimer = bool(self.MasterTimer)
         self.__stg.mutedChannelFilters = self.MutedChannelFilters \
             or ["*tip551*"]
         self.__stg.mutedPreScanAttrFilters = self.MutedPreScanAttrFilters or []
         self.__stg.adminDataNames = self.AdminDataNames or []
         self.__stg.defaultPreselectedComponents = \
             self.DefaultPreselectedComponents or []
         self.__stg.defaultCanFailDataSources = \
@@ -1887,14 +1888,18 @@
         [tango.DevBoolean,
          "add dynamic components for all pool motor positions",
          [False]],
         'MasterTimerFirst':
         [tango.DevBoolean,
          "the master timer channel of MG with the index: 0",
          [False]],
+        'MasterTimer':
+        [tango.DevBoolean,
+         "set the master timer/monitor channel for older MG",
+         [False]],
         'DefaultCanFailDataSources':
         [tango.DevVarStringArray,
          "list of default datasources in the CanFail mode",
          []],
         'TangoSourceErrorStates':
         [tango.DevVarStringArray,
          "list of tango error states for tango datasources",
```

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.30.0/nxsrecconfig/ProfileManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         self.timerFilters = ["*dgg*", "*/timer/*", "*/ctctrl0*"]
 
         #:  (:obj:`list` <:obj:`str`>) muted PreScan attribute filters
         self.mutedPreScanAttrFilters = []
 
         #: (:obj:`bool` ) master timer/monitor with the first index
         self.masterTimerFirst = False
+        #: (:obj:`bool` ) set master timer/monitor like for older MGs
+        self.masterTimer = False
         #: (:obj:`bool`) mntgrp with synchronization
         self.__withsynch = True
 
         #: (:obj:`bool`) preselection merges current ScanSnapshot
         self.__syncsnapshot = syncsnapshot
 
         #: (:obj:`bool`) add dynamic components for all pool motor positions
@@ -624,15 +626,16 @@
         synchronizer = {}
         # synchronization = props["synchronization"] \
         #     if "synchronization" in props.keys() else {}
         synchronization = {}
         self.__clearChannels(dsg, hel, compdatasources)
 
         # fill in dsg, timers hel
-        if "timer" in conf.keys() and "controllers" in conf.keys():
+        if "controllers" in conf.keys() and \
+           (not self.masterTimer or "timer" in conf.keys()):
             avtimers = PoolUtils.getTimers(self.__pools, self.timerFilters)
             tangods = self.__readChannels(
                 conf, timers, dsg, hel, synchronizer, synchronization)
             self.__readTangoChannels(
                 conf, tangods, dsg, hel, synchronizer, synchronization)
             otimers = self.__reorderTimers(conf, timers, dsg, hel, avtimers)
 
@@ -687,16 +690,15 @@
 
         for ch in channels:
             if ch in dsg.keys():
                 dsg[ch] = False
             if ch in hel:
                 hel.remove(ch)
 
-    @classmethod
-    def __readChannels(cls, conf, timers, dsg, hel, synchronizer,
+    def __readChannels(self, conf, timers, dsg, hel, synchronizer,
                        synchronization):
         """ reads channels from mntgrp configutation
 
         :param conf: mntgrp configuration
         :type jconf: :obj:`str`
         :param timers: timer dictionary
         :type timers: :obj:`dict` <:obj:`str`, :obj:`str`>
@@ -709,15 +711,16 @@
         :param synchronization: channel synchronization,
                 i.e. Trigger=0, Gate=1, Start=2
         :type synchronization: :obj:`dict` <:obj:`str`, :obj:`int`>
         :returns: tango datasources list with elements (name, label, source)
         :rtype: :obj:`list` < [:obj:`str` , :obj:`str` , :obj:`str` ] >
         """
         tangods = []
-        timers[conf["timer"]] = ''
+        if self.masterTimer:
+            timers[conf["timer"]] = ''
         for ctrlname, ctrl in conf["controllers"].items():
             if 'units' in ctrl.keys() and \
                     '0' in ctrl['units'].keys():
                 uctrl = ctrl['units']['0']
             else:
                 uctrl = ctrl
             if 'timer' in uctrl.keys():
@@ -806,18 +809,18 @@
         :type avtimers :obj:`list` <:obj:`str`>
         :returns: timer alias list
         :rtype: :obj:`list` <:obj:`str`>
         """
         dtimers = PoolUtils.getAliases(self.__pools, timers)
         avtimers = avtimers or []
         otimers = [tm for tm in dtimers.values() if tm in avtimers]
-        if dtimers[conf["timer"]] in otimers:
+        if "timer" in conf and dtimers[conf["timer"]] in otimers:
             otimers.remove(dtimers[conf["timer"]])
             otimers.insert(0, dtimers[conf["timer"]])
-        elif not otimers:
+        elif "timer" in conf and not otimers:
             otimers.insert(0, dtimers[conf["timer"]])
 
         tms = json.loads(self.__selector["Timer"])
         tms.extend(otimers)
 
         for tm in tms:
             if tm in hel:
@@ -928,24 +931,25 @@
         """
         mtimers = json.loads(self.__selector["Timer"])
         #   avtimers = PoolUtils.getTimers(self.__pools, self.timerFilters)
         #   mtimers = mtimers or []
         #   mtimers = [tm for tm in mtimers if tm in avtimers]
 
         timer = mtimers[0] if mtimers else ''
-        if not timer:
-            raise Exception(
-                "Timer or Monitor not defined")
-        fullname = PoolUtils.getFullDeviceNames(
-            self.__pools, [timer])[timer]
-        if not fullname:
-            raise Exception(
-                "Timer or Monitor cannot be found amount the servers")
-        cnf['monitor'] = fullname
-        cnf['timer'] = fullname
+        if self.masterTimer:
+            if not timer:
+                raise Exception(
+                    "Timer or Monitor not defined")
+            fullname = PoolUtils.getFullDeviceNames(
+                self.__pools, [timer])[timer]
+            if not fullname:
+                raise Exception(
+                    "Timer or Monitor cannot be found amount the servers")
+            cnf['monitor'] = fullname
+            cnf['timer'] = fullname
         if len(mtimers) > 1:
             ltimers.clear()
             ltimers.update(set(mtimers[1:]))
             if timer in ltimers:
                 ltimers.remove(timer)
         return timer
```

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Release.py` & `nxsrecselector-3.30.0/nxsrecconfig/Release.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.29.0"
+__version__ = "3.30.0"
```

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Selection.py` & `nxsrecselector-3.30.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Selector.py` & `nxsrecselector-3.30.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Settings.py` & `nxsrecselector-3.30.0/nxsrecconfig/Settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -446,14 +446,36 @@
 
     #: (:obj:`bool`) master channels with the 0 index
     masterTimerFirst = property(
         __getMasterTimerFirst,
         __setMasterTimerFirst,
         doc='master timer channels with the 0 index')
 
+    def __getMasterTimer(self):
+        """ get method for masterTimer attribute
+
+        :returns: master channels with the 0 index
+        :rtype: :obj:`bool`
+        """
+        return self.__profileManager.masterTimer
+
+    def __setMasterTimer(self, flag):
+        """ set method for masterTimer attribute
+
+        :param components: master channels with the 0 index
+        :type components: :obj:`bool`
+        """
+        self.__profileManager.masterTimer = flag
+
+    #: (:obj:`bool`) set master channels
+    masterTimer = property(
+        __getMasterTimer,
+        __setMasterTimer,
+        doc='set master timer/monitor for older MGs')
+
     def __getConfigDevice(self):
         """ get method for configDevice attribute
 
         :returns: name of configDevice
         :rtype: :obj:`str`
         """
         return self.__selector["ConfigDevice"]
```

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.30.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/Utils.py` & `nxsrecselector-3.30.0/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecconfig/__init__.py` & `nxsrecselector-3.30.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.30.0/nxsrecselector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.29.0
+Version: 3.30.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -62,29 +62,29 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
+        Debian bookworm, bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally, install module
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.29.0/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.30.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.29.0/setup.py` & `nxsrecselector-3.30.0/setup.py`

 * *Files identical despite different names*

