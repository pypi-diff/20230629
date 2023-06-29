# Comparing `tmp/rosetta-ce-1.2.7.tar.gz` & `tmp/rosetta-ce-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.2.7.tar", last modified: Thu Jun 29 06:43:10 2023, max compression
+gzip compressed data, was "rosetta-ce-1.2.8.tar", last modified: Thu Jun 29 13:52:46 2023, max compression
```

## Comparing `rosetta-ce-1.2.7.tar` & `rosetta-ce-1.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 06:43:10.627075 rosetta-ce-1.2.7/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.7/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-29 06:43:10.626583 rosetta-ce-1.2.7/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10750 2023-04-26 16:15:22.000000 rosetta-ce-1.2.7/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 06:43:10.620787 rosetta-ce-1.2.7/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.7/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 06:43:10.622598 rosetta-ce-1.2.7/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.7/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.7/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.7/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.7/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.7/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    32109 2023-06-28 17:26:22.000000 rosetta-ce-1.2.7/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     7785 2023-06-29 06:42:23.000000 rosetta-ce-1.2.7/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 06:43:10.624632 rosetta-ce-1.2.7/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-29 06:43:10.000000 rosetta-ce-1.2.7/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 06:43:10.000000 rosetta-ce-1.2.7/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 06:43:10.000000 rosetta-ce-1.2.7/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 06:43:10.000000 rosetta-ce-1.2.7/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 06:43:10.000000 rosetta-ce-1.2.7/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 06:43:10.627123 rosetta-ce-1.2.7/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 06:42:23.000000 rosetta-ce-1.2.7/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 06:43:10.626082 rosetta-ce-1.2.7/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.7/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.7/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.7/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 13:52:46.851410 rosetta-ce-1.2.8/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.8/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 13:52:46.851091 rosetta-ce-1.2.8/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.2.8/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 13:52:46.845378 rosetta-ce-1.2.8/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.8/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 13:52:46.847159 rosetta-ce-1.2.8/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.8/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.8/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.8/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.8/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.8/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    32828 2023-06-29 13:51:45.000000 rosetta-ce-1.2.8/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     7785 2023-06-29 06:42:23.000000 rosetta-ce-1.2.8/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 13:52:46.849271 rosetta-ce-1.2.8/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 13:52:46.000000 rosetta-ce-1.2.8/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 13:52:46.000000 rosetta-ce-1.2.8/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 13:52:46.000000 rosetta-ce-1.2.8/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 13:52:46.000000 rosetta-ce-1.2.8/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 13:52:46.000000 rosetta-ce-1.2.8/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 13:52:46.851456 rosetta-ce-1.2.8/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 13:51:58.000000 rosetta-ce-1.2.8/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 13:52:46.850593 rosetta-ce-1.2.8/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.8/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.8/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.8/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.2.7/LICENSE` & `rosetta-ce-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/PKG-INFO` & `rosetta-ce-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.7
+Version: 1.2.8
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 from rosetta import Observables, Events
 ```
 
 ## Usage
 Here are some examples of how to use Rosetta:
 ```python
 from rosetta import Converter, ConverterToEnum, ConverterFromEnum, Events, ObservableType, ObservableKnown, \
-    Observables, Sender, WorkerTypeEnum
+    Observables, Sender
 
 # Example usage of the Converter class to convert a CEF log into a LEEF log.
 converted_log = Converter.convert(from_type=ConverterFromEnum.CEF, to_type=ConverterToEnum.LEEF,
                                   data="cef_log=CEF:0|Security|Intrusion Detection System|1.0|Alert|10|src=192.168.0.1 dst=192.168.0.2 act=blocked")
 print(
     converted_log)  # {'message': 'converted', 'data': 'LEEF=1.0!Vendor=Security!Product=Intrusion Detection System!Version=1.0!EventID=Alert!Name=10!src=192.168.0.1!dst=192.168.0.2!act=blocked'}
 
