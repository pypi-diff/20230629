# Comparing `tmp/capture_it-0.0.8.tar.gz` & `tmp/capture_it-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capture_it-0.0.8.tar", last modified: Sat Oct  1 10:56:12 2022, max compression
+gzip compressed data, was "capture_it-0.0.9.tar", last modified: Wed Dec 28 13:46:55 2022, max compression
```

## Comparing `capture_it-0.0.8.tar` & `capture_it-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-01 10:56:12.789423 capture_it-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-07-10 12:40:24.000000 capture_it-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      803 2022-10-01 10:56:12.788428 capture_it-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      296 2022-07-10 12:40:24.000000 capture_it-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-01 10:56:12.762640 capture_it-0.0.8/capture_it/
--rw-rw-rw-   0        0        0      147 2022-10-01 10:52:13.000000 capture_it-0.0.8/capture_it/__init__.py
--rw-rw-rw-   0        0        0    17487 2022-10-01 10:49:58.000000 capture_it-0.0.8/capture_it/conection.py
--rw-rw-rw-   0        0        0     2277 2022-10-01 10:27:16.000000 capture_it-0.0.8/capture_it/executions.py
-drwxrwxrwx   0        0        0        0 2022-10-01 10:56:12.786461 capture_it-0.0.8/capture_it.egg-info/
--rw-rw-rw-   0        0        0      803 2022-10-01 10:56:12.000000 capture_it-0.0.8/capture_it.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2022-10-01 10:56:12.000000 capture_it-0.0.8/capture_it.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-01 10:56:12.000000 capture_it-0.0.8/capture_it.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2022-10-01 10:56:12.000000 capture_it-0.0.8/capture_it.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-01 10:56:12.000000 capture_it-0.0.8/capture_it.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-01 10:56:12.789423 capture_it-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2022-10-01 10:53:26.000000 capture_it-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-28 13:46:55.154639 capture_it-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-07-10 12:40:24.000000 capture_it-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      803 2022-12-28 13:46:55.153641 capture_it-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2022-07-10 12:40:24.000000 capture_it-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-12-28 13:46:55.123045 capture_it-0.0.9/capture_it/
+-rw-rw-rw-   0        0        0      147 2022-12-28 13:22:33.000000 capture_it-0.0.9/capture_it/__init__.py
+-rw-rw-rw-   0        0        0    20185 2022-12-28 13:34:03.000000 capture_it-0.0.9/capture_it/conection.py
+-rw-rw-rw-   0        0        0     6213 2022-12-28 13:22:33.000000 capture_it-0.0.9/capture_it/database.py
+-rw-rw-rw-   0        0        0     2625 2022-12-28 13:27:11.000000 capture_it-0.0.9/capture_it/executions.py
+drwxrwxrwx   0        0        0        0 2022-12-28 13:46:55.150653 capture_it-0.0.9/capture_it.egg-info/
+-rw-rw-rw-   0        0        0      803 2022-12-28 13:46:55.000000 capture_it-0.0.9/capture_it.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2022-12-28 13:46:55.000000 capture_it-0.0.9/capture_it.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-28 13:46:55.000000 capture_it-0.0.9/capture_it.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2022-12-28 13:46:55.000000 capture_it-0.0.9/capture_it.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-12-28 13:46:55.000000 capture_it-0.0.9/capture_it.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-28 13:46:55.155635 capture_it-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2022-12-28 13:21:07.000000 capture_it-0.0.9/setup.py
```

### Comparing `capture_it-0.0.8/LICENSE` & `capture_it-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `capture_it-0.0.8/PKG-INFO` & `capture_it-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capture_it
-Version: 0.0.8
+Version: 0.0.9
 Summary: Excel Facts File Generate from Networking Device Output|Config
 Home-page: https://github.com/aliasgar1978/capture_it
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `capture_it-0.0.8/capture_it/conection.py` & `capture_it-0.0.9/capture_it/conection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -----------------------------------------------------------------------------
 # Imports
 # -----------------------------------------------------------------------------
 from netmiko import ConnectHandler
 import paramiko, traceback
+import pandas as pd
 from time import sleep
 from nettoolkit import STR, IO, IP, LOG
