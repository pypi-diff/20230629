# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.9.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.9.tar", last modified: Tue May 16 01:57:42 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.3.1b0.tar", last modified: Thu Jun 29 15:08:32 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.9.tar` & `com.castsoftware.uc.oneclick-0.2.3.1b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.169070 com.castsoftware.uc.oneclick-0.2.2.9/
--rw-rw-rw-   0        0        0      517 2023-05-16 01:57:42.159360 com.castsoftware.uc.oneclick-0.2.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 01:57:41.871522 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 01:57:41.000000 com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.004331 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.057857 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3914 2023-05-13 12:48:37.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19803 2023-05-15 16:57:12.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:57:42.146823 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4432 2023-05-13 21:26:47.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7052 2023-05-13 21:24:21.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     8411 2023-05-15 20:34:04.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-13 12:48:23.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    10978 2023-05-13 14:37:06.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-05-15 16:56:38.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     6003 2023-05-15 13:33:19.000000 com.castsoftware.uc.oneclick-0.2.2.9/oneclick/setup.py
--rw-rw-rw-   0        0        0      752 2023-05-16 01:57:16.000000 com.castsoftware.uc.oneclick-0.2.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 01:57:42.169070 com.castsoftware.uc.oneclick-0.2.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.410026 com.castsoftware.uc.oneclick-0.2.3.1b0/
+-rw-rw-rw-   0        0        0      519 2023-06-29 15:08:32.396474 com.castsoftware.uc.oneclick-0.2.3.1b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.103520 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.201927 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.254447 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2745 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     4028 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    24987 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.384153 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4740 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     6814 2023-06-28 22:46:02.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9130 2023-06-28 22:43:16.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     2893 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-06-29 11:52:29.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2566 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    10978 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     3947 2023-06-28 21:49:06.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/setup.py
+-rw-rw-rw-   0        0        0      779 2023-06-29 15:07:41.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:08:32.410026 com.castsoftware.uc.oneclick-0.2.3.1b0/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.1b0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.9
+Version: 0.2.3.1b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.9
+Version: 0.2.3.1b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/aip_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,29 +24,29 @@
             aip_status = config.application[appl]['aip']
             if aip_status == '' or aip_status.startswith('Error'):
                 #add a new appication in AIP Console
                 cls._log.info(f'Running analysis for {config.project_name}\{appl}')
 
                 java_home = config.java_home
                 if len(java_home) > 0:
-                    java_home = f'{java_home}/bin/'
+                    java_home = f'{java_home}'
 
                 node_name = ""
                 if len(config.console_node) > 0:
                     node_name=f'--node-name={config.console_node}'
 
                 security_assessment=""
                 if config.enable_security_assessment:
                     security_assessment='--enable-security-assessment'
                 
                 blueprint=""
                 if config.blueprint:
                     blueprint='--blueprint'
 