@@ -121,15 +121,15 @@
 json_with_my_observables = Events.json(count=1, observables=observables_list)
 print(json_with_my_observables) # [{'event_type': 'vulnerability_discovered', 'timestamp': '2023-02-12T16:28:46', 'severity': 'high', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-3941-1955']}]
 
 incident_with_my_observables = Events.incidents(count=1, fields="id,type,duration,analyst,description,events", observables=observables_list)
 print(incident_with_my_observables) # [{'id': 1, 'duration': 2, 'type': 'Lateral Movement', 'analyst': 'Elizabeth', 'description': 'Software Discovery Forge Web Credentials: SAML Tokens Escape to Host System Binary Proxy Execution: Control Panel Hide Artifacts: Process Argument Spoofing Office Application Startup: Add-ins Compromise Infrastructure: Botnet.', 'events': [{'event': 'Apr 09 19:39:57 abc bind[56294]: ayman : COMMAND ; systemctl stop firewalld'}, {'event': 'CEF:0|Todd, Guzman and Morales|Firewall|1.0.4|afe3d30f-cff4-4084-a7a3-7de9ea21d0e9|Firewall block dns traffic from abc:26806 to 1.1.1.1:555|10|src=abc spt=26806 dst=1.1.1.1 url=https://example.org dpt=555 proto=dns act=block'}, {'event': 'LEEF:1.0|Leef|Payment Portal|1.0|19.90.247.108|abc|d4:27:4c:a7:40:50|2a:3f:f3:37:81:eb|src=192.168.10.20 dst=abc spt=47335 dpt=443 request=https://example.com/index.php method=Web-GET proto=HTTP/1.1 status=500 hash=719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2request_size=3640 response_size=4766 user_agent=Mozilla/5.0 (Macintosh; Intel Mac OS X 10_5_1) AppleWebKit/533.0 (KHTML, like Gecko) Chrome/47.0.819.0 Safari/533.0'}, {'event': '<Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event"><System><Provider Name="Microsoft-Windows-Security-Auditing" Guid="67eb0bb0-ab24-43ce-b7f1-6d6a6bb0ac27"/><EventID>4672</EventID><Version>0</Version><Level>0</Level><Task>12544</Task><Opcode>0</Opcode><Keywords>0x8020000000000000</Keywords><TimeCreated SystemTime="2023-01-15T04:07:58"/><EventRecordID>38</EventRecordID><Correlation/><Execution ProcessID="7182" ThreadID="7703" Channel="Security"/><Computer>abc</Computer><Security UserID="S-1-7181"/><EventData><Data Name="SubjectUserSid">S-1-7181</Data><Data Name="SubjectUserName">mahmoud</Data><Data Name="SubjectDomainName">johnson.net</Data><Data Name="SubjectLogonId">9638</Data><Data Name="PrivilegeList">Through moment tonight.</Data></EventData></Event>'}, {'event': {'event_type': 'vulnerability_discovered', 'timestamp': '2023-01-18T23:49:45', 'severity': 'critical', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-2023-29067']}}]}]
 
 # Example usage of the Sender class to send faked events to log analysis tool.
