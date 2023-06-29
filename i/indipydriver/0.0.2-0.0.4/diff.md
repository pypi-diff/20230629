# Comparing `tmp/indipydriver-0.0.2.tar.gz` & `tmp/indipydriver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-0.0.2.tar", last modified: Sat Jun 17 14:39:26 2023, max compression
+gzip compressed data, was "indipydriver-0.0.4.tar", last modified: Thu Jun 29 13:38:39 2023, max compression
```

## Comparing `indipydriver-0.0.2.tar` & `indipydriver-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.2/LICENSE
--rw-r--r--   0        0        0     2920 2023-06-16 07:51:30.000000 indipydriver-0.0.2/README.md
--rw-r--r--   0        0        0      541 2023-06-17 10:50:26.000000 indipydriver-0.0.2/indipydriver/__init__.py
--rw-r--r--   0        0        0     9886 2023-06-17 14:09:12.000000 indipydriver-0.0.2/indipydriver/comms.py
--rw-r--r--   0        0        0    20935 2023-06-12 18:46:59.000000 indipydriver-0.0.2/indipydriver/events.py
--rw-r--r--   0        0        0    20127 2023-06-16 08:13:04.000000 indipydriver-0.0.2/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    10454 2023-06-09 10:54:36.000000 indipydriver-0.0.2/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    41836 2023-06-10 14:51:56.000000 indipydriver-0.0.2/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-06-17 14:38:33.370278 indipydriver-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 indipydriver-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2261 2023-06-17 14:59:33.000000 indipydriver-0.0.4/README.md
+-rw-r--r--   0        0        0      541 2023-06-29 09:54:28.000000 indipydriver-0.0.4/indipydriver/__init__.py
+-rw-r--r--   0        0        0    12223 2023-06-25 17:20:07.000000 indipydriver-0.0.4/indipydriver/comms.py
+-rw-r--r--   0        0        0    20935 2023-06-12 18:46:59.000000 indipydriver-0.0.4/indipydriver/events.py
+-rw-r--r--   0        0        0    20634 2023-06-29 09:38:24.000000 indipydriver-0.0.4/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    11134 2023-06-23 22:47:31.000000 indipydriver-0.0.4/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    42856 2023-06-29 09:25:28.000000 indipydriver-0.0.4/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-06-29 09:53:53.000000 indipydriver-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 indipydriver-0.0.4/PKG-INFO
```

### Comparing `indipydriver-0.0.2/LICENSE` & `indipydriver-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.2/README.md` & `indipydriver-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,24 +20,16 @@
 
 This is called whenever data is received, the event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to poll your instruments, and if required send updates to the client.
 
-Having created your IPyDriver subclass, you would create member objects, being instances of SwitchMember, LightMember, TextMember, BLOBMember or NumberMember which provide attribute values to control your instrument.
-
-You would then create vector objects, being instances of SwitchVector, LightVector, TextVector, BLOBVector or NumberVector these containing the appropriate member objects.
-
-You would then create one or more 'Device' instances, containing the vector objects.
-
-And finally you would create an instance of your IPyDriver subclass, which in turn is set with the Devices.
-
 Finally you would run the driver asyncrun() method which runs the driver, typically called using:
 
 asyncio.run(driver.asyncrun())
 
 The driver can transmit/receive either by stdin/stdout, or by a port, typically localhost:7624 which is the INDI port number, and to which a client typically connects. If this is the only driver on the network, then the 'indiserver' (debian package indi-bin) software - which connects multiple drivers to a port - is not needed.
 
-An INDI web client is available on Pypi as project indiredis, and can connect to port 7624, and display the instrument controls.
-
 Documentation at https://indipydriver.readthedocs.io
+
+Installation from https://pypi.org/project/indipydriver
```

### Comparing `indipydriver-0.0.2/indipydriver/__init__.py` & `indipydriver-0.0.4/indipydriver/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 
 
-version = "0.0.2"
+version = "0.0.4"
```

### Comparing `indipydriver-0.0.2/indipydriver/comms.py` & `indipydriver-0.0.4/indipydriver/comms.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import xml.etree.ElementTree as ET
 
 import fcntl
 
 from datetime import datetime
 
