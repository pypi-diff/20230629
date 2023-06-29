# Comparing `tmp/serialdevicehandler-1.0.0.tar.gz` & `tmp/serialdevicehandler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdevicehandler-1.0.0.tar", last modified: Sun Jun 18 16:47:37 2023, max compression
+gzip compressed data, was "serialdevicehandler-1.0.1.tar", last modified: Thu Jun 29 07:40:08 2023, max compression
```

## Comparing `serialdevicehandler-1.0.0.tar` & `serialdevicehandler-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:47:37.173860 serialdevicehandler-1.0.0/
--rw-rw-rw-   0        0        0     3069 2023-06-18 16:47:37.171360 serialdevicehandler-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2737 2023-06-18 16:43:55.000000 serialdevicehandler-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 16:47:37.159358 serialdevicehandler-1.0.0/serialdevicehandler/
--rw-rw-rw-   0        0        0       37 2023-06-18 15:10:43.000000 serialdevicehandler-1.0.0/serialdevicehandler/__init__.py
--rw-rw-rw-   0        0        0     4568 2023-06-18 15:10:43.000000 serialdevicehandler-1.0.0/serialdevicehandler/main.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:47:37.169860 serialdevicehandler-1.0.0/serialdevicehandler.egg-info/
--rw-rw-rw-   0        0        0     3069 2023-06-18 16:47:37.000000 serialdevicehandler-1.0.0/serialdevicehandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-06-18 16:47:37.000000 serialdevicehandler-1.0.0/serialdevicehandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:47:37.000000 serialdevicehandler-1.0.0/serialdevicehandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-18 16:47:37.000000 serialdevicehandler-1.0.0/serialdevicehandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 16:47:37.173860 serialdevicehandler-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-06-18 15:27:46.000000 serialdevicehandler-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:40:08.784628 serialdevicehandler-1.0.1/
+-rw-rw-rw-   0        0        0     3085 2023-06-29 07:40:08.783627 serialdevicehandler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2753 2023-06-29 07:34:03.000000 serialdevicehandler-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:40:08.747176 serialdevicehandler-1.0.1/serialdevicehandler/
+-rw-rw-rw-   0        0        0       37 2023-06-29 06:48:32.000000 serialdevicehandler-1.0.1/serialdevicehandler/__init__.py
+-rw-rw-rw-   0        0        0     4589 2023-06-29 07:36:37.000000 serialdevicehandler-1.0.1/serialdevicehandler/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:40:08.779666 serialdevicehandler-1.0.1/serialdevicehandler.egg-info/
+-rw-rw-rw-   0        0        0     3085 2023-06-29 07:40:08.000000 serialdevicehandler-1.0.1/serialdevicehandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-29 07:40:08.000000 serialdevicehandler-1.0.1/serialdevicehandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:40:08.000000 serialdevicehandler-1.0.1/serialdevicehandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-29 07:40:08.000000 serialdevicehandler-1.0.1/serialdevicehandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:40:08.785622 serialdevicehandler-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      760 2023-06-29 07:35:26.000000 serialdevicehandler-1.0.1/setup.py
```

### Comparing `serialdevicehandler-1.0.0/PKG-INFO` & `serialdevicehandler-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdevicehandler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library to run commands on a device via serial port
 Home-page: https://github.com/Salliii/serialdevicehandler
 Author: Salliii
 Keywords: python,library,serial device,serial interface,commands,execute
 Description-Content-Type: text/markdown
 
 # Serial Device Handler
