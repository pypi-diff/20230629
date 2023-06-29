# Comparing `tmp/sac_tello-0.0.5.tar.gz` & `tmp/sac_tello-0.0.6.tar.gz`

## Comparing `sac_tello-0.0.5.tar` & `sac_tello-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/SAC-Tello.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/dictionaries/Michael.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/__init__.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/face_recognizer.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/rc_tello.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_cmd.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_drive.py
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_drone.py
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_hud.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_state.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.5/sac_tello/tello_video.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.5/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.5/LICENSE
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 sac_tello-0.0.5/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    44509 2020-02-02 00:00:00.000000 sac_tello-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/SAC-Tello.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/dictionaries/Michael.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/__init__.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/face_recognizer.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_cmd.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_drive.py
+-rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_drone.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_hud.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_rc.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_remote.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_state.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_video.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 sac_tello-0.0.6/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    46029 2020-02-02 00:00:00.000000 sac_tello-0.0.6/PKG-INFO
```

### Comparing `sac_tello-0.0.5/.idea/workspace.xml` & `sac_tello-0.0.6/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `sac_tello-0.0.5/.idea/workspace.xml` & `sac_tello-0.0.6/.idea/workspace.xml`

```diff
@@ -1,15 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="README update">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/sac_tello/tello_drive.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_drive.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/sac_tello/tello_hud.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_hud.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -18,15 +15,15 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
-        <entry key="$PROJECT_DIR$" value="mp-tello"/>
+        <entry key="$PROJECT_DIR$" value="main"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
@@ -193,15 +190,50 @@
     <task id="LOCAL-00019" summary="README update">
       <created>1688003293573</created>
       <option name="number" value="00019"/>
       <option name="presentableId" value="LOCAL-00019"/>
       <option name="project" value="LOCAL"/>
       <updated>1688003293573</updated>
     </task>
-    <option name="localTasksCounter" value="20"/>
+    <task id="LOCAL-00020" summary="UI updates">
+      <created>1688013354096</created>
+      <option name="number" value="00020"/>
+      <option name="presentableId" value="LOCAL-00020"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688013354096</updated>
+    </task>
+    <task id="LOCAL-00021" summary="Basic copy-paster setup.">
+      <created>1688014787024</created>
+      <option name="number" value="00021"/>
+      <option name="presentableId" value="LOCAL-00021"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688014787024</updated>
+    </task>
+    <task id="LOCAL-00022" summary="Minor corrections before sleep.">
+      <created>1688014960415</created>
+      <option name="number" value="00022"/>
+      <option name="presentableId" value="LOCAL-00022"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688014960415</updated>
+    </task>
+    <task id="LOCAL-00023" summary="RC Tello now working. Framerate not great.">
+      <created>1688048526679</created>
+      <option name="number" value="00023"/>
+      <option name="presentableId" value="LOCAL-00023"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688048526679</updated>
+    </task>
+    <task id="LOCAL-00024" summary="README update">
+      <created>1688049506792</created>
+      <option name="number" value="00024"/>
+      <option name="presentableId" value="LOCAL-00024"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688049506792</updated>
+    </task>
+    <option name="localTasksCounter" value="25"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -226,11 +258,15 @@
     <MESSAGE value="Basic Tello state receiver and logger."/>
     <MESSAGE value="Basic Tello video frame receiver."/>
     <MESSAGE value="Basic outline and code for multiprocessed tello drone. Testing Needed."/>
     <MESSAGE value="Tested and working."/>
     <MESSAGE value="Added optional heads-up-display."/>
     <MESSAGE value="Package stuff"/>
     <MESSAGE value="Reorg"/>
+    <MESSAGE value="UI updates"/>
+    <MESSAGE value="Basic copy-paster setup."/>
+    <MESSAGE value="Minor corrections before sleep."/>
+    <MESSAGE value="RC Tello now working. Framerate not great."/>
     <MESSAGE value="README update"/>
     <option name="LAST_COMMIT_MESSAGE" value="README update"/>
   </component>
 </project>
```

### Comparing `sac_tello-0.0.5/sac_tello/face_recognizer.py` & `sac_tello-0.0.6/sac_tello/face_recognizer.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.5/sac_tello/rc_tello.py` & `sac_tello-0.0.6/sac_tello/tello_cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,288 @@
-# File: rc_tello.py
+# File: tello_cmd.py
 # Author: Michael Huelsman
 # Copyright: Dr. Michael Andrew Huelsman 2023
 # License: GNU GPLv3
-# Created On: 31 Jan 2023
+# Created On: 26 Jun 2023
 # Purpose:
-#   A simple interface for controlling the Tello via RC commands.
+#   A class and function for managing sending commands to a Tello in a separate process.
 # Notes:
+#   This is intended for use in a multiprocessing capacity.
+#   Start by running tello_command_loop as the target of a Process object.
+#
+#   Two multiprocessing queues are used:
+#       cmd_q: Used by the parent to send commands to the Tello.
+#              Commands should be sent as a single string.
+#       conf_q: Used by the child to send confirmation of completion/failure to parent.
+#               Messages in queue are (boolean, string) pairs.
+#               boolean indicates success/failure, string give setails.
+#
+#   Commands (case insensitive) accepted:
+#       halt: Stops the process and closes the management object.
+#       takeoff: Makes the Tello takeoff.
+#       land: Makes the Tello land.
+#       up <dist>: Moves the Tello up to <dist> cm above ground level.
+#       down <dist>: Moves the Tello down to <dist> cm above ground level.
+#       left <dist>: Moves the Tello left <dist> cm.
+#       right <dist>:  Moves the Tello right <dist> cm.
+#       forward <dist>:  Moves the Tello forward <dist> cm.
+#       backward <dist>:  Moves the Tello backward <dist> cm.
+#       rotates [cw, ccw] <deg>: Rotates the Tello <deg> degrees [cw, ccw].
+#       flip [f, b, l, r]: Flips the drone in a direction ([f, b, l, r]).
+#       move <x> <y> <z> <spd>: Moves the Tello by the given (x, y, z) in cm at speed spd.
+#       stream [on, off]: Turns the Tello video stream [on, off].
+#       emergency: send command to shut down Tello (no confirmation).
 
-
+import multiprocessing as mp
 from socket import socket, AF_INET, SOCK_DGRAM
 from threading import Thread
-from time import time, perf_counter
+from time import perf_counter
 from datetime import datetime
-import cv2
-import pygame as pg
-from math import log1p
+import queue
+import os
 
-class TelloRC:
-    # Precond:
-    #   The computer creating the TelloRC instance is connected to the Tello's
-    #       Wi-Fi.
-    #
-    # Postcond:
-    #   Sets up a connection with the Tello Drone.
+
+def tello_command_loop(cmd_q: mp.Queue, conf_q: mp.Queue):
+    # Create a management object
+    manager = TelloCmd()
+    res = manager.startup()
+    conf_q.put((res, 'startup'))
+    if not res:
+        return
+    running = True
+    while running:
+        try:
+            cmd = str(cmd_q.get(False)).lower()
+            cmd = cmd.split(' ')
+            # Paring the send commands
+            try:
+                if cmd[0] == "halt":
+                    running = False
+                elif cmd[0] == "takeoff":
+                    res = manager.takeoff()
+                    conf_q.put((res, 'takeoff'))
+                elif cmd[0] == "land":
+                    res = manager.land()
+                    conf_q.put((res, 'land'))
+                elif cmd[0] == "up":
+                    res = manager.up(int(cmd[1]))
+                    conf_q.put((res, 'up'))
+                elif cmd[0] == "down":
+                    res = manager.down(int(cmd[1]))
+                    conf_q.put((res, 'down'))
+                elif cmd[0] == "left":
+                    res = manager.left(int(cmd[1]))
+                    conf_q.put((res, 'left'))
+                elif cmd[0] == "right":
+                    res = manager.right(int(cmd[1]))
+                    conf_q.put((res, 'right'))
+                elif cmd[0] == "forward":
+                    res = manager.forward(int(cmd[1]))
+                    conf_q.put((res, 'forward'))
+                elif cmd[0] == "backward":
+                    res = manager.backward(int(cmd[1]))
+                    conf_q.put((res, 'backward'))
+                elif cmd[0] == "rotate":
+                    res = False
+                    if cmd[1] == 'cw':
+                        res = manager.rotate_cw(int(cmd[2]))
+                    elif cmd[1] == 'ccw':
+                        res = manager.rotate_ccw(int(cmd[2]))
+                    conf_q.put((res, 'rotate ' + cmd[1]))
+                elif cmd[0] == "flip":
+                    res = False
+                    if cmd[1] == 'f':
+                        res = manager.flip_forward()
+                    elif cmd[1] == 'b':
+                        res = manager.flip_backward()
+                    elif cmd[1] == 'l':
+                        res = manager.flip_left()
+                    elif cmd[1] == 'r':
+                        res = manager.flip_right()
+                elif cmd[0] == "move":
+                    res = manager.move(int(cmd[1]),
+                                       int(cmd[2]),
+                                       int(cmd[3]),
+                                       int(cmd[4]))
+                    conf_q.put((res, 'move'))
+                elif cmd[0] == "stream":
+                    if cmd[1] == "on":
+                        res = manager.stream_on()
+                        conf_q.put((res, 'stream on'))
+                    elif cmd[1] == "off":
+                        res = manager.stream_on()
+                        conf_q.put((res, 'stream off'))
+                elif cmd[0] == "emergency":
+                    manager.emergency()
+            except ValueError:
+                conf_q.put((False, 'Invalid Argument'))
+        except queue.Empty:
+            pass
+    try:
+        while not cmd_q.empty():
+            cmd_q.get_nowait()
+    except queue.Empty:
+        pass
+    cmd_q.close()
+    manager.close()
+    
+
+# Class for handling sending Tello commands and logging data.
+class TelloCmd:
     def __init__(self):
         # Addresses
         self.local_addr = ('', 8889)
         self.tello_addr = ('192.168.10.1', 8889)
-
+    
         # Setup channels
         self.send_channel = socket(AF_INET, SOCK_DGRAM)
         self.send_channel.bind(self.local_addr)
-
+    
         self.stop = True
         self.connected = False
-
+    
         # Setup receiving thread
         self.receive_thread = Thread(target=self.__receive)
         self.receive_thread.daemon = True
-
+    
         # Setup logs
         self.log = []
-        self.rc_log = []
         self.MAX_TIME_OUT = 10  # measured in seconds