+from base64 import standard_b64encode
+
 
 # All xml data received from the client, or from snooped devices should be contained in one of the following tags
 TAGS = (b'getProperties',
         b'newTextVector',
         b'newNumberVector',
         b'newSwitchVector',
         b'newBLOBVector',
@@ -36,28 +38,78 @@
 
 
 # _ENDTAGS is a tuple of ( b'</defTextVector>', ...  ) data received will be tested to end with such an endtag
 _ENDTAGS = tuple(b'</' + tag + b'>' for tag in TAGS)
 
 
 
+def _makestart(element):
+    "Given an xml element, returns a string of its start, including < tag attributes >"
+    attriblist = ["<", element.tag]
+    for key,value in element.attrib.items():
+        attriblist.append(f" {key}=\"{value}\"")
+    attriblist.append(">")
+    return "".join(attriblist)
+
+
+def blob_xml_bytes(xmldata):
+    """A generator yielding blob xml byte strings
+       for a setBLOBVector.
+       reads member files, b64 encodes the data
+       closes the files, and yields the binary
+       string including tags."""
+
+    # yield initial setBLOBVector
+    setblobvector = _makestart(xmldata)
+    yield setblobvector.encode()
+
+    for oneblob in xmldata.iter('oneBLOB'):
+        # get the filepointer
+        fp = oneblob.text
+        # set seek(0) so is read from start of file
+        fp.seek(0)
+        bytescontent = fp.read()
+        fp.close()
+        if bytescontent == b"":
+            continue
+        size = oneblob.get("size")
+        if size == "0":
+            oneblob.set("size", str(len(bytescontent)))
+        # yield start of oneblob
+        start = _makestart(oneblob)
+        yield start.encode()
+        # yield body, b64 encoded
+        yield standard_b64encode(bytescontent)
+        yield b"</oneBLOB>"
+    yield b"</setBLOBVector>\n"
+
+
 class STDOUT_TX:
     "An object that transmits data on stdout, used by STDINOUT as one half of the communications path"
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on stdout"""
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit down stdout
             txdata = await writerque.get()
-            # and send it out on stdout
-            binarydata = ET.tostring(txdata)
-            binarydata += b"\n"
-            sys.stdout.buffer.write(binarydata)
-            sys.stdout.buffer.flush()
+            if (txdata.tag == "setBLOBVector") and len(txdata):
+                # txdata is a setBLOBVector containing blobs
+                # the generator blob_xml_bytes yields bytes
+                for binarydata in blob_xml_bytes(txdata):
+                    # transmit the data
+                    sys.stdout.buffer.write(binarydata)
+                    sys.stdout.buffer.flush()
+                    await asyncio.sleep(0)
+            else:
+                # its straight xml, send it out on stdout
+                binarydata = ET.tostring(txdata)
+                binarydata += b"\n"
+                sys.stdout.buffer.write(binarydata)
+                sys.stdout.buffer.flush()
             writerque.task_done()
 
 class STDIN_RX:
     """An object that receives data, parses it to ElementTree elements
        and passes it to the driver by appending it to the driver's readerque"""
 
     async def run_rx(self, readerque):
@@ -180,22 +232,32 @@
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
     def __init__(self, writer):
         self.writer = writer
 
     async def run_tx(self, writerque):
-        """gets data from writerque, and transmits it"""
+        """Gets data from writerque, and transmits it out on stdout"""
         while True:
             await asyncio.sleep(0)
+            # get block of data from writerque and transmit down stdout
             txdata = await writerque.get()
-            binarydata = ET.tostring(txdata)
-            # Send the next message to the port
-            self.writer.write(binarydata)
-            await self.writer.drain()
+            if txdata.tag == "setBLOBVector" and len(txdata):
+                # txdata is a setBLOBVector containing blobs
+                # the generator blob_xml_bytes yields bytes
+                for binarydata in blob_xml_bytes(txdata):
+                    # Send to the port
+                    self.writer.write(binarydata)
+                    await self.writer.drain()
+            else:
+                # its straight xml, send it out on the port
+                binarydata = ET.tostring(txdata)
+                # Send to the port
+                self.writer.write(binarydata)
+                await self.writer.drain()
             writerque.task_done()
 
 
 
 class Port_RX(STDIN_RX):
     """Produces xml.etree.ElementTree data from data received on the port,
        this is used by Portcomms as one half of the communications path.
```

### Comparing `indipydriver-0.0.2/indipydriver/events.py` & `indipydriver-0.0.4/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.2/indipydriver/ipydriver.py` & `indipydriver-0.0.4/indipydriver/ipydriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,16 +96,22 @@
         self.snoopque = asyncio.Queue(4)
         # data for each device is passed to each device dataque
 
         # An object for communicating can be set, if not set, then
         # self.comms = STDINOUT() will be set in the asyncrun call
         self.comms = None
 
+
+    def _reporterror(self, message):
+        "Prints message to stderr"
+        print(message, file=sys.stderr)
+
     def listen(self, host="localhost", port=7624):
-        "If called, listens on the given host/port"
+        """If called, listens on the given host and port. Only one connection is accepted,
+           further connection attempts while a client is already connected will be refused."""
         if not self.comms is None:
              raise RuntimeError("A communications method has already been set, there can only be one")
         self.comms = Portcomms(host, port)
 
     def __setitem__(self, devicename):
         raise KeyError
 
@@ -158,15 +164,15 @@
             await asyncio.sleep(0)
             root = await self.snoopque.get()
             devicename = root.get("device")
             if devicename is not None:
                 # if a device name is given, check
                 # it is not in this drivers devices
                 if devicename in self.devices:
-                    # cannnot snoop on self!!
+                    self._reporterror("Cannot snoop on a device already controlled by this driver")
                     self.snoopque.task_done()
                     continue
             try:
                 if root.tag == "message":
                     # create event
                     event = events.message(root)
                     await self.snoopevent(event)
@@ -221,15 +227,16 @@
             self.snoopque.task_done()
 
     async def send_message(self, message="", timestamp=None):
         "Send system wide message - without device name"
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp given in send_message must be a datetime.datetime object")
+            self._reporterror("The timestamp given in send_message must be a datetime.datetime object")
+            return
         xmldata = ET.Element('message')
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
         await self.writerque.put(xmldata)
 
@@ -238,15 +245,16 @@
            on the network, if devicename given, it must not be a device of this driver as
            the point of this is to snoop on remote devices."""
         xmldata = ET.Element('getProperties')
         if devicename is None:
             await self.writerque.put(xmldata)
             return
         if devicename in self.devices:
-            raise ValueError("Cannot snoop on a device already belonging to this driver")
+            self._reporterror("Cannot snoop on a device already controlled by this driver")
+            return
         xmldata.set("device", devicename)
         if vectorname is None:
             await self.writerque.put(xmldata)
             return
         xmldata.set("name", vectorname)
         await self.writerque.put(xmldata)
 
@@ -337,25 +345,30 @@
             p.devicename = self.devicename
             self.propertyvectors[p.name] = p
 
         self.data = self.propertyvectors
         # self.data is used by UserDict, it is an alias of self.propertyvectors
         # simply because 'propertyvectors' is more descriptive
 
+    def _reporterror(self, message):
+        "Prints message to stderr"
+        print(message, file=sys.stderr)
+
     async def send_device_message(self, message="", timestamp=None):
         """Send a message associated with this device, which the client could display.
            The timestamp should be either None or a datetime.datetime object. If the
            timestamp is None a datetime.datetime.utcnow() value will be inserted."""
         if not self.enable:
             # messages only sent if self.enable is True
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp given in send_message must be a datetime.datetime object")
+            self._reporterror("The timestamp given in send_message must be a datetime.datetime object")
+            return
         xmldata = ET.Element('message')
         xmldata.set("device", self.devicename)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
         await self.driver.writerque.put(xmldata)
@@ -367,15 +380,16 @@
            Setting device.enable to True re-enables communications.
            The message argument is any appropriate string which the client could display to the user.
            The timestamp should be either None or a datetime.datetime object. If the timestamp is None
            a datetime.datetime.utcnow() value will be inserted."""
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("The timestamp given in send_delProperty must be a datetime.datetime object")
+            self._reporterror("The timestamp given in send_delProperty must be a datetime.datetime object")
+            return
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
         await self.driver.writerque.put(xmldata)
```

### Comparing `indipydriver-0.0.2/indipydriver/propertymembers.py` & `indipydriver-0.0.4/indipydriver/propertymembers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
-import collections
-
-import asyncio
+import collections, io, asyncio
 
 from datetime import datetime
 
 import xml.etree.ElementTree as ET
 
-from base64 import standard_b64encode
 
 class PropertyMember:
     "Parent class of SwitchMember etc"
 
     def __init__(self, name, label=None):
         self.name = name
         if label:
@@ -39,14 +36,16 @@
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
+        if not value:
+            raise ValueError(f"The SwitchMember {self.name} value cannot be empty")
         newvalue = self.checkvalue(value, ['On', 'Off'])
         if self._membervalue != newvalue:
             # when a value has changed, set the changed flag
             self.changed = True
             self._membervalue = newvalue
 
     def defswitch(self):
@@ -74,14 +73,16 @@
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
+        if not value:
+            raise ValueError(f"The LightMember {self.name} value cannot be empty")
         newvalue = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         if self._membervalue != newvalue:
             # when a value has changed, set the changed flag
             self.changed = True
             self._membervalue = newvalue
 
     def deflight(self):
@@ -173,15 +174,17 @@
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         if not isinstance(value, str):
-            raise ValueError("The given number value must be a string object")
+            raise ValueError("The NumberMember {self.name} value must be a string object")
+        if not value:
+            raise ValueError(f"The NumberMember {self.name} value cannot be empty")
         if self._membervalue != value:
             # when a value has changed, set the changed flag
             self.changed = True
             self._membervalue = value
 
     def format_number(self, value):
         """This takes a float, and returns a formatted string
@@ -259,55 +262,66 @@
         xmldata.set("name", self.name)
         xmldata.text = self._membervalue
         return xmldata
 
 
 class BLOBMember(PropertyMember):
     """Contains a 'binary large object' such as an image, the value should be
-       a bytes object.
+       either a bytes object, a file-like object, or a path to a file.
 
        blobsize is the size of the BLOB before any compression, if left at
        zero, the length of the BLOB will be used.
 
        The BLOB format should be a string describing the BLOB, such as .jpeg
     """
 
-    def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=b''):
+    def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=None):
         super().__init__(name, label)
         if not isinstance(blobsize, int):