+from .database import append_to_xl
 # -----------------------------------------------------------------------------
 
 BAD_CONNECTION_MSG = ': BAD CONNECTION DETECTED, TEARED DOWN'
 cisco_banner ="""
 ! ---------------------------------------------------------------------------- !
 ! This output is generated using capture_it utility.
 ! Script written by : Aliasgar Hozaifa Lokhandwala (aholo2000@gmail.com)
@@ -260,25 +262,27 @@
 	Properties:
 		cmd (str): command executed
 		commandOP, output (str) - command output
 		fname (filename): full filename with path where output stored
 	"""    	
 
 	# INITIALIZE class vars
-	def __init__(self, conn, cmd, path):
+	def __init__(self, conn, cmd, path, parsed_output):
 		"""[summary]
 
 		Args:
 			conn (conn): connection object
 			cmd (str): a command to be executed
 			path (str): path where output to be stored
+			parsed_output(bool): generate parsed excel database for the command
 		"""    		
 		self.conn = conn
 		self.cmd = cmd
 		self.path = path
+		self.parsed_output = parsed_output
 		self._commandOP(conn)
 
 
 	def op_to_file(self, cumulative=False):
 		"""store output of command to file, cumulative (True,False,both) to store output in a single file, individual files, both
 
 		Args:
@@ -309,15 +313,17 @@
 
 	# capture output from connection
 	def _commandOP(self, conn):
 		self.output = ''
 
 		op = self.conn.net_connect.send_command(self.cmd, 
 				read_timeout=20, 
-				delay_factor=self.conn.delay_factor)
+				delay_factor=self.conn.delay_factor,
+				use_textfsm=self.parsed_output,
+				)
 
 		# exclude missed ones
 		if any([								
 			STR.found(op,'Connection refused')
 			]):                                 ### ADD More as needed ###
 			print(" CONNECTION WAS REFUSED ")
 			return None
@@ -366,29 +372,33 @@
 		ip (str): device ip
 		auth (dict): authentication parameters
 		cmds (list, set, tuple): set of commands to be executed.
 		path (str): path where output to be stored
 		cumulative (bool, optional): True,False,both. Defaults to False.
 	"""    	
 
-	def __init__(self, ip, auth, cmds, path, cumulative=False, forced_login=False):
+	def __init__(self, ip, auth, cmds, path, cumulative=False, forced_login=False, parsed_output=False):
 		"""initialize execution
 
 		Args:
 			ip (str): device ip
 			auth (dict): authentication parameters
 			cmds (list, set, tuple): set of commands to be executed.
 			path (str): path where output to be stored
 			cumulative (bool, optional): True,False,both. Defaults to False.
+			forced_login(bool): try to login/ssh device even if ping responce fails.
+			parsed_output(bool): generate parsed excel database for the device for show commands.
+		
 		"""    		
 		self.auth = auth
 		self.cmds = cmds
 		self.path = path
 		self.cumulative = cumulative
 		self.forced_login = forced_login
+		self.parsed_output = parsed_output
 		self.delay_factor, self.dev = None, None
 		pinging = self.check_ping(ip)
 		if forced_login or pinging:
 			self.get_device_type(ip)
 			try:
 				self.dev.dtype
 			except:
@@ -455,51 +465,59 @@
 					un=self.auth['un'], 
 					pw=self.auth['pw'], 
 					en=self.auth['en'], 
 					delay_factor=self.delay_factor,
 					devtype=self.dev.dtype,
 					) as c:
 			if self.is_connected(c):
-				self.command_capture(c)
+				cc = self.command_capture(c)
+				if self.parsed_output: cc.write_facts()
 
 	def command_capture(self, c):
 		"""start command captures on connection object
 
 		Args:
 			c (conn): connection object
 		"""    		
-		Captures(dtype=self.dev.dtype, 
+		cc = Captures(dtype=self.dev.dtype, 
 			conn=c, 
 			cmds=self.cmds, 
 			path=self.path, 
-			cumulative=self.cumulative)
+			cumulative=self.cumulative,
+			parsed_output=self.parsed_output
+			)
+		return cc
 
 # -----------------------------------------------------------------------------
 # Execution of Show Commands on a single device. 
 # -----------------------------------------------------------------------------
 
 class CLP():
 	"""parent for Command processing
 
 	Args:
 		dtype (str): device type
 		conn (conn): connection object
 		path (str): path to store the captured output	
 	"""    	