-        self.rc_sleep = 0.03  # how long the rc command sleeps between sends (seconds)
-
-        # Connecting the video
-        self.video_connect_str = 'udp://192.168.10.1:11111'
-        self.video_stream = None
-        self.video_thread = Thread(target=self.__receive_video)
-        self.video_thread.daemon = True
-        self.last_frame = None
-        self.stream_active = False
-        self.frame_width = 0
-        self.frame_height = 0
-
-        # Connecting to current state information
-        self.state_addr = ('192.168.10.1', 8890)
-        self.local_state_addr = ('', 8890)
-        self.state_channel = socket(AF_INET, SOCK_DGRAM)
-        self.state_channel.bind(self.local_state_addr)
-        self.last_state = None
-
-        self.receive_state_thread = Thread(target=self.__receive_state)
-        self.receive_state_thread.daemon = True
-
-        # Set up RC accounting
-        self.rc = [0, 0, 0, 0]
-
+        
     def startup(self):
         self.stop = False
         self.receive_thread.start()
-        if self.__connect(5) and self.stream_on():
-            self.receive_state_thread.start()
+        if self.__connect(5):
             return True
         return False
 
     # ======================================
     # COMMAND METHODS
     # ======================================
     # Section Notes:
     #   All commands check to see if the drone has been connected and put into SDK mode before sending commands.
 
     # Precond:
-    #   The value to set the forward throttle to.
+    #   None.
+    #
+    # Postcond
+    #   Sends the takeoff command.
+    #   If a non-okay response is given returns False, otherwise returns true.
+    def takeoff(self):
+        if not self.connected:
+            return False
+        res = self.__send("takeoff")
+        return res is not None and res == 'ok'
+
+    # Precond:
+    #   None.
+    #
+    # Postcond
+    #   Sends the land command.
+    #   If a non-okay response is given returns False, otherwise returns true.
+    def land(self):
+        if not self.connected:
+            return False
+        res = self.__send("land")
+        return res is not None and res == 'ok'
+
+    # Precond:
+    #   val is an integer representing the amount to move
     #
     # Postcond:
-    #   Set forward throttle.
-    def set_x(self, val):
-        nv = min(max(-100, int(val)), 100)
-        if nv != self.rc[1]:
-            self.rc[1] = nv
-            self.__send_rc()
+    #   Moves the drone up to val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def up(self, val):
+        if not self.connected or val not in range(20, 501):
+            return False
+        res = self.__send("up " + str(val))
+        return res is not None and res == 'ok'
 
     # Precond:
-    #   The value to set the right throttle to.
+    #   val is an integer representing the amount to move
     #
     # Postcond:
-    #   Set right throttle.
-    def set_y(self, val):
-        nv = min(max(-100, int(val)), 100)
-        if nv != self.rc[1]:
-            self.rc[0] = nv
-            self.__send_rc()
+    #   Moves the drone down to val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def down(self, val):
+        if not self.connected or val not in range(20, 501):
+            return False
+        res = self.__send("down " + str(val))
+        return res is not None and res == 'ok'
 
     # Precond:
-    #   The value to set the vertical throttle to.
+    #   val is an integer representing the amount to move
     #
     # Postcond:
-    #   Set vertical throttle.
-    def set_z(self, val):
-        nv = min(max(-100, int(val)), 100)
-        if nv != self.rc[1]:
-            self.rc[2] = nv
-            self.__send_rc()
+    #   Moves the drone right val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def right(self, val):
+        if not self.connected or val not in range(20, 501):
+            return False
+        res = self.__send("right " + str(val))
+        return res is not None and res == 'ok'
 
     # Precond:
-    #   The value to set the rotation throttle to.
+    #   val is an integer representing the amount to move
     #
     # Postcond:
-    #   Set rotation throttle.
-    def set_rot(self, val):
-        nv = min(max(-100, int(val)), 100)
-        if nv != self.rc[1]:
-            self.rc[3] = nv
-            self.__send_rc()
+    #   Moves the drone left val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def left(self, val):
+        if not self.connected or val not in range(20, 501):
+            return False
+        res = self.__send("left " + str(val))
+        return res is not None and res == 'ok'
 
     # Precond:
-    #   x, y, z, and rot are numberic calues indicating the rc settings.
+    #   val is an integer representing the amount to move
     #
     # Postcond:
-    #   Updates the rc and sends the command if anything has changed.
-    def set_rc(self, x, y, z, rot):
-        nx = min(max(-100, int(x)), 100)
-        ny = min(max(-100, int(y)), 100)
-        nz = min(max(-100, int(z)), 100)
-        nrot = min(max(-100, int(rot)), 100)
-        if [nx, ny, nz, nrot] != self.rc:
-            self.rc = [nx, ny, nz, nrot]
-            self.__send_rc()
+    #   Moves the drone forward val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def forward(self, val):
+        if not self.connected or val not in range(20, 501):
+            return False
+        res = self.__send("forward " + str(val))
+        return res is not None and res == 'ok'
 
     # Precond:
-    #   None.
+    #   val is an integer representing the amount to move
     #
-    # Postcond
-    #   Sends the takeoff command.
-    #   If a non-okay response is given returns False, otherwise returns true.
-    def takeoff(self):
-        if not self.connected:
+    # Postcond:
+    #   Moves the drone backward val centimeters.
+    #   Returns False if the command could not be sent for any reason.
+    def backward(self, val):
+        if not self.connected or val not in range(20, 501):
             return False
