# Comparing `tmp/py_canoe-0.0.9.tar.gz` & `tmp/py_canoe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_canoe-0.0.9.tar", last modified: Mon Feb 20 09:11:16 2023, max compression
+gzip compressed data, was "py_canoe-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_canoe-0.0.9.tar` & `py_canoe-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     3687 2023-01-08 13:58:50.420817 py_canoe-0.0.9/.gitignore
--rw-r--r--   0        0        0     1095 2022-12-18 06:54:26.356765 py_canoe-0.0.9/LICENSE
--rw-r--r--   0        0        0     1919 2023-01-08 14:05:18.352024 py_canoe-0.0.9/README.md
--rw-r--r--   0        0        0      147 2022-12-29 19:20:40.396297 py_canoe-0.0.9/_config.yml
--rw-r--r--   0        0        0     1852 2023-01-08 14:05:48.211135 py_canoe-0.0.9/docs/index.md
--rw-r--r--   0        0        0      507 2022-12-29 19:30:02.384245 py_canoe-0.0.9/mkdocs.yml
--rw-r--r--   0        0        0      668 2023-02-20 09:09:18.719935 py_canoe-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       60 2022-12-29 20:50:53.462597 py_canoe-0.0.9/requirements.txt
--rwxr-xr-x   0        0        0      635 2022-12-18 07:09:21.046723 py_canoe-0.0.9/scripts/deploy_docs_to_github.bat
--rwxr-xr-x   0        0        0     1526 2022-12-23 07:47:04.149976 py_canoe-0.0.9/scripts/install_dependencies.bat
--rwxr-xr-x   0        0        0      589 2022-12-29 20:53:32.885605 py_canoe-0.0.9/scripts/run_pytests.bat
--rwxr-xr-x   0        0        0      608 2022-12-29 20:55:26.820229 py_canoe-0.0.9/scripts/upload_package_to_pypi.bat
--rw-r--r--   0        0        0       60 2022-12-29 14:19:23.145681 py_canoe-0.0.9/src/__int__.py
--rw-r--r--   0        0        0    45909 2023-02-20 09:04:48.533893 py_canoe-0.0.9/src/py_canoe.py
--rw-r--r--   0        0        0       31 2022-12-30 06:25:57.049797 py_canoe-0.0.9/tests/__int__.py
--rw-r--r--   0        0        0     2192 2013-04-25 09:58:36.000000 py_canoe-0.0.9/tests/demo_cfg/CANdb/easy.dbc
--rw-r--r--   0        0        0  1080368 2017-08-17 03:05:36.000000 py_canoe-0.0.9/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
--rw-r--r--   0        0        0     3708 2017-08-08 10:44:58.000000 py_canoe-0.0.9/tests/demo_cfg/Nodes/SimDiagECU.can
--rw-r--r--   0        0        0      928 2022-12-18 14:20:27.552310 py_canoe-0.0.9/tests/demo_cfg/Nodes/system_events.can
--rw-r--r--   0        0        0      256 2023-01-18 04:30:20.988239 py_canoe-0.0.9/tests/demo_cfg/Nodes/system_variables.can
--rw-r--r--   0        0        0     5436 2022-12-29 06:11:00.229069 py_canoe-0.0.9/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
--rw-r--r--   0        0        0   194208 2023-01-08 10:49:57.336430 py_canoe-0.0.9/tests/demo_cfg/demo.cfg
--rw-r--r--   0        0        0     2038 2023-01-08 13:46:31.030145 py_canoe-0.0.9/tests/test_canoe.py
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     3699 2023-06-21 03:21:26.026953 py_canoe-0.1.1/.gitignore
+-rw-r--r--   0        0        0     5330 2023-06-21 02:44:58.263085 py_canoe-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1095 2023-06-21 02:44:58.263085 py_canoe-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1919 2023-06-21 02:44:58.263085 py_canoe-0.1.1/README.md
+-rw-r--r--   0        0        0      147 2023-06-21 02:44:58.263085 py_canoe-0.1.1/_config.yml
+-rw-r--r--   0        0        0     1852 2023-06-21 02:44:58.273095 py_canoe-0.1.1/docs/index.md
+-rw-r--r--   0        0        0      507 2023-06-21 02:44:58.273095 py_canoe-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      668 2023-06-21 02:44:58.273095 py_canoe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-21 02:44:58.273095 py_canoe-0.1.1/requirements.txt
+-rwxr-xr-x   0        0        0      635 2023-06-29 17:56:00.911096 py_canoe-0.1.1/scripts/deploy_docs_to_github.bat
+-rwxr-xr-x   0        0        0     1526 2023-06-29 17:56:00.911096 py_canoe-0.1.1/scripts/install_dependencies.bat
+-rwxr-xr-x   0        0        0      589 2023-06-21 02:44:58.273095 py_canoe-0.1.1/scripts/run_pytests.bat
+-rwxr-xr-x   0        0        0      608 2023-06-21 02:44:58.273095 py_canoe-0.1.1/scripts/upload_package_to_pypi.bat
+-rw-r--r--   0        0        0        0 2023-06-29 17:34:50.054974 py_canoe-0.1.1/src/__int__.py
+-rw-r--r--   0        0        0    47393 2023-06-29 17:34:50.054974 py_canoe-0.1.1/src/py_canoe.py
+-rw-r--r--   0        0        0       31 2023-06-21 02:44:58.283091 py_canoe-0.1.1/tests/__int__.py
+-rw-r--r--   0        0        0     2192 2023-06-21 02:44:58.283091 py_canoe-0.1.1/tests/demo_cfg/CANdb/easy.dbc
+-rw-r--r--   0        0        0  1106768 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
+-rw-r--r--   0        0        0    11560 2023-06-29 17:34:50.054974 py_canoe-0.1.1/tests/demo_cfg/Logs/demo_log.blf
+-rw-r--r--   0        0        0     3708 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/SimDiagECU.can
+-rw-r--r--   0        0        0      928 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/system_events.can
+-rw-r--r--   0        0        0      256 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/system_variables.can
+-rw-r--r--   0        0        0     5436 2023-06-21 02:44:58.303089 py_canoe-0.1.1/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
+-rw-r--r--   0        0        0   203010 2023-06-29 17:34:50.064968 py_canoe-0.1.1/tests/demo_cfg/demo.cfg
+-rw-r--r--   0        0        0   194788 2023-06-29 17:34:50.064968 py_canoe-0.1.1/tests/demo_cfg/demo_offline.cfg
+-rw-r--r--   0        0        0     3627 2023-06-29 17:38:24.013024 py_canoe-0.1.1/tests/test_canoe.py
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.1.1/PKG-INFO
```

### Comparing `py_canoe-0.0.9/.gitignore` & `py_canoe-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+.venv_py*/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `py_canoe-0.0.9/LICENSE` & `py_canoe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/README.md` & `py_canoe-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/docs/index.md` & `py_canoe-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/pyproject.toml` & `py_canoe-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/scripts/deploy_docs_to_github.bat` & `py_canoe-0.1.1/scripts/deploy_docs_to_github.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/scripts/install_dependencies.bat` & `py_canoe-0.1.1/scripts/install_dependencies.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/scripts/run_pytests.bat` & `py_canoe-0.1.1/scripts/run_pytests.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/scripts/upload_package_to_pypi.bat` & `py_canoe-0.1.1/scripts/upload_package_to_pypi.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/src/py_canoe.py` & `py_canoe-0.1.1/src/py_canoe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,236 +1,271 @@
 """Python package for controlling Vector CANoe tool"""
 
-__version__ = "0.0.9"
+__version__ = "0.1.1"
 
 # Import Python Libraries here
 import os
-import sys
 import logging
-import pythoncom
-import win32com.client
 from typing import Union
 from logging import handlers
+from win32com.client import *
+from win32com.client.connect import *
 from time import sleep as wait
 
 
+def DoEvents():
+    pythoncom.PumpWaitingMessages()
+    wait(.1)
+
+
 class CANoe:
     r"""The CANoe class represents the CANoe application.
     The CANoe class is the foundation for the object hierarchy.
     You can reach all other methods from the CANoe class instance.
 
     Examples:
         >>> # Example to open CANoe configuration, start measurement, stop measurement and close configuration.
         >>> canoe_inst = CANoe(py_canoe_log_dir=r'D:\.py_canoe')
         >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
         >>> canoe_inst.start_measurement()
         >>> wait(10)
         >>> canoe_inst.stop_measurement()
         >>> canoe_inst.quit()
     """
+    Started = False
+    Stopped = False
 
-    def __init__(self, py_canoe_log_dir=r'D:\.py_canoe') -> None:
+    def __init__(self, py_canoe_log_dir='') -> None:
         """
         Args:
-            py_canoe_log_dir (str): directory to store py_canoe log. default 'D:\\.py_canoe'
+            py_canoe_log_dir (str): directory to store py_canoe log. example 'D:\\.py_canoe'
         """
-        self.__canoe_app_obj = None
-        self.__CANOE_COM_APP_NAME = 'CANoe.Application'
-        self.__BUS_TYPES = {'CAN': 1, 'J1939': 2, 'TTP': 4, 'LIN': 5, 'MOST': 6, 'Kline': 14}
-        self.APP_DELAY = 1
         self.log = logging.getLogger('CANOE_LOG')
         self.__py_canoe_log_initialisation(py_canoe_log_dir)
-        self.__sys_vars_obj_dictionary = {}
-        self.__networks_obj_dictionary = {}
-        self.__network_devices_obj_dictionary = {}
+        self.__canoe_objects = {}
+        self.__dispatch_canoe()
+        self.wait_for_start = lambda: DoEventsUntil(lambda: CANoe.Started)
+        self.wait_for_stop = lambda: DoEventsUntil(lambda: CANoe.Stopped)
+        self.__triggered_canoe_quit = False
+        self.__BUS_TYPES = {'CAN': 1, 'J1939': 2, 'TTP': 4, 'LIN': 5, 'MOST': 6, 'Kline': 14}
         self.__diag_ecu_qualifiers_dictionary = {}
         self.__replay_blocks_obj_dictionary = {}
-        self.__simulation_nodes_obj_dictionary = {}
 
-    def __py_canoe_log_initialisation(self, py_canoe_log_dir=r'D:\.py_canoe'):
-        if not os.path.exists(py_canoe_log_dir):
-            os.makedirs(py_canoe_log_dir, exist_ok=True)
+    def __py_canoe_log_initialisation(self, py_canoe_log_dir):
         self.log.setLevel(logging.DEBUG)
         log_format = logging.Formatter("%(asctime)s [CANOE_LOG] [%(levelname)-5.5s]  %(message)s")
         ch = logging.StreamHandler(sys.stdout)
         ch.setFormatter(log_format)
         self.log.addHandler(ch)
-        fh = handlers.RotatingFileHandler(fr'{py_canoe_log_dir}\py_canoe.log', maxBytes=(1024 * 50), backupCount=20)
-        fh.setFormatter(log_format)
-        self.log.addHandler(fh)
-
-    def __dispatch_canoe(self) -> None:
-        if self.__canoe_app_obj is None:
-            pythoncom.CoInitialize()
-            self.__canoe_app_obj = win32com.client.Dispatch(self.__CANOE_COM_APP_NAME)
-            self.log.info('Dispatched CANoe win32com client.')
-        else:
-            self.log.info('CANoe win32com client already Dispatched')
-
-    def __fetch_canoe_cfg_general_data(self):
-        system_namespaces_obj = self.__canoe_app_obj.System.Namespaces
-        self.__ui_obj = self.__canoe_app_obj.UI
-        # self.__version_obj = self.__canoe_app_obj.Version
-
-        def fetch_variables(namespace_obj, namespace_name):
-            variables_obj = namespace_obj.Variables
-            for variable_obj in variables_obj:
-                variable_name = f"{namespace_name}::{variable_obj.Name}"
-                self.__sys_vars_obj_dictionary[variable_name] = variable_obj
-
-        def fetch_namespaces(namespace_obj, obj_name):
-            fetch_variables(namespace_obj, obj_name)
-            for ns in namespace_obj.Namespaces:
-                fetch_namespaces(ns, f'{obj_name}::{ns.Name}')
-
-        for namespace in system_namespaces_obj:
-            fetch_namespaces(namespace, namespace.Name)
-        for n in self.__canoe_app_obj.Networks:
-            self.__networks_obj_dictionary[n.Name] = n
-            self.__network_devices_obj_dictionary[n.Name] = {}
-            for d in n.Devices:
-                self.__network_devices_obj_dictionary[n.Name][d.Name] = d
+        if py_canoe_log_dir != '' and not os.path.exists(py_canoe_log_dir):
+            os.makedirs(py_canoe_log_dir, exist_ok=True)
+        if os.path.exists(py_canoe_log_dir):
+            fh = handlers.RotatingFileHandler(fr'{py_canoe_log_dir}\py_canoe.log', maxBytes=(1024 * 50), backupCount=20)
+            fh.setFormatter(log_format)
+            self.log.addHandler(fh)
+
+    def __dispatch_canoe(self):
+        app = DispatchEx('CANoe.Application')
+        app.Configuration.Modified = False
+        ver = app.Version
+        self.log.info(f'Dispatched CANoe Application {ver.major}.{ver.minor}.{ver.Build}...')
+        self.__canoe_objects['Application'] = app
+        self.__canoe_objects['Application.Configuration'] = self.__canoe_objects['Application'].Configuration
+        self.__canoe_objects['Application.Measurement'] = self.__canoe_objects['Application'].Measurement
+        self.__canoe_objects['Application.Measurement.Running'] = self.__canoe_objects['Application.Measurement'].Running
+        self.wait_for_start = lambda: DoEventsUntil(lambda: CANoe.Started)
+        self.wait_for_stop = lambda: DoEventsUntil(lambda: CANoe.Stopped)
+        WithEvents(self.__canoe_objects['Application.Measurement'], CanoeMeasurementEvents)
+
+    def __fetch_canoe_networks_data(self) -> dict:
+        self.__canoe_objects['Application.Networks'] = self.__canoe_objects['Application'].Networks
+        canoe_networks_dict = {}
+        for network in self.__canoe_objects['Application.Networks']:
+            network_name = network.Name
+            canoe_networks_dict[network_name] = {}
+            canoe_networks_dict[network_name]['network_obj'] = network
+            # canoe_networks_dict[network_name]['BusType'] = network.BusType
+            canoe_networks_dict[network_name]['Devices'] = {}
+            for device in network.Devices:
+                device_name = device.Name
+                canoe_networks_dict[network_name]['Devices'][device_name] = {}
+                canoe_networks_dict[network_name]['Devices'][device_name]['device_obj'] = device
                 try:
-                    self.__diag_ecu_qualifiers_dictionary[d.Name] = d.Diagnostic
+                    canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj'] = device.Diagnostic
+                    self.__diag_ecu_qualifiers_dictionary[device_name] = canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj']
                 except pythoncom.com_error:
-                    pass
-        for rb in self.__canoe_app_obj.Bus.ReplayCollection:
-            self.__replay_blocks_obj_dictionary[rb.Name] = rb
-        for sn in self.__canoe_app_obj.Configuration.SimulationSetup.Nodes:
-            self.__simulation_nodes_obj_dictionary[sn.Name] = sn
+                    canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj'] = None
+        return canoe_networks_dict
+
+    def __fetch_canoe_system_data(self) -> dict:
+        self.__canoe_objects['Application.System'] = self.__canoe_objects['Application'].System
+        self.__canoe_objects['Application.System.Namespaces'] = self.__canoe_objects['Application.System'].Namespaces
+        self.__canoe_objects['Application.System.VariablesFiles'] = self.__canoe_objects['Application.System'].VariablesFiles
+        canoe_system_dict = {'Namespaces': {},
+                             'VariablesFiles': {}}
+        namespaces_dict = {}
+        for namespace in self.__canoe_objects['Application.System.Namespaces']:
+            namespaces_dict[namespace.Name] = namespace
+        canoe_system_dict['Namespaces'] = namespaces_dict
+        variable_files_dict = {}
+        for variables_file in self.__canoe_objects['Application.System.VariablesFiles']:
+            variable_files_dict[variables_file.Name] = variables_file
+        canoe_system_dict['VariablesFiles'] = variable_files_dict
+        return canoe_system_dict
+
+    def __fetch_canoe_bus_data(self) -> dict:
+        self.__canoe_objects['Application.Bus'] = self.__canoe_objects['Application'].Bus
+        self.__canoe_objects['Application.Bus.ReplayCollection'] = self.__canoe_objects['Application.Bus'].ReplayCollection
+        self.__canoe_objects['Application.Bus.Nodes'] = self.__canoe_objects['Application.Bus'].Nodes
+        canoe_bus_dict = {}
+        replay_blocks_dict = {}
+        nodes_dict = {}
+        for replay_block in self.__canoe_objects['Application.Bus.ReplayCollection']:
+            replay_blocks_dict[replay_block.Name] = replay_block
+        for node in self.__canoe_objects['Application.Bus.Nodes']:
+            nodes_dict[node.Name] = node
+        canoe_bus_dict['replay_block_objs'] = self.__replay_blocks_obj_dictionary = replay_blocks_dict
+        canoe_bus_dict['node_objs'] = nodes_dict
+        return canoe_bus_dict
 
     def open(self, canoe_cfg: str, visible=True, auto_save=False, prompt_user=False) -> None:
         r"""Loads CANoe configuration.
 
         Args:
             canoe_cfg (str): The complete path for the CANoe configuration.
             visible (bool): True if you want to see CANoe UI. Defaults to True.
             auto_save (bool, optional): A boolean value that indicates whether the active configuration should be saved if it has been changed. Defaults to False.
             prompt_user (bool, optional): A boolean value that indicates whether the user should intervene in error situations. Defaults to False.
-        
+
         Examples:
             >>> # The following example opens a configuration
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
         """
+        if self.__triggered_canoe_quit:
+            self.__dispatch_canoe()
         if os.path.isfile(canoe_cfg):
             self.log.info(f'CANoe cfg "{canoe_cfg}" found.')
-            self.__dispatch_canoe()
-            self.__canoe_app_obj.Visible = visible
-            self.__canoe_app_obj.Open(canoe_cfg, auto_save, prompt_user)
+            self.__canoe_objects['Application'].Visible = visible
+            self.__canoe_objects['Application'].Open(canoe_cfg, auto_save, prompt_user)
             self.log.info(f'loaded CANoe config "{canoe_cfg}"')
-            self.__fetch_canoe_cfg_general_data()
-            self.log.info('Fetched CANoe System Variables.')
+            self.__fetch_canoe_networks_data()
+            self.__fetch_canoe_system_data()
+            self.__fetch_canoe_bus_data()
         else:
             self.log.info(f'CANoe cfg "{canoe_cfg}" not found.')
+        self.__triggered_canoe_quit = False
 
     def new(self, auto_save=False, prompt_user=False) -> None:
         """Creates a new configuration.
 
         Args:
             auto_save (bool, optional): A boolean value that indicates whether the active configuration should be saved if it has been changed. Defaults to False.
             prompt_user (bool, optional): A boolean value that indicates whether the user should intervene in error situations. Defaults to False.
-        
+
         Examples:
             >>> # The following example creates a new configuration
             >>> canoe_inst = CANoe()
             >>> canoe_inst.new()
         """
         self.__dispatch_canoe()
-        self.__canoe_app_obj.New(auto_save, prompt_user)
+        self.__canoe_objects['Application'].New(auto_save, prompt_user)
         self.log.info('created a new configuration')
 
     def quit(self) -> None:
         r"""Quits CANoe without saving changes in the configuration.
-        
+
         Examples:
             >>> # The following example quits CANoe
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.quit()
         """
-        if self.__canoe_app_obj.Measurement.Running:
+        if self.__canoe_objects['Application'].Measurement.Running:
             self.stop_measurement()
-        self.__canoe_app_obj.Configuration.Modified = False
-        self.__canoe_app_obj.Quit()
-        self.log.info('CANoe Closed without saving.')
+        self.__canoe_objects['Application'].Configuration.Modified = False
+        self.__canoe_objects['Application'].Quit()
+        self.__triggered_canoe_quit = True
+        self.log.info('CANoe Application Closed without saving configuration.')
 
     def start_measurement_in_animation_mode(self, animation_delay=100) -> None:
         r"""Starts the measurement in Animation mode.
 
         Args:
             animation_delay (int): The animation delay during the measurement in Offline Mode.
 
         Examples:
             >>> # The following example starts the measurement in Animation mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement_in_animation_mode()
         """
-        if not self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.AnimationDelay = animation_delay
-            self.__canoe_app_obj.Measurement.Animate()
+        if not self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.AnimationDelay = animation_delay
+            self.__canoe_objects['Application'].Measurement.Animate()
             self.log.info(f'Started the measurement in Animation mode with animation delay = {animation_delay}.')
 
     def break_measurement_in_offline_mode(self) -> None:
         r"""Interrupts the playback in Offline mode.
 
         Examples:
             >>> # The following example interrupts the playback in Offline mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.break_measurement_in_offline_mode()
         """
-        if self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.Break()
+        if self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.Break()
             self.log.info('Interrupted the playback in Offline mode.')
 
     def reset_measurement_in_offline_mode(self) -> None:
         r"""Resets the measurement in Offline mode.
 
         Examples:
             >>> # The following example resets the measurement in Offline mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.reset_measurement_in_offline_mode()
         """
-        self.__canoe_app_obj.Measurement.Reset()
+        self.__canoe_objects['Application'].Measurement.Reset()
         self.log.info('resetted measurement in offline mode.')
 
     def start_measurement(self) -> bool:
         r"""Starts the measurement.
 
         Returns:
             True if measurement started. else Flase.
 
         Examples:
             >>> # The following example starts the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
         """
-        if not self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.Start()
-            if not self.__canoe_app_obj.Measurement.Running:
-                self.log.info(f'waiting({self.APP_DELAY}s) for measurement to start running.')
-                wait(self.APP_DELAY)
-            self.log.info(f'CANoe Measurement Running Status: {self.__canoe_app_obj.Measurement.Running}')
-        return self.__canoe_app_obj.Measurement.Running
+        if not self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.Start()
+            if not self.__canoe_objects['Application'].Measurement.Running:
+                self.log.info(f'waiting for measurement to start...')
+                self.wait_for_start()
+            self.log.info(f'CANoe Measurement Started. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        else:
+            self.log.info(f'CANoe Measurement Already Running. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        return self.__canoe_objects['Application'].Measurement.Running
 
     def step_measurement_event_in_single_step(self) -> None:
         r"""Processes a measurement event in single step.
 
         Examples:
             >>> # The following example processes a measurement event in single step
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.step_measurement_event_in_single_step()
         """
-        if not self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.Step()
+        if not self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.Step()
             self.log.info('processed a measurement event in single step')
 
     def stop_measurement(self) -> bool:
         r"""Stops the measurement.
 
         Returns:
             True if measurement stopped. else Flase.
@@ -238,57 +273,54 @@
         Examples:
             >>> # The following example stops the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
         """
-        if self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.Stop()
-            for i in range(5):
-                if self.__canoe_app_obj.Measurement.Running:
-                    self.log.info(f'CANoe Simulation still running. waiting for {self.APP_DELAY} seconds.')
-                    wait(self.APP_DELAY)
-                else:
-                    break
-        self.log.info(f'Triggered stop measurement. Measurement running status = {self.__canoe_app_obj.Measurement.Running}')
-        return not self.__canoe_app_obj.Measurement.Running
+        if self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.Stop()
+            self.wait_for_stop()
+            self.log.info(f'CANoe Measurement Stopped. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        else:
+            self.log.info(f'CANoe Measurement Already Stopped. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        return not self.__canoe_objects['Application'].Measurement.Running
 
     def reset_measurement(self) -> bool:
         r"""reset the measurement.
 
         Returns:
             Measurement running status(True/False).
 
         Examples:
             >>> # The following example resets the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.reset_measurement()
         """
-        if self.__canoe_app_obj.Measurement.Running:
+        if self.__canoe_objects['Application'].Measurement.Running:
             self.stop_measurement()
         self.start_measurement()
-        self.log.info(f'Resetted measurement. Measurement running status = {self.__canoe_app_obj.Measurement.Running}')
-        return self.__canoe_app_obj.Measurement.Running
+        self.log.info(f'Resetted measurement. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        return self.__canoe_objects['Application'].Measurement.Running
 
     def stop_ex_measurement(self) -> None:
         r"""StopEx repairs differences in the behavior of the Stop method on deferred stops concerning simulated and real mode in CANoe.
 
         Examples:
             >>> # The following example full stops the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_ex_measurement()
         """
-        if self.__canoe_app_obj.Measurement.Running:
-            self.__canoe_app_obj.Measurement.StopEx()
-            self.log.info(f'Stopped measurement. Measurement running status = {self.__canoe_app_obj.Measurement.Running}')
+        if self.__canoe_objects['Application'].Measurement.Running:
+            self.__canoe_objects['Application'].Measurement.StopEx()
+            self.log.info(f'Stopped measurement. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
 
     def get_measurement_index(self) -> int:
         r"""gets the measurement index for the next measurement.
 
         Returns:
             Measurement Index.
 
@@ -296,15 +328,17 @@
             >>> # The following example gets the measurement index measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.get_measurement_index()
         """
-        return self.__canoe_app_obj.Measurement.MeasurementIndex
+        measurement_index = self.__canoe_objects['Application'].Measurement.MeasurementIndex
+        self.log.info(f'measurement_index value = {measurement_index}')
+        return measurement_index
 
     def set_measurement_index(self, index: int) -> int:
         r"""sets the measurement index for the next measurement.
 
         Args:
             index (int): index value to set.
 
@@ -315,17 +349,17 @@
             >>> # The following example sets the measurement index for the next measurement to 15
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.set_measurement_index(15)
         """
-        self.__canoe_app_obj.Measurement.MeasurementIndex = index
+        self.__canoe_objects['Application'].Measurement.MeasurementIndex = index
         self.log.info(f'CANoe measurement index set to {index}')
-        return self.__canoe_app_obj.Measurement.MeasurementIndex
+        return self.__canoe_objects['Application'].Measurement.MeasurementIndex
 
     def get_measurement_running_status(self) -> bool:
         r"""Returns the running state of the measurement.
 
         Returns:
             True if The measurement is running.
             False if The measurement is not running.
@@ -333,61 +367,69 @@
         Examples:
             >>> # The following example returns measurement running status (True/False)
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.get_measurement_running_status()
         """
-        self.log.info(f'CANoe Measurement Running Status = {self.__canoe_app_obj.Measurement.Running}')
-        return self.__canoe_app_obj.Measurement.Running
+        self.log.info(f'CANoe Measurement Running Status = {self.__canoe_objects["Application"].Measurement.Running}')
+        return self.__canoe_objects['Application'].Measurement.Running
 
     def save_configuration(self) -> bool:
         r"""Saves the configuration.
 
         Returns:
             True if configuration saved. else False.
 
         Examples:
             >>> # The following example saves the configuration if necessary
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.save_configuration()
         """
-        if not self.__canoe_app_obj.Configuration.Saved:
-            self.__canoe_app_obj.Configuration.Save()
+        if not self.__canoe_objects['Application'].Configuration.Saved:
+            self.__canoe_objects['Application'].Configuration.Save()
             self.log.info('CANoe Configuration saved.')
-        return self.__canoe_app_obj.Configuration.Saved
+        else:
+            self.log.info('CANoe Configuration already in saved state.')
+        return self.__canoe_objects['Application'].Configuration.Saved
 
-    def save_configuration_as(self, path: str, major: int, minor: int) -> bool:
+    def save_configuration_as(self, path: str, major: int, minor: int, create_dir=True) -> bool:
         r"""Saves the configuration as a different CANoe version.
 
         Args:
             path (str): The complete file name.
             major (int): The major version number of the target version.
             minor (int): The minor version number of the target version.
+            create_dir (bool): create dirrectory if not available. default value True.
 
         Returns:
             True if configuration saved. else False.
 
         Examples:
             >>> # The following example saves the configuration as a CANoe 10.0 version
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.save_configuration_as(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo_v12.cfg', 10, 0)"""
-        if not self.__canoe_app_obj.Configuration.Saved:
-            self.__canoe_app_obj.Configuration.Save()
-        self.__canoe_app_obj.Configuration.SaveAs(path, major, minor)
-        self.log.info(f'CANoe Configuration saved as {path}.')
-        return self.__canoe_app_obj.Configuration.Saved
+        config_path = '\\'.join(path.split('\\')[:-1])
+        if not os.path.exists(config_path) and create_dir:
+            os.makedirs(config_path, exist_ok=True)
+        if os.path.exists(config_path):
+            self.__canoe_objects['Application'].Configuration.SaveAs(path, major, minor)
+            self.log.info(f'CANoe Configuration saved as {path}.')
+            return self.__canoe_objects['Application'].Configuration.Saved
+        else:
+            self.log.info(f'tried creating {path}. but {config_path} directory not found.')
+            return False
 
     def get_signal_value(self, bus: str, channel: int, message: str, signal: str, raw_value=False) -> Union[float, int]:
         r"""get_signal_value Returns a Signal value.
 
         Args:
-            bus (str): The Bus(CAN, LIN, FlexRay, MOST, AFDX, Ethernet)(CAN, LIN, FlexRay, MOST, AFDX, Ethernet) on which the signal is sent.
+            bus (str): The Bus(CAN, LIN, FlexRay, MOST, AFDX, Ethernet) on which the signal is sent.
             channel (int): The channel on which the signal is sent.
             message (str): The name of the message to which the signal belongs.
             signal (str): The name of the signal.
             raw_value (bool): return raw value of the signal if true. Default(False) is physical value.
 
         Returns:
             signal vaue.
@@ -396,21 +438,21 @@
             >>> # The following example gets signal value
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> sig_val = canoe_inst.get_signal_value('CAN', 1, 'LightState', 'FlashLight')
             >>> print(sig_val)
         """
-        signal_obj = self.__canoe_app_obj.GetBus(bus).GetSignal(channel, message, signal)
+        signal_obj = self.__canoe_objects['Application'].GetBus(bus).GetSignal(channel, message, signal)
         signal_value = signal_obj.RawValue if raw_value else signal_obj.Value
         self.log.info(f'value of signal({bus}{channel}.{message}.{signal})={signal_value}.')
         return signal_value
 
     def set_signal_value(self, bus: str, channel: int, message: str, signal: str, value: Union[float, int], raw_value=False) -> None:
-        r"""set_signal_value sets a value to Signal. Works only when messages are sent using CANoe IL.  
+        r"""set_signal_value sets a value to Signal. Works only when messages are sent using CANoe IL.
 
         Args:
             bus (str): The Bus(CAN, LIN, FlexRay, MOST, AFDX, Ethernet) on which the signal is sent.
             channel (int): The channel on which the signal is sent.
             message (str): The name of the message to which the signal belongs.
             signal (str): The name of the signal.
             value (Union[float, int]): signal value.
@@ -419,15 +461,15 @@
         Examples:
             >>> # The following example sets signal value to 1
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.set_signal_value('CAN', 1, 'LightState', 'FlashLight', 1)
         """
-        signal_obj = self.__canoe_app_obj.GetBus(bus).GetSignal(channel, message, signal)
+        signal_obj = self.__canoe_objects['Application'].GetBus(bus).GetSignal(channel, message, signal)
         if raw_value:
             signal_obj.RawValue = value
         else:
             signal_obj.Value = value
         self.log.info(f'signal({bus}{channel}.{message}.{signal}) value set to {value}.')
 
     def check_signal_online(self, bus: str, channel: int, message: str, signal: str) -> bool:
@@ -437,23 +479,23 @@
             bus (str): The Bus(CAN, LIN, FlexRay, MOST, AFDX, Ethernet) on which the signal is sent.
             channel (int): The channel on which the signal is sent.
             message (str): The name of the message to which the signal belongs.
             signal (str): The name of the signal.
 
         Returns:
             TRUE if the measurement is running and the signal has been received. FALSE if not.
-        
+
         Examples:
             >>> # The following example checks signal is online.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.check_signal_online('CAN', 1, 'LightState', 'FlashLight')
         """
-        sig_online_status = self.__canoe_app_obj.GetBus(bus).GetSignal(channel, message, signal).IsOnline
+        sig_online_status = self.__canoe_objects['Application'].GetBus(bus).GetSignal(channel, message, signal).IsOnline
         self.log.info(f'signal({bus}{channel}.{message}.{signal}) online status = {sig_online_status}.')
         return sig_online_status
 
     def check_signal_state(self, bus: str, channel: int, message: str, signal: str) -> int:
         r"""Checks whether the measurement is running and the signal has been received.
 
         Args:
@@ -472,15 +514,15 @@
         Examples:
             >>> # The following example checks signal state.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.check_signal_state('CAN', 1, 'LightState', 'FlashLight')
         """
-        sig_state = self.__canoe_app_obj.GetBus(bus).GetSignal(channel, message, signal).State
+        sig_state = self.__canoe_objects['Application'].GetBus(bus).GetSignal(channel, message, signal).State
         self.log.info(f'signal({bus}{channel}.{message}.{signal}) state = {sig_state}.')
         return sig_state
 
     def get_j1939_signal_value(self, bus: str, channel: int, message: str, signal: str, source_addr: int, dest_addr: int,
                                raw_value=False) -> Union[float, int]:
         r"""get_j1939_signal Returns a Signal object.
 
@@ -500,15 +542,15 @@
             >>> # The following example gets j1939 signal value
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> sig_val = canoe_inst.get_j1939_signal_value('CAN', 1, 'LightState', 'FlashLight', 0, 1)
             >>> print(sig_val)
         """
-        signal_obj = self.__canoe_app_obj.GetBus(bus).GetJ1939Signal(channel, message, signal, source_addr, dest_addr)
+        signal_obj = self.__canoe_objects['Application'].GetBus(bus).GetJ1939Signal(channel, message, signal, source_addr, dest_addr)
         signal_value = signal_obj.RawValue if raw_value else signal_obj.Value
         self.log.info(f'value of signal({bus}{channel}.{message}.{signal})={signal_value}.')
         return signal_value
 
     def set_j1939_signal_value(self, bus: str, channel: int, message: str, signal: str, source_addr: int, dest_addr: int, value: Union[float, int],
                                raw_value=False) -> None:
         r"""get_j1939_signal Returns a Signal object.
@@ -529,152 +571,49 @@
         Examples:
             >>> # The following example gets j1939 signal value
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.set_j1939_signal_value('CAN', 1, 'LightState', 'FlashLight', 0, 1, 1)
         """
-        signal_obj = self.__canoe_app_obj.GetBus(bus).GetJ1939Signal(channel, message, signal, source_addr, dest_addr)
+        signal_obj = self.__canoe_objects['Application'].GetBus(bus).GetJ1939Signal(channel, message, signal, source_addr, dest_addr)
         if raw_value:
             signal_obj.RawValue = value
         else:
             signal_obj.Value = value
         self.log.info(f'signal({bus}{channel}.{message}.{signal}) value set to {value}.')
 
-    def get_system_variable_value(self, sys_var_name: str) -> Union[int, float, str]:
-        r"""get_system_variable_value Returns a system variable value.
-
-        Args:
-            sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
-
-        Returns:
-            System Variable value.
-
-        Examples:
-            >>> # The following example gets system variable value
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_inst.start_measurement()
-            >>> sys_var_val = canoe_inst.get_system_variable_value('sys_var_demo::speed')
-            >>>print(sys_var_val)
-        """
-        variable_value = None
-        if sys_var_name in self.__sys_vars_obj_dictionary.keys():
-            variable_value = self.__sys_vars_obj_dictionary[sys_var_name].Value
-            self.log.info(f'system variable({sys_var_name}) value = {variable_value}.')
-        else:
-            self.log.warning(f'system variable({sys_var_name}) not available in loaded CANoe config.')
-        return variable_value
-
-    def set_system_variable_value(self, sys_var_name: str, value: Union[int, float, str]) -> None:
-        r"""set_system_variable_value sets a value to system variable.
-
-        Args:
-            sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
-            value (Union[int, float, str]): variable value.
-
-        Examples:
-            >>> # The following example sets system variable value to 1
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_inst.start_measurement()
-            >>> canoe_inst.set_system_variable_value('sys_var_demo::speed', 1)
-        """
-        if sys_var_name in self.__sys_vars_obj_dictionary.keys():
-            self.__sys_vars_obj_dictionary[sys_var_name].Value = value
-            self.log.info(f'system variable({sys_var_name}) value set to {value}.')
-        else:
-            self.log.warning(f'system variable({sys_var_name}) not available in loaded CANoe config.')
-
-    def send_diag_request(self, diag_ecu_qualifier_name: str, request: str, request_in_bytes=True) -> str:
-        r"""The send_diag_request method represents the query of a diagnostic tester (client) to an ECU (server) in CANoe.
-
-        Args:
-            diag_ecu_qualifier_name (str): Diagnostic Node ECU Qualifier Name configured in "Diagnostic/ISO TP Configuration".
-            request (str): Diagnostic request in bytes or diagnostic node qualifier name.
-            request_in_bytes: True if Diagnostic request is bytes. False if you are using Qualifier name. Default is True.
-
-        Returns:
-            diagnostic response stream. Ex- "50 01 00 00 00 00"
-
-        Examples:
-            >>> # Example 1 - The following example sends diagnostic request "10 01"
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_inst.start_measurement()
-            >>> wait(1)
-            >>> resp = canoe_inst.send_diag_request('Door', '10 01')
-            >>> print(resp)
-            >>> canoe_inst.stop_measurement()
-            >>> # Example 2 - The following example sends diagnostic request "DefaultSession_Start"
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(canoe_cfg=r'C:\Users\Public\Documents\Vector\CANoe\Sample Configurations 11.0.81\.\CAN\Diagnostics\UDSBasic\UDSBasic.cfg')
-            >>> canoe_inst.start_measurement()
-            >>> wait(1)
-            >>> resp = canoe_inst.send_diag_request('Door', 'DefaultSession_Start', False)
-            >>> print(resp)
-            >>> canoe_inst.stop_measurement()
-        """
-        diag_response_data = ""
-        if diag_ecu_qualifier_name in self.__diag_ecu_qualifiers_dictionary.keys():
-            self.log.info(f'Diag Req --> {request}')
-            if request_in_bytes:
-                diag_req_in_bytes = bytearray()
-                request = ''.join(request.split(' '))
-                for i in range(0, len(request), 2):
-                    diag_req_in_bytes.append(int(request[i:i + 2], 16))
-                diag_req = self.__diag_ecu_qualifiers_dictionary[diag_ecu_qualifier_name].CreateRequestFromStream(diag_req_in_bytes)
-            else:
-                diag_req = self.__diag_ecu_qualifiers_dictionary[diag_ecu_qualifier_name].CreateRequest(request)
-            diag_req.Send()
-            while diag_req.Pending:
-                wait(0.1)
-            if diag_req.Responses.Count == 0:
-                self.log.info("Diagnostic Response Not Received.")
-            else:
-                for k in range(1, diag_req.Responses.Count + 1):
-                    diag_res = diag_req.Responses(k)
-                    if diag_res.Positive:
-                        self.log.info(f"+ve response received.")
-                    else:
-                        self.log.info(f"-ve response received.")
-                    diag_response_data = " ".join(f"{d:02X}" for d in diag_res.Stream).upper()
-                self.log.info(f'Diag Res --> {diag_response_data}')
-        else:
-            self.log.info(f'Diag ECU qualifier({diag_ecu_qualifier_name}) not available in loaded CANoe config.')
-        return diag_response_data
-
     def ui_activate_desktop(self, name: str) -> None:
         r"""Activates the desktop with the given name.
 
         Args:
             name (str): The name of the desktop to be activated.
 
         Examples:
             >>> # The following example switches to the desktop with the name "Configuration"
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.ui_activate_desktop("Configuration")
         """
-        self.__canoe_app_obj.UI.ActivateDesktop(name)
+        self.__canoe_objects['Application'].UI.ActivateDesktop(name)
         self.log.info(f'Activated / switched to "{name}" Desktop')
 
     def ui_open_baudrate_dialog(self) -> None:
         r"""opens the dialog for configuring the bus parameters. Make sure Measurement stopped when using this method.
 
         Examples:
             >>> # The following example opens the dialog for configuring the bus parameters
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.ui_open_baudrate_dialog()
         """
         self.log.info('opened the dialog for configuring the bus parameters')
-        self.__canoe_app_obj.UI.OpenBaudrateDialog()
+        self.__canoe_objects['Application'].UI.OpenBaudrateDialog()
 
     def write_text_in_write_window(self, text: str) -> None:
         r"""Outputs a line of text in the Write Window.
         Args:
             text (str): The text.
 
         Examples:
@@ -683,15 +622,15 @@
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> print(canoe_inst.read_text_from_write_window())
         """
-        self.__canoe_app_obj.UI.Write.Output(text)
+        self.__canoe_objects['Application'].UI.Write.Output(text)
         self.log.info(f'written "{text}" to Write Window')
 
     def read_text_from_write_window(self) -> str:
         r"""read the text contents from Write Window.
 
         Returns:
             The text content.
@@ -702,30 +641,30 @@
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> print(canoe_inst.read_text_from_write_window())
         """
-        return self.__canoe_app_obj.UI.Write.Text
+        return self.__canoe_objects['Application'].UI.Write.Text
 
     def clear_write_window_content(self) -> None:
         r"""Clears the contents of the Write Window.
 
         Examples:
             >>> # The following example clears content from Write Window.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> canoe_inst.clear_write_window_content()
         """
-        self.__canoe_app_obj.UI.Write.Clear()
+        self.__canoe_objects['Application'].UI.Write.Clear()
         self.log.info(f'Cleared Write Window Content.')
 
     def enable_write_window_output_file(self, output_file: str) -> None:
         r"""Enables logging of all outputs of the Write Window in the output file.
 
         Args:
             output_file (str): The complete path of the output file.
@@ -737,72 +676,28 @@
             >>> canoe_inst.enable_write_window_output_file(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\write_out.txt')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> canoe_inst.stop_measurement()
         """
-        self.__canoe_app_obj.UI.Write.EnableOutputFile(output_file)
+        self.__canoe_objects['Application'].UI.Write.EnableOutputFile(output_file)
         self.log.info(f'Enabled Write Window logging. file path --> {output_file}')
 
     def disable_write_window_output_file(self) -> None:
         r"""Disables logging of all outputs of the Write Window.
 
         Examples:
             >>> # The following example Disables logging of all outputs of the Write Window.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.disable_write_window_output_file()
         """
-        self.__canoe_app_obj.UI.Write.DisableOutputFile()
-        self.log.info(f'Enabled Write Window logging.')
-
-    def set_replay_block_file(self, block_name: str, recording_file_path: str) -> None:
-        r"""Method for setting CANoe replay block file.
-
-        Args:
-            block_name: CANoe replay block name
-            recording_file_path: CANoe replay recording file including path.
-
-        Examples:
-            >>> # The following example sets replay block file
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_inst.set_replay_block_file(block_name='replay block name', recording_file_path='replay file including path')
-            >>> canoe_inst.start_measurement()
-        """
-        if block_name in self.__replay_blocks_obj_dictionary.keys():
-            self.__replay_blocks_obj_dictionary[block_name].Path = recording_file_path
-            self.log.info(f'Replay block "{block_name}" updated with "{recording_file_path}" path.')
-        else:
-            self.log.warning(f'Replay block "{block_name}" not available.')
-
-    def control_replay_block(self, block_name: str, start_stop: bool) -> None:
-        r"""Method for setting CANoe replay block file.
-
-        Args:
-            block_name (str): CANoe replay block name
-            start_stop (bool): True to start replay block. False to Stop.
-
-        Examples:
-            >>> # The following example starts replay block
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_inst.set_replay_block_file(block_name='replay block name', recording_file_path='replay file including path')
-            >>> canoe_inst.start_measurement()
-            >>> canoe_inst.control_replay_block('replay block name', True)
-        """
-        if block_name in self.__replay_blocks_obj_dictionary.keys():
-            if start_stop:
-                self.__replay_blocks_obj_dictionary[block_name].Start()
-            else:
-                self.__replay_blocks_obj_dictionary[block_name].Stop()
-            self.log.info(f'Replay block "{block_name}" {"Started" if start_stop else "Stopped"}.')
-        else:
-            self.log.warning(f'Replay block "{block_name}" not available.')
+        self.__canoe_objects['Application'].UI.Write.DisableOutputFile()
+        self.log.info(f'Disabled Write Window logging.')
 
     def get_can_bus_statistics(self, channel: int) -> dict:
         r"""Returns CAN Bus Statistics.
 
         Args:
             channel (int): The channel of the statistic that is to be returned.
 
@@ -811,15 +706,15 @@
 
         Examples:
             >>> # The following example prints CAN channel 1 statistics
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> print(canoe_inst.get_can_bus_statistics(channel=1))
         """
-        bus_statistics_obj = self.__canoe_app_obj.Configuration.OnlineSetup.BusStatistics.BusStatistic(self.__BUS_TYPES['CAN'], channel)
+        bus_statistics_obj = self.__canoe_objects['Application'].Configuration.OnlineSetup.BusStatistics.BusStatistic(self.__BUS_TYPES['CAN'], channel)
         statistics_info = {
             # The bus load
             'bus_load': bus_statistics_obj.BusLoad,
             # The controller status
             'chip_state': bus_statistics_obj.ChipState,
             # The number of Error Frames per second
             'error': bus_statistics_obj.Error,
@@ -848,58 +743,14 @@
             # The total number of remote messages with standard identifier
             'standard_remote_total': bus_statistics_obj.StandardRemoteTotal,
             # The current number of the Tx error counter
             'tx_error_count': bus_statistics_obj.TxErrorCount,
         }
         return statistics_info
 
-    def get_canoe_configuration_details(self) -> dict:
-        r"""Returns Loaded CANoe configuration details.
-
-        Returns:
-            Returns Loaded CANoe configuration details.
-
-        Examples:
-            >>> # The following example returns CANoe application version relevant information.
-            >>> canoe_inst = CANoe()
-            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
-            >>> canoe_version_info = canoe_inst.get_canoe_configuration_details()
-            >>> print(canoe_version_info)
-        """
-        configuration_details = {
-            'canoe_app_full_name': self.__canoe_app_obj.Application.Version.FullName,
-            'canoe_app_full_name_with_sp': self.__canoe_app_obj.Application.Version.Name,
-            # The complete path to the currently loaded configuration
-            'canoe_cfg': self.__canoe_app_obj.Configuration.FullName,
-            # CANoe Mode(online/offline)
-            'canoe_mode': 'online' if self.__canoe_app_obj.Configuration.Mode == 0 else 'offline',
-            # Configuration ReadOnly ?
-            'cfg_read_only': self.__canoe_app_obj.Configuration.ReadOnly,
-            # CANoe configuration Networks count and Names List
-            'networks_count': len(self.__networks_obj_dictionary.keys()),
-            'networks_list': list(self.__networks_obj_dictionary.keys()),
-            # CANoe Simulation Setup Nodes count and Names List
-            'simulation_setup_nodes_count': len(self.__simulation_nodes_obj_dictionary.keys()),
-            'simulation_setup_nodes_list': list(self.__simulation_nodes_obj_dictionary.keys()),
-            # CANoe Replay Blocks count and Names List
-            'simulation_setup_replay_blocks_count': len(self.__replay_blocks_obj_dictionary.keys()),
-            'simulation_setup_replay_blocks_list': list(self.__replay_blocks_obj_dictionary.keys()),
-            # The number of buses count
-            'simulation_setup_buses_count': self.__canoe_app_obj.Configuration.SimulationSetup.Buses.Count,
-            # The number of generators contained
-            'simulation_setup_generators_count': self.__canoe_app_obj.Configuration.SimulationSetup.Generators.Count,
-            # The number of interactive generators contained
-            'simulation_setup_interactive_generators_count': self.__canoe_app_obj.Configuration.SimulationSetup.InteractiveGenerators.Count,
-        }
-        self.log.info('> CANoe Configuration Details <'.center(100, '='))
-        for k, v in configuration_details.items():
-            self.log.info(f'{k:<50}: {v}')
-        self.log.info(''.center(100, '='))
-        return configuration_details
-
     def get_canoe_version_info(self) -> dict:
         r"""The Version class represents the version of the CANoe application.
 
         Returns:
             "full_name" - The complete CANoe version.
             "name" - The CANoe version.
             "build" - The build number of the CANoe application.
@@ -910,18 +761,182 @@
         Examples:
             >>> # The following example returns CANoe application version relevant information.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_version_info = canoe_inst.get_canoe_version_info()
             >>> print(canoe_version_info)
         """
-        version_info = {'full_name': self.__canoe_app_obj.Application.Version.FullName,
-                        'name': self.__canoe_app_obj.Application.Version.Name,
-                        'build': self.__canoe_app_obj.Application.Version.Build,
-                        'major': self.__canoe_app_obj.Application.Version.Major,
-                        'minor': self.__canoe_app_obj.Application.Version.Minor,
-                        'patch': self.__canoe_app_obj.Application.Version.Patch}
+        version_info = {'full_name': self.__canoe_objects['Application'].Application.Version.FullName,
+                        'name': self.__canoe_objects['Application'].Version.Name,
+                        'build': self.__canoe_objects['Application'].Version.Build,
+                        'major': self.__canoe_objects['Application'].Version.major,
+                        'minor': self.__canoe_objects['Application'].Version.minor,
+                        'patch': self.__canoe_objects['Application'].Version.Patch}
         self.log.info('> CANoe Application.Version <'.center(100, '='))
         for k, v in version_info.items():
             self.log.info(f'{k:<10}: {v}')
         self.log.info(''.center(100, '='))
         return version_info
+
+    def get_system_variable_value(self, sys_var_name: str) -> Union[int, float, str]:
+        r"""get_system_variable_value Returns a system variable value.
+
+        Args:
+            sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
+
+        Returns:
+            System Variable value.
+
+        Examples:
+            >>> # The following example gets system variable value
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.start_measurement()
+            >>> sys_var_val = canoe_inst.get_system_variable_value('sys_var_demo::speed')
+            >>>print(sys_var_val)
+        """
+        namespace = '::'.join(sys_var_name.split('::')[:-1])
+        variable_name = sys_var_name.split('::')[-1]
+        namespace_object = self.__canoe_objects['Application'].System.Namespaces(namespace)
+        variable_value = namespace_object.Variables(variable_name).Value
+        self.log.info(f'system variable({sys_var_name}) value = {variable_value}.')
+        return variable_value
+
+    def set_system_variable_value(self, sys_var_name: str, value: Union[int, float, str]) -> None:
+        r"""set_system_variable_value sets a value to system variable.
+
+        Args:
+            sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
+            value (Union[int, float, str]): variable value.
+
+        Examples:
+            >>> # The following example sets system variable value to 1
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.start_measurement()
+            >>> canoe_inst.set_system_variable_value('sys_var_demo::speed', 1)
+        """
+        namespace = '::'.join(sys_var_name.split('::')[:-1])
+        variable_name = sys_var_name.split('::')[-1]
+        namespace_object = self.__canoe_objects['Application'].System.Namespaces(namespace)
+        namespace_object.Variables(variable_name).Value = value
+        self.log.info(f'system variable({sys_var_name}) value set to {value}.')
+
+    def send_diag_request(self, diag_ecu_qualifier_name: str, request: str, request_in_bytes=True) -> str:
+        r"""The send_diag_request method represents the query of a diagnostic tester (client) to an ECU (server) in CANoe.
+
+        Args:
+            diag_ecu_qualifier_name (str): Diagnostic Node ECU Qualifier Name configured in "Diagnostic/ISO TP Configuration".
+            request (str): Diagnostic request in bytes or diagnostic node qualifier name.
+            request_in_bytes: True if Diagnostic request is bytes. False if you are using Qualifier name. Default is True.
+
+        Returns:
+            diagnostic response stream. Ex- "50 01 00 00 00 00"
+
+        Examples:
+            >>> # Example 1 - The following example sends diagnostic request "10 01"
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.start_measurement()
+            >>> wait(1)
+            >>> resp = canoe_inst.send_diag_request('Door', '10 01')
+            >>> print(resp)
+            >>> canoe_inst.stop_measurement()
+            >>> # Example 2 - The following example sends diagnostic request "DefaultSession_Start"
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(canoe_cfg=r'C:\Users\Public\Documents\Vector\CANoe\Sample Configurations 11.0.81\.\CAN\Diagnostics\UDSBasic\UDSBasic.cfg')
+            >>> canoe_inst.start_measurement()
+            >>> wait(1)
+            >>> resp = canoe_inst.send_diag_request('Door', 'DefaultSession_Start', False)
+            >>> print(resp)
+            >>> canoe_inst.stop_measurement()
+        """
+        diag_response_data = ""
+        if diag_ecu_qualifier_name in self.__diag_ecu_qualifiers_dictionary.keys():
+            self.log.info(f'Diag Req --> {request}')
+            if request_in_bytes:
+                diag_req_in_bytes = bytearray()
+                request = ''.join(request.split(' '))
+                for i in range(0, len(request), 2):
+                    diag_req_in_bytes.append(int(request[i:i + 2], 16))
+                diag_req = self.__diag_ecu_qualifiers_dictionary[diag_ecu_qualifier_name].CreateRequestFromStream(diag_req_in_bytes)
+            else:
+                diag_req = self.__diag_ecu_qualifiers_dictionary[diag_ecu_qualifier_name].CreateRequest(request)
+            diag_req.Send()
+            while diag_req.Pending:
+                wait(0.1)
+            if diag_req.Responses.Count == 0:
+                self.log.info("Diagnostic Response Not Received.")
+            else:
+                for k in range(1, diag_req.Responses.Count + 1):
+                    diag_res = diag_req.Responses(k)
+                    if diag_res.Positive:
+                        self.log.info(f"+ve response received.")
+                    else:
+                        self.log.info(f"-ve response received.")
+                    diag_response_data = " ".join(f"{d:02X}" for d in diag_res.Stream).upper()
+                self.log.info(f'Diag Res --> {diag_response_data}')
+        else:
+            self.log.info(f'Diag ECU qualifier({diag_ecu_qualifier_name}) not available in loaded CANoe config.')
+        return diag_response_data
+
+    def set_replay_block_file(self, block_name: str, recording_file_path: str) -> None:
+        r"""Method for setting CANoe replay block file.
+
+        Args:
+            block_name: CANoe replay block name
+            recording_file_path: CANoe replay recording file including path.
+
+        Examples:
+            >>> # The following example sets replay block file
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.set_replay_block_file(block_name='replay block name', recording_file_path='replay file including path')
+            >>> canoe_inst.start_measurement()
+        """
+        if block_name in self.__replay_blocks_obj_dictionary.keys():
+            self.__replay_blocks_obj_dictionary[block_name].Path = recording_file_path
+            self.log.info(f'Replay block "{block_name}" updated with "{recording_file_path}" path.')
+        else:
+            self.log.warning(f'Replay block "{block_name}" not available.')
+
+    def control_replay_block(self, block_name: str, start_stop: bool) -> None:
+        r"""Method for setting CANoe replay block file.
+
+        Args:
+            block_name (str): CANoe replay block name
+            start_stop (bool): True to start replay block. False to Stop.
+
+        Examples:
+            >>> # The following example starts replay block
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.set_replay_block_file(block_name='replay block name', recording_file_path='replay file including path')
+            >>> canoe_inst.start_measurement()
+            >>> canoe_inst.control_replay_block('replay block name', True)
+        """
+        if block_name in self.__replay_blocks_obj_dictionary.keys():
+            if start_stop:
+                self.__replay_blocks_obj_dictionary[block_name].Start()
+            else:
+                self.__replay_blocks_obj_dictionary[block_name].Stop()
+            self.log.info(f'Replay block "{block_name}" {"Started" if start_stop else "Stopped"}.')
+        else:
+            self.log.warning(f'Replay block "{block_name}" not available.')
+
+class CanoeMeasurementEvents:
+    """Handler for CANoe measurement events"""
+
+    @staticmethod
+    def OnStart():
+        CANoe.Started = True
+        CANoe.Stopped = False
+
+    @staticmethod
+    def OnStop():
+        CANoe.Started = False
+        CANoe.Stopped = True
+
+
+def DoEventsUntil(cond):
+    while not cond():
+        DoEvents()
```