-            raise ValueError("The given blobsize must be an integer object")
-        if not isinstance(membervalue, bytes):
-            raise ValueError("The given BLOB membervalue must be a bytes object")
+            raise ValueError(f"The BLOBMember {self.name} blobsize must be an integer object")
+        # membervalue can be a byte string, path, string path or file like object
         self._membervalue = membervalue
         self.blobsize = blobsize
         self.blobformat = blobformat
 
+
     @property
     def membervalue(self):
         return self._membervalue
 
+
     @membervalue.setter
     def membervalue(self, value):
-        if not isinstance(value, bytes):
-            raise ValueError("The given BLOB value must be a bytes object")
-        # don't test for equality here since the byte data may be large
-        # just assume setting it implies a change
-        self.changed = True
+        if not value:
+            raise ValueError(f"The BLOBMember {self.name} value cannot be empty")
         self._membervalue = value
 
+
     def defblob(self):
         """Returns a defBlob, does not contain a membervalue"""
         xmldata = ET.Element('defBlob')
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         return xmldata
 
+
     def oneblob(self):
         """Returns xml of a oneBLOB"""
         xmldata = ET.Element('oneBLOB')
         xmldata.set("name", self.name)
-        if not self.blobsize:
-            self.blobsize = len(self._membervalue)
         xmldata.set("size", str(self.blobsize))
         xmldata.set("format", self.blobformat)