-        res = self.__send("takeoff")
+        res = self.__send("back " + str(val))
         return res is not None and res == 'ok'
 
     # Precond:
-    #   None.
+    #   val is an integer representing the amount to move
     #
-    # Postcond
-    #   Sends the land command.
-    #   If a non-okay response is given returns False, otherwise returns true.
-    def land(self):
-        if not self.connected:
+    # Postcond:
+    #   Rotates the drone clockwise val degrees.
+    #   Returns False if the command could not be sent for any reason.
+    def rotate_cw(self, val):
+        if not self.connected or val not in range(1, 361):
             return False
-        res = self.__send("land")
+        res = self.__send("cw " + str(val))
+        return res is not None and res == 'ok'
+
+    # Precond:
+    #   val is an integer representing the amount to move
+    #
+    # Postcond:
+    #   Rotates the drone counterclockwise val degrees.
+    #   Returns False if the command could not be sent for any reason.
+    def rotate_ccw(self, val):
+        if not self.connected or val not in range(1, 361):
+            return False
+        res = self.__send("ccw " + str(val))
         return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
     #   Flips the drone left.
@@ -212,81 +329,81 @@
     #       reason.
     def flip_backward(self):
         if not self.connected:
             return False
         res = self.__send("flip b")
         return res is not None and res == 'ok'
 
-    # ======================================
-    # VIDEO METHODS
-    # ======================================
-
     # Precond:
-    #   None.
+    #   x the amount to move in the x-axis.
+    #   y the amount to move in the y-axis.
+    #   z the amount to move in the z-axis.
+    #   spd is the speed of movement
     #
     # Postcond:
-    #   Turns the video stream on.
+    #   Moves the drone by the given x, y, and z values.
     #   Returns False if the command could not be sent or executed for any
     #       reason.
-    def stream_on(self):
-        if not self.connected:
+    def move(self, x, y, z, spd):
+        if not self.connected or not (20 < max(abs(x), abs(y), abs(z)) < 500) or spd not in range(10, 101):
             return False
-        res = self.__send("streamon")
-        if res is not None and res == 'ok':
-            # Set up the video stream
-            if not self.stream_active:
-                self.stream_active = True
-                self.video_stream = cv2.VideoCapture(self.video_connect_str)
-                self.video_stream.set(cv2.CAP_PROP_BUFFERSIZE, 2)
-                self.video_stream.set(cv2.CAP_PROP_FPS, 30)
-                self.frame_width = self.video_stream.get(cv2.CAP_PROP_FRAME_WIDTH)
-                self.frame_height = self.video_stream.get(cv2.CAP_PROP_FRAME_HEIGHT)
-                self.video_thread.start()
-                return True
-        return False
+        coord_str = ' '.join([str(x), str(y), str(z)])
+        res = self.__send("go " + coord_str)
+        return res is not None and res == 'ok'
 
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Turns the video stream off.
-    #   Returns False if the command could not be sent or executed for any
-    #       reason.
-    def stream_off(self):
-        if not self.connected:
-            return False
-        # Stop video feed if needed
-        if self.stream_active:
-            self.stream_active = False
-            self.video_thread.join()
-            self.video_stream = None
-            self.last_frame = None
-            res = self.__send("streamoff")
-            return res is not None and res == 'ok'
-        return False
-
+    #   Sends the emergency command, in triplicate. Does not wait for response.
+    def emergency(self):
+        for _ in range(3):
+            self.__send_nowait("emergency")
+    
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Returns the last frame taken by the Tello.
-    #   Returns None if the stream is off.
-    def get_frame(self):
-        return self.last_frame
-
+    #   Sends a command to the Tello turning its video stream on.
+    def stream_on(self):
+        res = self.__send("streamon")
+        return res is not None and res == 'ok'
+    
     # Precond:
     #   None.
     #
     # Postcond:
-    #   Returns the resolution of a frame.
-    def get_res(self):
-        return self.frame_width, self.frame_height
+    #   Sends a command to the Tello turing its video stream off.
+    def stream_off(self):
+        res = self.__send("streamoff")
+        return res is not None and res =='ok'
+    
+    # Precond:
+    #   fldr is a string containing the path to the folder to place the log file.
+    #
+    # Postcond:
+    #   Closes down communication with the drone and writes the log to a file.
+    def close(self, fldr: str = "logs"):
+        self.connected = False
+        self.stop = True
+        self.send_channel.close()
+        self.receive_thread.join()
+        t = datetime.now()
+        log_name = os.path.join(fldr, t.strftime("%Y-%m-%d_%H-%M-%S") + '-cmd.log')
+        if not os.path.exists(fldr):
+            os.mkdir(fldr)
+        with open(log_name, 'w') as fout:
+            count = 0
+            for entry in self.log:
+                print("Message[" + str(count) + "]:", entry[0], file=fout)
+                print("Response[" + str(count) + "]:", entry[1], file=fout)
+                count += 1
 
     # ======================================
-    # MANAGEMENT METHODS
+    # PRIVATE METHODS
     # ======================================
 
     # Precond:
     #   attempts is the number of times to try and connect.
     #
     # Postcond:
     #   Checks connection to the drone by sending a message to