### Comparing `py_canoe-0.0.9/tests/demo_cfg/CANdb/easy.dbc` & `py_canoe-0.1.1/tests/demo_cfg/CANdb/easy.dbc`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/tests/demo_cfg/Nodes/SimDiagECU.can` & `py_canoe-0.1.1/tests/demo_cfg/Nodes/SimDiagECU.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/tests/demo_cfg/Nodes/system_events.can` & `py_canoe-0.1.1/tests/demo_cfg/Nodes/system_events.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/tests/demo_cfg/Panels/sys_var_demo_panel.xvp` & `py_canoe-0.1.1/tests/demo_cfg/Panels/sys_var_demo_panel.xvp`

 * *Files identical despite different names*

### Comparing `py_canoe-0.0.9/tests/demo_cfg/demo.cfg` & `py_canoe-0.1.1/tests/demo_cfg/demo_offline.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-;CANoe Version |4|11|0|59616 demo 
+;CANoe Version |4|11|0|57077 demo_offline 
 Version: 11.0.81 Build 81
 32 PRO
 5
 APPDIR Vector.CANoe.SignalGenerators.DLL
 Vector.CANoe.SignalGenerators, Version=11.0.81.0, Culture=neutral, PublicKeyToken=null
 Vector.CANoe.SignalGenerators.ComponentWrapper
 1
 1.0.1
 VGlobalConfiguration 1 Begin_Of_Object
 17
 VGlobalParameters 2 Begin_Of_Object
 31
 2
 3,100,200,500