@@ -52,45 +52,46 @@
 
 ```python
 device = SerialDeviceHandler(port, baudrate, timeout)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
-| `port`      | Specifies the device port | `str` | Windows: `COM1`  Linux: `/dev/tty` |
+| `port`      | Specifies the device port | `str` | COM1 |
 | `baudrate`  | Specifies the device baudrate | `str` | 9600 |
 | `timeout`   | Specifies the command timeout | `int` | 0.2s |
 
 There are some attributes for statistical and other purposes.
 
-| attribute | description | expected type |
-| :-------- | :---------- | :------------ |
-| `is_open`       | Indicates whether the serial port is open | `bool` |
-| `eol_delimiter` | defines the end-of-line separator for line reading | `int` |
-| `total_rx`      | stores the total bytes received | `int` |
-| `total_tx`      | stores the total bytes transmitted | `int` |
+| attribute | description | expected type | default value |
+| :-------- | :---------- | :------------ | :------------ |
+| `is_open`       | Indicates whether the serial port is open | `bool` | False |
+| `eol_delimiter` | defines the end-of-line separator for line reading | `str` | \n |
+| `total_rx`      | stores the total bytes received | `int` | 0 |
+| `total_tx`      | stores the total bytes transmitted | `int` | 0 |
 
 
 <br>
 
 
 ### SerialDeviceHandler.execute()
 Use the `execute()` function to run a command.
 
 Syntax:
 
 ```python
-device.execute(command, pseudo, stdout)
+device.execute(command, <optional arguments>)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
 | `command` | Defines the command to be executed | `str` | n/a |
-| `pseudo`  | Execute as a pseudo command. No command is executed. Use it to capture bootups, etc. | `bool` | False |
 | `stdout`  | Live output while the command is running | `bool` | False |
+| `read_only` | read only execution | bool | False
+| `write_only` | write only execution | bool | False
 
 
 <br>
 
 
 ## Summary
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: serialdevicehandler Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: serialdevicehandler Version: 1.0.1 Summary: A
 python library to run commands on a device via serial port Home-page: https://
 github.com/Salliii/serialdevicehandler Author: Salliii Keywords:
 python,library,serial device,serial interface,commands,execute Description-
 Content-Type: text/markdown # Serial Device Handler [![PyPi version][shields-
 pypi_version]][url-pypi_version] [![Github Issues][shields-issues]][url-issues]
 Execute commands on a device via serial port.
 ## Installing Install using pip ```bash pip install serialdevicehandler ``` or
@@ -10,28 +10,28 @@
 ## Example ```python from serialdevicehandler import * device =
 serialdevicehandler(port="COM10", baudrate="115200") output = device.execute
 ("help") print(output) ```
 ## SerialDeviceHandler() `SerialDeviceHandler()` is the core class within the
 library. Syntax: ```python device = SerialDeviceHandler(port, baudrate,
 timeout) ``` | argument | description | expected type | default value | | :----
 --- | :---------- | :------------ | :------------ | | `port` | Specifies the
-device port | `str` | Windows: `COM1` Linux: `/dev/tty` | | `baudrate` |
-Specifies the device baudrate | `str` | 9600 | | `timeout` | Specifies the
-command timeout | `int` | 0.2s | There are some attributes for statistical and
-other purposes. | attribute | description | expected type | | :-------- | :----
------- | :------------ | | `is_open` | Indicates whether the serial port is
-open | `bool` | | `eol_delimiter` | defines the end-of-line separator for line
-reading | `int` | | `total_rx` | stores the total bytes received | `int` | |
-`total_tx` | stores the total bytes transmitted | `int` |
+device port | `str` | COM1 | | `baudrate` | Specifies the device baudrate |
+`str` | 9600 | | `timeout` | Specifies the command timeout | `int` | 0.2s |
+There are some attributes for statistical and other purposes. | attribute |
+description | expected type | default value | | :-------- | :---------- | :----
+-------- | :------------ | | `is_open` | Indicates whether the serial port is
+open | `bool` | False | | `eol_delimiter` | defines the end-of-line separator
+for line reading | `str` | \n | | `total_rx` | stores the total bytes received
+| `int` | 0 | | `total_tx` | stores the total bytes transmitted | `int` | 0 |
 ### SerialDeviceHandler.execute() Use the `execute()` function to run a
-command. Syntax: ```python device.execute(command, pseudo, stdout) ``` |
-argument | description | expected type | default value | | :------- | :--------
--- | :------------ | :------------ | | `command` | Defines the command to be
-executed | `str` | n/a | | `pseudo` | Execute as a pseudo command. No command
-is executed. Use it to capture bootups, etc. | `bool` | False | | `stdout` |
-Live output while the command is running | `bool` | False |
+command. Syntax: ```python device.execute(command, ) ``` | argument |
+description | expected type | default value | | :------- | :---------- | :-----
+------- | :------------ | | `command` | Defines the command to be executed |
+`str` | n/a | | `stdout` | Live output while the command is running | `bool` |
+False | | `read_only` | read only execution | bool | False | `write_only` |
+write only execution | bool | False
 ## Summary - SerialDeviceHandler() - _execute()_  [shields-pypi_version]:
 https://img.shields.io/pypi/v/
 serialdevicehandler?label=PyPi%20Version&style=for-the-badge [shields-issues]:
 https://img.shields.io/github/issues/Salliii/serialdevicehandler?style=for-the-
 badge  [url-pypi_version]: https://pypi.org/project/serialdevicehandler/ [url-
 issues]: https://github.com/Salliii/serialdevicehandler/issues
```