-                args = [f'{java_home}java.exe',
+                args = [abspath(f'{java_home}/bin/java.exe'),
                         '-jar',config.console_cli,
                         'add',
                         '-n',appl,
                         '-f', f'AIP/{config.project_name}/{appl}',
                         '-s',config.console_url,
                         '--apikey',config.console_key,
                         '--verbose',
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/highlight_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from oneclick.analysis.analysis import Analysis
 from subprocess import Popen,PIPE
 from oneclick.config import Config
 from cast_common.hlRestCall import HLRestCall
 from cast_common.util import run_process,create_folder
+from os.path import abspath
 
 import sys
 
 class HLAnalysis(Analysis):
 
     def __init__(cls, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
@@ -38,24 +39,25 @@
 
                     hl_sourceDir = f'{config.base}\\STAGED\\HL\\{config.project_name}\\{appl}'
                     hl_workingDir = f'{config.oneclick_work}\\{config.project_name}\\HL_ANALYSIS_RESULT\\{appl}'
                     create_folder(f'{config.oneclick_work}\\{config.project_name}\\HL_ANALYSIS_RESULT')
                     create_folder(hl_workingDir)
                     java_home = config.java_home
                     if len(java_home) > 0:
-                        java_home = f'{java_home}/bin/'
+                        java_home = f'{java_home}'
 
-                    args = [f'{config.java_home}java.exe',
+                    args = [abspath(f'{config.java_home}/bin/java.exe'),
                             '-jar',config.hl_cli,
                             '--sourceDir', hl_sourceDir,
                             '--workingDir' , hl_workingDir,
                             '--companyId', str(config.hl_instance),
                             '--analyzerDir',config.analyzer_dir,
                             '--perlInstallDir',config.perl_install_dir,
                             '--applicationId', str(app_id),
+                            '--serverUrl', config.hl_url.rsplit('/',1)[0],
                             '--login',config.hl_user,
                             '--password',config.hl_password]
                     try:
                         proc = run_process(args,wait=False)
                     except FileNotFoundError as e:
                         cls._log.error(f'Unable to launch analysis process {e}')
                         cls._log.error(args)
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,23 @@
     Read and validate configuration file
 """
 from cast_common.logger import Logger,DEBUG, INFO, WARN, ERROR
 from cast_common.util import create_folder
 from json import load
 from argparse import ArgumentParser
 from json import JSONDecodeError,dump
-from os.path import abspath,exists
+from os.path import abspath,exists,dirname
 from os import getcwd
 
 from argparse import ArgumentParser
 from oneclick.exceptions import NoConfigFound,InvalidConfiguration,InvalidConfigNoBase
 
+from django.core.validators import URLValidator
+from django.core.exceptions import ValidationError
+
 __author__ = "Nevin Kaplan"
 __copyright__ = "Copyright 2022, CAST Software"
 __email__ = "n.kaplan@castsoftware.com"
 
 class Config():
     log = None
     log_translate = {} 
@@ -111,14 +114,45 @@
                 self.base=args.baseFolder
                 self.project = args.projectName
                 self.company_name = args.companyName
 
                 self.start=args.start
                 self.start=args.end
 
+                # Run for MRI
+                if self.is_console_active == False:
+                    if yes_no_input('Run MRI analysis for all applications?'):
+                        while not self.is_console_active:
+                            if len(self.console_url) == 0:
+                                self.console_url=url_input('Missing console URL:',self.console_url)
+                            else:
+                                self.console_url=self.console_url
+                            if len(self.console_key) == 0:
+                                self.console_key=secret_input('Missing console KEY:',self.console_key)
+                            if len(self.console_cli) == 0:
+                                folder_input('\t"AIP Console automation tools" location',dirname(self.console_cli),"aip-console-tools-cli.jar",True)
+                    else:
+                        self._set_console_active=False                                
+
+                if self.is_hl_active == False:                
+                    if yes_no_input('Run Highlight analysis for all applications?'):
+                        while not self.is_hl_active:
+                            if len(self.hl_url) == 0:
+                                self.hl_url=url_input('Missing Highlight URL',self.hl_url)
+                            if len(self.hl_user) == 0:
+                                self.hl_user=string_input('Missing Highlight User ID',self.hl_user)
+                            if len(self.hl_password) == 0:
+                                self.hl_password=secret_input('Missing Highlight Password',self.hl_password)
+                            if len(self.hl_instance) == 0:
+                                self.hl_instance=string_input('Missing Highlight Instance ID',self.hl_instance)
+                            else:
+                                self.hl_instance=self.hl_instance
+
+                self.log.info(f'Run MRI analysis: {self.is_aip_active}')
+                self.log.info(f'Run Highlight analysis: {self.is_hl_active}')
                 self._save()
 
             except JSONDecodeError as e:
                 msg = str(e)
                 self.log.error(f'Configuration file {self._config_file} must be in a JSON format {msg}')
                 exit()
 
@@ -200,15 +234,15 @@
             self.highlight['Active']=False
         return self.rest['Highlight']
     @property
     def is_hl_active(self):
         return self.highlight['Active']
 
     def _set_hl_active(self):
-        self._set_active(self.highlight,['URL','user','password','instance','cli','perlInstallDir','analyzerDir'])
+        self._set_active(self.highlight,['URL','cli','perlInstallDir','analyzerDir','user','password','instance'])
 
     @property
     def hl_url(self):
         return self._get(self.highlight,'URL')
     @hl_url.setter
     def hl_url(self,value):
         if self._set_value(self.highlight,'URL',value):
@@ -279,20 +313,15 @@
         msg=[]
         if len(self.hl_cli) == 0:
             msg.append('hl_cli')
         if len(self.perlInstallDir) == 0:
             msg.append('perlInstallDir')
         if len(self.analyzerDir) == 0:
             msg.append('analyzerDir')
-        # if len(self.java_home) == 0:
-        #     msg.append('java_home')
-        # if len(self.cloc_version) == 0:
-        #     msg.append('cloc_version')
-
-        
+       
         if len(msg) > 0:
             fmt_msg=', '.join(msg)
             self.log.error(f'Invalid Highlight configuration, missing {fmt_msg} fields')
             is_ok=False
 
         return is_ok
 
@@ -383,14 +412,36 @@
     @property
     def blueprint(self):
         return self._get(self.console,'blueprint')
     @blueprint.setter
     def blueprint(self,value):
         self._set_console_active('blueprint',value,'')
 
+    @property
+    def is_console_config_valid(self)->bool:
+        if not self.is_console_active:
+            self.log.warning('MRI analysis is inactive')            
+            return True
+        is_ok=True
+        msg=[]
+        if len(self.console_url) == 0:
+            msg.append('URL')
+        if len(self.console_key) == 0:
+            msg.append('API_Key')
+        if len(self.console_cli) == 0:
+            msg.append('Console CLI')
+       
+        if len(msg) > 0:
+            fmt_msg=', '.join(msg)
+            self.log.error(f'Invalid MRI configuration, missing {fmt_msg} fields')
+            is_ok=False
+
+        return is_ok
+
+
     """ **************** Action Plan related entries ************************ """
     def _set_database_active(self,key,value,default=''):
         if self._set_value(self.db,key,value,default):
             self._set_active(self.db,['database','user','password','host','port'])
             self._save()
 
     @property
@@ -577,14 +628,99 @@
         return self._get(self.setting,'java-home')
     @java_home.setter
     def java_home(self,value):
         if self._set_value(self.setting,'java-home',value,''):
             self._save()
 
 
+def yes_no_input(prompt:str,default_value=True) -> bool:
+    while True:
+        if default_value:
+            default_value='Y'
+        else:
+            default_value='N'
+
+        val = input(f'{prompt} [{default_value}]?').upper()
+        if len(val) == 0: val = default_value
+
+        if val in ['Y','YES']:
+            return True
+        elif val in ['N','NO']:
+            return False
+        else:
+            print ('Expecting a Y[es] or N[o] response. ',end='')
+
+def folder_input(prompt:str,folder:str='',file:str=None,combine:bool=False) -> str:
+    if combine:
+        folder=folder.replace(file,'')
+
+    while True:
+        i = input(f'{prompt} [{abspath(folder)}]: ')
+        if len(i)==0:
+            folder = abspath(folder)
+        else:
+            folder = abspath(i)
+        if exists(folder):
+            if file is not None:
+                if exists(abspath(f'{folder}/{file}')):
+                    break
+                else:
+                    print (f'{folder} folder does not contain {file}, please try again')
+                    continue
+            else:
+                break
+        print (f'{folder} not found, please try again')
+
+    if combine:
+        folder = abspath(f'{folder}/{file}')
+    return folder
+
+def string_input(prompt:str,default_value=""):
+    while True:
+        if len(default_value)>0:
+            i = input(f'{prompt} [{default_value}]: ')
+        else:
+            i = input(f'{prompt}: ')
+
+        if len(i)==0:
+            if len(default_value) == 0:
+                print('Input required, please try again')
+                continue
+            else:
+                i = default_value
+        return i            
+
+def secret_input(prompt:str,default_value=""):
+    while True:
+        if len(default_value)>0:
+            i = input(f'{prompt} ***********: ')
+        else:
+            i = input(f'{prompt}: ')
+
+        if len(i)==0:
+            if len(default_value) == 0:
+                print('Input required, please try again')
+                continue
+            else:
+                i = default_value
+        return i            
+
+def url_input(prompt:str,url):
+    val = URLValidator()
+    while True:
+        i = input(f'{prompt} [{url}]: ')
+        if len(i)>0:
+            url = i
+        try:
+            val(url)
+            return url
+        except ValidationError as e:
+            print ("Bad URL, please try again")      
+
+
 #        def _set_value(self,base,key,value,default=''):
 
 
     
     # @property
     # def template(self):
     #     return self._config['template']
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cleanup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from datetime import datetime
-from os import mkdir,getcwd,walk,remove
+from os import mkdir,getcwd,walk,remove,chmod,rmdir
+from stat import S_IWUSR
 from os.path import abspath,join
-from shutil import rmtree
+#from shutil import rmtree
 from oneclick.discovery.sourceValidation import SourceValidation
 from oneclick.config import Config
 from cast_common.logger import INFO
 from cast_common.util import create_folder
 
+from pandas import Series,DataFrame
+
+import re 
+
 #todo: review cleanup lists for aip and hl, do we need separate or can we keep it as one and run HL from AIP folder?
 
 class cleanUpAIP(SourceValidation):
 
     def __init__(cls, config:Config, name = None, log_level:int=INFO):
         if name is None: 
             name = cls.__class__.__name__
@@ -19,86 +24,100 @@
     @property
     def cleanup_file_prefix(cls):
         return "AIP"
 
     def run(cls,config:Config):
         cls._log.debug('Source Code cleanup is in progress')
         
-        output_path = f'{config.oneclick_work}/{config.project_name}/LOGS'    
-        #create_folder(output_path)
+        output_path = abspath(f'{config.oneclick_work}/LOGS/{config.project_name}')
+        create_folder(output_path)
 
         dir = config.base
         dateTimeObj=datetime.now()
         file_suffix=dateTimeObj.strftime("%d-%b-%Y(%H.%M.%S.%f)")
         
-        exclusionFileList= f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFileList.txt'
+        exclusionFileList= abspath(f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFileList.txt')
         with open(exclusionFileList) as f:
             files_list = f.read().splitlines()
             f.close()
 
-        exclusionFolderList= f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFolderList.txt'
+        exclusionFolderList= abspath(f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFolderList.txt')
         with open(exclusionFolderList) as f:
             folder_list = f.read().splitlines()
             f.close()
 
         apps= config.application
         cls._log.info(f'Running {cls.__class__.__name__} for all applications')
         found = True
         while found:
             found = False
             for app in apps:
                 create_folder(f'{output_path}\\{app}')
-                clean_up_log_file= f"{output_path}\\{app}\\{cls.cleanup_file_prefix}{config.project_name}_{app}_deletedFiles_{file_suffix}.txt"
-                clean_up_log_folder= f"{output_path}\\{app}\\{cls.cleanup_file_prefix}{config.project_name}_{app}_deletedFolders_{file_suffix}.txt"
-
-                app_folder = f'{config.work}\\{cls.cleanup_file_prefix}\\{config.project_name}\\{app}'
-
-                with open (clean_up_log_folder, 'a+') as file2: 
-                    s=''
-                        
-                    count=0
-                    for subdir, dirs, files in walk(app_folder):
-                            for dir in dirs:
-                                if dir in folder_list:
-                                    folder=join(subdir, dir)
-                                    rmtree(folder)
-                        
-                                    s=str(count)+") Removed folder -> "+folder
-                                    count+=1
-                                    file2.write(s)
-                                    file2.write('\n') 
-                    file2.close()
-                cls._log.info(f'Removed {count} unwanted folders from {app_folder}')
-                if count > 0:
-                    config.application[app]['aip']=""
-                    config._save()
+                base = f'{output_path}\\{app}\\{cls.cleanup_file_prefix}{config.project_name}_{app}'
+                clean_up_log_file= f"{base}_deletedFiles_{file_suffix}.txt"
+                clean_up_log_folder= f"{base}_deletedFolders_{file_suffix}.txt"
 
+                app_folder = abspath(f'{config.work}\\{cls.cleanup_file_prefix}\\{config.project_name}\\{app}')
+                cls._log.info(f'Reviewing {app} ({app_folder})')
                 with open (clean_up_log_file, 'a+') as file1: 
-                    s=''
-                    count=0
-                    for subdir, dirs, files in walk(app_folder):
-                        for file in files:
-                            fileN=join(subdir, file) 
-                            for fileName in files_list:
-                                
-                                if fileN.endswith(fileName):
-                                    remove(fileN)
-                                
-                                    s=str(count)+") Removed file -> "+fileN
-                                    count+=1
-                                    file1.write(s)
-                                    file1.write('\n') 
-                    file1.close()
-                cls._log.info(f'Removed {count} unwanted files from {app_folder}')
-                if count > 0:
-                    config.application[app]['aip']=""
-                    config._save()
+                    with open (clean_up_log_folder, 'a+') as file2: 
+                        s=''                            
+                        folder_cnt=0
+                        file_cnt=0
+                        for subdir, dirs, files in walk(app_folder):
+                                for dir in dirs:
+                                    if cls.find_with_list(dir,folder_list):
+                                        folder=join(subdir, dir)
+                                        rmtree(folder)
+                                        folder_cnt+=1
+                                        log_it('folder',folder,file2)
+
+                                for file in files:
+                                    if cls.find_with_list(file,files_list):
+                                        file=join(subdir, file)
+                                        remove(file)
+                                        file_cnt+=1
+                                        log_it('file',file,file1)
+
+                cls._log.info(f'Removed {file_cnt} files and {folder_cnt} folders from {app_folder}')
+                # if count > 0:
+                #     config.application[app]['aip']=""
+                #     config._save()
 
         cls._log.debug('Source Code cleanup done')
 
+    def find_with_list(cls,find_in:str,pattern:list):
+        rslt = False
+        for p in pattern:
+            try:
+                if re.match(p,find_in):
+                    rslt = True
+                    break
+            except re.error as ex:
+                cls._log.warning(f'{ex.msg} for pattern {ex.pattern}')
+            
+        return rslt
+
+
+def log_it(typ,nm,fno):
+    s=f'Removed {typ} -> {nm})'
+    fno.write(s)
+    fno.write('\n') 
+
+
+
+def rmtree(top):
+    for root, dirs, files in walk(top, topdown=False):
+        for name in files:
+            filename = join(root, name)
+            chmod(filename, S_IWUSR)
+            remove(filename)
+        for name in dirs:
+            rmdir(join(root, name))
+    rmdir(top)    
 
 class cleanUpHL(cleanUpAIP):
     def __init__(cls,config:Config, log_level:int):
         super().__init__(config,cls.__class__.__name__,log_level)
 
     @property
     def cleanup_file_prefix(cls):
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cloc.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
     def run(cls,config:Config):
         cls.open_excel_writer(config)
         cls.cloc_path=abspath(f'{config.base}\\scripts\\{cls.config.cloc_version}')
         list_of_tech_file=abspath(f'{config.base}\\scripts\\ListOfTechnologies.csv')
         with open(list_of_tech_file) as f:
             tech_list = f.read().splitlines()
-            f.close()
-
+            
         process = {}
         cloc_run=False
         for appl in config.application:
             cls._log.info(f'Running {config.project_name}/{appl}')
             create_folder(f'{config.report}/{config.project_name}/{appl}')
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
             cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt')
@@ -113,46 +112,37 @@
             with open(cloc_output, 'r') as f:
                 content = f.read()
                 f.seek(0)
                 summary_list= [line.rstrip('\n').lstrip() for line in f]
                 #print(summary_list)
 
             #extracting required data from content of cloc_output.txt using python regex
-            pattern='(\S{1,}|\w{1,}[:])\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
+#            pattern='(\S{1,}|\w{1,}[:])\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
+            pattern='([\w #]{30})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
             statistics_list=findall(pattern,content)
             statistics_list= statistics_list[:-1]
             
             with open(cloc_output_ignored, 'r') as fp:
                 lines = len(fp.readlines())
-            statistics_list.append(('Unknown Files',lines,'0','0','0'))
+            statistics_list.append(('Unknown Files','0','0','0',str(lines)))
 
             df = DataFrame(statistics_list,columns=['LANGUAGE','FILES','BLANK','COMMENT','CODE'])
 
-            #making technolgy check as case sensitive
-            def all_lower(my_list):
-                return list(map(lambda x: x.lower(), my_list))
-            tech_list = all_lower(tech_list)
-            df['APPLICABLE']=df['LANGUAGE'].str.lower().isin(tech_list)
+            #making technolgy case insensitive
+            tech_list = list(map(lambda x: x.lower().strip(), tech_list))
+            df['APPLICABLE']=df['LANGUAGE'].str.lower().str.strip().isin(tech_list)
 
             #converting column values into int from string
-            df['FILES'] = df['FILES'].astype('int')
-            df['BLANK'] = df['BLANK'].astype('int')
-            df['COMMENT'] = df['COMMENT'].astype('int')
-            df['CODE'] = df['CODE'].astype('int')
-
-            #converting total line to formulas
-            # total_files='=SUBTOTAL(109,[FILES])'
-            # total_blank='=SUBTOTAL(109,[BLANK])'
-            # total_comment='=SUBTOTAL(109,[COMMENT])'
-            # total_code='=SUBTOTAL(9,E2:E'+str(len(df['FILES'])+1)+')'
-            
-            #converting total line to formulas
-#            df.loc[len(df.index)] = [' ', total_files, total_blank, total_comment, total_code, ' ']
-
-            format_table(ClocPreCleanup.writer,df,f'{cls.phase}({appl})')
+            numbers=['FILES','BLANK','COMMENT','CODE']
+            total_line=['']
+            for name in numbers:
+                df[name] = df[name].astype('int')
+            tab_name = f'{appl}-{cls.phase}'
+            tab_name = (tab_name[:30] + '..') if len(tab_name) > 30 else tab_name
+            workbook = format_table(ClocPreCleanup.writer,df,tab_name,total_line=True)
         return True
 
 
 
 class ClocPostCleanup(ClocPreCleanup):
 
     def __init__(cls, config: Config, log_level:int=INFO, name = None):
@@ -163,13 +153,14 @@
     
     @property
     def phase(cls):
         return 'After'
 
     def run(cls,config:Config):
         super().run(config)
+        sheet_names = ClocPreCleanup.writer.book.worksheets_objs.sort(key=lambda x: x.name)
         ClocPreCleanup.writer.close()
         pass
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/discoveryReport.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 import pandas
 from oneclick.discovery.sourceValidation import SourceValidation 
 from pandas import DataFrame,read_excel
 from os.path import abspath
-import docx
 from oneclick.config import Config
 from cast_common.util import convert_LOC
 
+from docx import Document
+from docx.enum.text import WD_ALIGN_PARAGRAPH,WD_LINE_SPACING
+from docx.shared import Length
+
 #todo: add totals to the cloc report (d1)
 #todo: if SQL problems, add bullet under SQL Delivery to describe (d1)
 
 class DiscoveryReport(SourceValidation):
 
     def __init__(cls, config:Config, log_level:int):
         super().__init__(config,cls.__class__.__name__,log_level)
 
 
     def cloc_report(cls,file:str,sheet:str):
         
         # read by 'Stats Before Code CleanUP' sheet of an Cloc_Output excel file
         df = read_excel(file,sheet_name=sheet)
-        #df = df[df['LANGUAGE']!='SUM:'] # remove the total row
-
-        # #extract total cout of applicable code from 'Stats Before Code CleanUP' sheet of an Cloc_Output excel file
-        # filt=(df['APPLICABLE']==True)
-        # pre_LOC=(df.loc[filt,'CODE'].sum())
-        # pre_LOC=pre_LOC//1000
-        #df=df.sum(axis = 0, skipna = True)
         return df
 
 
     def run(cls,config:Config):
 
         cloc_report = abspath(f'{config.report}/{config.project_name}/{config.project_name}-cloc.xlsx')
         discovery_report = abspath(f'{config.report}/{config.project_name}/{config.project_name}-source-code-discovery.docx')
         # create an instance of a word document
-        doc = docx.Document()
+        doc = Document()
         # add a heading of level 0 (largest heading)
         doc.add_heading('Source code discovery report', 0)
         #doc_para = doc.add_paragraph(f'Please find below the completed discovery for the Project {config.project_name}')
         doc_para = doc.add_paragraph(f'Please find below the completed discovery for Project {config.project_name}. Note that we used CLOC for quick discovery and completeness verification. The actual lines of code discovered by the CAST solution may differ slightly from below. ')
         doc.add_heading('Questions', 1)
         doc.add_paragraph('<Specific questions to be added manually if needed. Remove this section if no questions>')
 
@@ -46,57 +42,63 @@
 
         for appl in config.application:
             cls._log.info(f'Running {cls.__class__.__name__} for {appl}')
 
             sql_report = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-SQLReport.xlsx')
 
             # read by 'Stats Before Code CleanUP' sheet of an Cloc_Output excel file
-            before_df = cls.cloc_report(cloc_report,f'Before({appl})')
+            before_df = cls.cloc_report(cloc_report,f'{appl}-Before')
+            before_df=before_df[before_df['LANGUAGE'] != 'Totals']
+            before_df[before_df.columns]=before_df.apply(lambda x: x.str.strip() if isinstance(x, str) else x)
             #print(before_df)
 
             filt=(before_df['APPLICABLE']==False)
             l=before_df.loc[filt,['LANGUAGE','CODE']].sort_values(by=['CODE'], ascending=False) 
             non_code=''
             if len(l) == 1:
-                non_code= str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE']
+                str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE']
             elif len(l) > 1:
-                non_code= str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE'] +' non code files and ~'+ str(l.iloc[1]['CODE']//1000) +' KLOC of '+ l.iloc[1]['LANGUAGE']
+                non_code= str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE'].strip() +' non code files and ~'+ str(l.iloc[1]['CODE']//1000) +' KLOC of '+ l.iloc[1]['LANGUAGE']
 
             # read by 'Stats After Code CleanUP' sheet of an Cloc_Output excel file
-            after_df = cls.cloc_report(cloc_report,f'After({appl})')
+            after_df = cls.cloc_report(cloc_report,f'{appl}-After')
             #print(after_df)
 
             # read by 'Summary' sheet of an SQL_Output excel file
             sql_df = read_excel(sql_report,sheet_name='Summary')
             #sql_df = sql_df[sql_df['Total']>0]
 
             doc.add_heading(f'Application {appl} :', 2)
 
             # out of scope code base
-            total = int(before_df['CODE'].sum())
-            total, unit = convert_LOC(total)
-            doc.add_paragraph(f"This delivery contains a total of {len(after_df)-1} technologies/extensions discovered with a total of {total} {unit}.",style='List Bullet')
+            langs=len(before_df)
+            total, unit = convert_LOC(int(before_df['CODE'].sum()))
+            doc.add_paragraph(f"This delivery contains {langs} discovered technolog{'ies' if langs > 1 else 'y'}/extension{'s' if langs > 1 else ''}  and a total of {total} {unit}.",style='List Bullet')
 
             bsuport = after_df[after_df['APPLICABLE']==True]
             total = int(bsuport['CODE'].sum())
             total, unit = convert_LOC(total)
 
-            lang_list = list(bsuport['LANGUAGE'])
-            lang_list[-1]=f'and {lang_list[-1]}'
+            lang_list = list(bsuport['LANGUAGE'].str.strip())
+            langs = len(lang_list)
+            if langs >1:
+                lang_list[-1]=f'and {lang_list[-1]}'
             bsup_lang = ', '.join(lang_list)
-            doc.add_paragraph(f"{len(bsuport)} technologies/extensions are relevant for the CAST analysis, which include {bsup_lang}.",style='List Bullet')
+            doc.add_paragraph(f"{len(bsuport)} technolog{'ies' if langs > 1 else 'y'}/extension{'s are' if langs > 1 else ' is'} relevant for the CAST analysis, which include {bsup_lang}.",style='List Bullet')
 
             nsuport = after_df[after_df['APPLICABLE']==False]
             total = int(bsuport['CODE'].sum())
             total, unit = convert_LOC(total)
 
-            lang_list = list(nsuport['LANGUAGE'])
-            lang_list[-1]=f'and {lang_list[-1]}'
+            lang_list = list(nsuport['LANGUAGE'].str.strip())
+            langs = len(lang_list)
+            if langs > 1:
+                lang_list[-1]=f'and {lang_list[-1]}'
             bsup_lang = ', '.join(lang_list)
-            doc.add_paragraph(f"The remaining {len(nsuport)} technologies/extensions are not relevant and will not be analyzed. These include {bsup_lang}.",style='List Bullet')
+            doc.add_paragraph(f"The remaining technolog{'ies' if langs > 1 else 'y'}/extension{'s are' if langs > 1 else ' is'} not relevant and will not be analyzed. These include {bsup_lang}.",style='List Bullet')
 
             # in scope code base
             # asuport = after_df[before_df['APPLICABLE']==True]
             # total = int(asuport['CODE'].sum())
             # total, unit = convert_LOC(total)
             #doc.add_paragraph(f'After removing all Sample, Test and other non production related code there is ({total} {unit}) in scope for this project',style='List Bullet 2')
             #print(sql_df)
@@ -104,61 +106,73 @@
             procedures=sql_df['Total'][1]
             functions=sql_df['Total'][2]
             triggers=sql_df['Total'][3]
             views=sql_df['Total'][4]
             sql_items=''
 
             if tables == 0 and procedures == 0 and functions == 0 and triggers == 0 and views == 0:
-                doc.add_paragraph(f'The source code does not contains SQL items.',style='List Bullet')
+                doc.add_paragraph(f'The source code does not contain any SQL items.',style='List Bullet')
             else:
                 if tables>0:
                     sql_items = sql_items + str(tables) +' tables, '
                 if procedures>0:
                     sql_items = sql_items + str(procedures) +' stored procedures, '
                 if functions>0:
                     sql_items = sql_items + str(functions) +' functions, ' 
                 if triggers>0:
                     sql_items = sql_items + str(triggers) +' triggers, '
                 if views>0:
                     sql_items = sql_items + str(views) +' views '
                 
-                doc.add_paragraph(f'The database contains a total of '+sql_items+'.',style='List Bullet')
+                doc.add_paragraph(f'The database contains a total of {sql_items}.',style='List Bullet')
 
             # line = []
             # for index, row in sql_df.iterrows():
             #     line.append(f"{row['Unique']} {row['Catagory']}")
             #     if row['Catagory'] == 'SQL files':
             #         line[-1]=f'in {line[-1]}'
             #doc.add_paragraph(f"The delivery also inclues, {', '.join(line)}.",style='List Bullet')
             removed_code=before_df['CODE'].sum()-after_df['CODE'].sum()
-            doc.add_paragraph(f'We removed {removed_code} KLOC of sample, test and other non-production code from the source code.',style='List Bullet')
+            doc.add_paragraph(f'We removed {round(removed_code/1000,1)} KLOC of sample, test and other non-production code from the source code.',style='List Bullet')
             after_df=after_df.drop(after_df[after_df['APPLICABLE']==0.0].index)
             total = after_df['CODE'].sum()//1000
             doc.add_paragraph(f"Here is a high-level summary of the source code that will be analyzed by CAST, totaling {total} KLOC.",style='List Bullet')
 
             after_df = after_df[['LANGUAGE','FILES','CODE']]
             after_df = after_df[:-1]
             files_count=after_df['FILES'].sum()
             code_count=after_df['CODE'].sum()
             new_row = pandas.DataFrame({'LANGUAGE':'Totals', 'FILES':[files_count], 'CODE':[code_count]})
             after_df = pandas.concat([after_df,new_row])
             
             t = doc.add_table(after_df.shape[0]+1, after_df.shape[1])
             # add the header rows.
             for j in range(after_df.shape[-1]):
-                t.cell(0,j).text = after_df.columns[j]
+                t.cell(0,j).text = after_df.columns[j].strip()
+                if j > 0:
+                    t.cell(0,j).paragraphs[0].alignment=WD_ALIGN_PARAGRAPH.RIGHT
 
             # add the rest of the data frame
             for i in range(after_df.shape[0]):
                 for j in range(after_df.shape[-1]):
                     number = after_df.values[i,j]
                     if type(number) is int:
-                        number = "{}".format(number)
+                        number = "{:,}".format(number)
                     t.cell(i+1,j).text = number
-            
+                    if j > 0:
+                        t.cell(i+1,j).paragraphs[0].alignment=WD_ALIGN_PARAGRAPH.RIGHT
+            make_rows_bold(t.rows[len(after_df)])
+
             # Adding style to a table
             t.style = 'Medium Shading 1 Accent 1'
 
         # now save the document to a location
         doc.save(discovery_report)
         cls._log.info(f'Source Code Discovery report has been written to {discovery_report}')
-    pass
+
+
+def make_rows_bold(*rows):
+    for row in rows:
+        for cell in row.cells:
+            for paragraph in cell.paragraphs:
+                for run in paragraph.runs:
+                    run.font.bold = True
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/unzip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import walk,remove
 from os.path import abspath
 
-from shutil import unpack_archive
+#from shutil import unpack_archive
+from pyunpack import Archive
 
 from oneclick.discovery.sourceValidation import SourceValidation 
 from oneclick.config import Config
 
 class Unzip(SourceValidation):
 
    def __init__(cls, config:Config, log_level:int):
@@ -31,32 +32,38 @@
                   if file.endswith(".zip") or \
                      file.endswith(".7z") or \
                      file.endswith(".tar") or \
                      file.endswith(".gztar") or \
                      file.endswith(".bztar"):
                      found = True
                      
-                     full_name = f'{root}\\{file}'
+                     full_name = abspath(f'{root}\\{file}')
+                     dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
                      cls._log.info(f'Unzipping {full_name}')
-                     unpack_archive(full_name,root)
+
+                     Archive(full_name).extractall(dest,auto_create_dir=True)
+                     
                      remove(full_name)
 
             app_folder_hl = f'{config.work}\\HL\\{config.project_name}\\{app}'
             for root, dirs, files in walk(app_folder_hl):
                for file in files:
                   if file.endswith(".zip") or \
                      file.endswith(".7z") or \
                      file.endswith(".tar") or \
                      file.endswith(".gztar") or \
                      file.endswith(".bztar"):
                      found = True
                      
-                     full_name = f'{root}\\{file}'
+                     full_name = abspath(f'{root}\\{file}')
+                     dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
                      cls._log.info(f'Unzipping {full_name}')
-                     unpack_archive(full_name,root)
+
+                     Archive(full_name).extractall(dest,auto_create_dir=True)
+                     
                      remove(full_name)
 
       cls._log.info('Unzip step complete')
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.9/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.3.1b0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.9' #prod version
+version='0.2.3.1-beta' #prod version
 dependencies = [
-    'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
-    'django',
-    'com.castsoftware.uc.python.common==1.0.2',
+    'pandas','python-pptx==0.6.18','python-docx',
+    'argparse_formatter','django','pyunpack',
+    'patool','archive',
+    'com.castsoftware.uc.python.common',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