@@ -295,105 +412,36 @@
     #   Returns false if there was a problem connecting and attempts were
     #       exceeded.
     def __connect(self, attempts=5):
         for _ in range(attempts):
             res = self.__send("command")
             if res is not None and res == 'ok':
                 self.connected = True
-                self.stream_on()
                 return True
         return False
 
     # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Returns the last response received, if it exists.
-    def last_response(self):
-        if len(self.log) == 0:
-            return None
-        return self.log[-1][1]
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Returns the last state received from the Tello as a dictionary.
-    def state(self):
-        return self.last_state
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Sends the emergency command, in triplicate. Does not wait for response.
-    def emergency(self):
-        for _ in range(3):
-            self.__send_nowait("emergency")
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Closes down communication with the drone and writes the log to a file.
-    def close(self):
-        self.connected = False
-        self.stop = True
-        if self.stream_active:
-            self.stream_active = False
-            self.video_thread.join()
-            self.last_frame = None
-            self.video_stream = None
-        self.send_channel.close()
-        self.state_channel.close()
-        self.receive_thread.join()
-        self.receive_state_thread.join()
-        t = datetime.now()
-        log_name = t.strftime("%Y-%m-%d-%X") + '.log'
-        with open(log_name, 'w') as fout:
-            count = 0
-            for entry in self.log:
-                print("Message[" + str(count) + "]:", entry[0], file=fout)
-                print("Response[" + str(count) + "]:", entry[1], file=fout)
-                count += 1
-
-    # ======================================
-    # PRIVATE METHODS
-    # ======================================
-
-    # Precond:
     #   mess is a string containing the message to send.
     #
     # Postcond:
     #   Sends the given message to the Tello.
     #   Returns the response string if the message was received.
     #   Returns None if the message failed.
     def __send(self, msg):
         self.log.append([msg, None])
         self.send_channel.sendto(msg.encode('utf-8'), self.tello_addr)
         # Response wait loop
-        start = time()
+        start = perf_counter()
         while self.log[-1][1] is None:
-            if (time() - start) > self.MAX_TIME_OUT:
+            if (perf_counter() - start) > self.MAX_TIME_OUT:
                 self.log[-1][1] = "TIMED OUT"
                 return None
         return self.log[-1][1]
 
     # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Sends RC messages to the tello based on internal throttle numbers.
-    def __send_rc(self):
-        cmd = 'rc ' + ' '.join(map(str, self.rc))
-        self.rc_log.append(cmd)
-        self.__send_nowait(cmd)
-
-
-    # Precond:
     #   mess is a string containing the message to send.
     #
     # Postcond:
     #   Sends the given message to the Tello.
     #   Does not wait for a response.
     #   Used (internally) only for sending the emergency signal (which is sent
     #       in triplicate.)
@@ -410,147 +458,8 @@
         while not self.stop:
             try:
                 response, ip = self.send_channel.recvfrom(1024)
                 response = response.decode('utf-8')
                 self.log[-1][1] = response.strip()
             except OSError as exc:
                 if not self.stop:
-                    print("Caught exception socket.error : %s" % exc)
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Receives video messages from the Tello and logs them.
-    def __receive_video(self):
-        while not self.stop and self.stream_active:
-            ret, img = self.video_stream.read()
-            if ret:
-                self.last_frame = img
-        self.video_stream.release()
-        cv2.destroyAllWindows()
-
-    # Precond:
-    #   None.
-    #
-    # Postcond:
-    #   Receives states messages from the Tello and logs them.
-    def __receive_state(self):
-      while not self.stop:
-          try:
-              response, ip = self.state_channel.recvfrom(1024)
-              response = response.decode('utf-8')
-              response = response.strip()
-              vals = response.split(';')
-              state = {}
-              for item in vals:
-                  if item == '':
-                      continue
-                  label, val = item.split(':')
-                  state[label] = val
-              self.last_state = state
-          except OSError as exc:
-              if not self.stop:
-                  print("Caught exception socket.error : %s" % exc)
-
-
-class RCFlight:
-  def __init__(self):
-    self.tello = TelloRC()
-    self.input_thread = Thread(target=self.__inp_proc())
-    self.input_thread.daemon = True
-    self.vel_timing = 5
-    self.active = False
-    pg.init()
-  
-  def video_loop(self):
-    frame_start = perf_counter()
-    frame_delta = 1/30
-    display = pg.display.set_mode(self.tello.get_res())
-    while self.active:
-      img = self.tello.get_frame()
-      if img is not None:
-        img = pg.image.frombuffer(img.tobytes(), img.shape[1::-1], "BGR")
-        display.blit(img, (0, 0))
-        pg.display.flip()
-  
-  def __vel_curve(self, t):
-    return 100 * (log1p(t) / log1p(self.vel_timing))
-  
-  def __inp_proc(self):
-    poll_start = perf_counter()
-    poll_delta = 1/30
-    key_holds = {'w': 0, 's': 0, 'd': 0, 'a': 0, 'q': 0, 'e': 0, 'up': 0, 'down': 0}
-    while self.active:
-      delta = (perf_counter() - poll_start)
-      if delta >= poll_delta:
-        poll_start = perf_counter()
-        for event in pg.event.get():
-          if event.type == pg.QUIT:
-            self.active = False
-          elif event.type == pg.KEYDOWN:
-            if event.key == pg.K_t:
-              self.tello.takeoff()
-            elif event.key == pg.K_l:
-              self.tello.land()
-            elif event.key == pg.K_ESCAPE:
-              self.tello.emergency()
-        key_state = pg.key.get_pressed()
-        for key in key_holds:
-          if key_state[pg.key.key_code(key)]:
-            key_holds[key] += delta
-          else:
-            key_holds[key] = 0
-          key_holds[key] = max(0, min(5, key_holds[key]))
-        y = self.__vel_curve(key_holds['w']) - self.__vel_curve(key_holds['s'])
-        x = self.__vel_curve(key_holds['d']) - self.__vel_curve(key_holds['a'])
-        z = self.__vel_curve(key_holds['up']) - self.__vel_curve(key_holds['down'])
-        rot = self.__vel_curve(key_holds['e']) - self.__vel_curve(key_holds['q'])
-        self.tello.set_rc(x, y, z, rot)
-
-
-if __name__ == '__main__':
-    def vel_curve(t):
-        return 100 * (log1p(t) / log1p(5))
-    
-    
-    tello = TelloRC()
-    tello.startup()
-    pg.init()
-    display = pg.display.set_mode(tello.get_res())
-    running = True
-    frame_delta = 1 / 25
-    frame_start = perf_counter()
-    key_holds = {'w': 0, 's': 0, 'd': 0, 'a': 0, 'q': 0, 'e': 0, 'up': 0, 'down': 0}
-    while running:
-        delta = (perf_counter() - frame_start)
-        if delta >= frame_delta:
-            frame_start = perf_counter()
-            for event in pg.event.get():
-                if event.type == pg.QUIT:
-                    running = False
-                elif event.type == pg.KEYDOWN:
-                    if event.key == pg.K_t:
-                        tello.takeoff()
-                    elif event.key == pg.K_l:
-                        tello.land()
-                    elif event.key == pg.K_BACKSPACE:
-                        tello.rc = [0, 0, 0, 0]
-            key_state = pg.key.get_pressed()
-            for key in key_holds:
-                if key_state[pg.key.key_code(key)]:
-                    key_holds[key] += delta
-                else:
-                    key_holds[key] = 0
-                key_holds[key] = max(0, min(5, key_holds[key]))
-            y = vel_curve(key_holds['w']) - vel_curve(key_holds['s'])
-            x = vel_curve(key_holds['d']) - vel_curve(key_holds['a'])
-            z = vel_curve(key_holds['up']) - vel_curve(key_holds['down'])
-            rot = vel_curve(key_holds['e']) - vel_curve(key_holds['q'])
-            tello.set_rc(x, y, z, rot)
-            img = tello.get_frame()
-            if img is not None:
-                img = pg.image.frombuffer(img.tobytes(), img.shape[1::-1], "BGR")
-                display.blit(img, (0, 0))
-                pg.display.flip()
-    tello.close()
-    pg.quit()
+                    print("Caught exception socket.error : %s" % exc)
```

### Comparing `sac_tello-0.0.5/sac_tello/tello_drive.py` & `sac_tello-0.0.6/sac_tello/tello_drive.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 # License: GNU GPLv3
 # Created On: 27 Jun 2023
 # Purpose:
 #   A program for testing flying a tello drone from a ground station computer.
 # Notes:
 
 from tello_drone import TelloDrone
+from tello_rc import TelloRC
 from threading import Thread
 from tello_hud import TelloHud
 from time import sleep
 
 
 def drive_tello():
-    drone = TelloDrone()
+    drone = TelloRC()
     if not drone.start():
         print("Problem connecting.")
         return False
     hud = TelloHud(drone)
     hud.activate_hud()
-    drone.takeoff()
-    drone.forward(50)
-    drone.land()
+    drone.control()
     hud.deactivate_hud()
     drone.close()
 
     
 if __name__ == '__main__':
     drive_tello()
```

### Comparing `sac_tello-0.0.5/sac_tello/tello_drone.py` & `sac_tello-0.0.6/sac_tello/tello_drone.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,23 @@
         self.video_process.join()
         self.state_haltQ.put("halt")
         TelloDrone.__clear_q(self.state_recQ)
         self.state_process.join()
         self.cmdQ.put("halt")
         TelloDrone.__clear_q(self.cmd_confQ)
         self.cmd_process.join()
+        
+    # Precond:
+    #   None.
+    #
+    # Postcond:
+    #   Waits until all commands are complete.
+    def complete(self):
+        while len(self.commandQ) > 0:
+            sleep(1)
 
     # ======================================
     # COMMAND METHODS
     # ======================================
    
     # Precond:
     #   None.
```

### Comparing `sac_tello-0.0.5/sac_tello/tello_hud.py` & `sac_tello-0.0.6/sac_tello/tello_hud.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # License: GNU GPLv3
 # Created On: 27 Jun 2023
 # Purpose:
 #   A simple hud program that can be run on a separate thread.
 # Notes:
 
 from tello_drone import TelloDrone
-from time import perf_counter
+from tello_rc import TelloRC
+from time import perf_counter, sleep
 import pygame as pg
 from math import sin, cos, radians
 from threading import Thread
 
 
 class TelloHud:
-    def __init__(self, drone: TelloDrone):
+    def __init__(self, drone: TelloDrone | TelloRC):
         self.drone = drone
         self.running = False
         self.hud_thread = Thread(target=self.__hud_stream)
         self.hud_thread.daemon = True
         # Create base visuals for hud
         self.hud_rad = 50
         self.hud_base = pg.Surface((4*self.hud_rad, 4*self.hud_rad), pg.SRCALPHA, 32)
@@ -37,14 +38,15 @@
         pg.draw.line(self.hud_base, (0, 200, 0), roll_start.to_tuple(), roll_end.to_tuple(), 6)
     
     def activate_hud(self):
         if self.running:
             return
         self.running = True
         self.hud_thread.start()
+        sleep(5)
         
     def deactivate_hud(self):
         if not self.running:
             if self.hud_thread.is_alive():
                 self.hud_thread.join()
             return
         self.running = False
@@ -57,15 +59,15 @@
         # Setup Pygame
         pg.display.init()
         screen = pg.display.set_mode((640, 480))
         pg.font.init()
         hud_font = pg.font.Font(pg.font.get_default_font(), 20)
         # Setup video loop basics
         frame_timer = perf_counter()
-        frame_delta = 1/30
+        frame_delta = 1/24
         while self.running:
             if (perf_counter() - frame_timer) > frame_delta:
                 frame_timer = perf_counter()
                 frame = self.drone.get_frame()
                 if frame is not None:
                     frame = frame[0]
                     frame = pg.image.frombuffer(frame.tobytes(), frame.shape[1::-1], "BGR")
@@ -77,17 +79,16 @@
                     screen.blit(bat_text, (0, 0))
                     height_text = hud_font.render(f"ToF: {state['tof']:4}", True, (0, 200, 0), (0, 0, 0))
                     screen.blit(height_text, (0, bat_text.get_height()))
                     horizon = self.__artificial_horizon(50, int(state['pitch']), int(state['roll']))
                     horizon_pos = (screen.get_width() - horizon.get_width())//2, (screen.get_height() - horizon.get_height())//2
                     screen.blit(horizon, horizon_pos)
                 pg.display.flip()
-                for event in pg.event.get():
-                    if event.type == pg.QUIT:
-                        self.running = False
+                for event in pg.event.get(pg.QUIT):
+                    self.running = False
         pg.display.quit()
         
     def __artificial_horizon(self, rad: int, pitch:int, roll: int):
         result = pg.surface.Surface((4*rad, 4*rad), pg.SRCALPHA, 32)
         result.blit(self.hud_base, (0, 0))
         center = self.BasicVec(result.get_width() // 2, result.get_height() // 2)
         # Draw roll lines]
```

### Comparing `sac_tello-0.0.5/sac_tello/tello_state.py` & `sac_tello-0.0.6/sac_tello/tello_state.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.5/sac_tello/tello_video.py` & `sac_tello-0.0.6/sac_tello/tello_video.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.5/.gitignore` & `sac_tello-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.5/LICENSE` & `sac_tello-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.5/README.md` & `sac_tello-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -37,23 +37,25 @@
 ``` 
 
 A created drone object does **not** connect to the tello drone. This merely
 sets up everything that needs to be in place **before** a connection is made.
 
 To connect to the Tello, the TelloDrone class has a method called `start()`
 once the Tello is connected **remember** to call the `close()` method when
-done.
+done. The `start()` method returns `True` if the connection worked and `False`
+if not.
 
 For example a simple takeoff and land program looks like this:
 ```python
 from SAC_Tello import TelloDrone
 drone = TelloDrone()
 drone.start()
 drone.takeoff()
 drone.land()
+drone.complete()
 drone.close()
 ```
 
 The following are all commands that can be sent to the Tello:
 
 | Command       | Method        | Arguments                        |
 |---------------|---------------|----------------------------------| 
@@ -70,22 +72,26 @@
 | flip left     | flip_left     | None                             |
 | flip right    | flip_right    | None                             |
 | flip forward  | flip_forward  | None                             |
 | flip backward | flip_backward | None                             |
 | move          | move          | x: int, y: int, z: int, spd: int |
 | emergency     | emergency     | None                             |
 
+Commands are run in parallel and put into a queue for execution. In order
+to complete the remaining commands in the queue, simply call the `complete()`
+method of the TelloDrone object.
+
 ## Tello Heads-up Display
 
 As an additional feature SAC-Tello gives access to a near-real time video
 stream while the Tello is connected. To make this stream more useful a
 HUD was added. This HUD shows the following:
 - Current Battery life
 - Current Time-of-Flight sensor reading
-- Artificial Horizon indicating changes in pitch rnd roll
+- Artificial Horizon indicating changes in pitch and roll
 
 To use the HUD simply import and create a `TelloDrone` object and link it
 with a `TelloHud` object:
 ```python
 from SAC_Tello import TelloDrone, TelloHud
 drone = TelloDrone()
 hud = TelloHud(drone)
@@ -95,8 +101,46 @@
 drone.close()
 ```
 
 The HUD will launch a separate window when activated. This window can be
 closed at anytime by pressing the `X` in the upper right-hand corner.
 
 Note: Before the HUD is activated nothing will happen. Once the HUD is
-active you will need to deactivate before your program ends.
+active you will need to deactivate before your program ends.
+
+## Tello Remote Control
+
+SAC-Tello also comes with a class for using a ground station computer as
+a remote control for the tello. This remote control can be combined with
+the `TelloHud` class just like the `TelloDrone` class, but we will skip that
+here.
+
+To create and use the remote control simply include the following in your
+program:
+```python
+from SAC_Tello import TelloRC
+drone = TelloRC()
+drone.start()
+drone.control()
+drone.close()
+```
+
+The `control()` method begins polling loop for keyboard input. The controls
+are as follows:
+
+| Key Press  | Effect                |
+|------------|-----------------------|
+| T          | Takeoff               |
+| L          | Land                  |
+| ESCAPE     | Emergency Kill Switch | 
+| BACKSPACE  | End Remote Control    |
+
+| Key Held    | Effect                      |
+|-------------|-----------------------------|
+| W           | Increase Forward Velocity   |
+| A           | Increase Leftward Velocity  |
+| S           | Increase Backward Velocity  |
+| D           | Increase Rightward Velocity |
+| Q           | Rotate Counterclockwise     |
+| E           | Rotate Clockwise            |
+| Up Arrow    | Increase Hover Height       |
+| Down Arrow  | Decrease Hover Height       |
```

### Comparing `sac_tello-0.0.5/pyproject.toml` & `sac_tello-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "SAC-Tello"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Michael Huelsman", email="michael.huelsman@gmail.com" },
 ]
 description = "A Python-based DJI Tello interface which utilizes parallel processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `sac_tello-0.0.5/PKG-INFO` & `sac_tello-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAC-Tello
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python-based DJI Tello interface which utilizes parallel processing.
 Project-URL: Homepage, https://github.com/xLeachimx/SAC-Tello
 Project-URL: Bug Tracker, https://github.com/xLeachimx/SAC-Tello/issues
 Author-email: Michael Huelsman <michael.huelsman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -728,23 +728,25 @@
 ``` 
 
 A created drone object does **not** connect to the tello drone. This merely
 sets up everything that needs to be in place **before** a connection is made.
 
 To connect to the Tello, the TelloDrone class has a method called `start()`
 once the Tello is connected **remember** to call the `close()` method when
-done.
+done. The `start()` method returns `True` if the connection worked and `False`
+if not.
 
 For example a simple takeoff and land program looks like this:
 ```python
 from SAC_Tello import TelloDrone
 drone = TelloDrone()
 drone.start()
 drone.takeoff()
 drone.land()