-worker = Sender(data_type=WorkerTypeEnum.SYSLOG, destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
+worker = Sender(data_type="SYSLOG", destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
 worker.start()
 
 # Starting worker: worker_2023-04-26 17:50:15.671101
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1
```

### Comparing `rosetta-ce-1.2.7/README.md` & `rosetta-ce-1.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from rosetta import Observables, Events
 ```
 
 ## Usage
 Here are some examples of how to use Rosetta:
 ```python
 from rosetta import Converter, ConverterToEnum, ConverterFromEnum, Events, ObservableType, ObservableKnown, \
-    Observables, Sender, WorkerTypeEnum
+    Observables, Sender
 
 # Example usage of the Converter class to convert a CEF log into a LEEF log.
 converted_log = Converter.convert(from_type=ConverterFromEnum.CEF, to_type=ConverterToEnum.LEEF,
                                   data="cef_log=CEF:0|Security|Intrusion Detection System|1.0|Alert|10|src=192.168.0.1 dst=192.168.0.2 act=blocked")
 print(
     converted_log)  # {'message': 'converted', 'data': 'LEEF=1.0!Vendor=Security!Product=Intrusion Detection System!Version=1.0!EventID=Alert!Name=10!src=192.168.0.1!dst=192.168.0.2!act=blocked'}
 
@@ -107,15 +107,15 @@
 json_with_my_observables = Events.json(count=1, observables=observables_list)
 print(json_with_my_observables) # [{'event_type': 'vulnerability_discovered', 'timestamp': '2023-02-12T16:28:46', 'severity': 'high', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-3941-1955']}]
 
 incident_with_my_observables = Events.incidents(count=1, fields="id,type,duration,analyst,description,events", observables=observables_list)
 print(incident_with_my_observables) # [{'id': 1, 'duration': 2, 'type': 'Lateral Movement', 'analyst': 'Elizabeth', 'description': 'Software Discovery Forge Web Credentials: SAML Tokens Escape to Host System Binary Proxy Execution: Control Panel Hide Artifacts: Process Argument Spoofing Office Application Startup: Add-ins Compromise Infrastructure: Botnet.', 'events': [{'event': 'Apr 09 19:39:57 abc bind[56294]: ayman : COMMAND ; systemctl stop firewalld'}, {'event': 'CEF:0|Todd, Guzman and Morales|Firewall|1.0.4|afe3d30f-cff4-4084-a7a3-7de9ea21d0e9|Firewall block dns traffic from abc:26806 to 1.1.1.1:555|10|src=abc spt=26806 dst=1.1.1.1 url=https://example.org dpt=555 proto=dns act=block'}, {'event': 'LEEF:1.0|Leef|Payment Portal|1.0|19.90.247.108|abc|d4:27:4c:a7:40:50|2a:3f:f3:37:81:eb|src=192.168.10.20 dst=abc spt=47335 dpt=443 request=https://example.com/index.php method=Web-GET proto=HTTP/1.1 status=500 hash=719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2request_size=3640 response_size=4766 user_agent=Mozilla/5.0 (Macintosh; Intel Mac OS X 10_5_1) AppleWebKit/533.0 (KHTML, like Gecko) Chrome/47.0.819.0 Safari/533.0'}, {'event': '<Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event"><System><Provider Name="Microsoft-Windows-Security-Auditing" Guid="67eb0bb0-ab24-43ce-b7f1-6d6a6bb0ac27"/><EventID>4672</EventID><Version>0</Version><Level>0</Level><Task>12544</Task><Opcode>0</Opcode><Keywords>0x8020000000000000</Keywords><TimeCreated SystemTime="2023-01-15T04:07:58"/><EventRecordID>38</EventRecordID><Correlation/><Execution ProcessID="7182" ThreadID="7703" Channel="Security"/><Computer>abc</Computer><Security UserID="S-1-7181"/><EventData><Data Name="SubjectUserSid">S-1-7181</Data><Data Name="SubjectUserName">mahmoud</Data><Data Name="SubjectDomainName">johnson.net</Data><Data Name="SubjectLogonId">9638</Data><Data Name="PrivilegeList">Through moment tonight.</Data></EventData></Event>'}, {'event': {'event_type': 'vulnerability_discovered', 'timestamp': '2023-01-18T23:49:45', 'severity': 'critical', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-2023-29067']}}]}]
 
 # Example usage of the Sender class to send faked events to log analysis tool.
-worker = Sender(data_type=WorkerTypeEnum.SYSLOG, destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
+worker = Sender(data_type="SYSLOG", destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
 worker.start()
 
 # Starting worker: worker_2023-04-26 17:50:15.671101
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1
```

### Comparing `rosetta-ce-1.2.7/rosetta/constants/sensors.py` & `rosetta-ce-1.2.8/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/rosetta/constants/sources.py` & `rosetta-ce-1.2.8/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/rosetta/constants/systems.py` & `rosetta-ce-1.2.8/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/rosetta/rconverter.py` & `rosetta-ce-1.2.8/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/rosetta/rfaker.py` & `rosetta-ce-1.2.8/rosetta/rfaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,22 +297,26 @@
             command = random.choice(observables.cmd) if observables and observables.cmd \
                 else random.choice(UNIX_CMD)
             syslog_messages.append(f"{timestamp.strftime('%Y-%m-%d %H:%M:%S')} {host} {process}[{pid}]: {user}"
                                    f" : {action} ; {command}")
         return syslog_messages
 
     @classmethod
-    def cef(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
+    def cef(cls, count: int, vendor: Optional[str] = None, product: Optional[str] = None, version: Optional[str] = None,
+            timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake CEF (Common Event Format) messages.
 
         Args:
             count: The number of CEF messages to generate.
-            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
-            observables: An observables object. If not provided, random objservable will be generated and used.
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
+            vendor: Optional. The vendor.
+            product: Optional. The product.
+            version: Optional. The version.
+            observables: Optional. An observables object. If not provided, random objservable will be generated and used.
         Returns:
             A list of fake CEF messages in string format.
 
         Raises:
             None.
 
         Example Usage:
@@ -325,22 +329,23 @@
              dpt=3087 proto=TCP act=DENY',
              'CEF:0|Acme|Firewall|1.0.0|a3faedaa-5109-4849-b9ec-1ad6c5f8a5ec|Firewall ALLOW TCP traffic
              from example.com:25068 to 81.171.9.216:6157|2|src=example.com spt=25068 dst=81.171.9.216
              dpt=6157 proto=TCP act=ALLOW']
         """
         cef_messages = []
         faker = cls._create_faker()
-        version = faker.numerify("1.0.#")
+        version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
             timestamp += timedelta(seconds=1)
             uuid = faker.uuid4()
-            vendor = faker.company()
+            vendor = vendor or faker.company()
+            product = product or "Firewall"
             src_port = faker.random_int(min=1024, max=65535)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             dst_ip = random.choice(observables.dst_ip) if observables and observables.dst_ip \
                 else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
             url = random.choice(observables.url) if observables and observables.url \
                 else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
@@ -349,27 +354,32 @@
             protocol = random.choice(observables.protocol) if observables and observables.protocol \
                 else random.choice(PROTOCOLS)
             action = random.choice(observables.action) if observables and observables.action \
                 else random.choice(ACTIONS)
             event_id = random.choice(observables.event_id) if observables and observables.event_id \
                 else faker.random_int(min=1, max=10)
             event_description = f"Firewall {action} {protocol} traffic from {host}:{src_port} to {dst_ip}:{dst_port}"
-            cef_messages.append(f"CEF:0|{vendor}|Firewall|{version}|{uuid}|{timestamp}|"
+            cef_messages.append(f"CEF:0|{vendor}|{product}|{version}|{uuid}|{timestamp}|"
                                 f"{event_description}|{event_id}|src={host} spt={src_port} dst={dst_ip} url={url}"
                                 f"dpt={dst_port} proto={protocol} act={action}")
         return cef_messages
 
     @classmethod
-    def leef(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
+    def leef(cls, count, timestamp: Optional[datetime] = None, vendor: Optional[str] = None,
+             product: Optional[str] = None, version: Optional[str] = None,
+             observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake LEEF (Log Event Extended Format) messages.
 
         Parameters:
             count (int): The number of LEEF messages to generate.
-            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
+            vendor: Optional. The vendor.
+            product: Optional. The product.
+            version: Optional. The version.
             observables: An observables object. If not provided, random objservable will be generated and used.
 
         Returns:
             A list of generated LEEF messages.
 
         Example:
             To generate 10 fake LEEF messages:
@@ -384,19 +394,22 @@
              'LEEF:1.0|Leef|Payment Portal|1.0|192.168.0.1|mycomputer|08:00:27:da:2e:2e|08:00:27:da:2e:2f|src=10.0.0.2
               dst=mycomputer spt=57251 dpt=443 request=https://example.com/admin.php?sessionid=12345 method=POST
                proto=HTTP/1.1 status=404 request_size=1216 response_size=9729 user_agent=Mozilla/5.0
                (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3']
         """
         leef_messages = []
         faker = cls._create_faker()
+        version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
             timestamp += timedelta(seconds=1)
+            vendor = vendor or faker.company()
+            product = product or "Application Server"
             src_port = faker.random_int(min=1024, max=65535)
             request_size = faker.random_int(min=100, max=10000)
             response_size = faker.random_int(min=100, max=10000)
             user_agent = faker.user_agent()
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
@@ -406,15 +419,15 @@
             file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
                 else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD, count=1)
             method = random.choice(observables.technique).get('mechanism') if observables and observables.technique \
                 else random.choice(TECHNIQUES).get('mechanism')
             error_code = random.choice(observables.error_code) if observables and observables.error_code \
                 else random.choice(ERROR_CODE)
 
-            leef_log = f"LEEF:1.0|Leef|Payment Portal|1.0|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|" \
+            leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|" \
                        f"{faker.mac_address()}|{faker.mac_address()}|"
             leef_log += f"src={src_ip} dst={host} spt={src_port} dpt=443 request={url} "
             leef_log += f"method={method} proto=HTTP/1.1 status={str(error_code)} hash={file_hash}"
             leef_log += f"request_size={request_size} " \
                         f"response_size={response_size} "
             leef_log += f"user_agent={user_agent}"
             leef_messages.append(leef_log)
```

### Comparing `rosetta-ce-1.2.7/rosetta/rsender.py` & `rosetta-ce-1.2.8/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.2.8/rosetta_ce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.7
+Version: 1.2.8
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 from rosetta import Observables, Events
 ```
 
 ## Usage
 Here are some examples of how to use Rosetta:
 ```python
 from rosetta import Converter, ConverterToEnum, ConverterFromEnum, Events, ObservableType, ObservableKnown, \
-    Observables, Sender, WorkerTypeEnum
+    Observables, Sender
 
 # Example usage of the Converter class to convert a CEF log into a LEEF log.
 converted_log = Converter.convert(from_type=ConverterFromEnum.CEF, to_type=ConverterToEnum.LEEF,
                                   data="cef_log=CEF:0|Security|Intrusion Detection System|1.0|Alert|10|src=192.168.0.1 dst=192.168.0.2 act=blocked")
 print(
     converted_log)  # {'message': 'converted', 'data': 'LEEF=1.0!Vendor=Security!Product=Intrusion Detection System!Version=1.0!EventID=Alert!Name=10!src=192.168.0.1!dst=192.168.0.2!act=blocked'}
 
@@ -121,15 +121,15 @@
 json_with_my_observables = Events.json(count=1, observables=observables_list)
 print(json_with_my_observables) # [{'event_type': 'vulnerability_discovered', 'timestamp': '2023-02-12T16:28:46', 'severity': 'high', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-3941-1955']}]
 
 incident_with_my_observables = Events.incidents(count=1, fields="id,type,duration,analyst,description,events", observables=observables_list)
 print(incident_with_my_observables) # [{'id': 1, 'duration': 2, 'type': 'Lateral Movement', 'analyst': 'Elizabeth', 'description': 'Software Discovery Forge Web Credentials: SAML Tokens Escape to Host System Binary Proxy Execution: Control Panel Hide Artifacts: Process Argument Spoofing Office Application Startup: Add-ins Compromise Infrastructure: Botnet.', 'events': [{'event': 'Apr 09 19:39:57 abc bind[56294]: ayman : COMMAND ; systemctl stop firewalld'}, {'event': 'CEF:0|Todd, Guzman and Morales|Firewall|1.0.4|afe3d30f-cff4-4084-a7a3-7de9ea21d0e9|Firewall block dns traffic from abc:26806 to 1.1.1.1:555|10|src=abc spt=26806 dst=1.1.1.1 url=https://example.org dpt=555 proto=dns act=block'}, {'event': 'LEEF:1.0|Leef|Payment Portal|1.0|19.90.247.108|abc|d4:27:4c:a7:40:50|2a:3f:f3:37:81:eb|src=192.168.10.20 dst=abc spt=47335 dpt=443 request=https://example.com/index.php method=Web-GET proto=HTTP/1.1 status=500 hash=719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2request_size=3640 response_size=4766 user_agent=Mozilla/5.0 (Macintosh; Intel Mac OS X 10_5_1) AppleWebKit/533.0 (KHTML, like Gecko) Chrome/47.0.819.0 Safari/533.0'}, {'event': '<Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event"><System><Provider Name="Microsoft-Windows-Security-Auditing" Guid="67eb0bb0-ab24-43ce-b7f1-6d6a6bb0ac27"/><EventID>4672</EventID><Version>0</Version><Level>0</Level><Task>12544</Task><Opcode>0</Opcode><Keywords>0x8020000000000000</Keywords><TimeCreated SystemTime="2023-01-15T04:07:58"/><EventRecordID>38</EventRecordID><Correlation/><Execution ProcessID="7182" ThreadID="7703" Channel="Security"/><Computer>abc</Computer><Security UserID="S-1-7181"/><EventData><Data Name="SubjectUserSid">S-1-7181</Data><Data Name="SubjectUserName">mahmoud</Data><Data Name="SubjectDomainName">johnson.net</Data><Data Name="SubjectLogonId">9638</Data><Data Name="PrivilegeList">Through moment tonight.</Data></EventData></Event>'}, {'event': {'event_type': 'vulnerability_discovered', 'timestamp': '2023-01-18T23:49:45', 'severity': 'critical', 'host': 'abc', 'file_hash': '719283fd5600eb631c23b290530e4dac9029bae72f15299711edbc800e8e02b2', 'cve': ['CVE-2023-29067']}}]}]
 
 # Example usage of the Sender class to send faked events to log analysis tool.
-worker = Sender(data_type=WorkerTypeEnum.SYSLOG, destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
+worker = Sender(data_type="SYSLOG", destination="udp:127.0.0.1:514", observables=observables_list, count=5, interval=2)
 worker.start()
 
 # Starting worker: worker_2023-04-26 17:50:15.671101
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1 
 # Worker: worker_2023-04-26 17:50:15.671101 sending log message to 127.0.0.1
```

### Comparing `rosetta-ce-1.2.7/setup.py` & `rosetta-ce-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.2.7",
+    version="1.2.8",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.2.7/tests/test_rconverter.py` & `rosetta-ce-1.2.8/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/tests/test_rfaker.py` & `rosetta-ce-1.2.8/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.7/tests/test_rsender.py` & `rosetta-ce-1.2.8/tests/test_rsender.py`

 * *Files identical despite different names*