-1000000 1.000000 0 1000 1 1 0 0 1 1 1 0 0 0 1 0 0 0
+1000000 1.000000 0 100 1 1 0 0 1 1 1 0 0 0 1 0 0 0
 1
 0
 0 1
 ResetSignalsOnMeasurementStart=1
 VDatabaseContainerStreamer 3 Begin_Of_Object
 8
 1
@@ -35,19 +35,19 @@
 0
 0
 0
 End_Of_Object VDatabaseContainerStreamer 3
 0
 0
 1
-<VFileName V7 QL> 1 "demo.cfg" 
+<VFileName V7 QL> 1 "demo_offline.cfg" 
+0
 0
 0
 0
-1
 VPersistentEnvarSelectionData 3 Begin_Of_Object
 1
 1 1 0 0
 ~
 ~
 End_Of_Object VPersistentEnvarSelectionData 3
 VPersistentExtensionData 3 Begin_Of_Object
@@ -590,20 +590,20 @@
 VGlobalVariableSettings 3 Begin_Of_Object
 1
 65001
 End_Of_Object VGlobalVariableSettings 3
 VGeneralLoggingBlockSettings 3 Begin_Of_Object
 1
 2000
-62
+68
 0
 End_Of_Object VGeneralLoggingBlockSettings 3
 0
 0