+drone.complete()
 drone.close()
 ```
 
 The following are all commands that can be sent to the Tello:
 
 | Command       | Method        | Arguments                        |
 |---------------|---------------|----------------------------------| 
@@ -761,22 +763,26 @@
 | flip left     | flip_left     | None                             |
 | flip right    | flip_right    | None                             |
 | flip forward  | flip_forward  | None                             |
 | flip backward | flip_backward | None                             |
 | move          | move          | x: int, y: int, z: int, spd: int |
 | emergency     | emergency     | None                             |
 
+Commands are run in parallel and put into a queue for execution. In order
+to complete the remaining commands in the queue, simply call the `complete()`
+method of the TelloDrone object.
+
 ## Tello Heads-up Display
 
 As an additional feature SAC-Tello gives access to a near-real time video
 stream while the Tello is connected. To make this stream more useful a
 HUD was added. This HUD shows the following:
 - Current Battery life
 - Current Time-of-Flight sensor reading
-- Artificial Horizon indicating changes in pitch rnd roll
+- Artificial Horizon indicating changes in pitch and roll
 
 To use the HUD simply import and create a `TelloDrone` object and link it
 with a `TelloHud` object:
 ```python
 from SAC_Tello import TelloDrone, TelloHud
 drone = TelloDrone()
 hud = TelloHud(drone)
@@ -786,8 +792,46 @@
 drone.close()
 ```
 
 The HUD will launch a separate window when activated. This window can be
 closed at anytime by pressing the `X` in the upper right-hand corner.
 
 Note: Before the HUD is activated nothing will happen. Once the HUD is
-active you will need to deactivate before your program ends.
+active you will need to deactivate before your program ends.
+
+## Tello Remote Control
+
+SAC-Tello also comes with a class for using a ground station computer as
+a remote control for the tello. This remote control can be combined with
+the `TelloHud` class just like the `TelloDrone` class, but we will skip that
+here.
+
+To create and use the remote control simply include the following in your
+program:
+```python
+from SAC_Tello import TelloRC
+drone = TelloRC()
+drone.start()
+drone.control()
+drone.close()
+```
+
+The `control()` method begins polling loop for keyboard input. The controls
+are as follows:
+
+| Key Press  | Effect                |
+|------------|-----------------------|
+| T          | Takeoff               |
+| L          | Land                  |
+| ESCAPE     | Emergency Kill Switch | 
+| BACKSPACE  | End Remote Control    |
+
+| Key Held    | Effect                      |
+|-------------|-----------------------------|
+| W           | Increase Forward Velocity   |
+| A           | Increase Leftward Velocity  |
+| S           | Increase Backward Velocity  |
+| D           | Increase Rightward Velocity |
+| Q           | Rotate Counterclockwise     |
+| E           | Rotate Clockwise            |
+| Up Arrow    | Increase Hover Height       |
+| Down Arrow  | Decrease Hover Height       |
```

