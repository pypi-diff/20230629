# Comparing `tmp/sac_tello-0.0.6.tar.gz` & `tmp/sac_tello-0.0.7.tar.gz`

## Comparing `sac_tello-0.0.6.tar` & `sac_tello-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/SAC-Tello.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/dictionaries/Michael.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/__init__.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/face_recognizer.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_cmd.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_drive.py
--rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_drone.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_hud.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_rc.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_remote.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_state.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.6/sac_tello/tello_video.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.6/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.6/LICENSE
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 sac_tello-0.0.6/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    46029 2020-02-02 00:00:00.000000 sac_tello-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/SAC-Tello.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/dictionaries/Michael.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/__init__.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/face_encoder.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_cmd.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_drive.py
+-rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_drone.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_face_hud.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_hud.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_rc.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_remote.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_state.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.7/sac_tello/tello_video.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 sac_tello-0.0.7/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    48260 2020-02-02 00:00:00.000000 sac_tello-0.0.7/PKG-INFO
```

### Comparing `sac_tello-0.0.6/.idea/workspace.xml` & `sac_tello-0.0.7/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `sac_tello-0.0.6/.idea/workspace.xml` & `sac_tello-0.0.7/.idea/workspace.xml`

```diff
@@ -1,13 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="README update">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-    </list>
+    <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="Updated readme and init file."/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -15,15 +13,15 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
-        <entry key="$PROJECT_DIR$" value="main"/>
+        <entry key="$PROJECT_DIR$" value="frace_recog"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
@@ -225,30 +223,50 @@
     <task id="LOCAL-00024" summary="README update">
       <created>1688049506792</created>
       <option name="number" value="00024"/>
       <option name="presentableId" value="LOCAL-00024"/>
       <option name="project" value="LOCAL"/>
       <updated>1688049506792</updated>
     </task>
-    <option name="localTasksCounter" value="25"/>
+    <task id="LOCAL-00025" summary="Version update">
+      <created>1688049535085</created>
+      <option name="number" value="00025"/>
+      <option name="presentableId" value="LOCAL-00025"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688049535085</updated>
+    </task>
+    <task id="LOCAL-00026" summary="Face recognition and face hud completed.">
+      <created>1688068551382</created>
+      <option name="number" value="00026"/>
+      <option name="presentableId" value="LOCAL-00026"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688068551382</updated>
+    </task>
+    <task id="LOCAL-00027" summary="Updated readme and init file.">
+      <created>1688069662748</created>
+      <option name="number" value="00027"/>
+      <option name="presentableId" value="LOCAL-00027"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688069662748</updated>
+    </task>
+    <option name="localTasksCounter" value="28"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Basic Drone Shell w/ landing and takeoff. Not yet tested."/>
     <MESSAGE value="Basic Movement commands added."/>
     <MESSAGE value="Added video controls."/>
     <MESSAGE value="Added face recognizer"/>
     <MESSAGE value="Added the ability to save known encodings."/>
     <MESSAGE value="Small change"/>
     <MESSAGE value="RC Tello in place, still needs testing"/>
     <MESSAGE value="Minor adjustments. Needs testing."/>
@@ -263,10 +281,13 @@
     <MESSAGE value="Package stuff"/>
     <MESSAGE value="Reorg"/>
     <MESSAGE value="UI updates"/>
     <MESSAGE value="Basic copy-paster setup."/>
     <MESSAGE value="Minor corrections before sleep."/>
     <MESSAGE value="RC Tello now working. Framerate not great."/>
     <MESSAGE value="README update"/>
-    <option name="LAST_COMMIT_MESSAGE" value="README update"/>
+    <MESSAGE value="Version update"/>
+    <MESSAGE value="Face recognition and face hud completed."/>
+    <MESSAGE value="Updated readme and init file."/>
+    <option name="LAST_COMMIT_MESSAGE" value="Updated readme and init file."/>
   </component>
 </project>
```

### Comparing `sac_tello-0.0.6/sac_tello/tello_cmd.py` & `sac_tello-0.0.7/sac_tello/tello_cmd.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_drive.py` & `sac_tello-0.0.7/sac_tello/tello_drive.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_drone.py` & `sac_tello-0.0.7/sac_tello/tello_drone.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_hud.py` & `sac_tello-0.0.7/sac_tello/tello_hud.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         pg.draw.line(self.hud_base, (0, 200, 0), roll_start.to_tuple(), roll_end.to_tuple(), 6)
     
     def activate_hud(self):
         if self.running:
             return
         self.running = True
         self.hud_thread.start()