-120
+167
 0
 1
 SecurityManager::VSecurityManager 3 Begin_Of_Object
 2
 0
 0
 End_Of_Object SecurityManager::VSecurityManager 3
@@ -614,15 +614,15 @@
 VErtOptions 3 Begin_Of_Object
 1
 0
 End_Of_Object VErtOptions 3
 End_Of_Object VGlobalParameters 2
 VDesktopManager 2 Begin_Of_Object
 1
-1
+0
 4
 VDesktop 3 Begin_Of_Object
 1
 Trace
 {9A300368-5C43-4C52-8A1F-83F68E1E0BCD}
 Begin_Of_Multi_Line_String
 3
@@ -643,17 +643,17 @@
 3
 <?xml version="1.0"?><!--
 
   Actipro Docking/MDI for WinForms
   Copyright (c) 2001-2014 Actipro Software LLC.  All rights reserved.
   http://www.actiprosoftware.com
 
---><ToolWindowLayout Version="1.0"><LayoutData><HostContainerControl><ToolWindowContainer Dock="Bottom" Size="958, 205" SelectedToolWindowGuid="4007d333-cefc-4f4a-852e-30b62a93a1d7"><ToolWindow Key="{31AD4644-E941-452D-832D-80EF52A05036}" Guid="4007d333-cefc-4f4a-852e-30b62a93a1d7" DockedSize="201, 201" FloatingSize="423, 189" HasOptions="False" ImageIndex="-1" Text="Write" TitleBarText="Write"><AutoHideStateInfo RootDock="Bottom" /><DockedInsideHostStateInfo RootDock="Bottom" IsAttached="False" /><DockedOutsideHostStateInfo IsAttached="False" /></ToolWindow></ToolWindowContainer></HostContainerControl><AutoHide Dock="Left" /><AutoHide Dock="Right" /><AutoHide Dock="Top" /><AutoHide Dock="Bottom" /><TabbedDocuments Orientation="Horizontal" /><FloatingContainers /><Hidden><ToolWindow Key="{F5E09530-AAE7-48d9-B925-CEF5027AA97D}" Guid="32e4b564-02ec-46fd-9296-f6315c198b9d" State="DockableInsideHost" DockedSize="325, 325" FloatingSize="325, 380"><AutoHideStateInfo RootDock="Left" /><Docke
+--><ToolWindowLayout Version="1.0"><LayoutData><HostContainerControl><ToolWindowContainer Dock="Bottom" Size="1920, 201" SelectedToolWindowGuid="4007d333-cefc-4f4a-852e-30b62a93a1d7"><ToolWindow Key="{31AD4644-E941-452D-832D-80EF52A05036}" Guid="4007d333-cefc-4f4a-852e-30b62a93a1d7" DockedSize="201, 197" FloatingSize="423, 189" HasOptions="False" ImageIndex="-1" Text="Write" TitleBarText="Write"><AutoHideStateInfo RootDock="Bottom" /><DockedInsideHostStateInfo RootDock="Bottom" IsAttached="False" /><DockedOutsideHostStateInfo IsAttached="False" /></ToolWindow></ToolWindowContainer></HostContainerControl><AutoHide Dock="Left" /><AutoHide Dock="Right" /><AutoHide Dock="Top" /><AutoHide Dock="Bottom" /><TabbedDocuments Orientation="Horizontal" /><FloatingContainers /><Hidden><ToolWindow Key="{F5E09530-AAE7-48d9-B925-CEF5027AA97D}" Guid="32e4b564-02ec-46fd-9296-f6315c198b9d" State="DockableInsideHost" DockedSize="325, 325" FloatingSize="325, 380"><AutoHideStateInfo RootDock="Left" /><Dock
 kPersistNoLineBreak
-dInsideHostStateInfo RootDock="Left" IsAttached="False" /><DockedOutsideHostStateInfo IsAttached="False" /></ToolWindow></Hidden></LayoutData><CustomData /></ToolWindowLayout>
+edInsideHostStateInfo RootDock="Left" IsAttached="False" /><DockedOutsideHostStateInfo IsAttached="False" /></ToolWindow></Hidden></LayoutData><CustomData /></ToolWindowLayout>
 End_Of_Serialized_Data 3
 End_Of_Object VDesktop 3
 VDesktop 3 Begin_Of_Object
 1
 Analysis
 {CBE571D9-1968-4A46-89F5-A949CD457AA6}
 Begin_Of_Multi_Line_String
@@ -863,15 +863,15 @@
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 1
 1
 0
 0
 1
-958 652
+1920 657
 END_OF_DESKTOP_DATA
 6
 0 1 -1 -1 -1 -1 22 22 953 535
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 0
 0
@@ -955,139 +955,132 @@
 VDAOGBFunctionBlock 4 Begin_Of_Object
 1
 1
 0
 TABPredecessor:
 0
 TABSuccessor:
-2
-VPlugConf 5 Begin_Of_Object
-1
-End_Of_Object VPlugConf 5
-VDAOGBFunctionBlock 5 Begin_Of_Object
-1
-2
-0
-TABPredecessor:
-1
-TABSuccessor:
 38
-VChannelFilterConfiguration 6 Begin_Of_Object
+VOfflineSrcConfiguration 5 Begin_Of_Object
 3
-VMigratedGenericConfiguration<class_VChannelFilterData> 7 Begin_Of_Object
+VMigratedGenericConfiguration<struct_VOfflineCfgData> 6 Begin_Of_Object
 1
-VChannelFilterData 8 Begin_Of_Object
+VOfflineCfgData 7 Begin_Of_Object
 2
+VReplayCfgBase 8 Begin_Of_Object
 1
-VBusChannelData 9 Begin_Of_Object
 1
-2
-2
+<VFileName V7 QL> 1 "Logs\demo_log.blf" 
+1
+End_Of_Object VReplayCfgBase 8
+VCfgBreakCondition 8 Begin_Of_Object
+1
+VDataBreakCondition 9 Begin_Of_Object
+1
+0
+VEvCondBlock 10 Begin_Of_Object
 1
+VEvCondGroup 11 Begin_Of_Object
 2
+VEvCondPrimitive 12 Begin_Of_Object
 1
 1
-End_Of_Object VBusChannelData 9
-End_Of_Channel_Data
+End_Of_Object VEvCondPrimitive 12
 1