### Comparing `serialdevicehandler-1.0.0/README.md` & `serialdevicehandler-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,45 +43,46 @@
 
 ```python
 device = SerialDeviceHandler(port, baudrate, timeout)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
-| `port`      | Specifies the device port | `str` | Windows: `COM1`  Linux: `/dev/tty` |
+| `port`      | Specifies the device port | `str` | COM1 |
 | `baudrate`  | Specifies the device baudrate | `str` | 9600 |
 | `timeout`   | Specifies the command timeout | `int` | 0.2s |
 
 There are some attributes for statistical and other purposes.
 
-| attribute | description | expected type |
-| :-------- | :---------- | :------------ |
-| `is_open`       | Indicates whether the serial port is open | `bool` |
-| `eol_delimiter` | defines the end-of-line separator for line reading | `int` |
-| `total_rx`      | stores the total bytes received | `int` |
-| `total_tx`      | stores the total bytes transmitted | `int` |
+| attribute | description | expected type | default value |
+| :-------- | :---------- | :------------ | :------------ |
+| `is_open`       | Indicates whether the serial port is open | `bool` | False |
+| `eol_delimiter` | defines the end-of-line separator for line reading | `str` | \n |
+| `total_rx`      | stores the total bytes received | `int` | 0 |
+| `total_tx`      | stores the total bytes transmitted | `int` | 0 |
 
 
 <br>
 
 
 ### SerialDeviceHandler.execute()
 Use the `execute()` function to run a command.
 
 Syntax:
 
 ```python
-device.execute(command, pseudo, stdout)
+device.execute(command, <optional arguments>)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
 | `command` | Defines the command to be executed | `str` | n/a |
-| `pseudo`  | Execute as a pseudo command. No command is executed. Use it to capture bootups, etc. | `bool` | False |
 | `stdout`  | Live output while the command is running | `bool` | False |
+| `read_only` | read only execution | bool | False
+| `write_only` | write only execution | bool | False
 
 
 <br>
 
 
 ## Summary