-	def __init__(self, dtype, conn, path):
+	def __init__(self, dtype, conn, path, parsed_output):
 		"""Initialize object
 
 		Args:
 			dtype (str): device type
 			conn (conn): connection object
-			path (str): path to store the captured output	
+			path (str): path to store the captured output
+			parsed_output(bool): generate parsed excel database for the device for all commands.				
 		"""    		
 		self.dtype = dtype
 		self.conn = conn
 		self.path = path
+		self.parsed_output = parsed_output
+		self.parsed_cmd_df = {}
+		self.cmd_exec_logs = []
 		self.hn = self.conn.hn
 		self.ip = self.conn.devvar['ip']
 		self.configure(False)						# fixed disable as now
 
 	def configure(self, config_mode=False):
 		"""set configuration mode
 
@@ -529,24 +547,53 @@
 			cmd (str): command to be executed
 			cumulative (bool, optional): True/False/both. Defaults to False.
 			banner (bool, optional): set a banner property to object if given. Defaults to False.
 
 		Returns:
 			[type]: [description]
 		"""    		
-		# cmdObj = COMMAND(conn=self.conn, cmd=cmd, path=self.path)
-		try:
+		self.cmd_exec_logs.append({'command':cmd})
+		cmdObj = self._cmd_capture_raw(cmd, cumulative, banner)
+		if cmdObj is not None:
+			self._cmd_capture_parsed(cmd, cumulative, banner)
+		return cmdObj
 
-			cmdObj = COMMAND(conn=self.conn, cmd=cmd, path=self.path)
-			cmdObj.banner = banner
+	def _cmd_capture_raw(self, cmd, cumulative=False, banner=False):
+		try:
+			cmdObj = COMMAND(conn=self.conn, cmd=cmd, path=self.path, parsed_output=False)
+		except:
+			print(f"{self.hn} : Error executing command {cmd}")
+			self.cmd_exec_logs[-1]['raw'] = False
+			return None
+		try:
+			cmdObj.banner = banner		
 			file = cmdObj.op_to_file(cumulative=cumulative)
+			self.cmd_exec_logs[-1]['raw'] = True
 			return cmdObj
 		except:
-			print(f"{self.hn} : Error executing command {cmd}")
+			print(f"{self.hn} : Error writing output for command {cmd}\n{cmdObj.output}")
+			print(self.cmd_exec_logs)
+			self.cmd_exec_logs[-1]['raw'] = False
+			return False
+
+	def _cmd_capture_parsed(self, cmd, cumulative=False, banner=False):
+		try:
+			cmdObj_parsed = COMMAND(conn=self.conn, cmd=cmd, path=self.path, parsed_output=True)
+		except:
+			print(f"{self.hn} : Error executing command - Run2 {cmd}")
+			self.cmd_exec_logs[-1]['parsed'] = False
 			return None
+		try:
+			self.parsed_cmd_df[cmd] = pd.DataFrame(cmdObj_parsed.output)
+			self.cmd_exec_logs[-1]['parsed'] = True
+		except:
+			print(f"{self.hn} : Error parsing output for command {cmd}")
+			print(f"{self.hn} : data facts may not be available for command: {cmd}\n{cmdObj_parsed.output}")
+			self.cmd_exec_logs[-1]['parsed'] = False
+			return False
 
 
 
 class Captures(CLP):
 	"""Capture output
 
 	Args:
@@ -554,25 +601,26 @@
 		conn (conn): connection object
 		cmds (set, list, tuple): set of commands 
 		path (str): path to store the captured output
 		cumulative (bool, optional): True/False/both. Defaults to False.
 
 	"""    	
 
-	def __init__(self, dtype, conn, cmds, path, cumulative=False):
+	def __init__(self, dtype, conn, cmds, path, cumulative=False, parsed_output=False):
 		"""Initiate captures
 
 		Args:
 			dtype (str): device type
 			conn (conn): connection object
 			cmds (set, list, tuple): set of commands 
 			path (str): path to store the captured output
 			cumulative (bool, optional): True/False/both. Defaults to False.
+			parsed_output(bool): generate parsed excel database for the device for the captures.
 		"""    		
-		super().__init__(dtype, conn, path)
+		super().__init__(dtype, conn, path, parsed_output)
 		self.cmds = cmds
 		self.op = ''
 		self.cumulative = cumulative
 		self.grp_cmd_capture()
 
 
 	def grp_cmd_capture(self):