-End_Of_Object VChannelFilterData 8
-End_Of_Object VMigratedGenericConfiguration<class_VChannelFilterData> 7
 0
 0
-End_Of_Object VChannelFilterConfiguration 6
-VDOCrossing 6 Begin_Of_Object
-2
-3
+End_Of_Object VEvCondGroup 11
+End_Of_Object VEvCondBlock 10
+End_Of_Object VDataBreakCondition 9
+End_Of_Object VCfgBreakCondition 8
+0
+0
 0
-VDAOGBHSStd 7 Begin_Of_Object
-1
-4
 0
-0 0
-TABPredecessor:
-43
-TABSuccessor:
-45
-VDODynamicLine 8 Begin_Of_Object
-1
-5
 0
 0
-VDAOSwitch 9 Begin_Of_Object
+End_Of_Object VOfflineCfgData 7
+End_Of_Object VMigratedGenericConfiguration<struct_VOfflineCfgData> 6
+VChannelMapping 6 Begin_Of_Object
 1
-45
+0
+End_Of_Object VChannelMapping 6
+End_Of_Object VOfflineSrcConfiguration 5
+VDAOSwitch 5 Begin_Of_Object
+1
+38
 0
 TABPredecessor:
-4
+1
 TABSuccessor:
-46
-VDAOGBHSStd 10 Begin_Of_Object
+39
+VDAOGBHSStd 6 Begin_Of_Object
 1
-46
+39
 0
 0 0
 TABPredecessor:
-45
+38
 TABSuccessor:
-48
-VDODynamicLine 11 Begin_Of_Object
+41
+VDODynamicLine 7 Begin_Of_Object
 1
-47
+40
 0
 0
-VDOFRamification 12 Begin_Of_Object
+VDOFRamification 8 Begin_Of_Object
 1
-48
+41
 0
 TABPredecessor:
-46
+39
 TABSuccessor:
-50
+43
 5
-VDORefinement 13 Begin_Of_Object
+VDORefinement 9 Begin_Of_Object
 1
-49
+42
 0
 13
-VDAOGBHSStd 14 Begin_Of_Object
+VDAOGBHSStd 10 Begin_Of_Object
 1
-50
+43
 0
 0 0
 TABPredecessor:
-48
+41
 TABSuccessor:
-52
-VDODynamicLine 15 Begin_Of_Object
+45
+VDODynamicLine 11 Begin_Of_Object
 1
-51
+44
 0
 0
-VDAOGBFunctionBlock 16 Begin_Of_Object
+VDAOGBFunctionBlock 12 Begin_Of_Object
 1
-52
+45
 0
 TABPredecessor:
-50
+43
 TABSuccessor:
-55
-VNetMSControlConfiguration 17 Begin_Of_Object
+48
+VNetMSControlConfiguration 13 Begin_Of_Object
 1
-VNETControlConfiguration 18 Begin_Of_Object
+VNETControlConfiguration 14 Begin_Of_Object
 1
-VConfigurationRoot 19 Begin_Of_Object
+VConfigurationRoot 15 Begin_Of_Object
 1
-End_Of_Object VConfigurationRoot 19
-VNETControlBox 19 Begin_Of_Object
+End_Of_Object VConfigurationRoot 15
+VNETControlBox 15 Begin_Of_Object
 2
-VUniqueBox 20 Begin_Of_Object
-1
-VBoxRoot 21 Begin_Of_Object
+VUniqueBox 16 Begin_Of_Object
 1
+VBoxRoot 17 Begin_Of_Object
 1
+2
 1 1 0 1 -1 -1 -1 -1 0 0 512 362
 CAN Statistics
 1
 
 MDI_DOCK_INFO_END
 5
 1
@@ -1184,21 +1177,21 @@
 0 0
 END_OF_DESKTOP_DATA
 END_OF_DESKTOP_DATA_COLLECTION
 0
 END_OF_DESKTOP_MEMBER
 {DF1D1FB8-3F6B-4B58-9502-C920BE0A79B0}
 0
-End_Of_Object VBoxRoot 21
+End_Of_Object VBoxRoot 17
 1 2 0 1 -1 -1 -1 -1 0 0 482 266
-End_Of_Object VUniqueBox 20
+End_Of_Object VUniqueBox 16
 1
 1 2 0 1 -1 -1 -1 -1 0 0 482 266
 0
-End_Of_Object VNETControlBox 19
+End_Of_Object VNETControlBox 15
 135
 APPDIR Vector.CANalyzer.CAN.StatisticsMonitor.DLL
 Vector.CANalyzer.CAN.StatisticsMonitor, Version=11.0.81.0, Culture=neutral, PublicKeyToken=null
 Vector.CANalyzer.CAN.StatisticsMonitor.StatisticsMonitor
 1
 1
 APPDIR CANw_Net.DLL
@@ -1327,145 +1320,145 @@
 mPatch
 4
 --TextFormatter: End of Object--
 --TextFormatter: End of Object--
 TypeRef:2
 2
 --TextFormatter: End of Object--
-End_Of_Object VNETControlConfiguration 18
-End_Of_Object VNetMSControlConfiguration 17
-VDOLine 17 Begin_Of_Object
+End_Of_Object VNETControlConfiguration 14
+End_Of_Object VNetMSControlConfiguration 13
+VDOLine 13 Begin_Of_Object
 1
-53
+46
 0
 130 0
 NULL
-End_Of_Object VDOLine 17
+End_Of_Object VDOLine 13
 
 EndOfComment
 0
 1
-End_Of_Object VDAOGBFunctionBlock 16
-End_Of_Object VDODynamicLine 15
-End_Of_Object VDAOGBHSStd 14
+End_Of_Object VDAOGBFunctionBlock 12
+End_Of_Object VDODynamicLine 11
+End_Of_Object VDAOGBHSStd 10
 NULL
-End_Of_Object VDORefinement 13
-VDORefinement 13 Begin_Of_Object
+End_Of_Object VDORefinement 9
+VDORefinement 9 Begin_Of_Object
 1
-54
+47
 0
 7
-VDAOGBHSStd 14 Begin_Of_Object
+VDAOGBHSStd 10 Begin_Of_Object
 1
-55
+48
 0
 0 0
 TABPredecessor:
-52
+45
 TABSuccessor:
-57
-VDODynamicLine 15 Begin_Of_Object
+50
+VDODynamicLine 11 Begin_Of_Object
 1
-56
+49
 0
 0
-VDAOGBFunctionBlock 16 Begin_Of_Object
+VDAOGBFunctionBlock 12 Begin_Of_Object
 1
-57
+50
 0
 TABPredecessor:
-55
+48
 TABSuccessor:
-60
-VTraceConfiguration 17 Begin_Of_Object
+53
+VTraceConfiguration 13 Begin_Of_Object
 1
-VTraceControlCfg 18 Begin_Of_Object
+VTraceControlCfg 14 Begin_Of_Object
 8
-VTraceSearchCfg 19 Begin_Of_Object
+VTraceSearchCfg 15 Begin_Of_Object
 1
-VEvCondBlock 20 Begin_Of_Object
+VEvCondBlock 16 Begin_Of_Object
 1
-VEvCondGroup 21 Begin_Of_Object
+VEvCondGroup 17 Begin_Of_Object
 2
-VEvCondPrimitive 22 Begin_Of_Object
+VEvCondPrimitive 18 Begin_Of_Object
 1
 1
-End_Of_Object VEvCondPrimitive 22
+End_Of_Object VEvCondPrimitive 18
 1
 0
 0
-End_Of_Object VEvCondGroup 21
-End_Of_Object VEvCondBlock 20
+End_Of_Object VEvCondGroup 17
+End_Of_Object VEvCondBlock 16
 0
-End_Of_Object VTraceSearchCfg 19
-VTraceFilterCfg 19 Begin_Of_Object
+End_Of_Object VTraceSearchCfg 15
+VTraceFilterCfg 15 Begin_Of_Object
 1
 0
 1
-VTraceAnalysisFilterGroup 20 Begin_Of_Object
+VTraceAnalysisFilterGroup 16 Begin_Of_Object
 2
 1
 Filter Group 0
 2
-VTraceAnalysisSingleFilter 21 Begin_Of_Object
+VTraceAnalysisSingleFilter 17 Begin_Of_Object
 3
 1
 1
 0
-End_Of_Object VTraceAnalysisSingleFilter 21
-VTraceAnalysisSingleFilter 21 Begin_Of_Object
+End_Of_Object VTraceAnalysisSingleFilter 17
+VTraceAnalysisSingleFilter 17 Begin_Of_Object
 3
 0
 0
 0
-End_Of_Object VTraceAnalysisSingleFilter 21
+End_Of_Object VTraceAnalysisSingleFilter 17
 1
-End_Of_Object VTraceAnalysisFilterGroup 20
-End_Of_Object VTraceFilterCfg 19
+End_Of_Object VTraceAnalysisFilterGroup 16
+End_Of_Object VTraceFilterCfg 15
 1
 0
 0
 0
-39
+37
 0
 0
 1
 1
-18
+14
 ver=4: T T T T T T
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 2
 0
 3
 1
-18
+14
 ver=3;Door:ver=4: T T T T T
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 4
 0
 5
 0
 6
 1
-18
+14
 GFver=4;ver=4: T F F T T F F F F F;F _Statistics;T CANoe;T DiVa;T sys_var_demo;T demo
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 7
 0
 8
 0
 9
 0
 10
 0
 11
 1
-18
+14
 ver=4: T T T T
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 12
 0
 13
 0
 14
 0
 15
@@ -1508,1452 +1501,1448 @@
 0
 34
 0
 35
 0
 36
 0
-37
-0
-38
-0
 0
 1
-VTraceColumnConfiguration 19 Begin_Of_Object
+VTraceColumnConfiguration 15 Begin_Of_Object
 3
 1
 Initial
 115
-VTNColumnData 20 Begin_Of_Object
+VTNColumnData 16 Begin_Of_Object
 3
 0
 104
 0
 Time
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 1
 37
 1
 Chn
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 2
 45
 2
 ID
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 3
 120
 3
 Name
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 4
 170
 -1
 ID / Name
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 5
 43
 5
 Dir
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 6
 45
 6
 DLC
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 7
 270
 7
 Data
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 8
 37
 -1
 Attr
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 9
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 10
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 11
 100
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 12
 100
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 13
 150
 -1
 Frame Duration
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 14
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 15
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 16
 70
 4
 Event Type
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 17
 100
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 18
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 19
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 20
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 21
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 22
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 23
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 24
 85
 -1
 Bus Idle
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 25
 85
 -1
 Bus Busy
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 26
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 27
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 28
 110
 -1
 HH:MM:SS
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 29
 85
 -1
 Diff time
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 30
 50
 -1
 Bustype
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 31
 120
 -1
 Send node
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 32
 50
 -1
 Bus
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 33
 80
 -1
 Database
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 34
 50
 -1
 Counter
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 35
 90
 -1
 Start of Frame
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 36
 50
 -1
 PGN
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 37
 50
 -1
 DP
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 38
 50
 -1
 Prio
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 39
 50
 -1
 Specific 10
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 40
 50
 -1
 Specific 11
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 41
 50
 -1
 Specific 12
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 42
 50
 -1
 Specific 13
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 43
 50
 -1
 Specific 14
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 44
 50
 -1
 Specific 15
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 45
 50
 -1
 Specific 16
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 46
 50
 -1
 Specific 17
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 47
 50
 -1
 Specific 18
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 48
 50
 -1
 Specific 19
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 49
 50
 -1
 Specific 20
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 50
 150
 -1
 Data ASCII
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 51
 150
 -1
 Comment
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 52
 10
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 53
 10
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 54
 50
 -1
 Namespace
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 55
 120
 -1
 Diff time (ref. event)
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 56
 50
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 57
 100
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 58
 100
 -1
 ---
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 59
 120
 -1
 Date / Time
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 60
 50
 -1
 Receive Node
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 61
 50
 -1
 VL No.
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 62
 200
 -1
 Sub VL ID
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 63
 50
 -1
 Transmitter
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 64
 200
 -1
 Receiver
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 65
 50
 -1
 Tx Port ID
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 66
 50
 -1
 Rx Port ID
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 67
 65
 -1
 Port Char.
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 68
 50
 -1
 IP Frag.
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 69
 150
 -1
 Master Port Name
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 70
 65
 -1
 BAG
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 71
 65
 -1
 Seq. No.
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 72
 50
 -1
 Line
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 73
 50
 -1
 Interface ID
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 74
 50
 -1
 Equipment
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 75
 50
 -1
 Partition
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 76
 50
 -1
 BRS
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 77
 50
 -1
 ESI
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 78
 45
 -1
 Data length
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 79
 10
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 80
 10
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 81
 10
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 82
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 83
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 84
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 85
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 86
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 87
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 88
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 89
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 90
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 91
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 92
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 93
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 94
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 95
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 96
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 97
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 98
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 99
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 100
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 101
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 102
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 103
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 104
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 105
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 106
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 107
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 108
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 109
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 110
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 111
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 112
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 113
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-VTNColumnData 20 Begin_Of_Object
+End_Of_Object VTNColumnData 16
+VTNColumnData 16 Begin_Of_Object
 3
 114
 50
 -1
  
 1
 0
 1
 0
-End_Of_Object VTNColumnData 20
-End_Of_Object VTraceColumnConfiguration 19
+End_Of_Object VTNColumnData 16
+End_Of_Object VTraceColumnConfiguration 15
 0
 0
-VTraceControlFixedModeExpansionItems 19 Begin_Of_Object
+VTraceControlFixedModeExpansionItems 15 Begin_Of_Object
 3
 4
-VConfigMessage 20 Begin_Of_Object
+VConfigMessage 16 Begin_Of_Object
 5
-VConfigBusObject 21 Begin_Of_Object
+VConfigBusObject 17 Begin_Of_Object
 1
-VConfigBusEvent 22 Begin_Of_Object
+VConfigBusEvent 18 Begin_Of_Object
 1
-VConfigEvent 23 Begin_Of_Object
+VConfigEvent 19 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 23
+End_Of_Object VConfigEvent 19
 2
 1
-End_Of_Object VConfigBusEvent 22
-End_Of_Object VConfigBusObject 21
+End_Of_Object VConfigBusEvent 18
+End_Of_Object VConfigBusObject 17
 9
 1
-VDatabaseBusMessageId 21 Begin_Of_Object
+VDatabaseBusMessageId 17 Begin_Of_Object
 3
 291
 2
 1
 0
 0
 0
 EngineState
 0
 easy
 0
 1
-End_Of_Object VDatabaseBusMessageId 21
+End_Of_Object VDatabaseBusMessageId 17
 NULL
 0
 0
 0
-End_Of_Object VConfigMessage 20
-VConfigMessage 20 Begin_Of_Object
+End_Of_Object VConfigMessage 16
+VConfigMessage 16 Begin_Of_Object
 5
-VConfigBusObject 21 Begin_Of_Object
+VConfigBusObject 17 Begin_Of_Object
 1
-VConfigBusEvent 22 Begin_Of_Object
+VConfigBusEvent 18 Begin_Of_Object
 1
-VConfigEvent 23 Begin_Of_Object
+VConfigEvent 19 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 23
+End_Of_Object VConfigEvent 19
 1
 1
-End_Of_Object VConfigBusEvent 22
-End_Of_Object VConfigBusObject 21
+End_Of_Object VConfigBusEvent 18
+End_Of_Object VConfigBusObject 17
 10
 1
-VDatabaseBusMessageId 21 Begin_Of_Object
+VDatabaseBusMessageId 17 Begin_Of_Object
 3
 291
 1
 1
 0
 0
 0
 EngineState
 0
 easy
 0
 1
-End_Of_Object VDatabaseBusMessageId 21
+End_Of_Object VDatabaseBusMessageId 17
 NULL
 0
 0
 0
-End_Of_Object VConfigMessage 20
-VConfigMessage 20 Begin_Of_Object
+End_Of_Object VConfigMessage 16
+VConfigMessage 16 Begin_Of_Object
 5
-VConfigBusObject 21 Begin_Of_Object
+VConfigBusObject 17 Begin_Of_Object
 1
-VConfigBusEvent 22 Begin_Of_Object
+VConfigBusEvent 18 Begin_Of_Object
 1
-VConfigEvent 23 Begin_Of_Object
+VConfigEvent 19 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 23
+End_Of_Object VConfigEvent 19
 2
 1
-End_Of_Object VConfigBusEvent 22
-End_Of_Object VConfigBusObject 21
+End_Of_Object VConfigBusEvent 18
+End_Of_Object VConfigBusObject 17
 9
 1