```

#### html2text {}

```diff
@@ -6,28 +6,28 @@
 ## Example ```python from serialdevicehandler import * device =
 serialdevicehandler(port="COM10", baudrate="115200") output = device.execute
 ("help") print(output) ```
 ## SerialDeviceHandler() `SerialDeviceHandler()` is the core class within the
 library. Syntax: ```python device = SerialDeviceHandler(port, baudrate,
 timeout) ``` | argument | description | expected type | default value | | :----
 --- | :---------- | :------------ | :------------ | | `port` | Specifies the
-device port | `str` | Windows: `COM1` Linux: `/dev/tty` | | `baudrate` |
-Specifies the device baudrate | `str` | 9600 | | `timeout` | Specifies the
-command timeout | `int` | 0.2s | There are some attributes for statistical and
-other purposes. | attribute | description | expected type | | :-------- | :----
------- | :------------ | | `is_open` | Indicates whether the serial port is
-open | `bool` | | `eol_delimiter` | defines the end-of-line separator for line
-reading | `int` | | `total_rx` | stores the total bytes received | `int` | |
-`total_tx` | stores the total bytes transmitted | `int` |
+device port | `str` | COM1 | | `baudrate` | Specifies the device baudrate |
+`str` | 9600 | | `timeout` | Specifies the command timeout | `int` | 0.2s |
+There are some attributes for statistical and other purposes. | attribute |
+description | expected type | default value | | :-------- | :---------- | :----
+-------- | :------------ | | `is_open` | Indicates whether the serial port is
+open | `bool` | False | | `eol_delimiter` | defines the end-of-line separator
+for line reading | `str` | \n | | `total_rx` | stores the total bytes received
+| `int` | 0 | | `total_tx` | stores the total bytes transmitted | `int` | 0 |
 ### SerialDeviceHandler.execute() Use the `execute()` function to run a
-command. Syntax: ```python device.execute(command, pseudo, stdout) ``` |
-argument | description | expected type | default value | | :------- | :--------
--- | :------------ | :------------ | | `command` | Defines the command to be
-executed | `str` | n/a | | `pseudo` | Execute as a pseudo command. No command
-is executed. Use it to capture bootups, etc. | `bool` | False | | `stdout` |
-Live output while the command is running | `bool` | False |
+command. Syntax: ```python device.execute(command, ) ``` | argument |
+description | expected type | default value | | :------- | :---------- | :-----
+------- | :------------ | | `command` | Defines the command to be executed |
+`str` | n/a | | `stdout` | Live output while the command is running | `bool` |
+False | | `read_only` | read only execution | bool | False | `write_only` |
+write only execution | bool | False
 ## Summary - SerialDeviceHandler() - _execute()_  [shields-pypi_version]:
 https://img.shields.io/pypi/v/
 serialdevicehandler?label=PyPi%20Version&style=for-the-badge [shields-issues]:
 https://img.shields.io/github/issues/Salliii/serialdevicehandler?style=for-the-
 badge  [url-pypi_version]: https://pypi.org/project/serialdevicehandler/ [url-
 issues]: https://github.com/Salliii/serialdevicehandler/issues
```

### Comparing `serialdevicehandler-1.0.0/serialdevicehandler/main.py` & `serialdevicehandler-1.0.1/serialdevicehandler/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import serial
 import os
 
 
 class SerialDeviceHandler(object):
-    def __init__(self, port=None, baudrate=None, timeout=None) -> None:
+    def __init__(self, port="COM1", baudrate="9600", timeout=0.2) -> None:
 
         self.serial_interface = serial.Serial()
-        self.serial_interface.port = str( port if port != None else ("COM1" if os.name == "nt" else "/dev/tty") )
-        self.serial_interface.baudrate = str( baudrate if baudrate != None else "9600" )
-        self.serial_interface.timeout = float( max(timeout, 0.2) if timeout != None else 0.2 )
+        self.serial_interface.port = port
+        self.serial_interface.baudrate = baudrate
+        self.serial_interface.timeout = max(timeout, 0.2)
 
         self.buffer = str()
         self.is_open = bool()
         self.is_executing = bool()
         self.eol_delimiter = str("\n")
 
         self.total_rx = int(0)
@@ -87,15 +87,15 @@
             # add to linebuffer
             linebuffer += byte_in
             self.total_rx += len(byte_in)
 
         return linebuffer
     
 
-    def __read__(self, stdout: bool) -> str:
+    def __read__(self, live_out: bool) -> str:
         """ get serial response, process and return it """
 
         last_chance = False
 
         # repeat reading until it finishes correctly
         while self.is_executing:
 