-        xmldata.text = standard_b64encode(self._membervalue).decode('ascii')
+        # the value set in the xmldata object should be a file-like object
+        if isinstance(self._membervalue, bytes):
+            xmldata.text = io.BytesIO(self._membervalue)
+        elif hasattr(self._membervalue, "read") and callable(self._membervalue.read):
+            # a file-like object
+            xmldata.text = self._membervalue
+        else:
+            # could be a path to a file
+            try:
+                xmldata.text = open(self._membervalue, "rb")
+            except:
+                raise ValueError(f"The BLOBMember {self.name} value cannot be openned")
+         # old value was
+        # xmldata.text = standard_b64encode(self._membervalue).decode('ascii')
         return xmldata
```

### Comparing `indipydriver-0.0.2/indipydriver/propertyvectors.py` & `indipydriver-0.0.4/indipydriver/propertyvectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import collections, datetime
+import collections, datetime, sys
 
 import asyncio
 
 import xml.etree.ElementTree as ET
 
 from .events import EventException, getProperties, newSwitchVector, newTextVector, newBLOBVector, enableBLOB, newNumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, NumberMember, BLOBMember
@@ -26,14 +26,18 @@
 
         # this will be set when the device is initialised
         self.devicename = None
 
         # this will be set when the driver asyncrun is run
         self.driver = None
 