-VDatabaseBusMessageId 21 Begin_Of_Object
+VDatabaseBusMessageId 17 Begin_Of_Object
 3
 801
 2
 1
 0
 0
 0
 LightState
 0
 easy
 0
 1
-End_Of_Object VDatabaseBusMessageId 21
+End_Of_Object VDatabaseBusMessageId 17
 NULL
 0
 0
 0
-End_Of_Object VConfigMessage 20
-VConfigMessage 20 Begin_Of_Object
+End_Of_Object VConfigMessage 16
+VConfigMessage 16 Begin_Of_Object
 5
-VConfigBusObject 21 Begin_Of_Object
+VConfigBusObject 17 Begin_Of_Object
 1
-VConfigBusEvent 22 Begin_Of_Object
+VConfigBusEvent 18 Begin_Of_Object
 1
-VConfigEvent 23 Begin_Of_Object
+VConfigEvent 19 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 23
+End_Of_Object VConfigEvent 19
 1
 1
-End_Of_Object VConfigBusEvent 22
-End_Of_Object VConfigBusObject 21
+End_Of_Object VConfigBusEvent 18
+End_Of_Object VConfigBusObject 17
 10
 1
-VDatabaseBusMessageId 21 Begin_Of_Object
+VDatabaseBusMessageId 17 Begin_Of_Object
 3
 801
 1
 1
 0
 0
 0
 LightState
 0
 easy
 0
 1
-End_Of_Object VDatabaseBusMessageId 21
+End_Of_Object VDatabaseBusMessageId 17
 NULL
 0
 0
 0
-End_Of_Object VConfigMessage 20
+End_Of_Object VConfigMessage 16
 0
 0
 0
 0
-End_Of_Object VTraceControlFixedModeExpansionItems 19
-18
+End_Of_Object VTraceControlFixedModeExpansionItems 15
+14
 C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe
-End_Of_Serialized_Data 18
-18
+End_Of_Serialized_Data 14
+14
 Trace-Fenster
-End_Of_Serialized_Data 18
-18
+End_Of_Serialized_Data 14
+14
 
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 0
 776880451
 1
 1
-18
-VLogExportPersister 19 Begin_Of_Object
+14
+VLogExportPersister 15 Begin_Of_Object
 7
 1416
 44616685
 Trace-Fenster
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 0
@@ -2985,34 +2974,34 @@
 0
 730
 0
 0.10000000000000001
 0
 0
 1
-End_Of_Object VLogExportPersister 19
+End_Of_Object VLogExportPersister 15
 
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 0
 0
 0
 290
 0
 150
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe" 
-End_Of_Object VTraceControlCfg 18
-VNETTraceControlBox 18 Begin_Of_Object
+End_Of_Object VTraceControlCfg 14
+VNETTraceControlBox 14 Begin_Of_Object
 1
-VNETControlBox 19 Begin_Of_Object
+VNETControlBox 15 Begin_Of_Object
 2
-VUniqueBox 20 Begin_Of_Object
-1
-VBoxRoot 21 Begin_Of_Object
+VUniqueBox 16 Begin_Of_Object
 1
+VBoxRoot 17 Begin_Of_Object
 1
+2
 1 1 0 1 -1 -1 -1 -1 0 0 1275 541
 Trace
 1
 
 MDI_DOCK_INFO_END
 5
 1
@@ -3062,79 +3051,79 @@
 END_OF_DESKTOP_DATA
 END_OF_DESKTOP_DATA_COLLECTION
 0
 0 0
 END_OF_DESKTOP_MEMBER
 {31FB7B33-3D93-4EE7-A007-8DB311A944A4}
 0
-End_Of_Object VBoxRoot 21
+End_Of_Object VBoxRoot 17
 1 -1 0 0 0 0 0 0 0 0 0 0
-End_Of_Object VUniqueBox 20
+End_Of_Object VUniqueBox 16
 0
 0
-End_Of_Object VNETControlBox 19
-End_Of_Object VNETTraceControlBox 18
-End_Of_Object VTraceConfiguration 17
-VDOLine 17 Begin_Of_Object
+End_Of_Object VNETControlBox 15
+End_Of_Object VNETTraceControlBox 14
+End_Of_Object VTraceConfiguration 13
+VDOLine 13 Begin_Of_Object
 1
-58
+51
 0
 130 0
 NULL
-End_Of_Object VDOLine 17
+End_Of_Object VDOLine 13
 
 EndOfComment
 0
 1
-End_Of_Object VDAOGBFunctionBlock 16
-End_Of_Object VDODynamicLine 15
-End_Of_Object VDAOGBHSStd 14
+End_Of_Object VDAOGBFunctionBlock 12
+End_Of_Object VDODynamicLine 11
+End_Of_Object VDAOGBHSStd 10
 NULL
-End_Of_Object VDORefinement 13
-VDORefinement 13 Begin_Of_Object
+End_Of_Object VDORefinement 9
+VDORefinement 9 Begin_Of_Object
 1
-59
+52
 0
 4
-VDAOGBHSStd 14 Begin_Of_Object
+VDAOGBHSStd 10 Begin_Of_Object
 1
-60
+53
 0
 0 0
 TABPredecessor:
-57
+50
 TABSuccessor:
-62
-VDODynamicLine 15 Begin_Of_Object
+55
+VDODynamicLine 11 Begin_Of_Object
 1
-61
+54
 0
 0
-VDAOGBFunctionBlock 16 Begin_Of_Object
+VDAOGBFunctionBlock 12 Begin_Of_Object
 1
-62
+55
 0
 TABPredecessor:
-60
+53
 TABSuccessor:
-65
-VNETDataListControlHost 17 Begin_Of_Object
+58
+VNETDataListControlHost 13 Begin_Of_Object
 1
-VConfigurationRoot 18 Begin_Of_Object
+VConfigurationRoot 14 Begin_Of_Object
 1
-End_Of_Object VConfigurationRoot 18
-VNETDataBox 18 Begin_Of_Object
+End_Of_Object VConfigurationRoot 14
+VNETDataBox 14 Begin_Of_Object
 1
-VNETControlBox 19 Begin_Of_Object
+VNETControlBox 15 Begin_Of_Object
 2
-VUniqueBox 20 Begin_Of_Object
-1
-VBoxRoot 21 Begin_Of_Object
+VUniqueBox 16 Begin_Of_Object
 1
+VBoxRoot 17 Begin_Of_Object
 1
+2
 1 2 0 1 -1 -1 -1 -1 513 0 1030 265
 Data
 1
 
 MDI_DOCK_INFO_END
 5
 1
@@ -3184,21 +3173,21 @@
 END_OF_DESKTOP_DATA
 END_OF_DESKTOP_DATA_COLLECTION
 0
 0 0
 END_OF_DESKTOP_MEMBER
 {AA76F618-2087-4A48-B611-BF29871F1267}
 0
-End_Of_Object VBoxRoot 21
+End_Of_Object VBoxRoot 17
 1 -1 0 0 0 0 0 0 0 0 0 0
-End_Of_Object VUniqueBox 20
+End_Of_Object VUniqueBox 16
 0
 0
-End_Of_Object VNETControlBox 19
-End_Of_Object VNETDataBox 18
+End_Of_Object VNETControlBox 15
+End_Of_Object VNETDataBox 14
 1
 9
 0
 20 150 16 100 40 40 50 100 60 100 1
 35 35
 30
 70 70 70 100
@@ -3207,15 +3196,15 @@
 0 0
 0
 0 0 0 0
 0
 1 0
 5000 0 10000 0 10000
 1 0
-VLogCfgData 18 Begin_Of_Object
+VLogCfgData 14 Begin_Of_Object
 11
 0
 0
 0
 0
 0
 0
@@ -3224,23 +3213,23 @@
 1024
 60
 0
 0
 0
 3
 0
-62
+68
 1
 1
 0
 2
 0
 0
-18
-VLogExportPersister 19 Begin_Of_Object
+14
+VLogExportPersister 15 Begin_Of_Object
 7
 1416
 11060201
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 0
@@ -3272,17 +3261,17 @@
 0
 730
 0
 0.10000000000000001
 0
 0
 1
-End_Of_Object VLogExportPersister 19
+End_Of_Object VLogExportPersister 15
 
-End_Of_Serialized_Data 18
+End_Of_Serialized_Data 14
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\Data.mdf" 
 0
 1
 0
 10
 80
 0
@@ -3295,72 +3284,72 @@
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\Data.mdf" 
 1
 0
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\{LoggingBlock}.mdf" 
 0
 356ad63b-74fc-432d-a11b-224784791bd5
 1
-End_Of_Object VLogCfgData 18
+End_Of_Object VLogCfgData 14
 1
 [End_of_Control]
-End_Of_Object VNETDataListControlHost 17
-VDOLine 17 Begin_Of_Object
+End_Of_Object VNETDataListControlHost 13
+VDOLine 13 Begin_Of_Object
 1
-63
+56
 0
 130 0
 NULL
-End_Of_Object VDOLine 17
+End_Of_Object VDOLine 13
 
 EndOfComment
 0
 1
-End_Of_Object VDAOGBFunctionBlock 16
-End_Of_Object VDODynamicLine 15
-End_Of_Object VDAOGBHSStd 14
+End_Of_Object VDAOGBFunctionBlock 12
+End_Of_Object VDODynamicLine 11
+End_Of_Object VDAOGBHSStd 10
 NULL
-End_Of_Object VDORefinement 13
-VDORefinement 13 Begin_Of_Object
+End_Of_Object VDORefinement 9
+VDORefinement 9 Begin_Of_Object
 1
-64
+57
 0
 5
-VDAOGBHSStd 14 Begin_Of_Object
+VDAOGBHSStd 10 Begin_Of_Object
 1
-65
+58
 0
 0 0
 TABPredecessor:
-62
+55
 TABSuccessor:
-67
-VDODynamicLine 15 Begin_Of_Object
+60
+VDODynamicLine 11 Begin_Of_Object
 1
-66
+59
 0
 0
-VDAOGBFunctionBlock 16 Begin_Of_Object
+VDAOGBFunctionBlock 12 Begin_Of_Object
 1
-67
+60
 0
 TABPredecessor:
-65
+58
 TABSuccessor:
-70
-VGraphBoxConf 17 Begin_Of_Object
+63
+VGraphBoxConf 13 Begin_Of_Object
 1
-VNETGraphBox 18 Begin_Of_Object
+VNETGraphBox 14 Begin_Of_Object
 1
-VNETControlBox 19 Begin_Of_Object
+VNETControlBox 15 Begin_Of_Object
 2
-VUniqueBox 20 Begin_Of_Object
-1
-VBoxRoot 21 Begin_Of_Object
+VUniqueBox 16 Begin_Of_Object
 1
+VBoxRoot 17 Begin_Of_Object
 1
+2
 1 3 0 1 -1 -1 -1 -1 55 198 872 636
 Graphics
 1
 
 MDI_DOCK_INFO_END
 5
 1
@@ -3457,22 +3446,22 @@
 0 0
 END_OF_DESKTOP_DATA
 END_OF_DESKTOP_DATA_COLLECTION
 0
 END_OF_DESKTOP_MEMBER
 {DDA24D23-CEC5-4F19-BC3F-BFC4A28BA823}
 0
-End_Of_Object VBoxRoot 21
+End_Of_Object VBoxRoot 17
 1 -1 0 0 0 0 0 0 0 0 0 0
-End_Of_Object VUniqueBox 20
+End_Of_Object VUniqueBox 16
 1
 1 -1 0 0 0 0 0 0 0 0 0 0
 0
-End_Of_Object VNETControlBox 19
-End_Of_Object VNETGraphBox 18
+End_Of_Object VNETControlBox 15
+End_Of_Object VNETGraphBox 14
 81
 APPDIR Vector.CANalyzer.Graphic.DLL
 Vector.CANalyzer.Graphic, Version=11.0.81.0, Culture=neutral, PublicKeyToken=null
 Vector.CANalyzer.Graphic.ComponentWrapper
 1
 1
 APPDIR CANw_Net.DLL
@@ -3547,130 +3536,130 @@
 mPatch
 0
 --TextFormatter: End of Object--
 --TextFormatter: End of Object--
 TypeRef:2
 2
 --TextFormatter: End of Object--
-VSignalObjectStreamer 18 Begin_Of_Object
+VSignalObjectStreamer 14 Begin_Of_Object
 1
 2
-VSysVarObject 19 Begin_Of_Object
+VSysVarObject 15 Begin_Of_Object
 2
-VHostSignal 20 Begin_Of_Object
+VHostSignal 16 Begin_Of_Object
 2
 3
 speed
 0
-End_Of_Object VHostSignal 20
-19
-ValueObjectConfiguration::VConfiguredSysVar 20 Begin_Of_Object
+End_Of_Object VHostSignal 16
+15
+ValueObjectConfiguration::VConfiguredSysVar 16 Begin_Of_Object
 1
-ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredSysVar> 21 Begin_Of_Object
+ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredSysVar> 17 Begin_Of_Object
 1
-ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 22 Begin_Of_Object
+ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 18 Begin_Of_Object
 1
-VConfigSysVar 23 Begin_Of_Object
+VConfigSysVar 19 Begin_Of_Object
 1
-VConfigEvent 24 Begin_Of_Object
+VConfigEvent 20 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 24
+End_Of_Object VConfigEvent 20
 sys_var_demo
 speed
-End_Of_Object VConfigSysVar 23
-End_Of_Object ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 22
-End_Of_Object ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredSysVar> 21
+End_Of_Object VConfigSysVar 19
+End_Of_Object ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 18
+End_Of_Object ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredSysVar> 17
 -1
 1
-End_Of_Object ValueObjectConfiguration::VConfiguredSysVar 20
+End_Of_Object ValueObjectConfiguration::VConfiguredSysVar 16
 
-End_Of_Serialized_Data 19
+End_Of_Serialized_Data 15
 0
-End_Of_Object VSysVarObject 19
+End_Of_Object VSysVarObject 15
 [MeasurementObject]
 speed
 "km/h" 223 800080 0. 200. -100. 100. 20 0 0 1 576000000 0 1 0 0
-VSignalObject 19 Begin_Of_Object
+VSignalObject 15 Begin_Of_Object
 1
-VSignalObjectBase 20 Begin_Of_Object
+VSignalObjectBase 16 Begin_Of_Object
 1
-VHostSignal 21 Begin_Of_Object
+VHostSignal 17 Begin_Of_Object
 2
 0
 CAN1::easy::Light::LightState::FlashLight
 0
-End_Of_Object VHostSignal 21
+End_Of_Object VHostSignal 17
 2
-VSignalState 21 Begin_Of_Object
+VSignalState 17 Begin_Of_Object
 1
 0
 1
-End_Of_Object VSignalState 21
-End_Of_Object VSignalObjectBase 20
-19
-ValueObjectConfiguration::VConfiguredDBSignal 20 Begin_Of_Object
+End_Of_Object VSignalState 17
+End_Of_Object VSignalObjectBase 16
+15
+ValueObjectConfiguration::VConfiguredDBSignal 16 Begin_Of_Object
 3
-ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredDBSignal> 21 Begin_Of_Object
+ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredDBSignal> 17 Begin_Of_Object
 1
-ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 22 Begin_Of_Object
+ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 18 Begin_Of_Object
 1
-VConfigCANFrame 23 Begin_Of_Object
+VConfigCANFrame 19 Begin_Of_Object
 5
-VConfigMessage 24 Begin_Of_Object
+VConfigMessage 20 Begin_Of_Object
 5
-VConfigBusObject 25 Begin_Of_Object
+VConfigBusObject 21 Begin_Of_Object
 1
-VConfigBusEvent 26 Begin_Of_Object
+VConfigBusEvent 22 Begin_Of_Object
 1
-VConfigEvent 27 Begin_Of_Object
+VConfigEvent 23 Begin_Of_Object
 1
-End_Of_Object VConfigEvent 27
+End_Of_Object VConfigEvent 23
 1
 1
-End_Of_Object VConfigBusEvent 26
-End_Of_Object VConfigBusObject 25
+End_Of_Object VConfigBusEvent 22
+End_Of_Object VConfigBusObject 21
 31
 1
-VDatabaseBusMessageId 25 Begin_Of_Object
+VDatabaseBusMessageId 21 Begin_Of_Object
 3
 801
 1
 1
 0
 0
 0
 LightState
 0
 easy
 0
 1