@@ -123,39 +123,44 @@
                     self.is_executing = False
 
                     # process buffer
                     buffer = self.__process_buffer__()
                     return buffer
 
                 # print out
-                if stdout:
+                if live_out:
                     print(line_in.decode("unicode-escape"), end="")
     
 
-    def execute(self, command: str, pseudo=False, stdout=False) -> str:
+    def execute(self, command: str, live_out=False, write_only=False, read_only=False) -> str:
         """ executes the given command and returns the serial response """
 
+        output = None
+
         # open port
         self.__open__()
 
         # set executing state
         self.is_executing = True
 
         # repeat the same command until it finishes correctly. Prevents the command from getting lost, when there is no available device
         while self.is_executing:
 
             # write command
-            if not pseudo:
+            if not read_only:
                 for char in command:
                     self.serial_interface.write(str(char).encode())
                     self.total_tx += len(char)
-            
+                    if write_only:
+                        self.is_executing = False
+
             # execute
             self.serial_interface.write("\n".encode())
             self.total_tx += 1
 
             # start reading
-            output = self.__read__(stdout)
+            if not write_only:
+                output = self.__read__(live_out)
         
         # close port
         self.__close__()
-        return output
+        return output
```

### Comparing `serialdevicehandler-1.0.0/serialdevicehandler.egg-info/PKG-INFO` & `serialdevicehandler-1.0.1/serialdevicehandler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdevicehandler
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library to run commands on a device via serial port
 Home-page: https://github.com/Salliii/serialdevicehandler
 Author: Salliii
 Keywords: python,library,serial device,serial interface,commands,execute
 Description-Content-Type: text/markdown
 
 # Serial Device Handler
@@ -52,45 +52,46 @@
 
 ```python
 device = SerialDeviceHandler(port, baudrate, timeout)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
-| `port`      | Specifies the device port | `str` | Windows: `COM1`  Linux: `/dev/tty` |
+| `port`      | Specifies the device port | `str` | COM1 |
 | `baudrate`  | Specifies the device baudrate | `str` | 9600 |
 | `timeout`   | Specifies the command timeout | `int` | 0.2s |
 
 There are some attributes for statistical and other purposes.
 
-| attribute | description | expected type |
-| :-------- | :---------- | :------------ |
-| `is_open`       | Indicates whether the serial port is open | `bool` |
-| `eol_delimiter` | defines the end-of-line separator for line reading | `int` |
-| `total_rx`      | stores the total bytes received | `int` |
-| `total_tx`      | stores the total bytes transmitted | `int` |
+| attribute | description | expected type | default value |
+| :-------- | :---------- | :------------ | :------------ |
+| `is_open`       | Indicates whether the serial port is open | `bool` | False |
+| `eol_delimiter` | defines the end-of-line separator for line reading | `str` | \n |
+| `total_rx`      | stores the total bytes received | `int` | 0 |
+| `total_tx`      | stores the total bytes transmitted | `int` | 0 |
 
 
 <br>
 
 
 ### SerialDeviceHandler.execute()
 Use the `execute()` function to run a command.
 
 Syntax:
 
 ```python