@@ -593,7 +641,26 @@
 			try:
 				output = cc.output
 			except:
 				output = f": Error executing command {cmd}"
 			cmd_line = self.hn + ">" + cmd + "\n"
 			self.op += cmd_line + "\n" + output + "\n\n"
 			banner = ""
+
+	def add_exec_logs(self):
+		"""creates a dataframe for log tab on excel parsed output 
+		--> None
+		"""
+		self.parsed_cmd_df['logs'] = pd.DataFrame(self.cmd_exec_logs)
+
+	def write_facts(self):
+		"""write out the parsed outputs in excel database. each command output will create a separate excel tab.
+		--> None
+		"""
+		try:
+			self.add_exec_logs()
+			xl_file = self.path + self.conn.hn + ".xlsx"
+			print(f"writing facts to excel: {xl_file}")
+			append_to_xl(xl_file, self.parsed_cmd_df, overwrite=True)
+			print(f"facts write to excel: {xl_file} ...success!")
+		except:
+			print(f"facts write to excel: {xl_file} ...failed!")
```

### Comparing `capture_it-0.0.8/capture_it/executions.py` & `capture_it-0.0.9/capture_it/executions.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 # -----------------------------------------------------------------------------
 
 class Execute_By_Login(Multi_Execution):
 	"""Execute the device capture by logging in to device.
 
 	"""    	
 
-	def __init__(self, ip_list, auth, cmds, path, cumulative=False, forced_login=False):
+	def __init__(self, ip_list, auth, cmds, path, cumulative=False, forced_login=False, parsed_output=False):
 		"""Initiatlize the connections for the provided iplist, authenticate with provided auth parameters, and execute given commands.
 
 		Args:
 			ip_list (set, list, tuple): set of ip addresses to be logging for capture
 			auth (dict): authentication parameters ( un, pw, en)
 			cmds (set, list, tuple): set of commands to be captured
 			path (str): path where output should be stored.
 			cumulative (bool, optional): True: will store all commands output in a single file, 
 				False will store each command output in differet file. Defaults to False.
 				and 'both' will do both.
+			forced_login(bool): try to login to device via ssh even if ping was failed.
+			parsed_output(bool): generate the excel database file for the device for the captured outputs. ( database will be generated for which the parser functions are available )
 
 		Raises:
 			Exception: raise exception if any issue with authentication or connections.
 		"""    		
 		self.devices = STR.to_set(ip_list) if isinstance(ip_list, str) else set(ip_list)
 		self.auth = auth
 		if not isinstance(cmds, dict):
 			raise Exception("commands to be executed are to be in proper dict format")
 		self.cmds = cmds
 		self.path = path
 		self.cumulative = cumulative
 		self.forced_login = forced_login
+		self.parsed_output = parsed_output
 		super().__init__(self.devices)
 		self.start()
 		# self.end()
 
 	def is_valid(self, ip):
 		"""Validation function to check if provided ip is valid IPv4 or IPv6 address
 
@@ -58,8 +61,8 @@
 		"""execution function for a single device. hn == ip address in this case.
 
 		Args:
 			hn (str): ip address of a reachable device
 		"""    		
 		Execute_Device(hn, auth=self.auth, 
 			cmds=self.cmds, path=self.path, cumulative=self.cumulative,
-			forced_login=self.forced_login)
+			forced_login=self.forced_login, parsed_output=self.parsed_output)
```

### Comparing `capture_it-0.0.8/capture_it.egg-info/PKG-INFO` & `capture_it-0.0.9/capture_it.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capture-it
-Version: 0.0.8
+Version: 0.0.9
 Summary: Excel Facts File Generate from Networking Device Output|Config
 Home-page: https://github.com/aliasgar1978/capture_it
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `capture_it-0.0.8/setup.py` & `capture_it-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,25 @@
     'repoze.sphinx.autointerface',
     'sphinx-copybutton',
     'sphinxcontrib-autoprogram',
 ]
 
 setuptools.setup(
     name="capture_it",
-    version="0.0.8",
+    version="0.0.9",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="Excel Facts File Generate from Networking Device Output|Config",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aliasgar1978/capture_it",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
-    install_requires= ['nettoolkit', 'paramiko', 'netmiko'],
+    install_requires= ['nettoolkit', 'paramiko', 'netmiko', 'pandas', 'ntc-templates'],
     extras_require={'docs': docs_extras},
 )
```