+    def _reporterror(self, message):
+        "Prints message to stderr"
+        print(message, file=sys.stderr)
+
     @property
     def device(self):
         return self.driver.devices[self.devicename]
 
     async def send_delProperty(self, message="", timestamp=None):
         """Informs the client this vector is not available, it also sets an 'enable' attribute to
            False, which stops any data being transmitted between the client and this property vector.
@@ -43,15 +47,16 @@
            The message argument is any appropriate string which the client could display to the user.
 
            The timestamp should be either None or a datetime.datetime object. If the timestamp is None
            a datetime.datetime.utcnow() value will be inserted."""
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp given in send_delProperty must be a datetime.datetime object")
+            self._reporterror("Aborting sending delProperty: The given send_delProperty timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
@@ -69,22 +74,28 @@
 
     @property
     def state(self):
         return self._state
 
     @state.setter
     def state(self, value):
-        self._state = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
+        try:
+            self._state = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     def send_defVector(self, timestamp=None, timeout=0, message=''):
         "overridden in child classes"
         pass
 
     def __setitem__(self, membername, value):
-        self.data[membername].membervalue = value
+        try:
+            self.data[membername].membervalue = value
+        except ValueError as ex:
+            self._reporterror(ex)
 
     def __getitem__(self, membername):
         return self.data[membername].membervalue
 
 
 class SwitchVector(PropertyVector):
 
@@ -111,23 +122,29 @@
 
     @property
     def perm(self):
         return self._perm
 
     @perm.setter
     def perm(self, value):
-        self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        try:
+            self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     @property
     def rule(self):
         return self._rule
 
     @rule.setter
     def rule(self, value):
-        self._rule = self.checkvalue(value, ['OneOfMany','AtMostOne','AnyOfMany'])
+        try:
+            self._rule = self.checkvalue(value, ['OneOfMany','AtMostOne','AnyOfMany'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -153,23 +170,25 @@
            timestamp should be a datetime.datetime object or None, in which
            case a datetime.datetime.utcnow() value will be inserted.
 
            The timeout value should be '0' if not used, or a string of a
            numeric value indicating to the client how long this data is valid.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending defSwitchVector: The given send_defVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending defSwitchVector: The given send_defVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('defSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
         xmldata.set("perm", self.perm)
@@ -203,23 +222,25 @@
 
            If allvalues is False, only values that have changed will be sent, saving bandwidth.
            If no values have changed, the vector will not be sent, if you need to ensure the
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setSwitchVector: The given send_setVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setSwitchVector: The given send_setVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -254,23 +275,25 @@
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setSwitchVector: The given send_setVectorMembers timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setSwitchVector: The given send_setVectorMembers timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -337,15 +360,16 @@
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending defLightVector: The given send_defVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('defLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
@@ -383,15 +407,16 @@
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setLightVector: The given send_setVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
@@ -421,15 +446,16 @@
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setLightVector: The given send_setVectorMembers timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
@@ -457,15 +483,18 @@
 
     @property
     def perm(self):
         return self._perm
 
     @perm.setter
     def perm(self, value):
-        self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        try:
+            self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -490,23 +519,25 @@
            timestamp should be a datetime.datetime object or None, in which
            case a datetime.datetime.utcnow() value will be inserted.
 
            The timeout value should be '0' if not used, or a string value
            indicating to the client how long this data is valid.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending defTextVector: The given send_defVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending defTextVector: The given send_defVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('defTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
         xmldata.set("perm", self.perm)
@@ -539,23 +570,25 @@
 
            If allvalues is False, only values that have changed will be sent, saving bandwidth.
            If no values have changed, the vector will not be sent, if you need to ensure the
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setTextVector: The given send_setVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setTextVector: The given send_setVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -579,23 +612,25 @@
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setTextVector: The given send_setVectorMembers timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setTextVector: The given send_setVectorMembers timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -621,15 +656,18 @@
 
     @property
     def perm(self):
         return self._perm
 
     @perm.setter
     def perm(self, value):
-        self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        try:
+            self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -654,23 +692,25 @@
            timestamp should be a datetime.datetime object or None, in which
            case a datetime.datetime.utcnow() value will be inserted.
 
            The timeout value should be '0' if not used, or a string value
            indicating to the client how long this data is valid.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending defNumberVector: The given send_defVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending defNumberVector: The given send_defVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('defNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
         xmldata.set("perm", self.perm)
@@ -703,23 +743,25 @@
 
            If allvalues is False, only values that have changed will be sent, saving bandwidth.
            If no values have changed, the vector will not be sent, if you need to ensure the
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setNumberVector: The given send_setVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setNumberVector: The given send_setVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -743,23 +785,25 @@
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setNumberVector: The given send_setVectorMembers timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setNumberVector: The given send_setVectorMembers timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
@@ -776,24 +820,42 @@
 
     def __init__(self, name, label, group, perm, state, blobmembers):
         super().__init__(name, label, group, state)
         self.perm = perm
         # self.data is a dictionary of blob name : blobmember
         for blob in blobmembers:
             if not isinstance(blob, BLOBMember):
+                self._reporterror("Members of a BLOBVector must all be BLOBMembers")
                 raise TypeError("Members of a BLOBVector must all be BLOBMembers")
             self.data[blob.name] = blob
 
+    def set_blobsize(self, membername, blobsize):
+        """Sets the size attribute in the blob member. If the default of zero is used,
+           the size will be set to the number of bytes in the BLOB. The INDI standard
+           specifies the size should be that of the BLOB before any compression,
+           therefore if you are sending a compressed file, you should set the blobsize
+           prior to compression with this method."""
+        if not isinstance(blobsize, int):
+            self._reporterror("blobsize rejected, must be an integer object")
+            return
+        member = self.data.get[membername]
+        if not member:
+            return
+        member.blobsize = blobsize
+
     @property
     def perm(self):
         return self._perm
 
     @perm.setter
     def perm(self, value):
-        self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        try:
+            self._perm = self.checkvalue(value, ['ro','wo','rw'])
+        except ValueError as ex:
+            self._reporterror(ex)
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -822,119 +884,73 @@
            timestamp should be a datetime.datetime object or None, in which
            case a datetime.datetime.utcnow() value will be inserted.
 
            The timeout value should be '0' if not used, or a string value
            indicating to the client how long this data is valid.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending defBLOBVector: The given send_defVector timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending defBLOBVector: The given send_defVector timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('defBLOBVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
         xmldata.set("perm", self.perm)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
             xmldata.append(blob.defblob())
-            # after a defblob sent, assume new client connection, and set all members as changed
-            # so they will all be included in the first 'send_setVector'
-            blob.changed = True
         await self.driver.writerque.put(xmldata)
 
-    async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
-        """Transmits the vector (setBLOBVector) and members with their values to the client.
-           Typically the vector 'state' should be set, and any changed member value prior to
-           transmission.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which case a
-           datetime.datetime.utcnow() value will be inserted.
-
-           The timeout value should be '0' if not used, or a string value
-           indicating to the client how long this data is valid.
-
-           If allvalues is True, all values are sent.
-
-           If allvalues is False, only values that have changed will be sent, saving bandwidth.
-           If no values have changed, the vector will not be sent, if you need to ensure the
-           vector message, state or time values are sent to the client, then use the more
-           explicit send_setVectorMembers method instead.
-        """
-        if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
-        if not self.device.enable:
-            return
-        if not self.enable:
-            return
-        if not timestamp:
-            timestamp = datetime.datetime.utcnow()
-        if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
-        xmldata = ET.Element('setBLOBVector')
-        xmldata.set("device", self.devicename)
-        xmldata.set("name", self.name)
-        xmldata.set("state", self.state)
-        # note - limit timestamp characters to :21 to avoid long fractions of a second
-        xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
-        xmldata.set("timeout", timeout)
-        if message:
-            xmldata.set("message", message)
-        # set a flag to test if at least one member is included
-        membersincluded = False
-        for blob in self.data.values():
-            # only send member if its value has changed or if allvalues is True
-            if allvalues or blob.changed:
-                xmldata.append(blob.oneblob())
-                blob.changed = False
-                membersincluded = True
-        if membersincluded:
-            # only send xmldata if a member is included in the vector
-            await self.driver.writerque.put(xmldata)
+    # NOTE: BLOBVectors do not have a send_setVector method
+    #       only the more explicit send_setVectorMembers is available
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setBLOBVector) and members with their values to the client.
-           Similar to the send_setVector method however the members list specifies the
-           member names which will have their values sent.
+           The members list specifies the member names which will have their values sent.
 
-           This allows members to be explicitly specified. If the members list is empty
-           then a vector will still be sent, empty of members, which may be required if
-           just a state or message is to be sent.
+           Members contain either a bytes string, a file-like object, or a path to a file. If
+           a file-like object is given, it's close() method will automatically be called after
+           the BLOB is sent, so you do not have to close it.
         """
         if not isinstance(timeout, str):
-            raise ValueError("The given timeout value must be a string object")
+            self._reporterror("Aborting sending setBLOBVector: The given send_setVectorMembers timeout value must be a string object")
+            return
         if not self.device.enable:
             return
         if not self.enable:
             return
         if not timestamp:
             timestamp = datetime.datetime.utcnow()
         if not isinstance(timestamp, datetime.datetime):
-            raise TypeError("timestamp must be a datetime.datetime object")
+            self._reporterror("Aborting sending setBLOBVector: The given send_setVectorMembers timestamp must be a datetime.datetime object")
+            return
         xmldata = ET.Element('setBLOBVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
-            if blob.name in members:
-                xmldata.append(blob.oneblob())
-                blob.changed = False
+            if (blob.name in members) and (blob.membervalue is not None):
+                try:
+                    xmldata.append(blob.oneblob())
+                except ValueError as ex:
+                    self._reporterror(ex)
         await self.driver.writerque.put(xmldata)
```

### Comparing `indipydriver-0.0.2/pyproject.toml` & `indipydriver-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.2"
+version = "0.0.4"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-0.0.2/PKG-INFO` & `indipydriver-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 0.0.2
+Version: 0.0.4
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -35,25 +35,17 @@
 
 This is called whenever data is received, the event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to poll your instruments, and if required send updates to the client.
 
-Having created your IPyDriver subclass, you would create member objects, being instances of SwitchMember, LightMember, TextMember, BLOBMember or NumberMember which provide attribute values to control your instrument.
-
-You would then create vector objects, being instances of SwitchVector, LightVector, TextVector, BLOBVector or NumberVector these containing the appropriate member objects.
-
-You would then create one or more 'Device' instances, containing the vector objects.
-
-And finally you would create an instance of your IPyDriver subclass, which in turn is set with the Devices.
-
 Finally you would run the driver asyncrun() method which runs the driver, typically called using:
 
 asyncio.run(driver.asyncrun())
 
 The driver can transmit/receive either by stdin/stdout, or by a port, typically localhost:7624 which is the INDI port number, and to which a client typically connects. If this is the only driver on the network, then the 'indiserver' (debian package indi-bin) software - which connects multiple drivers to a port - is not needed.
 
-An INDI web client is available on Pypi as project indiredis, and can connect to port 7624, and display the instrument controls.
-
 Documentation at https://indipydriver.readthedocs.io
 
+Installation from https://pypi.org/project/indipydriver
+
```