-End_Of_Object VDatabaseBusMessageId 25
+End_Of_Object VDatabaseBusMessageId 21
 NULL
 0
 0
 0
-End_Of_Object VConfigMessage 24
-End_Of_Object VConfigCANFrame 23
-End_Of_Object ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 22
-End_Of_Object ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredDBSignal> 21
+End_Of_Object VConfigMessage 20
+End_Of_Object VConfigCANFrame 19
+End_Of_Object ValueObjectConfiguration::Detail::AbstractConfiguredValueObject 18
+End_Of_Object ValueObjectConfiguration::Detail::VConfiguredValueObjectBase<class_ValueObjectConfiguration::IConfiguredDBSignal> 17
 FlashLight
 87
 1
 1
 CAN1
 easy
 Light
 801
 LightState
 0
 4294967295
-End_Of_Object ValueObjectConfiguration::VConfiguredDBSignal 20
+End_Of_Object ValueObjectConfiguration::VConfiguredDBSignal 16
 
-End_Of_Serialized_Data 19
-End_Of_Object VSignalObject 19
+End_Of_Serialized_Data 15
+End_Of_Object VSignalObject 15
 [MeasurementObject]
 CAN1::easy::Light::LightState::FlashLight
 "" 159 8080 0. 1. -100. 100. 1 0 0 1 576000000 1 1 0 0
 [GraphWindow:x_x_x_x_x_x_WindowBk_Grid_AxisBk_XAxisFr_YAxisFr_x_x_x_x_x_x]
 0 100000 100000 200000 576000000 1 ffffff b2b2b2 ffffff 0 0 0 0 1 1 1 0
 0 30 5000
 0
@@ -3679,15 +3668,15 @@
 16777215
 0
 2
 0
 1
 41943040
 0
-VLogExportPersister 19 Begin_Of_Object
+VLogExportPersister 15 Begin_Of_Object
 7
 1416
 25200253
 Graphics Window
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 0
@@ -3719,15 +3708,15 @@
 0
 730
 0
 0.10000000000000001
 0
 0
 1
-End_Of_Object VLogExportPersister 19
+End_Of_Object VLogExportPersister 15
 12
 20 25 110 20 18 55 55 55 55 55 57 13 
 322
 0
 0
 0
 0
@@ -3759,15 +3748,15 @@
 8388736 0
 1
 1 1
 
 CAN1::easy::Light::LightState::FlashLight
 32896 0
 0
-VLogCfgData 19 Begin_Of_Object
+VLogCfgData 15 Begin_Of_Object
 11
 0
 0
 0
 0
 0
 0
@@ -3776,23 +3765,23 @@
 1024
 60
 0
 0
 0
 3
 0
-62
+68
 1
 1
 0
 2
 0
 0
-19
-VLogExportPersister 20 Begin_Of_Object
+15
+VLogExportPersister 16 Begin_Of_Object
 7
 1416
 11060201
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 0
@@ -3824,17 +3813,17 @@
 0
 730
 0
 0.10000000000000001
 0
 0
 1
-End_Of_Object VLogExportPersister 20
+End_Of_Object VLogExportPersister 16
 
-End_Of_Serialized_Data 19
+End_Of_Serialized_Data 15
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\Graphics.mdf" 
 0
 1
 0
 10
 80
 0
@@ -3847,15 +3836,15 @@
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\Graphics.mdf" 
 1
 0
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\{LoggingBlock}.mdf" 
 0
 317d9fcd-89c5-4085-b12f-63b0587544d1
 1
-End_Of_Object VLogCfgData 19
+End_Of_Object VLogCfgData 15
 0 128
 0 0 0 0
 1 40 20 15
 0 -1
 1
 1
 0
@@ -3867,64 +3856,64 @@
 1 1 1 0 0 0 0 0 0 0 0 0 
 0 1 2 -1 -1 -1 -1 -1 -1 -1 -1 -1 
 20 25 130 55 55 55 55 55 57 57 82 30 
 322 80
 0
 0
 30000000000
-End_Of_Object VSignalObjectStreamer 18
-End_Of_Object VGraphBoxConf 17
-VDOLine 17 Begin_Of_Object
+End_Of_Object VSignalObjectStreamer 14
+End_Of_Object VGraphBoxConf 13
+VDOLine 13 Begin_Of_Object
 1
-68
+61
 0
 130 0
 NULL
-End_Of_Object VDOLine 17
+End_Of_Object VDOLine 13
 
 EndOfComment
 0
 1
-End_Of_Object VDAOGBFunctionBlock 16
-End_Of_Object VDODynamicLine 15
-End_Of_Object VDAOGBHSStd 14
+End_Of_Object VDAOGBFunctionBlock 12
+End_Of_Object VDODynamicLine 11
+End_Of_Object VDAOGBHSStd 10
 NULL
-End_Of_Object VDORefinement 13
-VDORefinement 13 Begin_Of_Object
+End_Of_Object VDORefinement 9
+VDORefinement 9 Begin_Of_Object
 1
-69
+62
 0
 6
-VDAOGBHSStd 14 Begin_Of_Object
+VDAOGBHSStd 10 Begin_Of_Object
 1
-70
+63
 0
 1 0
 TABPredecessor:
-67
+60
 TABSuccessor:
-72
-VDODynamicLine 15 Begin_Of_Object
+65
+VDODynamicLine 11 Begin_Of_Object
 1
-71
+64
 0
 0
-VDAOGBFunctionBlock 16 Begin_Of_Object
+VDAOGBFunctionBlock 12 Begin_Of_Object
 1
-72
+65
 0
 TABPredecessor:
-70
+63
 TABSuccessor:
-74
-VTriggerConfiguration 17 Begin_Of_Object
+67
+VTriggerConfiguration 13 Begin_Of_Object
 2
-VMigratedGenericConfiguration<struct_VTriggerCfgData> 18 Begin_Of_Object
+VMigratedGenericConfiguration<struct_VTriggerCfgData> 14 Begin_Of_Object
 1
-VTriggerCfgData 19 Begin_Of_Object
+VTriggerCfgData 15 Begin_Of_Object
 5
 2
 0
 0
 0
 0
 0
@@ -3936,40 +3925,40 @@
 0
 200000
 1
 1
 1
 1
 50000
-VEvCondBlock 20 Begin_Of_Object
+VEvCondBlock 16 Begin_Of_Object
 1
-VEvCondGroup 21 Begin_Of_Object
+VEvCondGroup 17 Begin_Of_Object
 2
-VEvCondPrimitive 22 Begin_Of_Object
+VEvCondPrimitive 18 Begin_Of_Object
 1
 1
-End_Of_Object VEvCondPrimitive 22
+End_Of_Object VEvCondPrimitive 18
 1
 0
 0
-End_Of_Object VEvCondGroup 21
-End_Of_Object VEvCondBlock 20
-VEvCondBlock 20 Begin_Of_Object
+End_Of_Object VEvCondGroup 17
+End_Of_Object VEvCondBlock 16
+VEvCondBlock 16 Begin_Of_Object
 1
-VEvCondGroup 21 Begin_Of_Object
+VEvCondGroup 17 Begin_Of_Object
 2
-VEvCondPrimitive 22 Begin_Of_Object
+VEvCondPrimitive 18 Begin_Of_Object
 1
 1
-End_Of_Object VEvCondPrimitive 22
+End_Of_Object VEvCondPrimitive 18
 1
 0
 0
-End_Of_Object VEvCondGroup 21
-End_Of_Object VEvCondBlock 20
+End_Of_Object VEvCondGroup 17
+End_Of_Object VEvCondBlock 16
 0
 0
 0
 116
 0
 0
 0
@@ -3977,21 +3966,21 @@
 0
 0
 0
 0
 0
 0
 0
-End_Of_Object VTriggerCfgData 19
-End_Of_Object VMigratedGenericConfiguration<struct_VTriggerCfgData> 18
-VTriggerBox 18 Begin_Of_Object
-1
-VBoxRoot 19 Begin_Of_Object
+End_Of_Object VTriggerCfgData 15
+End_Of_Object VMigratedGenericConfiguration<struct_VTriggerCfgData> 14
+VTriggerBox 14 Begin_Of_Object
 1
+VBoxRoot 15 Begin_Of_Object
 1
+2
 1 -1 0 1 0 0 0 0 208 222 817 579
 Logging
 1
 
 MDI_DOCK_INFO_END
 5
 1
@@ -4041,36 +4030,36 @@
 END_OF_DESKTOP_DATA
 END_OF_DESKTOP_DATA_COLLECTION
 0
 0 0
 END_OF_DESKTOP_MEMBER
 {B4420F90-8E30-47C5-ADE2-9C9639240574}
 0
-End_Of_Object VBoxRoot 19
-End_Of_Object VTriggerBox 18
+End_Of_Object VBoxRoot 15
+End_Of_Object VTriggerBox 14
 0
-End_Of_Object VTriggerConfiguration 17
-VDOLine 17 Begin_Of_Object
+End_Of_Object VTriggerConfiguration 13
+VDOLine 13 Begin_Of_Object
 1
-73
+66
 0
 10 0
-VDAOGBFunctionBlock 18 Begin_Of_Object
+VDAOGBFunctionBlock 14 Begin_Of_Object
 1
-74
+67
 0
 TABPredecessor:
-72
+65
 TABSuccessor:
 0
-VLoggingConfiguration 19 Begin_Of_Object
+VLoggingConfiguration 15 Begin_Of_Object
 4
-VMigratedGenericConfiguration<class_VLogCfgData> 20 Begin_Of_Object
+VMigratedGenericConfiguration<class_VLogCfgData> 16 Begin_Of_Object
 1
-VLogCfgData 21 Begin_Of_Object
+VLogCfgData 17 Begin_Of_Object
 11
 0
 1
 1
 1
 0
 0
@@ -4079,23 +4068,23 @@
 1024
 60
 1
 0
 0
 3
 0
-62
+68
 1
 1
 0
 2
 0
 0
-21
-VLogExportPersister 22 Begin_Of_Object
+17
+VLogExportPersister 18 Begin_Of_Object
 7
 1416
 11060201
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 <VFileName V7 QL> 1 "" 
 0
@@ -4127,17 +4116,17 @@
 0
 730
 0
 0.10000000000000001
 0
 0
 1
-End_Of_Object VLogExportPersister 22
+End_Of_Object VLogExportPersister 18
 
-End_Of_Serialized_Data 21
+End_Of_Serialized_Data 17
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\Logging.blf" 
 0
 1
 0
 10
 80
 0
@@ -4150,89 +4139,155 @@
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe" 
 1
 1
 <VFileName V7 QL> 1 "C:\Users\Public\Documents\Vector\CANoe\11.0 (x64)\Templates\CANoe\{LoggingBlock}.blf" 
 0
 20049e46-aec9-4a57-acbf-126e41f2029d
 1
-End_Of_Object VLogCfgData 21
-End_Of_Object VMigratedGenericConfiguration<class_VLogCfgData> 20
+End_Of_Object VLogCfgData 17
+End_Of_Object VMigratedGenericConfiguration<class_VLogCfgData> 16
 1
-End_Of_Object VLoggingConfiguration 19
-VDOLine 19 Begin_Of_Object
+End_Of_Object VLoggingConfiguration 15
+VDOLine 15 Begin_Of_Object
 1
-75
+68
 0
 60 0
 NULL
-End_Of_Object VDOLine 19
+End_Of_Object VDOLine 15
 
 EndOfComment
 1
 1
-End_Of_Object VDAOGBFunctionBlock 18
-End_Of_Object VDOLine 17
+End_Of_Object VDAOGBFunctionBlock 14
+End_Of_Object VDOLine 13
 
 EndOfComment
 0
 1
-End_Of_Object VDAOGBFunctionBlock 16
-End_Of_Object VDODynamicLine 15
-End_Of_Object VDAOGBHSStd 14
-NULL
-End_Of_Object VDORefinement 13
-End_Of_Object VDOFRamification 12
+End_Of_Object VDAOGBFunctionBlock 12
 End_Of_Object VDODynamicLine 11
 End_Of_Object VDAOGBHSStd 10
-End_Of_Object VDAOSwitch 9
+NULL
+End_Of_Object VDORefinement 9
+End_Of_Object VDOFRamification 8
+End_Of_Object VDODynamicLine 7
+End_Of_Object VDAOGBHSStd 6
+End_Of_Object VDAOSwitch 5
+
+EndOfComment
+1
+1
+End_Of_Object VDAOGBFunctionBlock 4
+VDAOGBFunctionBlock 4 Begin_Of_Object
+1
+33
+0
+TABPredecessor:
+0
+TABSuccessor:
+34
+VPlugConf 5 Begin_Of_Object
+1
+End_Of_Object VPlugConf 5
+VDAOGBFunctionBlock 5 Begin_Of_Object
+1
+34
+0
+TABPredecessor:
+33
+TABSuccessor:
+70
+VChannelFilterConfiguration 6 Begin_Of_Object
+3
+VMigratedGenericConfiguration<class_VChannelFilterData> 7 Begin_Of_Object
+1
+VChannelFilterData 8 Begin_Of_Object
+2
+1
+VBusChannelData 9 Begin_Of_Object
+1
+2
+2
+1
+2
+1
+1
+End_Of_Object VBusChannelData 9
+End_Of_Channel_Data
+1
+End_Of_Object VChannelFilterData 8
+End_Of_Object VMigratedGenericConfiguration<class_VChannelFilterData> 7
+0
+0
+End_Of_Object VChannelFilterConfiguration 6
+VDOCrossing 6 Begin_Of_Object
+2
+35
+0
+VDAOGBHSStd 7 Begin_Of_Object
+1
+36
+0
+0 0
+TABPredecessor:
+75
+TABSuccessor:
+38
+VDODynamicLine 8 Begin_Of_Object
+1
+37
+0
+0
+NULL
 End_Of_Object VDODynamicLine 8
 End_Of_Object VDAOGBHSStd 7
 NULL
 VDODynamicLine 7 Begin_Of_Object
 1
-37
+69
 1
 20
 VDAOGBHSStd 8 Begin_Of_Object
 1
-38
+70
 1
 1 0
 TABPredecessor:
-2
+34
 TABSuccessor:
-43
+75
 VDODynamicLine 9 Begin_Of_Object
 1
-39
+71
 1
 0
 VDODynamicLine 10 Begin_Of_Object
 1
-40
+72
 1
 10
 VDODynamicLine 11 Begin_Of_Object
 1
-41
+73
 0
 20
 VDOLine 12 Begin_Of_Object
 1
-42
+74
 0
 10 0
 VDAOGBFunctionBlock 13 Begin_Of_Object
 1
-43
+75
 0
 TABPredecessor:
-38
+70
 TABSuccessor:
-4
+36
 VLoggingConfiguration 14 Begin_Of_Object
 4
 VMigratedGenericConfiguration<class_VLogCfgData> 15 Begin_Of_Object
 1
 VLogCfgData 16 Begin_Of_Object
 11
 0
@@ -4246,15 +4301,15 @@
 1024
 60
 0
 0
 0
 3
 1
-62
+68
 1
 1
 0
 2
 1
 0
 16
@@ -4345,77 +4400,19 @@
 1
 End_Of_Object VDAOGBFunctionBlock 5
 
 EndOfComment
 1
 1
 End_Of_Object VDAOGBFunctionBlock 4
-VDAOGBFunctionBlock 4 Begin_Of_Object
-1
-44
-0
-TABPredecessor:
-0
-TABSuccessor:
-45
-VOfflineSrcConfiguration 5 Begin_Of_Object
-3
-VMigratedGenericConfiguration<struct_VOfflineCfgData> 6 Begin_Of_Object
-1
-VOfflineCfgData 7 Begin_Of_Object
-2
-VReplayCfgBase 8 Begin_Of_Object
-1
-0
-1
-End_Of_Object VReplayCfgBase 8
-VCfgBreakCondition 8 Begin_Of_Object
-1
-VDataBreakCondition 9 Begin_Of_Object
-1
-0
-VEvCondBlock 10 Begin_Of_Object
-1
-VEvCondGroup 11 Begin_Of_Object
-2
-VEvCondPrimitive 12 Begin_Of_Object
-1
-1
-End_Of_Object VEvCondPrimitive 12
-1
-0
-0
-End_Of_Object VEvCondGroup 11
-End_Of_Object VEvCondBlock 10
-End_Of_Object VDataBreakCondition 9
-End_Of_Object VCfgBreakCondition 8
-0
-0
-0
-0
-0
-0
-End_Of_Object VOfflineCfgData 7
-End_Of_Object VMigratedGenericConfiguration<struct_VOfflineCfgData> 6
-VChannelMapping 6 Begin_Of_Object
-1
-0
-End_Of_Object VChannelMapping 6
-End_Of_Object VOfflineSrcConfiguration 5
-NULL
-
-EndOfComment
-1
-1
-End_Of_Object VDAOGBFunctionBlock 4
 0
 End_Of_Object VDOLocalInfoStruct 3
 67305472
 0