-        sleep(5)
         
     def deactivate_hud(self):
         if not self.running:
             if self.hud_thread.is_alive():
                 self.hud_thread.join()
             return
         self.running = False
```

### Comparing `sac_tello-0.0.6/sac_tello/tello_rc.py` & `sac_tello-0.0.7/sac_tello/tello_rc.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_remote.py` & `sac_tello-0.0.7/sac_tello/tello_remote.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_state.py` & `sac_tello-0.0.7/sac_tello/tello_state.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/sac_tello/tello_video.py` & `sac_tello-0.0.7/sac_tello/tello_video.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/.gitignore` & `sac_tello-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/LICENSE` & `sac_tello-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.6/pyproject.toml` & `sac_tello-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "SAC-Tello"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Michael Huelsman", email="michael.huelsman@gmail.com" },
 ]
 description = "A Python-based DJI Tello interface which utilizes parallel processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `sac_tello-0.0.6/PKG-INFO` & `sac_tello-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAC-Tello
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python-based DJI Tello interface which utilizes parallel processing.
 Project-URL: Homepage, https://github.com/xLeachimx/SAC-Tello
 Project-URL: Bug Tracker, https://github.com/xLeachimx/SAC-Tello/issues
 Author-email: Michael Huelsman <michael.huelsman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -794,14 +794,73 @@
 
 The HUD will launch a separate window when activated. This window can be
 closed at anytime by pressing the `X` in the upper right-hand corner.
 
 Note: Before the HUD is activated nothing will happen. Once the HUD is
 active you will need to deactivate before your program ends.
 
+## Tello Face Detection
+
+Another feature provided by SAC-Tello is access to face recognition via the
+tello's camera. In order to access the face recognition we must first make
+a `FaceEncoder` object. `FaceEncoder` objects take images and names and log
+a person's facial characteristics for later comparison. To register a face
+with the encoder we need to call the `encode_face` method and give it a name
+and the filename of a image containing that person's face. For example:
+
+```python
+from SAC_Tello import FaceEncoder
+face_encoder = FaceEncoder()
+face_encoder.encode_face("Jim", "jim_selfie.jpg")
+```
+
+Once we have given all the faces we want to recognize to the `FaceEncoder`
+object we can pass in the current camera frame from the tello drone. The
+example below simply lists out the names of all people detected by the drone.
+```python
+from SAC_Tello import FaceEncoder
+from SAC_Tello import TelloDrone
+face_encoder = FaceEncoder()
+face_encoder.encode_face("Jim", "jim_selfie.jpg")
+drone = TelloDrone()
+drone.start()
+while drone.get_frame() is None:
+    pass
+faces = face_encoder.detect_faces(drone.get_frame())
+for name, frame_location in faces:
+    print(name, "is in the frame.")
+drone.close()
+```
+
+Of course this only looks at the first frame from the camera. To make it easier
+to see the face recognition in action SAC-Tello provides a face recognition
+version of the heads-up display. This is contained in the `TelloFaceHud` class
+and works similarly to the `TelloHud` class. For example the following code
+will allow for RC control of the Tello while streaming video that recognizes
+faces and displays names:
+
+```python
+from SAC_Tello import FaceEncoder
+from SAC_Tello import TelloRC
+from SAC_Tello import TelloFaceHud
+face_encoder = FaceEncoder()
+face_encoder.encode_face("Jim", "jim_selfie.jpg")
+drone = TelloRC()
+hud = TelloFaceHud(drone, face_encoder)
+hud.activate_hud()
+drone.control()
+hud.deactivate_hud()
+drone.close()
+```
+
+Note: It may take a long time to encode all faces and so you should encode
+faces first, then use them. If a `FaceEncoder` object detects a face it does
+not recognize it will attribute the name `unknown` to it. Face recongition
+in this package not entirely reliable and results may vary.
+
 ## Tello Remote Control
 
 SAC-Tello also comes with a class for using a ground station computer as
 a remote control for the tello. This remote control can be combined with
 the `TelloHud` class just like the `TelloDrone` class, but we will skip that
 here.
```