-device.execute(command, pseudo, stdout)
+device.execute(command, <optional arguments>)
 ```
 
 | argument | description | expected type | default value |
 | :------- | :---------- | :------------ | :------------ |
 | `command` | Defines the command to be executed | `str` | n/a |
-| `pseudo`  | Execute as a pseudo command. No command is executed. Use it to capture bootups, etc. | `bool` | False |
 | `stdout`  | Live output while the command is running | `bool` | False |
+| `read_only` | read only execution | bool | False
+| `write_only` | write only execution | bool | False
 
 
 <br>
 
 
 ## Summary
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: serialdevicehandler Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: serialdevicehandler Version: 1.0.1 Summary: A
 python library to run commands on a device via serial port Home-page: https://
 github.com/Salliii/serialdevicehandler Author: Salliii Keywords:
 python,library,serial device,serial interface,commands,execute Description-
 Content-Type: text/markdown # Serial Device Handler [![PyPi version][shields-
 pypi_version]][url-pypi_version] [![Github Issues][shields-issues]][url-issues]
 Execute commands on a device via serial port.
 ## Installing Install using pip ```bash pip install serialdevicehandler ``` or
@@ -10,28 +10,28 @@
 ## Example ```python from serialdevicehandler import * device =
 serialdevicehandler(port="COM10", baudrate="115200") output = device.execute
 ("help") print(output) ```
 ## SerialDeviceHandler() `SerialDeviceHandler()` is the core class within the
 library. Syntax: ```python device = SerialDeviceHandler(port, baudrate,
 timeout) ``` | argument | description | expected type | default value | | :----
 --- | :---------- | :------------ | :------------ | | `port` | Specifies the
-device port | `str` | Windows: `COM1` Linux: `/dev/tty` | | `baudrate` |
-Specifies the device baudrate | `str` | 9600 | | `timeout` | Specifies the
-command timeout | `int` | 0.2s | There are some attributes for statistical and
-other purposes. | attribute | description | expected type | | :-------- | :----
------- | :------------ | | `is_open` | Indicates whether the serial port is
-open | `bool` | | `eol_delimiter` | defines the end-of-line separator for line
-reading | `int` | | `total_rx` | stores the total bytes received | `int` | |
-`total_tx` | stores the total bytes transmitted | `int` |
+device port | `str` | COM1 | | `baudrate` | Specifies the device baudrate |
+`str` | 9600 | | `timeout` | Specifies the command timeout | `int` | 0.2s |
+There are some attributes for statistical and other purposes. | attribute |
+description | expected type | default value | | :-------- | :---------- | :----
+-------- | :------------ | | `is_open` | Indicates whether the serial port is
+open | `bool` | False | | `eol_delimiter` | defines the end-of-line separator
+for line reading | `str` | \n | | `total_rx` | stores the total bytes received
+| `int` | 0 | | `total_tx` | stores the total bytes transmitted | `int` | 0 |
 ### SerialDeviceHandler.execute() Use the `execute()` function to run a
-command. Syntax: ```python device.execute(command, pseudo, stdout) ``` |
-argument | description | expected type | default value | | :------- | :--------
--- | :------------ | :------------ | | `command` | Defines the command to be
-executed | `str` | n/a | | `pseudo` | Execute as a pseudo command. No command
-is executed. Use it to capture bootups, etc. | `bool` | False | | `stdout` |
-Live output while the command is running | `bool` | False |
+command. Syntax: ```python device.execute(command, ) ``` | argument |
+description | expected type | default value | | :------- | :---------- | :-----
+------- | :------------ | | `command` | Defines the command to be executed |
+`str` | n/a | | `stdout` | Live output while the command is running | `bool` |
+False | | `read_only` | read only execution | bool | False | `write_only` |
+write only execution | bool | False
 ## Summary - SerialDeviceHandler() - _execute()_  [shields-pypi_version]:
 https://img.shields.io/pypi/v/
 serialdevicehandler?label=PyPi%20Version&style=for-the-badge [shields-issues]:
 https://img.shields.io/github/issues/Salliii/serialdevicehandler?style=for-the-
 badge  [url-pypi_version]: https://pypi.org/project/serialdevicehandler/ [url-
 issues]: https://github.com/Salliii/serialdevicehandler/issues
```

### Comparing `serialdevicehandler-1.0.0/setup.py` & `serialdevicehandler-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 with open("README.md", "r", encoding="utf-8") as readme:
     DESC_LONG = readme.read()
 
 
 setuptools.setup(
     name="serialdevicehandler",
@@ -22,9 +22,9 @@
 
 
 """
     Setup:
     python .\setup.py sdist bdist_wheel
 
     Upload to PyPi:
-    twine upload .\dist\*
+    twine upload .\dist\<packname>-<version>
 """
```