-0
+1
 2
 VDOLocalInfoStruct 3 Begin_Of_Object
 End_Of_Object VDOLocalInfoStruct 3
 End_Of_Serialized_Data 2
 0.000000
 0 0
 End_Of_Object VGBAnlyzBox 2
@@ -4451,15 +4448,15 @@
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 1
 0
 0
 0
 1
-958 652
+1920 657
 END_OF_DESKTOP_DATA
 6
 0 1 -1 -1 -1 -1 44 44 975 557
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 0
 1
@@ -4535,15 +4532,15 @@
 End_Of_Object VBoxRoot 5
 1 -1 0 0 0 0 0 0 0 0 0 0
 End_Of_Object VUniqueBox 4
 End_Of_Object VGrMnBox 3
 VDOLocalInfoStruct 3 Begin_Of_Object
 4
 1
-191
+205
 VDAOBus 4 Begin_Of_Object
 1
 1
 3
 VDAOGBFunctionBlock 5 Begin_Of_Object
 1
 68
@@ -6922,27 +6919,27 @@
 End_Of_Object VDAOGBFunctionBlock 5
 End_Of_Object VDAOBus 4
 NULL
 0
 End_Of_Object VDOLocalInfoStruct 3
 0.000000
 0 0
-1 0 2 59421 1 233 1 2882400001 3411 3644 176 727 2882400002  0 0 0 59421 1 280 1 2882400001 3406 3406 178 178 2882400002  0 0 0 1803879512 0 0   3 
+1 0 2 59421 1 233 1 2882400001 530 763 176 727 2882400002  0 0 0 59421 1 280 1 2882400001 525 725 178 378 2882400002  0 0 0 0 0 0   3 
 SS_BEGIN_COMMON_INFO
 1
 0
 SS_END_COMMON_INFO
 
 EOF_MBSSDATA
 2
 CAN1
 1
 1
 1
-1888910509248 1 0 1 0 0 1 0 0 0 2000 1 
+0 1 0 1 0 0 1 0 0 0 2000 1 
 SS_BEGIN_COMMON_INFO
 1
 3
 Channels
 1
 Databases
 1
@@ -6957,15 +6954,15 @@
 _End_VPRBSManager
 NodeSignalPanelBustypeCount 0
 EOF_BUS
 CAN2
 1
 1
 2
-1888910502288 1 0 0 0 0 1 0 0 0 2000 1 
+0 1 0 0 0 0 1 0 0 0 2000 1 
 SS_BEGIN_COMMON_INFO
 1
 3
 Channels
 1
 Databases
 1
@@ -7006,15 +7003,15 @@
 0
 0
 1
 1920 858
 END_OF_DESKTOP_DATA
 6
 0 1 -1 -1 -1 -1 0 402 423 595
-6 1 0 0 0 0 0 0 423 189 0 0 1 36756 1904 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 1 0 0 0 1 201 0 59422 1 
+6 1 0 0 0 0 0 0 423 189 0 0 1 36756 1904 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 1 0 0 0 1 197 0 59422 1 
 END_OF_DOCK_INFO
 1
 0
 0
 0
 1
 1275 836
@@ -7112,15 +7109,15 @@
 End_Of_Serialized_Data 3
 End_Of_Object VWriteControlAdapter 3
 
 End_Of_Serialized_Data 2
 End_Of_Object VWriteBox 2
 VWinStore 2 Begin_Of_Object
 1
-22 0 1 -1 -1 -1 -1 2876 0 3840 1053
+22 2 3 -32000 -32000 -1 -1 960 0 1924 1053
 End_Of_Child_List
 End_Of_Object VWinStore 2
 VWinStore 2 Begin_Of_Object
 1
 22 0 1 -1 -1 -1 -1 0 21 1021 739
 End_Of_Child_List
 End_Of_Object VWinStore 2
@@ -7408,15 +7405,15 @@
 1
 End_Of_Object VPanelAdapter 3
 
 End_Of_Serialized_Data 2
 End_Of_Object VPanelBox 2
 VPersistentPath 2 Begin_Of_Object
 1
-<VFileName V7 QL> 1 "demo.cpd" 
+<VFileName V7 QL> 1 "demo_offline.cpd" 
 End_Of_Object VPersistentPath 2
 0
 3
 0
 0
 VPlugInsPersistentWrapper 2 Begin_Of_Object
 1
@@ -10532,15 +10529,15 @@
 ArrayElement
 0
 Int32
 _size
 1
 Int32
 _version
-188
+202
 --TextFormatter: End of Object--
 TypeRef:8
 9
 Array
 _items
 14
 APPDIR Vector.CANalyzer.StartValues.DLL
@@ -10785,15 +10782,15 @@
 1024
 60
 1
 0
 0
 3
 0
-62
+68
 1
 1
 0
 2
 0
 0
 3
@@ -11962,19 +11959,14 @@
 --TextFormatter: End of Object--
 VCommonMacroSettings
 VCommonMacroSettings 2 Begin_Of_Object
 1
 3
 YYYY-MM-DD_hh-mm-ss
 End_Of_Object VCommonMacroSettings 2
-EthernetSettings
-NEthernet::VGlobalSettings 2 Begin_Of_Object
-1
-1
-End_Of_Object NEthernet::VGlobalSettings 2
 VSymbolSelectionDialogSettings
 VSymbolSelectionDialogSettings 2 Begin_Of_Object
 1
 
 End_Of_Object VSymbolSelectionDialogSettings 2
 FunctionBusData
 NFunctionBus::NDataModel::VFunctionBusData 2 Begin_Of_Object
@@ -11989,15 +11981,15 @@
 VNETControlBox 4 Begin_Of_Object
 2
 VUniqueBox 5 Begin_Of_Object
 1
 VBoxRoot 6 Begin_Of_Object
 1
 3
-1 -1 0 1 0 0 0 0 254 165 1018 664
+1 -1 0 1 -1 -1 -1 -1 254 165 931 459
 Offline Mode
 1
 
 MDI_DOCK_INFO_END
 5
 1
 6
@@ -12008,23 +12000,23 @@
 -1
 0
 0
 0
 0 0
 END_OF_DESKTOP_DATA
 6
-0 1 0 0 -1 -1 254 165 1018 664
+0 1 -1 -1 -1 -1 254 165 931 459
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 0
 -1
 0
 0
-0
-0 0
+1
+1920 657
 END_OF_DESKTOP_DATA
 6
 0 1 0 0 -1 -1 254 165 1018 664
 6 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 -1 -1 32767 0 0 0 0 0 0 0 0 0 0 -1 -1 0 0 0 0 0 0 
 END_OF_DOCK_INFO
 0
 -1
@@ -12098,48 +12090,75 @@
 {0F499E6B-AA60-4299-BA24-2C8C272F79C8}
 0
 End_Of_Object VBoxRoot 6
 1 -1 0 0 0 0 0 0 0 0 0 0
 End_Of_Object VUniqueBox 5
 1
 1 -1 0 0 0 0 0 0 0 0 0 0
-1
+0
 End_Of_Object VNETControlBox 4
-144
+171
 APPDIR Vector.CANalyzer.OfflineMode.GUI.DLL
 Vector.CANalyzer.OfflineMode.GUI, Version=11.0.81.0, Culture=neutral, PublicKeyToken=null
 Vector.CANalyzer.OfflineMode.GUI.ComponentWrapper
 1
 1
 APPDIR CANw_Net.DLL
 CANw_Net, Version=11.0.81.0, Culture=neutral, PublicKeyToken=null
 Vector.CANalyzer.ApplicationSerializer
 2
 Application
 2
 String
 OverallModel
-110
+137
 <?xml version="1.0" encoding="utf-8"?>
 <OfflineConfigOverallModel xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
 <DataModel xmlns="" i:type="OfflineConfigDataModel">
 <LogFileMergeMode>ByMeasurementTime</LogFileMergeMode>
 <RootGroup xmlns="" i:type="RootGroup">
-<OfflineSources xmlns:d4p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays" />
-<Id>96d8f0c1-b710-4dac-a139-7dae022761e4</Id>
+<OfflineSources xmlns:d4p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
+<d4p1:anyType xmlns="" i:type="LogFile">
+<FileName>Logs\demo_log.blf</FileName>
+<CurrentTargetIds>
+<d4p1:string>8d5e35d3-5f4c-47d3-8fa8-ab7ce93976c3</d4p1:string>
+</CurrentTargetIds>
+<Id>80150363-7cd2-46d2-99e4-c66fcb3a53fd</Id>
+<IsActive>true</IsActive>
+<ChannelMappingSetId i:nil="true" />
+</d4p1:anyType>
+</OfflineSources>
+<Id>e8877284-28dc-45fc-8140-a68155e9ae1d</Id>
 </RootGroup>
-<ChannelMappingSets xmlns:d3p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays" />
+<ChannelMappingSets xmlns:d3p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
+<d3p1:anyType xmlns="" i:type="ChannelMappingSet">
+<ChannelMappingDtos>
+<d3p1:anyType xmlns="" i:type="ChannelMapping">
+<Source>1</Source>
+<Bus>CAN</Bus>
+<Destination>1</Destination>
+</d3p1:anyType>
+<d3p1:anyType xmlns="" i:type="ChannelMapping">
+<Source>2</Source>
+<Bus>CAN</Bus>
+<Destination>2</Destination>
+</d3p1:anyType>
+</ChannelMappingDtos>
+<DisplayName>ChannelMappingSet_1</DisplayName>
+<Id>e871d49a-4485-4de8-a243-2acb181bb805</Id>
+</d3p1:anyType>
+</ChannelMappingSets>
 <DefaultChannelMappingSetId i:nil="true" />
 </DataModel>
 <GuiModel xmlns="" i:type="OfflineConfigGuiModel">
 <ConfigDialogState xmlns="" i:type="ConfigDialogState">
-<Left i:nil="true" />
-<Top i:nil="true" />
-<Width i:nil="true" />
-<Height i:nil="true" />
+<Left>667</Left>
+<Top>284</Top>
+<Width>585</Width>
+<Height>481</Height>
 </ConfigDialogState>
 <FrontEndViewState xmlns="" i:type="FrontEndViewState">
 <ColumnStates xmlns:d4p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
 <d4p1:anyType xmlns="" i:type="ColumnState">
 <FieldName>IsActive</FieldName>
 <IsVisible>true</IsVisible>
 <VisiblePosition>0</VisiblePosition>
@@ -12607,19 +12626,14 @@
 End_Of_Object VNETStandaloneComponent 3
 End_Of_Object VFunctionBusSetupWrapper 2
 ApplicationModelSetup
 VApplicationModelSetup 2 Begin_Of_Object
 1
 0
 End_Of_Object VApplicationModelSetup 2
-EthernetPortBasedVLANSettings
-NEthernet::VPortBasedVLANSettings 2 Begin_Of_Object
-1
-0
-End_Of_Object NEthernet::VPortBasedVLANSettings 2
 DiagnosticParameterWindow
 VDiagnosticParameterWindowWrapper 2 Begin_Of_Object
 1
 VNETStandaloneComponent 3 Begin_Of_Object
 1
 VNETControlBox 4 Begin_Of_Object
 2
```

### Comparing `py_canoe-0.0.9/tests/test_canoe.py` & `py_canoe-0.1.1/tests/test_canoe.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,56 +5,93 @@
 file_path = os.path.dirname(os.path.abspath(__file__)).replace('/', '\\')
 root_path = '\\'.join(file_path.split('\\')[:-1])
 sys.path.extend([file_path, fr'{root_path}\src'])
 
 from py_canoe import CANoe
 canoe_inst = CANoe()
 
-def test_get_canoe_configuration_details():
+def test_canoe_open_new_save_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    canoe_inst.get_canoe_configuration_details()
+    canoe_inst.new(auto_save=True)
+    assert canoe_inst.save_configuration_as(fr'{file_path}\demo_cfg\demo_v10.cfg', 10, 0)
+    wait(2)
+
+def test_canoe_basic_measurement_methods():
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    meas_index = canoe_inst.get_measurement_index()
+    print(f'CANoe measurement index value = {meas_index}')
+    assert canoe_inst.start_measurement()
+    assert canoe_inst.stop_measurement()
+    meas_index = canoe_inst.get_measurement_index()
+    print(f'CANoe measurement index value = {meas_index}')
+    canoe_inst.set_measurement_index(meas_index+1)
+    meas_index = canoe_inst.get_measurement_index()
+    print(f'CANoe measurement index value = {meas_index}')
+    canoe_inst.get_measurement_running_status()
+    canoe_inst.reset_measurement()
+    assert canoe_inst.stop_measurement()
 
-
-def test_check_measurement():
-    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    start_resp = canoe_inst.start_measurement()
-    stop_resp = canoe_inst.stop_measurement()
-    assert start_resp
-    assert stop_resp
-
-def test_diag_request():
+def test_diag_request_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    canoe_inst.start_measurement()
+    assert canoe_inst.start_measurement()
     wait(1)
     resp = canoe_inst.send_diag_request('Door', '10 01')
-    canoe_inst.stop_measurement()
+    assert canoe_inst.stop_measurement()
     assert resp == '50 01 00 00 00 00'
 
-def test_write_window():
+def test_signal_value_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    canoe_inst.start_measurement()
-    wait(1)
-    canoe_inst.write_text_in_write_window("hello from python!")
-    wait(1)
-    text = canoe_inst.read_text_from_write_window()
-    canoe_inst.stop_measurement()
-    assert "hello from python!" in text
-
-def test_set_get_signal_value():
-    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    canoe_inst.start_measurement()
+    assert canoe_inst.start_measurement()
     wait(1)
     canoe_inst.set_signal_value('CAN', 1, 'LightState', 'FlashLight', 1)
     wait(1)
+    canoe_inst.check_signal_online('CAN', 1, 'LightState', 'FlashLight')
+    canoe_inst.check_signal_state('CAN', 1, 'LightState', 'FlashLight')
     sig_val = canoe_inst.get_signal_value('CAN', 1, 'LightState', 'FlashLight')
-    canoe_inst.stop_measurement()
+    assert canoe_inst.stop_measurement()
     assert sig_val == 1
+    wait(2)
 
-def test_set_get_system_variable_value():
+def test_system_variable_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
-    canoe_inst.start_measurement()
+    assert canoe_inst.start_measurement()
     wait(1)
     canoe_inst.set_system_variable_value('demo::level_two_1::sys_var2', 20)
     wait(1)
     sys_var_val = canoe_inst.get_system_variable_value('demo::level_two_1::sys_var2')
-    canoe_inst.stop_measurement()
+    assert canoe_inst.stop_measurement()
     assert sys_var_val == 20
+    wait(2)
+
+def test_canoe_open_close_methods():
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    wait(1)
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    wait(1)
+
+def test_write_window_methods():
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    wait(1)
+    canoe_inst.enable_write_window_output_file(fr'{file_path}\demo_cfg\Logs\write_win.txt')
+    wait(1)
+    assert canoe_inst.start_measurement()
+    wait(1)
+    canoe_inst.write_text_in_write_window("hello from python!")
+    wait(1)
+    text = canoe_inst.read_text_from_write_window()
+    assert canoe_inst.stop_measurement()
+    canoe_inst.disable_write_window_output_file()
+    assert "hello from python!" in text
+    wait(2)
+
+def test_canoe_animation_mode_methods():
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo_offline.cfg')
+    canoe_inst.step_measurement_event_in_single_step()
+    wait(2)
+    canoe_inst.start_measurement_in_animation_mode()
+    wait(2)
+    canoe_inst.break_measurement_in_offline_mode()
+    wait(2)
+    canoe_inst.reset_measurement_in_offline_mode()
+    wait(2)
+    assert canoe_inst.stop_measurement()
+    wait(2)
```

### Comparing `py_canoe-0.0.9/PKG-INFO` & `py_canoe-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_canoe
-Version: 0.0.9
+Version: 0.1.1
 Summary: Python package for controlling Vector CANoe tool
 Author-email: chaitu-ycr <chaitu.ycr@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
```

