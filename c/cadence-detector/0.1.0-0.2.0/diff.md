# Comparing `tmp/cadence_detector-0.1.0.tar.gz` & `tmp/cadence_detector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadence_detector-0.1.0.tar", last modified: Sun Apr 23 15:30:35 2023, max compression
+gzip compressed data, was "cadence_detector-0.2.0.tar", last modified: Thu Jun 29 08:02:41 2023, max compression
```

## Comparing `cadence_detector-0.1.0.tar` & `cadence_detector-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-23 15:30:35.157046 cadence_detector-0.1.0/
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1058 2023-04-18 10:24:48.000000 cadence_detector-0.1.0/LICENSE
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1233 2023-04-23 15:30:35.156613 cadence_detector-0.1.0/PKG-INFO
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      672 2023-04-22 15:45:43.000000 cadence_detector-0.1.0/README.md
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      704 2023-04-23 15:30:15.000000 cadence_detector-0.1.0/pyproject.toml
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       38 2023-04-23 15:30:35.157137 cadence_detector-0.1.0/setup.cfg
-drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-23 15:30:35.147659 cadence_detector-0.1.0/src/
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-22 08:05:31.000000 cadence_detector-0.1.0/src/__init__.py
-drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-23 15:30:35.152179 cadence_detector-0.1.0/src/cadence_detector/
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1604 2023-04-15 10:45:19.000000 cadence_detector-0.1.0/src/cadence_detector/CadenceDetectData.py
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)    44235 2023-04-18 17:10:28.000000 cadence_detector-0.1.0/src/cadence_detector/CadenceDetectStateMachine.py
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)    56649 2023-04-18 17:10:28.000000 cadence_detector-0.1.0/src/cadence_detector/CadenceDetector.py
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        1 2023-04-22 08:31:36.000000 cadence_detector-0.1.0/src/cadence_detector/__init__.py
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     2277 2023-04-22 14:52:32.000000 cadence_detector-0.1.0/src/cadence_detector/cadence_detector.py
-drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-23 15:30:35.155947 cadence_detector-0.1.0/src/cadence_detector.egg-info/
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1233 2023-04-23 15:30:35.000000 cadence_detector-0.1.0/src/cadence_detector.egg-info/PKG-INFO
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      473 2023-04-23 15:30:35.000000 cadence_detector-0.1.0/src/cadence_detector.egg-info/SOURCES.txt
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        1 2023-04-23 15:30:35.000000 cadence_detector-0.1.0/src/cadence_detector.egg-info/dependency_links.txt
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       26 2023-04-23 15:30:35.000000 cadence_detector-0.1.0/src/cadence_detector.egg-info/requires.txt
--rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       26 2023-04-23 15:30:35.000000 cadence_detector-0.1.0/src/cadence_detector.egg-info/top_level.txt
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:02:41.078523 cadence_detector-0.2.0/
+-rw-r--r--   0 matanba  (223682273) 418804322     1058 2023-04-18 10:24:48.000000 cadence_detector-0.2.0/LICENSE
+-rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-06-29 08:02:41.078066 cadence_detector-0.2.0/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) 418804322      672 2023-04-22 15:45:43.000000 cadence_detector-0.2.0/README.md
+-rw-r--r--   0 matanba  (223682273) 418804322      704 2023-06-29 07:59:49.000000 cadence_detector-0.2.0/pyproject.toml
+-rw-r--r--   0 matanba  (223682273) 418804322       38 2023-06-29 08:02:41.078680 cadence_detector-0.2.0/setup.cfg
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:02:41.069667 cadence_detector-0.2.0/src/
+-rw-r--r--   0 matanba  (223682273) 418804322        0 2023-04-22 08:05:31.000000 cadence_detector-0.2.0/src/__init__.py
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:02:41.073074 cadence_detector-0.2.0/src/cadence_detector/
+-rw-r--r--   0 matanba  (223682273) 418804322     1624 2023-05-26 12:12:19.000000 cadence_detector-0.2.0/src/cadence_detector/CadenceDetectData.py
+-rw-r--r--   0 matanba  (223682273) 418804322    57954 2023-06-29 07:41:31.000000 cadence_detector-0.2.0/src/cadence_detector/CadenceDetectStateMachine.py
+-rw-r--r--   0 matanba  (223682273) 418804322    63695 2023-06-29 07:27:31.000000 cadence_detector-0.2.0/src/cadence_detector/CadenceDetector.py
+-rw-r--r--   0 matanba  (223682273) 418804322        1 2023-04-22 08:31:36.000000 cadence_detector-0.2.0/src/cadence_detector/__init__.py
+-rw-r--r--   0 matanba  (223682273) 418804322     2277 2023-04-22 14:52:32.000000 cadence_detector-0.2.0/src/cadence_detector/cadence_detector.py
+drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-06-29 08:02:41.077407 cadence_detector-0.2.0/src/cadence_detector.egg-info/
+-rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-06-29 08:02:41.000000 cadence_detector-0.2.0/src/cadence_detector.egg-info/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) 418804322      473 2023-06-29 08:02:41.000000 cadence_detector-0.2.0/src/cadence_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 matanba  (223682273) 418804322        1 2023-06-29 08:02:41.000000 cadence_detector-0.2.0/src/cadence_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 matanba  (223682273) 418804322       26 2023-06-29 08:02:41.000000 cadence_detector-0.2.0/src/cadence_detector.egg-info/requires.txt
+-rw-r--r--   0 matanba  (223682273) 418804322       26 2023-06-29 08:02:41.000000 cadence_detector-0.2.0/src/cadence_detector.egg-info/top_level.txt
```

### Comparing `cadence_detector-0.1.0/LICENSE` & `cadence_detector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.1.0/PKG-INFO` & `cadence_detector-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence_detector
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadence_detector-0.1.0/README.md` & `cadence_detector-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.1.0/pyproject.toml` & `cadence_detector-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cadence_detector"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Matan Ben-Asher", email="mbenasher@yahoo.com" },
 ]
 description = "A python package for cadence detection"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cadence_detector-0.1.0/src/cadence_detector/CadenceDetectData.py` & `cadence_detector-0.2.0/src/cadence_detector/CadenceDetectData.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     HCArrivalExpected = 8
     PCCArrival = 9
     PACAppoggExpected = 10
     IACAppoggExpected = 11
     IACArrivalExpected = 12
     HCAppoggExpected = 13
     BassAppoggExpected = 14
+    PCHArrival = 15
 
 class CDHarmonicChordDegrees(Enum):
     I = 1
     II = 2
     III = 3
     IV = 4
     V = 5
```

### Comparing `cadence_detector-0.1.0/src/cadence_detector/CadenceDetectStateMachine.py` & `cadence_detector-0.2.0/src/cadence_detector/CadenceDetectStateMachine.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,44 +3,55 @@
 import numpy as np
 import copy
 
 class CDStateMachine(object):
     def __init__(self, isChallenger=False, minInitialMeasures=0, minPostCadenceMeasures=0):
         self.NumParts = 0
         self.MeasureCounter = 0 # measure counter is for the entire movement and not included in reset
-        self.MinInitialMeasures = minInitialMeasures
+        self.MinInitialMeasures = {CDCadentialStates.PACArrival: minInitialMeasures, CDCadentialStates.IACArrival: minInitialMeasures, CDCadentialStates.HCArrival: round(minInitialMeasures/2)}
         self.MinPostCadenceMeasures = minPostCadenceMeasures
+        self.MinPostCadenceMeasuresHC = minPostCadenceMeasures+1
         self.IsChallenger = isChallenger
         self.reset()
 
     def reset(self):
         # initiliaze with invalid states
         self.PrevCadentialState = CDCadentialStates.Idle
         self.CurrCadentialState = CDCadentialStates.Idle
-        self.CurrHarmonicState = CDHarmonicState([], [], [],  0, 0, 0, 0, 0, 0, [], [])
-        self.PrevHarmonicState = self.CurrHarmonicState
         self.CurrCadentialOutput = CDCadentialStates.Idle
         self.CurrHarmonicState = CDHarmonicState([], chord.Chord(), chord.Chord(), 0, 0, 0, 0, 0, meter.TimeSignature(), [], [])
+        self.PrevHarmonicState = self.CurrHarmonicState
+        self.LastNonAlbertiHarmonicState = self.CurrHarmonicState
         self.ChangeFlagOneShot = 0
         self.KeyChangeOneShot = 0
         self.FirstKeyDetectionDone = 0
         self.CadentialKeyChange = 0
         self.TriggerString = str("")
-        self.PostCadenceMeasureCounter = self.MinPostCadenceMeasures
+        self.PostPACMeasureCounter = self.MinPostCadenceMeasures
+        self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
         self.CheckBassPartFromChord = False
         self.PACPending = False
         self.RevertLastPAC = False
         self.HCPending = False
         self.RevertLastHC = False
+        self.RevertLastIAC = False
         self.HarmonicStateOfLastCadence = 0
         self.SopranoOfLastCadence = 0
         self.WeightOfLastCadence = 0
+        self.PrevMeasureAlberti = False
+        self.PrevMeasureArpeggio = False
+
+    def resetPostCadentialCounters(self):
+        self.PostPACMeasureCounter = self.MinPostCadenceMeasures
+        self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
 
     def updateHarmonicState(self, Key, Chord, ChordWithRests, ChordDegree, ChordInversion, ChordFigure, Alberti, Arpeggio, RomamNumeral, RealNotes):
 
+        if not (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
+            self.LastNonAlbertiHarmonicState = copy.deepcopy(self.CurrHarmonicState)
         self.PrevHarmonicState = copy.deepcopy(self.CurrHarmonicState)
         self.KeyChangeOneShot = 0
         if self.CurrHarmonicState.Key and self.CurrHarmonicState.Key != Key:
             self.KeyChangeOneShot = 1
         self.CurrHarmonicState.Key = Key
         self.CurrHarmonicState.Chord = Chord
         self.CurrHarmonicState.ChordWithBassRests = ChordWithRests
@@ -58,15 +69,17 @@
         self.ChangeFlagOneShot = 0
         if self.PrevCadentialState != self.CurrCadentialState:
             self.ChangeFlagOneShot = 1
             self.TriggerString = str("T") + str(self.PrevCadentialState.value) + str(u'\u208B') + str(self.CurrCadentialState.value)
             self.TriggerString = self.TriggerString.translate(SUB)
             self.PrevCadentialState = self.CurrCadentialState
             if self.CurrCadentialState == CDCadentialStates.PACArrival or self.CurrCadentialState == CDCadentialStates.PCCArrival:
-                self.PostCadenceMeasureCounter = -1
+                self.PostPACMeasureCounter = -1
+            elif self.CurrCadentialState == CDCadentialStates.HCArrival or self.CurrCadentialState == CDCadentialStates.PCHArrival:
+                self.PostHCMeasureCounter = -1
 
     def getBassFromChord(self, chord, favor_by_part=False):
         retVal = False
         if not chord.isRest:
             # first checking the bass part (even if it is not the lowest note in the chord)
             for p in chord:
                 if 'MyBasso' in p.groups:
@@ -80,30 +93,32 @@
                 if not retVal or retVal.midi > lowestPitch.midi:
                     highestPitch = sorted_pitches[-1]
                     # this is an ugly hack to overcome the cases where part id is lost in chordify
                     if (highestPitch.midi-lowestPitch.midi) > 11 or lowestPitch.midi <= 72:
                         retVal = lowestPitch
         return retVal
 
-    def compareBassWithPitch(self, pitchClass, mode='any', favor_by_part=False):
+    def compareBassWithPitch(self, pitchClass, mode='any', favor_by_part=False, HarmonicState=None):
+        if HarmonicState is None:
+            HarmonicState = self.CurrHarmonicState
         retVal = False
         bassPitch = []
         if mode in ['any', 'restless']:
             if not retVal:
-                bassPitch = self.getBassFromChord(self.CurrHarmonicState.Chord, favor_by_part=favor_by_part)
+                bassPitch = self.getBassFromChord(HarmonicState.Chord, favor_by_part=favor_by_part)
                 if bassPitch:
                     retVal = bassPitch.pitchClass==pitchClass
         if mode in ['any', 'orig']:
             if not bassPitch:
-                bassPitch = self.getBassFromChord(self.CurrHarmonicState.ChordWithBassRests, favor_by_part=favor_by_part)
+                bassPitch = self.getBassFromChord(HarmonicState.ChordWithBassRests, favor_by_part=favor_by_part)
                 if bassPitch:
                     retVal = bassPitch.pitchClass==pitchClass
         return retVal
 
-    def isSopraneOnDegree(self,deg):
+    def isSopranoOnDegree(self, deg):
         retVal = 0
         if not isinstance(deg, list):
             deg = [deg]
         for curr_deg in deg:
             target_pitch_class = self.CurrHarmonicState.Key.pitchFromDegree(curr_deg).pitchClass
             if self.CurrHarmonicState.Chord.pitches[-1].pitchClass == target_pitch_class:
                 retVal = 1
@@ -171,18 +186,26 @@
         retPitch = 0
         for p in chord.pitches:
             if partString in p.groups:
                 retPitch = p
                 break
         return retPitch
 
-    def isDominantBass(self, favor_by_part=False):
-        dominantPitchClass = self.CurrHarmonicState.Key.pitchFromDegree(5).pitchClass
+    def isDominantBass(self, favor_by_part=False, HarmonicState=None):
+        if HarmonicState is None:
+            HarmonicState = self.CurrHarmonicState
+        dominantPitchClass = HarmonicState.Key.pitchFromDegree(5).pitchClass
         # chordify may miss the correct bass, check all notes by frequency ascending
-        retVal = self.compareBassWithPitch(dominantPitchClass, mode='any', favor_by_part=favor_by_part)
+        retVal = self.compareBassWithPitch(dominantPitchClass, mode='any', favor_by_part=favor_by_part, HarmonicState=HarmonicState)
+        return retVal
+
+    def isSubDominantBass(self, favor_by_part=False):
+        subDominantPitchClass = self.CurrHarmonicState.Key.pitchFromDegree(4).pitchClass
+        # chordify may miss the correct bass, check all notes by frequency ascending
+        retVal = self.compareBassWithPitch(subDominantPitchClass, mode='any', favor_by_part=favor_by_part)
         return retVal
 
     def isMediantBass(self, favor_by_part=False):
         dominantPitchClass = self.CurrHarmonicState.Key.pitchFromDegree(3).pitchClass
         # chordify may miss the correct bass, check all notes by frequency ascending
         retVal = self.compareBassWithPitch(dominantPitchClass, mode='any', favor_by_part=favor_by_part)
         return retVal
@@ -196,24 +219,53 @@
         return not (self.CurrHarmonicState.Chord.third is None)
 
     def isMatchingQuality(self):
         return not self.harmonyHasThird() or\
                (self.CurrHarmonicState.RomanNumeral.quality == self.CurrHarmonicState.Key.mode)
 
     def harmonyHasSeventh(self, HarmonicState):
-        return not (HarmonicState.Chord.seventh is None)
+        return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=4)
+        #return not (HarmonicState.Chord.seventh is None)
 
     def harmonyHasTonic(self,  HarmonicState):
         return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=1)
 
     def harmonyHasMediant(self, HarmonicState):
         return self.harmonyContainsPitchDegree(HarmonicState=HarmonicState, degree=3)
 
+    # TBD - should obsolete this function
     def verifyNotI64(self, HarmonicState):
-        return not (self.harmonyHasTonic(HarmonicState) or self.harmonyHasMediant(HarmonicState))
+        return not (self.harmonyHasTonic(HarmonicState) or self.harmonyHasMediant(HarmonicState)) or self.harmonyHasSeventh(HarmonicState)
+
+    def isI64(self, HarmonicState):
+        return self.harmonyContainsOnlyPitchDegrees(HarmonicState=HarmonicState, degrees=[1, 3, 5]) and\
+               (self.harmonyHasTonic(HarmonicState) or self.harmonyHasMediant(HarmonicState)) and\
+               self.isDominantBass(HarmonicState=HarmonicState)
+
+    def harmonyContainsOnlyPitchDegrees(self, HarmonicState, degrees):
+        pitch_classes = [HarmonicState.Key.pitchFromDegree(degree).pitchClass for degree in degrees]
+        return self.harmonyContainsOnlyPitchClasses(HarmonicState=HarmonicState, pitch_classes=pitch_classes)
+
+    def harmonyContainsOnlyPitchClasses(self, HarmonicState, pitch_classes):
+        retVal = True
+        if not HarmonicState.ChordWithBassRests.isRest:
+            for p in HarmonicState.ChordWithBassRests.pitches:
+                if p.pitchClass not in pitch_classes:
+                    retVal = False
+                    break
+        return retVal
+
+    def isDominantHarmony(self, HarmonicState):
+        dominant_harmony_degrees = [5, 2, 4] # first without leading tone
+        pitch_classes = [HarmonicState.Key.pitchFromDegree(degree).pitchClass for degree in dominant_harmony_degrees]
+        leading_tone_pitch_class = HarmonicState.Key.pitchFromDegree(7).pitchClass
+        if HarmonicState.Key.mode == 'minor':
+            leading_tone_pitch_class = (leading_tone_pitch_class + 1) % 12 # raise the leading tone
+        pitch_classes.append(leading_tone_pitch_class)
+        return self.harmonyContainsOnlyPitchClasses(HarmonicState=HarmonicState, pitch_classes=pitch_classes)
 
     def harmonyContainsPitchDegree(self, HarmonicState, degree):
         retVal = False
         if not HarmonicState.ChordWithBassRests.isRest:
             PitchClass = HarmonicState.Key.pitchFromDegree(degree).pitchClass
             retVal = PitchClass in [p.pitchClass for p in HarmonicState.ChordWithBassRests.pitches]
         return retVal
@@ -259,14 +311,47 @@
             pSecondaryDominantUpperLeadingTone = RaisedFifth.pitchClass
             for p in self.CurrHarmonicState.Chord.pitches:
                 if p.pitchClass == pSecondaryDominantUpperLeadingTone:
                     retVal = 1
                     break
         return retVal
 
+    def isDominantEmbellishment(self):
+        retVal = 0
+        VpitchClass = self.CurrHarmonicState.Key.pitchFromDegree(5).pitchClass
+        if self.CurrHarmonicState.Key.mode == 'major':
+            # Vb,V#,VIIb,IIb,II#
+            embellishment_offsets = [-1, 1, 3, 6, 8]
+        else:
+            # Vb,V#,VIIb,IIb
+            embellishment_offsets = [-1, 1, 3, 6]
+        embellishments = [(VpitchClass + eo) % 12 for eo in embellishment_offsets]
+        if not self.CurrHarmonicState.Chord.isRest:
+            for p in self.CurrHarmonicState.Chord.pitches:
+                if p.pitchClass in embellishments:
+                    retVal = 1
+                    break
+        return retVal
+
+    def isVMajorExclusive(self, HarmonicState):
+        retVal = 1
+        VpitchClass = self.CurrHarmonicState.Key.pitchFromDegree(5).pitchClass
+        # V,VII,II
+        major_triad_offsets = [0, 4, 7]
+        VchordPitchClass = [(VpitchClass + mto) % 12 for mto in major_triad_offsets]
+        if not HarmonicState.Chord.isRest:
+            for p in HarmonicState.Chord.pitches:
+                if p.pitchClass not in VchordPitchClass:
+                    retVal = 0
+                    break
+        return retVal
+
+    def verifyHCHarmony(self, HarmonicState):
+        return self.isVMajorExclusive(HarmonicState)
+
     def isUnison(self):
         retVal = 1
         Pitch0 = self.CurrHarmonicState.Chord.pitches[0].pitchClass
         for p in self.CurrHarmonicState.Chord.pitches:
             if p.pitchClass != Pitch0:
                 retVal = 0
                 break
@@ -292,23 +377,24 @@
 
     def verifyPACGrouping(self, HarmonicState):
         return self.verifyGrouping(HarmonicState=HarmonicState, start_stop='any') or self.tryGetBeatStrength()==1.0
 
     def verifyIACGrouping(self, HarmonicState):
         return self.verifyGrouping(HarmonicState=HarmonicState, start_stop='stop')
 
-    def verifyHCGrouping(self, HarmonicState):
-        return self.verifyGrouping(HarmonicState=HarmonicState, start_stop='stop')
+    def verifyHCGrouping(self, HarmonicState, start_stop='stop'):
+        return self.verifyGrouping(HarmonicState=HarmonicState, start_stop=start_stop) and self.tryGetBeatStrength()>=0.25
 
     def verifyCadenceVoiceLeading(self, prev_soprano_pitch, curr_soprano_pitch, cadence_type='PAC'):
         retVal = True
         if curr_soprano_pitch and prev_soprano_pitch:
             midi_diff = curr_soprano_pitch.midi - prev_soprano_pitch.midi
             allowed_interval_table = {'PAC': np.array([0, 1, -2, -3, -4, 5, -7]), # anticipated tonic, minor second up, major second down, major/minor third down, fourth up, fifth down
-                                      'IAC': np.array([0, 2, 3, 4, -1, -2, -3, -4])}  # anticipated third or fifth, major second up, major/minor second down, major/minor third up and down
+                                      'IAC': np.array([0, 1, 2, 3, 4, -1, -2, -3, -4, 5]),  # anticipated third or fifth, major/minor second up, major/minor second down, major/minor third up and down, fourth up
+                                      'HC': np.array([0, 1, 2, -1, -2, -5, -7])}
             allowed_intervals = allowed_interval_table[cadence_type]
             allowed_intervals_full = np.concatenate((allowed_intervals, allowed_intervals-12, allowed_intervals+12)) # check also an octave down and up, Mozart K533-1, Haydn17_3_4
             retVal = midi_diff in allowed_intervals_full
         return retVal
 
     def verifySopranoVoiceLeading(self, cadence_type='PAC'):
         curr_soprano_pitch = self.getSopranoPitch(self.CurrHarmonicState)
@@ -376,221 +462,302 @@
                 curr_state = curr_state
             elif self.CurrHarmonicState.ChordWithBassRests.isRest and not self.PrevHarmonicState.Chord.isRest:
                 if self.tryGetBeatStrength() < 1.0:
                     #if sudden rest and not on strongest beat, check if previous harmony was dominant
                     if isinstance(self.PrevHarmonicState.Key, key.Key):
                         dominantPitchClass = self.PrevHarmonicState.Key.pitchFromDegree(5).pitchClass
                         bassPitch = self.getBassFromChord(self.PrevHarmonicState.Chord)
-                        if bassPitch and bassPitch.pitchClass == dominantPitchClass and self.verifyNotI64(HarmonicState=self.PrevHarmonicState):
-                            curr_state = CDCadentialStates.HCArrival
-                            self.WeightOfLastCadence = self.tryGetBeatStrength()
+                        if bassPitch and bassPitch.pitchClass == dominantPitchClass and not self.isI64(HarmonicState=self.PrevHarmonicState) and self.verifySopranoVoiceLeading(cadence_type='HC'):
+                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                 else:
                     curr_state = curr_state
-            elif self.isSecondaryDominantLeadingTone():# or (self.CurrHarmonicState.Key.mode=='major' and self.isSecondaryDominantUpperLeadingTone()): #this can create false HCs, need to consider non-cadential chromatic situations
+            elif self.isDominantEmbellishment():# this can create false HCs, need to consider non-cadential chromatic situations
                 curr_state = CDCadentialStates.HCArrivalExpected
-            elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
-                #if alberti and weak beat do nothing
-                curr_state = curr_state
             elif self.CurrHarmonicState.ChordWithBassRests.isRest:
                 curr_state = curr_state
             elif self.compareBassWithPitch(self.CurrHarmonicState.Key.pitchFromDegree(4).pitchClass, mode='any'):
                 #== bass in 4th degree - IV or II6 go to expecting cadence
                 curr_state = CDCadentialStates.CadExpected
             elif self.compareBassWithPitch(self.CurrHarmonicState.Key.pitchFromDegree(6).pitchClass, mode='any'):
                 #== bass in 6th degree - VI or IV6 go to expecting cadence
                 curr_state = CDCadentialStates.CadExpected
             elif self.tryGetBeatStrength() >= 0.5 and self.compareBassWithPitch(self.CurrHarmonicState.Key.pitchFromDegree(3).pitchClass, mode='any'):
                 #== bass in 3rd degree - iii or I6 on strong beat go to expecting cadence
                 curr_state = CDCadentialStates.CadExpected
 
-        # ==========================================
-        # ====expecting cadence, wait for V=========
-        # ==========================================
+        # ===================================================
+        # ====expecting cadence, wait for V Dominant=========
+        # ===================================================
         elif curr_state == CDCadentialStates.CadExpected or curr_state == CDCadentialStates.CadAvoided or curr_state == CDCadentialStates.IACArrival:
             # only stay in CadAvoided once (currently for display purposes)
-            if curr_state == CDCadentialStates.CadAvoided or curr_state == CDCadentialStates.IACArrival:
+            if curr_state == CDCadentialStates.CadAvoided:
                 curr_state = CDCadentialStates.CadExpected
-            if self.CurrHarmonicState.ChordWithBassRests.isRest:
+            elif curr_state == CDCadentialStates.IACArrival and not (self.isTonicBass() and self.isSopranoOnDegree(1)):
+                curr_state = CDCadentialStates.CadExpected
+            elif curr_state == CDCadentialStates.IACArrival and self.tryGetBeatStrength() == 1:
+                curr_state = CDCadentialStates.CadExpected
+            # now start the real state logic
+            if curr_state == CDCadentialStates.IACArrival and (self.isTonicBass() and self.isSopranoOnDegree(1)):
+                self.RevertLastIAC = True
+                curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state, verify_beat_strength=False)
+            elif self.isDominantEmbellishment():
+                curr_state = CDCadentialStates.HCArrivalExpected
+            elif self.CurrHarmonicState.ChordWithBassRests.isRest:
                 curr_state = curr_state
-            #ignoring arppegios unless they contain dominant seventh chord
-            elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio) and not (self.isDominantBass() and self.harmonyHasSeventh(self.CurrHarmonicState)):
+            #ignoring arppegios
+            elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                 #if alberti or arpeggio bass unless explicit V chord
-                curr_state = curr_state
-            elif self.isDominantBass(favor_by_part=True) and self.verifyNotI64(self.CurrHarmonicState):
-                if (self.CurrHarmonicState.ChordDegree == CDHarmonicChordDegrees.V.value or self.tryGetBeatStrength()>=0.5):
+                if self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState) and self.harmonyHasSeventh(self.CurrHarmonicState):
                     curr_state = CDCadentialStates.CadInevitable
-            elif self.isDominantBass(favor_by_part=True) and not self.verifyNotI64(self.CurrHarmonicState): #I64 can be HC appoggiaturra
-                curr_state = CDCadentialStates.HCAppoggExpected
-            elif self.isSecondaryDominantLeadingTone() or self.isSecondaryDominantUpperLeadingTone(): #this can create false HCs, need to consider non-cadential chromatic situations
+                else:
+                    curr_state = curr_state
+            elif self.isDominantBass() and self.harmonyHasSeventh(self.CurrHarmonicState):
+                curr_state = CDCadentialStates.CadInevitable
+            elif self.isTonicBass():
                 curr_state = CDCadentialStates.HCArrivalExpected
+            elif self.isDominantBass(favor_by_part=True):
+                if not self.isI64(self.CurrHarmonicState):
+                    if self.verifySopranoVoiceLeading(cadence_type='HC') and \
+                        ((self.tryGetBeatStrength()==1 and self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState)) or
+                         self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState, start_stop='stop')) and\
+                            self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                    else:
+                        curr_state = CDCadentialStates.CadInevitable
+                else:
+                    curr_state = CDCadentialStates.HCAppoggExpected
 
         # ========================================================
         # ====inevitable cadence (PAC or IAC), wait for Is========
         # ========================================================
         elif curr_state==CDCadentialStates.CadInevitable or curr_state==CDCadentialStates.IACArrivalExpected:
-            #on dominant and then a complete rest --> HC
+            #on dominant and then a complete rest --> HC with constraints
             if self.CurrHarmonicState.ChordWithBassRests.isRest:
-                if curr_state==CDCadentialStates.CadInevitable and self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and self.verifyNotI64(HarmonicState=self.PrevHarmonicState) and not self.harmonyHasSeventh(HarmonicState=self.PrevHarmonicState):
-                    curr_state = CDCadentialStates.HCArrival
-                    self.WeightOfLastCadence = self.tryGetBeatStrength()
+                if self.verifySopranoVoiceLeading(cadence_type='HC') and\
+                        self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and\
+                        self.verifyHCHarmony(HarmonicState=self.PrevHarmonicState):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                 else:
                     curr_state = curr_state
-            elif self.isBassPartRest() and self.isDominantBass(favor_by_part=True) and self.verifyHCGrouping(HarmonicState=self.PrevHarmonicState) and self.verifyNotI64(HarmonicState=self.CurrHarmonicState) and not self.harmonyHasSeventh(HarmonicState=self.CurrHarmonicState):
-                if curr_state==CDCadentialStates.CadInevitable:
-                    curr_state = CDCadentialStates.HCArrival
-                    self.WeightOfLastCadence = self.tryGetBeatStrength()
-                else:
-                    curr_state = curr_state
-            elif self.isSecondaryDominantLeadingTone():
+            # on dominant and then bass rest --> HC with constraints
+            elif self.isBassPartRest() and\
+                    self.isDominantBass(favor_by_part=True) and\
+                    self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState) and\
+                    self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState):
+                curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+            elif self.isDominantEmbellishment():
                 curr_state = CDCadentialStates.HCArrivalExpected
+            elif (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()):
+                curr_state = CDCadentialStates.HCAppoggExpected
             elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                 #if alberti and weak beat do nothing
                 curr_state = curr_state
             else:
-                # for the case where in IAC expected and dominant appears again, the back to Cad inevitable (TBD, separate these states)
-                if not self.isBassPartRest() and self.isDominantBass(favor_by_part=True) and not (curr_state==CDCadentialStates.IACArrivalExpected and self.isSopraneOnDegree(1)):
+                # for the case where in IAC expected and dominant appears again, back to Cad inevitable
+                if curr_state==CDCadentialStates.IACArrivalExpected and self.isDominantBass(favor_by_part=True) and not self.isBassPartRest():
                     curr_state = CDCadentialStates.CadInevitable
                 # meter - look for cadences on strong beat:
                 elif self.tryGetBeatStrength() >= 0.25:#cadence can only occur on strong beats
                     # harmony  - chordal degree and bass analysis
                     # bass rest on strong beat --> HC
-                    if curr_state==CDCadentialStates.CadInevitable and\
-                            self.getBassFromChord(self.CurrHarmonicState.ChordWithBassRests)==0 and\
+                    if self.isDominantBass(favor_by_part=True) and\
+                            self.isBassPartRest() and\
                             self.tryGetBeatStrength() < 1.0 and\
                             self.verifyHCGrouping(self.CurrHarmonicState) and\
-                            self.verifyNotI64(self.CurrHarmonicState):
-                        curr_state = CDCadentialStates.HCArrival
-                        self.WeightOfLastCadence = self.tryGetBeatStrength()
+                            self.verifyHCHarmony(self.CurrHarmonicState) and\
+                            self.verifySopranoVoiceLeading(cadence_type='HC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                     elif self.isTonicBass():
                         # harmony  - chordal inversion
-                        if (self.CurrHarmonicState.ChordInversion == CDHarmonicChordInversions.Root.value or self.isRootedHarmony()) and self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState):
+                        if (self.CurrHarmonicState.ChordInversion == CDHarmonicChordInversions.Root.value or self.isRootedHarmony()) and\
+                                self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState):
                             # ==I after V after IV or II6, cadential arrival
                             # melody  - soprano degree
-                            if self.isSopraneOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
+                            if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
                                 if curr_state==CDCadentialStates.CadInevitable:
-                                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival)
+                                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
                                 elif self.verifySopranoVoiceLeading(cadence_type='IAC') and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
-                                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival)
-                            #sporano not on 1, either IAC or appoggiatura
-                            elif self.isSopraneOnDegree(3) and self.verifySopranoVoiceLeading(cadence_type='IAC') and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
-                                curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival)
+                                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                            #soprano not on 1, either IAC or appoggiatura
+                            elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC') and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
+                                curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
                             # expecting appoggiatura on strong beats
                             elif self.tryGetBeatStrength() >= 0.5 and self.verifyPACGrouping(self.CurrHarmonicState):
-                                curr_state = self.checkAppoggiatura(curr_state)
+                                curr_state = self.checkAppoggiaturaOrAvoidance('PAC' if curr_state==CDCadentialStates.CadInevitable else 'IAC')
                             # appogiatura can also not be detected as I
                         elif self.tryGetBeatStrength() >= 0.5 and self.verifyPACGrouping(self.CurrHarmonicState):
                             # expecting appogiaturas only on strongest beats (TBD - this might be overfit to haydn)
-                            curr_state = self.checkAppoggiatura(curr_state)
+                            curr_state = self.checkAppoggiaturaOrAvoidance('PAC' if curr_state==CDCadentialStates.CadInevitable else 'IAC')
                     # on strong beat: going from V to anything other than V or I is avoiding the cadence or bass appoggiatura
                     elif self.tryGetBeatStrength() >= 0.5 and self.verifyPACGrouping(self.CurrHarmonicState) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
                         # expecting bass appogiaturas only on strongest beats
                         curr_state = self.checkBassAppoggiatura(curr_state)
                     elif not self.isDominantBass():
-                        curr_state = CDCadentialStates.CadAvoided
-
+                        if self.tryGetBeatStrength() >= 0.5:
+                            curr_state = CDCadentialStates.CadAvoided
+                        else:
+                            curr_state = CDCadentialStates.CadExpected
                 # on weaker beat (but not completely weak) leave this state if not dominant bass:
-                elif self.tryGetBeatStrength() > 0.25 and not self.isDominantBass():
+                elif self.tryGetBeatStrength() >= 0.1 and not self.isDominantBass() and not self.isLeadingToneBass():
                     # if we left dominant but not to I then cadence avoided, but could be HC so wait for V again - TBD, perhaps this avoidance goes further back
                     curr_state = CDCadentialStates.HCArrivalExpected
 
         # =============================================================================================
         # ====HC expected, V on strong beat = HC, V on weak beat, return to cadence inevitable ========
         # =============================================================================================
 
         elif curr_state == CDCadentialStates.HCArrivalExpected:
 
-            if self.CurrHarmonicState.ChordWithBassRests.isRest:
+            if self.isDominantBass(favor_by_part=True) and self.harmonyHasSeventh(self.CurrHarmonicState):
+                curr_state = CDCadentialStates.CadInevitable
+            elif self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio:
+                if self.isDominantBass(favor_by_part=True, HarmonicState=self.LastNonAlbertiHarmonicState) and\
+                        self.harmonyHasSeventh(self.CurrHarmonicState) and\
+                        not self.isDominantEmbellishment():
+                    curr_state = CDCadentialStates.CadInevitable
+                else:
+                    curr_state = curr_state
+            elif self.tryGetBeatStrength() < 0.5 and\
+                    self.isDominantBass(favor_by_part=True) and\
+                    self.isDominantHarmony(HarmonicState=self.CurrHarmonicState):#weak beat returning to dominant, return to cad inevitable
+                curr_state = CDCadentialStates.CadInevitable
+            elif self.CurrHarmonicState.ChordWithBassRests.isRest:
                 curr_state = CDCadentialStates.CadExpected
-
-            else:
-                if self.tryGetBeatStrength() < 0.5:
-                    if self.isDominantBass(favor_by_part=True):#weak beat returning to dominant, return to cad inevitable
-                        curr_state = CDCadentialStates.CadInevitable
-
-                else: #strong beats (TBD - syncopa?)
-
-                    if self.isDominantBass(favor_by_part=True) and (self.harmonyHasSeventh(self.CurrHarmonicState) or not self.verifyHCGrouping(self.CurrHarmonicState)): #V7 or V without grouping return to cad inevitable
-                        curr_state = CDCadentialStates.CadInevitable
-
-                    elif self.isDominantBass(favor_by_part=True) and\
-                            self.verifyHCGrouping(self.CurrHarmonicState)\
-                            and self.verifyNotI64(HarmonicState=self.CurrHarmonicState): # and self.CurrHarmonicState.ChordDegree == CDHarmonicChordDegrees.V.value and self.isRootedHarmony():# and self.harmonyHasThird():# V on strong beat while expecting - HC
-                        curr_state = CDCadentialStates.HCArrival
-                        self.WeightOfLastCadence = self.tryGetBeatStrength()
-
-                    elif self.isDominantBass(favor_by_part=True) and (self.tryGetBeatStrength() == 1.0 or self.harmonyHasTonic(self.CurrHarmonicState)):#appoggiatura on strongest beat, or if V64
-                         curr_state = CDCadentialStates.HCAppoggExpected
-
-                    elif not self.isDominantBass(): #strong beat and not dominant, cadence avoided
-                        curr_state = CDCadentialStates.CadAvoided
+            elif self.tryGetBeatStrength() >= 0.5: #strong beats
+                if self.isDominantBass(favor_by_part=True) and\
+                        (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
+                        not self.isI64(HarmonicState=self.CurrHarmonicState) and\
+                        self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
+                        self.verifySopranoVoiceLeading(cadence_type='HC'):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                # appoggiatura on strongest beat, or if V64
+                elif self.isDominantBass(favor_by_part=True) and\
+                        (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()) and\
+                        self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any'):
+                    curr_state = CDCadentialStates.HCAppoggExpected
+                elif self.isDominantBass(favor_by_part=True) and\
+                        ((self.harmonyHasSeventh(self.CurrHarmonicState) and not self.isDominantEmbellishment()) or\
+                         not (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1)): #V7 or V without grouping return to cad inevitable
+                    curr_state = CDCadentialStates.CadInevitable
+                elif self.isDominantBass(favor_by_part=True) and self.tryGetBeatStrength() == 1.0:#appoggiatura on strongest beat, or if V64
+                    curr_state = CDCadentialStates.HCAppoggExpected
+                elif not (self.isDominantBass() or self.isDominantEmbellishment()): #strong beat and not dominant or embellishment, cadence avoided
+                    curr_state = CDCadentialStates.CadAvoided
+                elif self.isDominantBass(favor_by_part=True) and self.verifyHCGrouping(HarmonicState=self.CurrHarmonicState, start_stop='any') and not self.harmonyHasSeventh(self.CurrHarmonicState):
+                    curr_state = CDCadentialStates.HCAppoggExpected
 
 
         elif curr_state == CDCadentialStates.PACAppoggExpected or curr_state == CDCadentialStates.BassAppoggExpected:
 
             if self.CurrHarmonicState.ChordWithBassRests.isRest or (self.tryGetBeatStrength() == 1): # and not self.isTonicBass()): # rest or new measure not on tonic, exit appoggiatura:
                 if self.isDominantBass():
-                    curr_state = CDCadentialStates.CadInevitable
+                    if (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
+                            self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
+                            self.verifySopranoVoiceLeading(cadence_type='HC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                    elif self.isI64(self.CurrHarmonicState):  # I64 can be HC appoggiaturra on dominant bass
+                        curr_state = CDCadentialStates.HCAppoggExpected
+                    else:
+                        curr_state = CDCadentialStates.CadInevitable
+                elif self.isTonicBass() and\
+                        self.CurrHarmonicState.Chord.isConsonant() and\
+                        not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
+                    if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and\
+                            (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                    elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC') and\
+                            self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                    else:
+                        curr_state = CDCadentialStates.CadExpected
                 else:
                     curr_state = CDCadentialStates.CadExpected
             else:
             # ==appoggiatura, check bass still on key and if soprano is root then PAC otherwise IAC
             # ==for bass appoggiatura check  that soprano is still on tonic and that bass is also.
             # ==grouping is not required becuase it was verified on the appoggiatura entrance
             # ==in case of alberti or arppeggio the original bass on entrance remains, so tonic bass verification is not required.
-                if curr_state ==  CDCadentialStates.BassAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
+                if curr_state == CDCadentialStates.BassAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
                     curr_state = curr_state
-                elif self.isTonicBass() or (curr_state == CDCadentialStates.PACAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio)) and self.CurrHarmonicState.Chord.isConsonant() and not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
-                    if self.isSopraneOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival)
-                    elif self.isSopraneOnDegree(3) and self.verifySopranoVoiceLeading(cadence_type='IAC') and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival)
-                elif not (self.isSopraneOnDegree(1) or self.isDominantBass() or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
+                elif self.isTonicBass() or\
+                        (curr_state == CDCadentialStates.PACAppoggExpected and (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio)) and\
+                        self.CurrHarmonicState.Chord.isConsonant() and\
+                        not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
+                    if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and\
+                            (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                    elif self.isSopranoOnDegree(3) and self.verifySopranoVoiceLeading(cadence_type='IAC') and \
+                            self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                elif self.isDominantBass(favor_by_part=True) and\
+                        (self.verifyHCGrouping(self.CurrHarmonicState, start_stop='any') or self.tryGetBeatStrength()==1) and\
+                        self.verifyHCHarmony(HarmonicState=self.CurrHarmonicState) and\
+                        self.verifySopranoVoiceLeading(cadence_type='HC'):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                elif not (self.isSopranoOnDegree(1) or self.isDominantBass() or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
+                    curr_state = CDCadentialStates.CadAvoided
+                elif (self.IsChallenger and self.verifyPACGrouping(self.CurrHarmonicState)):
                     curr_state = CDCadentialStates.CadAvoided
 
 
         elif curr_state == CDCadentialStates.IACAppoggExpected:
             # ==appoggiatura, check bass still on key and if soprano is root then PAC otherwise IAC
-            if self.isSecondaryDominantLeadingTone():
+            if self.isDominantEmbellishment() or (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()):
                 curr_state = CDCadentialStates.HCArrivalExpected
             elif self.CurrHarmonicState.ChordWithBassRests.isRest or self.tryGetBeatStrength() == 1: # rest or new measure, exit appoggiatura
                 curr_state = CDCadentialStates.CadExpected
             else:
                 if self.isTonicBass():
-                    if ((self.isSopraneOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC')) or (self.isSopraneOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC'))) and (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
+                    if ((self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC')) or
+                        (self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC'))) and\
+                            (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
                         if self.CurrHarmonicState.Chord.isConsonant() and not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
-                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival)
+                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
                 elif self.isDominantBass(): # dominant bass, go to PAC appogiatura
-                    curr_state = self.checkAppoggiatura(curr_state)
-                elif not (self.isSopraneOnDegree(1) or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
+                    curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
+                elif not (self.isSopranoOnDegree(1) or self.isMediantBass()):#continue the appogiattura if dominant or mediant bass
                     curr_state = CDCadentialStates.CadAvoided
 
 
         elif curr_state == CDCadentialStates.HCAppoggExpected:
             # ==HC with appoggiatura, don't exit as long as bass is dominant
             if self.CurrHarmonicState.ChordWithBassRests.isRest:
                 curr_state = CDCadentialStates.CadExpected
             else:
-                if self.isDominantBass(favor_by_part=True):
-                    if self.CurrHarmonicState.ChordDegree == CDHarmonicChordDegrees.V.value and self.harmonyHasSeventh(self.CurrHarmonicState): #V7, return to cad inevitable
-                        curr_state = CDCadentialStates.CadInevitable
-                    elif self.CurrHarmonicState.ChordDegree == CDHarmonicChordDegrees.V.value and\
-                            self.verifyNotI64(HarmonicState=self.CurrHarmonicState) and\
-                            self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState):
-                        curr_state = CDCadentialStates.HCArrival
-                        self.WeightOfLastCadence = self.tryGetBeatStrength()
-                    elif self.tryGetBeatStrength() >= 0.5: # dominant and not HC, exit HC appoggiatura state
-                        curr_state = CDCadentialStates.CadInevitable
-                elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
+                if (self.isI64(HarmonicState=self.CurrHarmonicState) and not self.isBassPartRest()) or self.isDominantEmbellishment(): # stay in HC appogg as long as I64 or dominant embellishment
                     curr_state = curr_state
-                elif self.isTonicBass() and self.tryGetBeatStrength() >= 0.5 and self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState) and self.verifySopranoVoiceLeading(cadence_type='PAC'):#PAC arrival can happen here
-                    if self.isSopraneOnDegree(1):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival)
-                    elif (self.isSopraneOnDegree(3) or self.isSopraneOnDegree(5)) and self.verifySopranoVoiceLeading(cadence_type='IAC'):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival)
-                else:
+                elif self.isDominantBass(favor_by_part=True) and\
+                        self.verifyHCHarmony(self.CurrHarmonicState) and\
+                        self.verifySopranoVoiceLeading(cadence_type='HC'):
+                    curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
+                #elif self.isDominantBass(favor_by_part=True) and\
+                #        (self.harmonyHasSeventh(self.CurrHarmonicState) or self.tryGetBeatStrength() >= 0.5): #V7 or strong beat, return to cad inevitable
+                #    curr_state = CDCadentialStates.CadInevitable
+                #elif self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=4): #also V7
+                #    curr_state = CDCadentialStates.CadInevitable
+                elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
+                    # V7 in alberti
+                    if self.isDominantBass(favor_by_part=True, HarmonicState=self.LastNonAlbertiHarmonicState) and\
+                            self.harmonyHasSeventh(self.CurrHarmonicState) and\
+                            not self.isDominantEmbellishment():
+                        curr_state = CDCadentialStates.CadInevitable
+                    else:
+                        curr_state = curr_state
+                elif self.isTonicBass() and self.tryGetBeatStrength() >= 0.5 and\
+                        self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState) and\
+                        self.isDominantHarmony(HarmonicState=self.PrevHarmonicState):
+                    if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                    elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC'):
+                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                    else:
+                        curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
+                elif self.tryGetBeatStrength() >= 0.25 and self.isDominantBass(favor_by_part=True) and (self.harmonyHasSeventh(self.CurrHarmonicState) or self.tryGetBeatStrength() >= 0.5): #V7 or strong beat, return to cad inevitable
+                    curr_state = CDCadentialStates.CadInevitable
+                elif not self.isDominantBass():
                     curr_state = CDCadentialStates.CadAvoided
 
         elif curr_state == CDCadentialStates.PACArrival or curr_state == CDCadentialStates.PCCArrival:
             #conditions for exiting PAC state:
             #1. complete rest
             #2. new measure
             #3. bass not on tonic
@@ -601,21 +768,21 @@
                     not self.isPartInChord(self.CurrHarmonicState.Chord,'MySoprano') or\
                     self.getCurrSopranoPitch().midi < self.SopranoOfLastCadence.midi:
                 self.exitPACState()
                 self.updateCadentialState()
                 return
             else:
                 # soprano still on tonic
-                if self.isSopraneOnDegree(1):
+                if self.isSopranoOnDegree(1):
                     self.PACPending = False
                     self.exitPACState()
                     self.updateCadentialState()
                     return
                 elif self.tryGetBeatStrength() >= 0.25 and\
-                        (self.isSopraneOnDegree(3)) and\
+                        (self.isSopranoOnDegree(3)) and\
                         (self.CurrHarmonicState.Chord.isTriad() or
                          self.CurrHarmonicState.Chord.isIncompleteMajorTriad() or
                          self.CurrHarmonicState.Chord.isIncompleteMinorTriad()):
                     currSopranoPitch = self.getCurrSopranoPitch()
                     lastSopranoPitch = self.SopranoOfLastCadence
                     # a higher third in soprano following a PAC causes it retroactively to become a IAC!
                     print(currSopranoPitch,lastSopranoPitch)
@@ -627,102 +794,135 @@
                             # moving down to 3, confirms the PAC, move to idle and call update state again
                             self.PACPending = False
                             self.exitPACState()
                             self.updateCadentialState()
                             return
 
 
-        elif curr_state == CDCadentialStates.HCArrival:
-            if self.CurrHarmonicState.ChordWithBassRests.isRest or self.PrevHarmonicState.ChordWithBassRests.isRest:# a rest confirms the cadence
+        elif curr_state == CDCadentialStates.HCArrival or curr_state == CDCadentialStates.PCHArrival:
+            if self.CurrHarmonicState.ChordWithBassRests.isRest or self.PrevHarmonicState.ChordWithBassRests.isRest:# a full rest confirms the cadence
                 curr_state = CDCadentialStates.Idle if self.MinPostCadenceMeasures > 0 else CDCadentialStates.CadInevitable
             elif (self.CurrHarmonicState.Alberti or self.CurrHarmonicState.Arpeggio):
-                # if alberti and weak beat do nothing
-                curr_state = curr_state
+                # if alberti and weak beat verify still not V7
+                if self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=4) and\
+                        self.isDominantBass(HarmonicState=self.LastNonAlbertiHarmonicState):
+                    curr_state = CDCadentialStates.CadInevitable
+                    self.RevertLastHC = True
+                    self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
+                else: # stay in state for an other Alberti or arpeggio
+                    curr_state = curr_state
             else:
                 # == After HC we are still expecting a cadence, but we need to see how this does not create false positives
-                if self.isDominantBass():
-                    if self.harmonyHasSeventh(self.CurrHarmonicState): #V7, return to cad inevitable! (TBD - and cancel the previous HC??)
-                        curr_state = CDCadentialStates.CadInevitable
+                if self.isDominantBass() and self.harmonyHasSeventh(self.CurrHarmonicState): #V7, return to cad inevitable (and cancel the previous HC?)
+                    curr_state = CDCadentialStates.CadInevitable
+                    #if self.tryGetBeatStrength() <= 0.25: # this causes HC misses - example Haydn op.55,2,2 mm.34
+                    #    self.RevertLastHC = True
+                    #    self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
+                #elif self.isSubDominantBass(): # V2, cancel previous HC
+                #    self.RevertLastHC = True
+                #    self.PostHCMeasureCounter = self.MinPostCadenceMeasuresHC
+                #    curr_state = CDCadentialStates.CadAvoided
                 # === very strict condition from HC to PAC
-                elif (self.isTonicBass() or self.isSopraneOnDegree(1)) and\
+                elif (self.isTonicBass() or self.isSopranoOnDegree(1)) and\
                         (self.tryGetBeatStrength() > self.WeightOfLastCadence or self.tryGetBeatStrength() > 0.25) and\
                         self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState) and\
                         self.verifySopranoVoiceLeading(cadence_type='PAC'):
-                    if self.isTonicBass() and self.isSopraneOnDegree(1):
-                        curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival)
-                    elif self.isTonicBass():
-                        curr_state = self.checkAppoggiatura(curr_state=curr_state)
+                    if self.isTonicBass():
+                        if self.isSopranoOnDegree(1):
+                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
+                        elif self.isSopranoOnDegree(3):
+                            curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
+                        else:
+                            curr_state = self.checkAppoggiaturaOrAvoidance('PAC')
+                    elif self.isDominantBass() and self.isI64(HarmonicState=self.CurrHarmonicState):
+                        curr_state = CDCadentialStates.HCArrivalExpected
                     else:
                         curr_state = self.checkBassAppoggiatura(curr_state=curr_state)
-                    self.WeightOfLastCadence = 0
-                else:#bass has left domninant, go back to cad expected
+                elif not self.isDominantBass():#bass has left domninant, go back to cad expected
                     curr_state = CDCadentialStates.CadExpected
+                else:
+                    curr_state = curr_state
 
         #====set output to state and then set cadential arrivals back to idle state
         self.CurrCadentialOutput = curr_state
         self.CurrCadentialState = curr_state
         #print(self.CurrCadentialState)
         #==must check for change for flow debugging
         self.checkStateChanged()
 
-    def checkAppoggiatura(self, curr_state):
-        if (curr_state == CDCadentialStates.CadInevitable or curr_state == CDCadentialStates.HCArrival) and \
+    def checkAppoggiaturaOrAvoidance(self, app_type='PAC'):
+        if app_type == 'PAC' and \
                 ((self.CurrHarmonicState.Key.mode == 'major' and self.isSopranoOnSemitonesFromTonic([11, 2, 4])) or
                  (self.CurrHarmonicState.Key.mode == 'minor' and self.isSopranoOnSemitonesFromTonic([10, 11, 2, 3]))):
             curr_state = CDCadentialStates.PACAppoggExpected
-        elif curr_state == CDCadentialStates.IACArrivalExpected and self.isSopranoOnSemitonesFromTonic([3, 5]) and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
+        elif app_type == 'IAC' and self.isSopranoOnSemitonesFromTonic([3, 5]) and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
             curr_state = CDCadentialStates.IACAppoggExpected
+        elif app_type == 'HC' and \
+                ((self.CurrHarmonicState.Key.mode == 'major' and self.isSopranoOnSemitonesFromTonic([0, 1, 4, 6, 9])) or
+                 (self.CurrHarmonicState.Key.mode == 'minor' and self.isSopranoOnSemitonesFromTonic([0, 1, 3, 6, 8]))):
+            curr_state = CDCadentialStates.HCAppoggExpected
         else:
             curr_state = CDCadentialStates.CadAvoided
         return curr_state
 
     def checkBassAppoggiatura(self, curr_state):
         if self.isDominantBass(favor_by_part=True) or self.isMediantBass(favor_by_part=True) or self.isBassPartRest():
-            if (curr_state == CDCadentialStates.CadInevitable or curr_state == CDCadentialStates.HCArrival) and self.isSopraneOnDegree(1):
+            if (curr_state in [CDCadentialStates.CadInevitable, CDCadentialStates.HCArrival, CDCadentialStates.PCHArrival]) and self.isSopranoOnDegree(1):
                 curr_state = CDCadentialStates.BassAppoggExpected
-            elif curr_state == CDCadentialStates.IACArrivalExpected and (self.isSopraneOnDegree([1, 2, 3]) or self.isLeadingToneSoprano()):
+            elif curr_state == CDCadentialStates.IACArrivalExpected and (self.isSopranoOnDegree([1, 2, 3]) or self.isLeadingToneSoprano()):
                 curr_state = CDCadentialStates.IACAppoggExpected
             elif curr_state == CDCadentialStates.IACArrivalExpected and (self.isSopranoAtSemitoneFromDegree(1, 3)):
                 curr_state = CDCadentialStates.IACAppoggExpected
+            elif self.isDominantBass(favor_by_part=True):
+                curr_state = CDCadentialStates.CadInevitable
             else:
                 curr_state = CDCadentialStates.CadAvoided
         else:
             curr_state = CDCadentialStates.CadAvoided
         return curr_state
 
     def exitPACState(self):
         if self.PACPending:
             self.CurrCadentialState = CDCadentialStates.CadExpected
             self.RevertLastPAC = True
-            self.PostCadenceMeasureCounter = self.MinPostCadenceMeasures #set the counter high to catch the next cadence
+            self.PostPACMeasureCounter = self.MinPostCadenceMeasures #set the counter high to catch the next cadence
         else:
             # move to idle (confirming the PAC) and call update state again
             if self.MinPostCadenceMeasures > 0:
                 self.CurrCadentialState = CDCadentialStates.Idle
             # if no minimum post cadence measures required, expect post cadential cadences
             else:
                 self.CurrCadentialState = CDCadentialStates.CadExpected
             self.RevertLastPAC = False
         self.PACPending = False
 
     def updateCounters(self):
         #beat strenth==1 means new measure
-        if self.tryGetBeatStrength()==1:
-            self.PostCadenceMeasureCounter = self.PostCadenceMeasureCounter + 1
-            self.MeasureCounter = self.MeasureCounter + 1
-
-    def setCadenceOrPostCadence(self,Cadence):
-        if Cadence==CDCadentialStates.PACArrival and self.PostCadenceMeasureCounter < self.MinPostCadenceMeasures:
-            state = CDCadentialStates.PCCArrival
-        elif self.MeasureCounter <= self.MinInitialMeasures:
-            state = CDCadentialStates.IACArrival
+        if self.tryGetBeatStrength() == 1:
+            self.PostPACMeasureCounter += 1
+            self.PostHCMeasureCounter += 1
+            self.MeasureCounter += 1
+
+    def setCadenceOrPostCadence(self, cadence=None, state=None, verify_beat_strength=True):
+        if not verify_beat_strength or self.tryGetBeatStrength() >= 0.125:
+            if self.MeasureCounter >= self.MinInitialMeasures[cadence]:
+                if cadence == CDCadentialStates.PACArrival and self.PostPACMeasureCounter < self.MinPostCadenceMeasures:
+                    state = CDCadentialStates.PCCArrival
+                elif cadence == CDCadentialStates.HCArrival and self.PostHCMeasureCounter < self.MinPostCadenceMeasuresHC:
+                    state = CDCadentialStates.PCHArrival
+                else:
+                    state = cadence
+            else: # too early, return to cadence expected again
+                state = CDCadentialStates.CadExpected
+            if state == CDCadentialStates.HCArrival or state == CDCadentialStates.PCHArrival:
+                self.WeightOfLastCadence = self.tryGetBeatStrength()
+            self.SopranoOfLastCadence = self.getCurrSopranoPitch()
+            self.HarmonicStateOfLastCadence = copy.deepcopy(self.CurrHarmonicState)
         else:
-            state = Cadence
-        self.SopranoOfLastCadence = self.getCurrSopranoPitch()
-        self.HarmonicStateOfLastCadence = copy.deepcopy(self.CurrHarmonicState)
+            state = state
         return state
 
     def getCadentialOutput(self):
         return self.CurrCadentialOutput
 
     def getCadentialOutputString(self):
         Lyric = str("")
@@ -731,14 +931,16 @@
                 Lyric = str("PAC")
             elif self.getCadentialOutput() == CDCadentialStates.PCCArrival:
                 Lyric = str("PCC")
             elif self.getCadentialOutput() == CDCadentialStates.IACArrival:
                 Lyric = str("IAC")
             elif self.getCadentialOutput() == CDCadentialStates.HCArrival:
                 Lyric = str("HC")
+            elif self.getCadentialOutput() == CDCadentialStates.PCHArrival:
+                Lyric = str("PCH")
             elif self.getCadentialOutput() == CDCadentialStates.CadAvoided:
                 Lyric = str("CA")
             elif not (self.getCadentialOutput() == CDCadentialStates.Idle):
                 Lyric = Lyric + self.TriggerString
 
         if self.KeyChangeOneShot == 1 or self.FirstKeyDetectionDone == 0 or self.CadentialKeyChange == 1:
             Lyric = Lyric + str("\nKey: ") + str(self.CurrHarmonicState.Key)
@@ -755,8 +957,18 @@
         return Lyric
 
     def getRevertLastPACAndReset(self):
         retVal = self.RevertLastPAC
         self.RevertLastPAC = False
         return retVal
 
+    def getRevertLastHCAndReset(self):
+        retVal = self.RevertLastHC
+        self.RevertLastHC = False
+        return retVal
+
+    def getRevertLastIACAndReset(self):
+        retVal = self.RevertLastIAC
+        self.RevertLastIAC = False
+        return retVal
+
```

### Comparing `cadence_detector-0.1.0/src/cadence_detector/CadenceDetector.py` & `cadence_detector-0.2.0/src/cadence_detector/CadenceDetector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .CadenceDetectStateMachine import *
 import music21 as m21
 import math
 import os
 import pickle
+import pickle
 import enum
 import copy
 import sys
 
 class CadenceDetector:
     def __init__(self,
                  maxNumMeasures=500,
@@ -55,14 +56,17 @@
         self.RepeatedMeasureByVolta = []
         self.IncompleteMeasures = []
         self.EmptyMeasures = []
         self.FinalBarlines = []
         self.analysis_full = []
         self.analysis_filtered = []
         self.analysis_transition_strings = []
+        self.PrevMeasureAlberti = False
+        self.PrevMeasureArpeggio = False
+
 
     def loadMusic21Corpus(self,fileString):
         self.NoteStream = m21.corpus.parse(fileString)
         self.analyze()
 
     def loadFileAndGetMeasures(self, fileString):
         print("Loading score...")
@@ -507,15 +511,15 @@
 
     def mapSearsKeyToMusic21Key(self,SearStringKey, SearStringMode):
         Music21StringKey = SearStringKey.replace("b","-")
         Music21StringMode = SearStringMode.replace("M","m")
         return m21.key.Key(Music21StringKey,Music21StringMode)
 
     def isArpeggioPattern(self, pitches, lengths, arp_len, up_down=None):
-        if len(pitches) < arp_len or not all(lengths[0] == l for l in lengths[1:4]):
+        if len(pitches) < arp_len or not all(lengths[0] == l for l in lengths[1:-1]): # the final note in an arpeggio can be longer
             retVal = False
         else:
             retVal = True
             if up_down == 'up':
                 if all(x.midi > pitches[0].midi for x in pitches[1:]):
                     prev_pitch = []
                     for p in pitches:
@@ -538,19 +542,20 @@
         return retVal
 
     def isAlbertiPattern(self, pitches, lengths, pattern_len):
         equal_durations = all(lengths[0] == l for l in lengths[1:4])
         lowest_pitch_first = all(x.midi >= pitches[0].midi for x in pitches[1:4])
         lowest_pitch_third = all(x.midi >= pitches[2].midi for x in pitches[1:4])
         repetitve_pitch = (pitches[1].midi == pitches[3].midi or pitches[0].midi == pitches[2].midi)
+        consecutive_pitch = np.any(np.diff([x.midi for x in pitches]) == 0)
         # for pattern length 6 (3/4,3/8,6/8) verify last two as well, either continuing the same pattern or repeating the bass
         if pattern_len == 6:
             equal_durations = all(lengths[0] == l for l in lengths)
-            repetitve_pitch = repetitve_pitch and (pitches[3].midi == pitches[5].midi or pitches[0] == pitches[4])           
-        is_alberti = equal_durations and repetitve_pitch and (lowest_pitch_first or lowest_pitch_third)
+            repetitve_pitch = repetitve_pitch and (pitches[3].midi == pitches[5].midi or pitches[0] == pitches[4])
+        is_alberti = equal_durations and repetitve_pitch and (lowest_pitch_first or lowest_pitch_third) and not consecutive_pitch
         bass_pitch_index = None
         if lowest_pitch_first:
             bass_pitch_index = 0
         elif lowest_pitch_third:
             bass_pitch_index = 2
         return is_alberti, bass_pitch_index
 
@@ -569,41 +574,50 @@
     def detectAlbertiOrArpeggioBassInMeasure(self, measure_chords, bass_chords, pattern_len, arp_type):
         #first exact bassline from chords
         measure_general_notes = measure_chords.recurse().getElementsByClass('GeneralNote')
         bass_general_notes = bass_chords.recurse().getElementsByClass('GeneralNote')
         lowest_pitches_in_bass = self.extractBassLine(bass_general_notes)
         arp_patterns = []
 
-        for i in range(0, len(bass_general_notes), pattern_len):
-            if i+pattern_len <= len(bass_general_notes):
-                curr_pitches = lowest_pitches_in_bass['pitches'][i:i+pattern_len]
-                curr_lengths = lowest_pitches_in_bass['lengths'][i:i+pattern_len]
-                if None not in curr_pitches:
-                    if arp_type == 'alberti':
-                        isArp, bass_pitch_index = self.isAlbertiPattern(pitches=curr_pitches, lengths=curr_lengths, pattern_len=pattern_len)
-                    elif arp_type == 'arp_up':
-                        isArp = self.isArpeggioPattern(pitches=curr_pitches, lengths=curr_lengths, arp_len=pattern_len, up_down='up')
-                        bass_pitch_index = 0
-                    elif arp_type =='arp_down':
-                        isArp = self.isArpeggioPattern(pitches=curr_pitches, lengths=curr_lengths, arp_len=pattern_len, up_down='down')
-                        bass_pitch_index = 0
+        # need to loop like this because we advance the index based on finding arpeggios
+        i = 0
+        while i <= len(bass_general_notes)-pattern_len:
+            curr_pitches = lowest_pitches_in_bass['pitches'][i:i+pattern_len]
+            curr_lengths = lowest_pitches_in_bass['lengths'][i:i+pattern_len]
+            isArp = False
+            if None not in curr_pitches:
+                if any([cl > 1 for cl in curr_lengths]): # do not consider arps greater than quarter notes
+                    isArp = False
+                elif arp_type == 'alberti':
+                    isArp, bass_pitch_index = self.isAlbertiPattern(pitches=curr_pitches, lengths=curr_lengths, pattern_len=pattern_len)
+                elif arp_type == 'arp_up':
+                    isArp = self.isArpeggioPattern(pitches=curr_pitches, lengths=curr_lengths, arp_len=pattern_len, up_down='up')
+                    bass_pitch_index = 0
+                elif arp_type =='arp_down':
+                    isArp = self.isArpeggioPattern(pitches=curr_pitches, lengths=curr_lengths, arp_len=pattern_len, up_down='down')
+                    bass_pitch_index = 0
+                else:
+                    isArp = False
+                if isArp:
+                    epsilon = 0.1  # this epsilon is required to mark the last alberti beat including its length, but not the next beat
+                    # already assuming they are all equal length
+                    beat_diff = bass_general_notes[i+1].beat-bass_general_notes[i].beat # for some reason quarter length does not always provide this, TBD use seconds map
+                    if bass_pitch_index == 0:
+                        arp_patterns.append({'start': bass_general_notes[i + 1].beat,
+                                             'stop': bass_general_notes[i + pattern_len - 1].beat + beat_diff - epsilon})
                     else:
-                        isArp = False
-                    if isArp:
-                        epsilon = 0.1  # this epsilon is required to mark the last alberti beat including its length, but not the next beat
-                        if bass_pitch_index == 0:
-                            arp_patterns.append({'start': bass_general_notes[i + 1].beat,
-                                                 'stop': bass_general_notes[i + pattern_len - 1].beat + bass_general_notes[i + pattern_len - 1].duration.quarterLength - epsilon})
-                        else:
-                            # mark from beginning of pattern not including first note, to bass pitch index not included
-                            arp_patterns.append({'start': bass_general_notes[i + 1].beat,
-                                                 'stop': bass_general_notes[i + bass_pitch_index - 1].beat + bass_general_notes[i + bass_pitch_index - 1].duration.quarterLength - epsilon})
-                            # mark from note after bass pitch index to the end
-                            arp_patterns.append({'start': bass_general_notes[i + bass_pitch_index + 1].beat,
-                                                 'stop': bass_general_notes[i + pattern_len - 1].beat + bass_general_notes[i + pattern_len - 1].duration.quarterLength - epsilon})
+                        # mark from beginning of pattern not including first note, to bass pitch index not included
+                        arp_patterns.append({'start': bass_general_notes[i + 1].beat,
+                                             'stop': bass_general_notes[i + bass_pitch_index - 1].beat + beat_diff - epsilon})
+                        # mark from note after bass pitch index to the end
+                        arp_patterns.append({'start': bass_general_notes[i + bass_pitch_index + 1].beat,
+                                             'stop': bass_general_notes[i + pattern_len - 1].beat + beat_diff - epsilon})
+            # advance index by pattern length if alberti found, otherwise advance to next beat
+            i = i + pattern_len if isArp else i + 1
+
 
         arp_beats = [0] * len(measure_general_notes)
         for i,gen_note in enumerate(measure_general_notes):
             for pat in arp_patterns:
                 if pat['start'] <= gen_note.beat <= pat['stop']:
                     arp_beats[i] = True
                     break
@@ -655,15 +669,15 @@
         measure_zero = self.ChordStream.measure(0)
         curr_time_sig = self.check_and_update_timesig(measure_zero, [])
 
         # loop on measures:
         try:
             for currMeasureIndex in range(0,self.NumMeasures):
                 # debug per measure
-                if currMeasureIndex == 20:
+                if currMeasureIndex == 18:
                     bla = 0
                 # true measures start with 1, pickups will start from zero, but not all corpora will abide to this
                 # for example, data that originates from midi cannot contain this info
                 # to overcome this, we attempt to find the pickup via initial rests and discard it
                 # also, we count the empty measures and index them out while writing the label
                 measure_number = currMeasureIndex + 1
                 # print(f"measure number {measure_number}")
@@ -695,32 +709,40 @@
 
                 AlbertiBeats4 = self.detectAlbertiOrArpeggioBassInMeasure(CurrMeasuresRestless, CurrMeasureBass, pattern_len=4, arp_type='alberti')
                 AlbertiBeats = AlbertiBeats4
                 if curr_time_sig.ratioString in ['3/4', '6/8', '3/8']:
                     AlbertiBeats6 = self.detectAlbertiOrArpeggioBassInMeasure(CurrMeasuresRestless, CurrMeasureBass, pattern_len=6, arp_type='alberti')
                     AlbertiBeats = [x or y for (x, y) in zip(AlbertiBeats4, AlbertiBeats6)]
 
+                # consider Alberti only after the second consecutive measure
+                # AlbertiBeatsFiltered = [x and self.PrevMeasureAlberti for x in AlbertiBeats]
+                # self.PrevMeasureAlberti = any(AlbertiBeats)
+
                 ArpeggioBeats4 = self.detectAlbertiOrArpeggioBassInMeasure(CurrMeasuresRestless, CurrMeasureBass, pattern_len=4, arp_type='arp_up')
                 ArpeggioBeats = ArpeggioBeats4
                 if curr_time_sig.ratioString in ['3/4', '6/8', '3/8']:
                     ArpeggioBeats3 = self.detectAlbertiOrArpeggioBassInMeasure(CurrMeasuresRestless, CurrMeasureBass, pattern_len=3, arp_type='arp_up')
                     ArpeggioBeats = [x or y for (x, y) in zip(ArpeggioBeats3, ArpeggioBeats4)]
 
+                # consider Arpeggio only after the second consecutive measure
+                ArpeggioBeatsFiltered = [x and self.PrevMeasureArpeggio for x in ArpeggioBeats]
+                self.PrevMeasureArpeggio = any(ArpeggioBeats)
+
                 LyricPerBeat = []
 
                 if self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothing or\
                         self.KeyDetectionMode==CDKeyDetectionModes.KSWithSmoothingCadenceSensitive:
                     #smooth keys here, per measure (TBD - per chord?):
                     self.smoothKeyInterpretations(currMeasureIndex)
                     #sort and return top 2
                     self.Top2Keys = self.getTopNKeyInterpretations(2)
                 else:
                     currKey = self.KeyPerMeasure[currMeasureIndex]#lists start with 0
 
-                for thisChord, thisChordWithBassRests, alberti, arpeggio, thisRealNotes in zip(CurrMeasuresRestless.recurse().getElementsByClass('GeneralNote'),CurrMeasures.recurse().getElementsByClass('GeneralNote'), AlbertiBeats, ArpeggioBeats, NotesPerChordBeatPerPart):
+                for thisChord, thisChordWithBassRests, alberti, arpeggio, thisRealNotes in zip(CurrMeasuresRestless.recurse().getElementsByClass('GeneralNote'),CurrMeasures.recurse().getElementsByClass('GeneralNote'), AlbertiBeats, ArpeggioBeatsFiltered, NotesPerChordBeatPerPart):
                     if self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothing or\
                             self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothingCadenceSensitive:
                         currKeyString = self.Top2Keys[0][0]
                         currKey = m21.key.Key(currKeyString)
                         challengerKeyString = self.Top2Keys[1][0]
                         challengerKey = m21.key.Key(challengerKeyString)
                         self.updateKeysAndSwapStateMachines(currKeyString, challengerKeyString)
@@ -737,34 +759,47 @@
                         if thisChordWithBassRests.isRest:
                             self.HarmonicStateMachineChallenger.updateHarmonicState(challengerKey, thisChord, thisChordWithBassRests, [], [], [], alberti, arpeggio, [], thisRealNotes)
                         else:
                             rn2 = m21.roman.romanNumeralFromChord(thisChordWithBassRests, challengerKey)
                             self.HarmonicStateMachineChallenger.updateHarmonicState(challengerKey, thisChord, thisChordWithBassRests, rn2.scaleDegree, rn2.inversion(), rn2.figure, alberti, arpeggio, rn2, thisRealNotes)
 
                     #TBD - should we handle this reversion in challenger?
-                    if self.HarmonicStateMachine.getRevertLastPACAndReset() and len(LyricPerBeat)>0: #this limits PAC reversion to within measure
+                    if self.HarmonicStateMachine.getRevertLastPACAndReset() and len(LyricPerBeat) > 0: #this limits PAC reversion to within measure
                         LastPACTuple = LyricPerBeat[-1]
                         UpdatedLyric = "IAC"
                         LyricPerBeat[-1] = [LastPACTuple[0], UpdatedLyric]
                         print("Reverting last PAC to IAC")
+                    if self.HarmonicStateMachine.getRevertLastHCAndReset() and len(LyricPerBeat) > 0:  # this limits HC reversion to within measure
+                        LastHCTuple = LyricPerBeat[-1]
+                        UpdatedLyric = ""
+                        LyricPerBeat[-1] = [LastHCTuple[0], UpdatedLyric]
+                        print("Reverting last HC")
+                    if self.HarmonicStateMachine.getRevertLastIACAndReset() and len(LyricPerBeat) > 0:  # this limits IAC reversion to within measure
+                        LastIACTuple = LyricPerBeat[-1]
+                        UpdatedLyric = ""
+                        LyricPerBeat[-1] = [LastIACTuple[0], UpdatedLyric]
+                        print("Reverting last IAC")
 
                     Lyric = self.HarmonicStateMachine.getCadentialOutputString()
                     LyricChallenger = self.HarmonicStateMachineChallenger.getCadentialOutputString()
                     # Cadence Sensitive Key Detection Mode
                     if self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothingCadenceSensitive:
                         # and self.HarmonicStateMachineChallenger.CurrHarmonicState.Key.tonic != self.HarmonicStateMachine.CurrHarmonicState.Key.tonic: #don't be sensitive to candece in parallel key:
                         # Cadence check in main key (for key re-enforcement)
 
                         resort = False
                         for cad in self.ReenforcementFactors:
                             if cad in Lyric:
-                                self.reenforceKeyByFactor(currKeyString, self.ReenforcementFactors[cad])
+                                # avoid reinforcement of HC if challenger is on dominant
+                                reenforce = not (currKey.getDominant().pitchClass == challengerKey.tonic.pitchClass and challengerKey.mode=='major' and (cad == 'HC'))
+                                if reenforce:
+                                    self.reenforceKeyByFactor(currKeyString, self.ReenforcementFactors[cad])
                             # Challenger Check (for key switching, but ignore HCs in subdominant key (becuase they are more likely PACs in main key))
                             if cad in LyricChallenger:
-                                reenforce =  not (challengerKey.tonic.pitchClass == self.getSubDominantPitchClass(currKey) and (cad == 'HC')) # and not (challengerKey.tonic.pitchClass == currKey.getDominant().pitchClass and (cad == 'PAC'))
+                                reenforce =  not (challengerKey.tonic.pitchClass == self.getSubDominantPitchClass(currKey) and challengerKey.mode=='major' and (cad == 'HC'))
                                 if reenforce:
                                     self.reenforceKeyByFactor(challengerKeyString, self.ReenforcementFactors[cad])
                                     resort = True
                         if resort:
                             # re-sort and return Top2Keys
                             self.Top2Keys = self.getTopNKeyInterpretations(2)
                             if challengerKeyString == self.Top2Keys[0][0]:
@@ -777,25 +812,19 @@
 
                     if Lyric:   # only work on non-empty lyrics
                         thisChord.lyric = Lyric
                         LyricPerBeat.append([thisChord.beat,Lyric])
                         #TBD - do we still need to print this?
                         self.analysis_transition_strings.append(f"{measuresSecondsMap[currMeasureIndex]['offsetSeconds'] + measuresSecondsMap[currMeasureIndex]['durationSeconds']*(thisChord.beat-1)/CurrMeasuresRestless.duration.quarterLength:.1f} {self.HarmonicStateMachine.getCadentialOutput().value}")
 
-                #if self.HarmonicStateMachine.PACPending and len(LyricPerBeat) > 0:  # PAC reversion at end of measure in case PAC state was not exited within the measure
-                #    for i,curr_tup in enumerate(LyricPerBeat):
-                #        if 'PAC' in curr_tup[1]:
-                #            UpdatedLyric = "IAC"
-                #            LyricPerBeat[i] = [curr_tup[0], UpdatedLyric]
-                #            print("Reverting last PAC to IAC")
-
                 #checking cadences on entire measure
                 for LyricTuple in LyricPerBeat:
                     Lyric = LyricTuple[1]
-                    if "PAC" in Lyric or "IAC" in Lyric or "HC" in Lyric or "PCC" in Lyric:
+                    LyricsToPrint = ["PAC", "IAC", "HC", "PCC", "PCH"]
+                    if any([s in Lyric for s in LyricsToPrint]):
                         # incomplete and empty counters count measures that should be discarded
                         measure_to_write = measure_number - self.hasPickupMeasure - empty_measure_counter
                         print('Measure ', measure_to_write, ' offset ', measuresSecondsMap[currMeasureIndex]['offsetSeconds'], " ", Lyric)
                         self.analysis_full.append({"Measure": measure_to_write, "Offset": measuresSecondsMap[currMeasureIndex]['offsetSeconds'], "Lyric": Lyric})
                     elif "Key" in Lyric:
                         print(Lyric)
 
@@ -816,15 +845,15 @@
                 #LyricPerBeat.append((1, f'{currKeyString} {self.CurrSmoothedInterpretations[currKeyString]}'))
                 #LyricPerBeat.append((1, f'{challengerKeyString} {self.CurrSmoothedInterpretations[challengerKeyString]}'))
 
                 # write coefs per measure for offline analysis
                 coefs_per_measure.append(copy.deepcopy(self.CurrSmoothedInterpretations))
 
                 Parts = CurrMeasuresNotes.recurse().getElementsByClass(m21.stream.Part)
-                Lyrics_to_filter = ['CA'] # for filtering the display
+                Lyrics_to_filter = ['CA', '{', '}'] # for filtering the display
                 for thisLyric in LyricPerBeat:
                     if thisLyric[1] not in Lyrics_to_filter:
                         found = 0
                         for index in range(0, self.NumParts):
                             for thisNote in Parts[-1-index].flat.notesAndRests:  # adding lyric from last part up, assuming its the bass line
                                 if thisNote.beat == thisLyric[0]:
                                     thisNote.lyric = thisLyric[1]
@@ -844,115 +873,206 @@
 
         for c in self.ChordStreamRestless.recurse().getElementsByClass('Chord'):
             c.closedPosition(forceOctave=4, inPlace=True)
         # this adds the restless chord stream to the note stream
         # self.NoteStream.insert(0, self.ChordStream)
         self.filter_notestream_by_language_model()
         self.filter_analysis_by_language_model()
+        self.cleanup_lyrics(['{', '}'])
         self.write_analysis_to_files()
 
         if self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothingCadenceSensitive or self.KeyDetectionMode == CDKeyDetectionModes.KSWithSmoothing:
             print("Writing cadence corrected keys to file...")
             keyfileName = self.fileName.replace(".", "_")
             FullPath = os.path.join(self.WritePath, keyfileName)
             KeyFile = f"{FullPath}_Key_{self.KeyDetectionMode}.txt"
             with open(KeyFile, 'wb') as f:
                 pickle.dump(self.CorrectedKeyPerMeasure, f)
             CoefsFile = f"{FullPath}_Coefs_{self.KeyDetectionMode}.txt"
             with open(CoefsFile, 'wb') as f:
                 pickle.dump(coefs_per_measure, f)
 
+    def isilos(self, sub, list_or_string):
+        if isinstance(list_or_string, list):
+            ret_val = any(sub in s for s in list_or_string)
+        else:
+            ret_val = sub in list_or_string
+        return ret_val
+
+    def cleanup_lyrics(self, lyric_list):
+        print('cleaning up lyrics')
+        for part in self.Parts:
+            for measure in part.recurse().getElementsByClass(m21.stream.Measure):
+                for thisNote in measure.recurse().getElementsByClass(m21.note.GeneralNote):
+                    for lyric in lyric_list:
+                        thisNote.lyric = thisNote.lyric.replace(lyric, '')
 
     def filter_notestream_by_language_model(self):
         print('Filtering lyrics by language model...')
         PrevMeasureNotes = None
         PrevMeasureLyrics = None
-        PrevParts = None
+        AnchorCadenceMeasureNumber = 0
+        PrevParts = []
+        empty_measure_counter = 0
         for currMeasureIndex in range(0, self.NumMeasures):
+            if self.EmptyMeasures[currMeasureIndex]:
+                empty_measure_counter = empty_measure_counter + 1
+                continue
             measure_number = currMeasureIndex + 1
-            CurrMeasuresNotes = self.NoteStream.measure(measure_number)
-            CurrParts = CurrMeasuresNotes.recurse().getElementsByClass(m21.stream.Part)
-            CurrMeasuresLyrics = []
+            CurrMeasureNotes = self.NoteStream.measure(measure_number)
+            CurrParts = CurrMeasureNotes.recurse().getElementsByClass(m21.stream.Part)
+
+            measure_number_for_score = measure_number - self.hasPickupMeasure - empty_measure_counter
+            even_meas_since_anchor = (measure_number_for_score - AnchorCadenceMeasureNumber) % 2 == 0
+
+            CurrMeasureLyrics = []
             for part in CurrParts:
                 for thisNote in part.flat.notesAndRests:
-                    CurrMeasuresLyrics.append(thisNote.lyric)
+                    CurrMeasureLyrics.append(thisNote.lyric)
+
+            def remove_lyric_from_parts(lyric_list, parts):
+                for part in parts:
+                    for thisNote in part.flat.notesAndRests:
+                        for lyric in lyric_list:
+                            thisNote.lyric = thisNote.lyric.replace(lyric, '')
+
             if PrevMeasureNotes and PrevMeasureLyrics:
-                # PAC, HC or PCC cancel previous HC
-                if 'HC' in PrevMeasureLyrics and ('PAC' in CurrMeasuresLyrics or 'HC' in CurrMeasuresLyrics or 'PCC' in CurrMeasuresLyrics):
-                    print(f'Filtering HC in measure {measure_number-1}')
-                    for part in PrevParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('HC', '')
-                # PAC and PCC cancels HC in same measure
-                if 'HC' in CurrMeasuresLyrics and ('PAC' in CurrMeasuresLyrics or 'PCC' in CurrMeasuresLyrics):
-                    print(f'Filtering HC in measure {measure_number}')
-                    for part in CurrParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('HC', '')
-                # HC cancels previous IAC
-                if 'IAC' in PrevMeasureLyrics and 'HC' in CurrMeasuresLyrics:
-                    print(f'Filtering IAC in measure {measure_number - 1}')
-                    for part in PrevParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('IAC', '')
-                # HC cancels current IAC
-                if 'HC' in CurrMeasuresLyrics and 'IAC' in CurrMeasuresLyrics:
-                    print(f'Filtering IAC in measure {measure_number}')
-                    for part in CurrParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('IAC', '')
-                # HC cancels forward IAC
-                if 'HC' in PrevMeasureLyrics and 'IAC' in CurrMeasuresLyrics:
-                    print(f'Filtering IAC in measure {measure_number}')
-                    for part in CurrParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('IAC', '')
-                # PAC cancels forward HC
-                if 'PAC' in PrevMeasureLyrics and 'HC' in CurrMeasuresLyrics:
-                    print(f'Filtering HC in measure {measure_number}')
-                    for part in CurrParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('HC', '')
-                if 'PAC' in CurrMeasuresLyrics and 'HC' in CurrMeasuresLyrics:
-                    print(f'Filtering HC in measure {measure_number}')
-                    for part in CurrParts:
-                        for thisNote in part.flat.notesAndRests:
-                            thisNote.lyric = thisNote.lyric.replace('HC', '')
-            PrevMeasureNotes = CurrMeasuresNotes
-            PrevMeasureLyrics = CurrMeasuresLyrics
+                # HC --> PAC
+                if (self.isilos('HC', PrevMeasureLyrics) or self.isilos('PCH', PrevMeasureLyrics)) and (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)):
+                    if even_meas_since_anchor:
+                        print(f'Filtering HC in measure {measure_number_for_score-1}')
+                        remove_lyric_from_parts(['HC', 'PCH'], PrevParts)
+                # PAC --> HC
+                if self.isilos('PAC', PrevMeasureLyrics) and (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)):
+                    if not even_meas_since_anchor:
+                        print(f'Filtering HC in measure {measure_number_for_score}')
+                        remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
+                # PAC + HC
+                if (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)) and (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)):
+                    print(f'Filtering HC in measure {measure_number_for_score}')
+                    remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
+                # HC --> IAC
+                if (self.isilos('HC', PrevMeasureLyrics) or self.isilos('PCH', PrevMeasureLyrics)) and (self.isilos('IAC', CurrMeasureLyrics)):
+                    if even_meas_since_anchor:
+                        print(f'Filtering HC in measure {measure_number_for_score - 1}')
+                        remove_lyric_from_parts(['HC','PCH'], PrevParts)
+                    else:
+                        print(f'Filtering IAC in measure {measure_number_for_score}')
+                        remove_lyric_from_parts(['IAC'], CurrParts)
+                # IAC --> HC
+                if self.isilos('IAC', PrevMeasureLyrics) and (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)):
+                    if even_meas_since_anchor:
+                        print(f'Filtering IAC in measure {measure_number_for_score - 1}')
+                        remove_lyric_from_parts(['IAC'], PrevParts)
+                    else:
+                        print(f'Filtering HC in measure {measure_number_for_score}')
+                        remove_lyric_from_parts(['HC', 'PCH'], CurrParts)
+                # HC+IAC
+                if (self.isilos('HC', CurrMeasureLyrics) or self.isilos('PCH', CurrMeasureLyrics)) and self.isilos('IAC', CurrMeasureLyrics):
+                    print(f'Filtering IAC in measure {measure_number_for_score}')
+                    remove_lyric_from_parts(['IAC'], CurrParts)
+                # PAC+IAC
+                if (self.isilos('PAC', CurrMeasureLyrics) or self.isilos('PCC', CurrMeasureLyrics)) and self.isilos('IAC', CurrMeasureLyrics):
+                    print(f'Filtering IAC in measure {measure_number_for_score}')
+                    remove_lyric_from_parts(['IAC'], CurrParts)
+                # PAC --> IAC
+                if (self.isilos('PAC', PrevMeasureLyrics) or self.isilos('PCC', PrevMeasureLyrics)) and self.isilos('IAC', CurrMeasureLyrics):
+                    print(f'Filtering IAC in measure {measure_number_for_score}')
+                    remove_lyric_from_parts(['IAC'], CurrParts)
+
+            # get lyrics again after filtering
+            CurrMeasureLyrics = []
+            for part in CurrParts:
+                for thisNote in part.flat.notesAndRests:
+                    CurrMeasureLyrics.append(thisNote.lyric)
+            PrevMeasureLyrics = []
+            for part in PrevParts:
+                for thisNote in part.flat.notesAndRests:
+                    PrevMeasureLyrics.append(thisNote.lyric)
+
+            # update anchor cadence from prev part
+            anchor_cad_strings = ['PAC', 'PCC']
+            if PrevMeasureLyrics and any(self.isilos(s, PrevMeasureLyrics) for s in anchor_cad_strings):
+                AnchorCadenceMeasureNumber = measure_number_for_score - 1
+
+            PrevMeasureNotes = CurrMeasureNotes
+            PrevMeasureLyrics = CurrMeasureLyrics
             PrevParts = CurrParts
 
+
     def filter_analysis_by_language_model(self):
         print('Filtering analysis results by language model...')
         self.analysis_full_filtered = copy.deepcopy(self.analysis_full)
         items_to_remove = []
-        prev_cad = None
+        prev_cad = {'Measure':0, 'Lyric':[]}
+        anchor_cad = {'Measure':0, 'Lyric':[]}
         for item in self.analysis_full_filtered:
             curr_cad = item
-            if prev_cad:
-                if curr_cad['Measure'] - prev_cad['Measure'] <= 1:
-                    # PAC, HC or PCC cancel previous HC
-                    if prev_cad['Lyric'] == 'HC' and curr_cad['Lyric'] in ['PAC', 'HC', 'PCC']:
-                        print(f"Filtering HC in measure {prev_cad['Measure']}")
-                        if prev_cad not in items_to_remove: items_to_remove.append(prev_cad)
-                    # HC cancels IAC backward
-                    if prev_cad['Lyric'] == 'IAC' and curr_cad['Lyric'] == 'HC':
+            # check if cadence in analysis line
+            cad_strings = ['PAC', 'PCC', 'HC', 'PCH', 'IAC']
+            if not any(s in curr_cad['Lyric'] for s in cad_strings):
+                continue
+            even_meas_since_anchor = (curr_cad['Measure'] - anchor_cad['Measure']) % 2 == 0
+            if curr_cad['Measure'] - prev_cad['Measure'] <= 1:
+                # HC --> PAC and HC+PAC
+                if ('HC' in prev_cad['Lyric'] or 'PCH' in prev_cad['Lyric']) and ('PAC' in curr_cad['Lyric'] or 'PCC' in curr_cad['Lyric']):
+                    if even_meas_since_anchor:
+                        if prev_cad not in items_to_remove:
+                            print(f"Filtering HC in measure {prev_cad['Measure']}")
+                            items_to_remove.append(prev_cad)
+                # PAC --> HC and PAC+HC
+                if ('PAC' in prev_cad['Lyric'] or 'PCC' in prev_cad['Lyric']) and ('HC' in curr_cad['Lyric'] or 'PCH' in curr_cad['Lyric']):
+                    if not even_meas_since_anchor or curr_cad['Measure'] == prev_cad['Measure']:
+                        if curr_cad not in items_to_remove:
+                            print(f"Filtering HC in measure {curr_cad['Measure']}")
+                            items_to_remove.append(curr_cad)
+                # HC --> IAC
+                if ('HC' in prev_cad['Lyric'] or 'PCH' in prev_cad['Lyric']) and 'IAC' in curr_cad['Lyric']:
+                    if even_meas_since_anchor and curr_cad['Measure'] > prev_cad['Measure']:
+                        if prev_cad not in items_to_remove:
+                            print(f"Filtering HC in measure {prev_cad['Measure']}")
+                            items_to_remove.append(prev_cad)
+                    else:
+                        if curr_cad not in items_to_remove:
+                            print(f"Filtering IAC in measure {curr_cad['Measure']}")
+                            items_to_remove.append(curr_cad)
+                # IAC --> HC
+                if 'IAC' in prev_cad['Lyric'] and ('HC' in curr_cad['Lyric'] or 'PCH' in curr_cad['Lyric']):
+                    if even_meas_since_anchor or curr_cad['Measure'] == prev_cad['Measure']:
+                        if prev_cad not in items_to_remove:
+                            print(f"Filtering IAC in measure {prev_cad['Measure']}")
+                            items_to_remove.append(prev_cad)
+                    else:
+                        if curr_cad not in items_to_remove:
+                            print(f"Filtering HC in measure {curr_cad['Measure']}")
+                            items_to_remove.append(curr_cad)
+                # IAC --> PAC
+                if 'IAC' in prev_cad['Lyric'] and ('PAC' in curr_cad['Lyric'] or 'PCC' in curr_cad['Lyric']):
+                    if prev_cad not in items_to_remove:
                         print(f"Filtering IAC in measure {prev_cad['Measure']}")
-                        if prev_cad not in items_to_remove: items_to_remove.append(prev_cad)
-                    # HC cancels IAC forward
-                    if prev_cad['Lyric'] == 'HC' and curr_cad['Lyric'] == 'IAC':
+                        items_to_remove.append(prev_cad)
+                # PAC --> IAC
+                if 'IAC' in curr_cad['Lyric'] and ('PAC' in prev_cad['Lyric'] or 'PCC' in prev_cad['Lyric']):
+                    if curr_cad not in items_to_remove:
                         print(f"Filtering IAC in measure {curr_cad['Measure']}")
-                        if curr_cad not in items_to_remove: items_to_remove.append(curr_cad)
-                    # PAC cancels HC forward
-                    if prev_cad['Lyric'] == 'PAC' and curr_cad['Lyric'] == 'HC':
-                        print(f"Filtering HC in measure {curr_cad['Measure']}")
-                        if curr_cad not in items_to_remove: items_to_remove.append(curr_cad)
-            prev_cad = curr_cad
+                        items_to_remove.append(curr_cad)
+
+
+            # update cadence only if not removed
+            if curr_cad not in items_to_remove:
+                if prev_cad not in items_to_remove:
+                    # update anchor cadence only on PAC and HC
+                    anchor_cad_strings = ['PAC', 'PCC']
+                    if any(s in prev_cad['Lyric'] for s in anchor_cad_strings):
+                        anchor_cad = prev_cad
+                # update prev cad always
+                prev_cad = curr_cad
+
         for item in items_to_remove:
-            self.analysis_full_filtered.remove(item)
+            self.analysis_full_filtered = list(filter(lambda a: a != item, self.analysis_full_filtered))
 
     def write_analysis_to_files(self):
         fileName = self.fileName.replace(".", "_")
         FullPath = os.path.join(self.WritePath, fileName)
         text_file = open(f"{FullPath}_Analyzed.txt", "w")
         print(f"NumMeasures: {self.NumMeasures}", file=text_file)
         text_fileOffsets = open(f"{FullPath}_Analyzed_OffsetsNums.txt", "w")
@@ -965,16 +1085,19 @@
                 CadString = "PAC"
             elif "IAC" in Lyric:
                 CadString = "IAC"
             elif "HC" in Lyric:
                 CadString = "HC"
             elif "PCC" in Lyric:
                 CadString = "PCC"
+            elif "PCH" in Lyric:
+                CadString = "PCH"
             CadStringToNumMap = {"PAC": CDCadentialStates.PACArrival.value, "IAC": CDCadentialStates.IACArrival.value,
-                                 "HC": CDCadentialStates.HCArrival.value, "PCC": CDCadentialStates.PCCArrival.value}
+                                 "HC": CDCadentialStates.HCArrival.value, "PCC": CDCadentialStates.PCCArrival.value,
+                                 "PCH": CDCadentialStates.PCHArrival.value}
             print(f"{item['Measure']} {item['Offset']} {CadStringToNumMap[CadString]}", file=text_fileOffsets)
 
         for item in self.analysis_transition_strings:
             print(item, file=text_fileTransitions)
 
         text_file.close()
         text_fileOffsets.close()
@@ -997,14 +1120,17 @@
         if currKeyString != self.PrevKeyString:
             tempStateMachine = copy.deepcopy(self.HarmonicStateMachine)
             if currKeyString == self.PrevChallengerKeyString:
                 self.HarmonicStateMachine = copy.deepcopy(self.HarmonicStateMachineChallenger)
                 self.HarmonicStateMachine.CadentialKeyChange = 1
             if challengerKeyString == self.PrevKeyString:
                 self.HarmonicStateMachineChallenger = copy.deepcopy(tempStateMachine)
+            # reset post cadential counters
+            self.HarmonicStateMachine.resetPostCadentialCounters()
+            self.HarmonicStateMachineChallenger.resetPostCadentialCounters()
         self.PrevKeyString = currKeyString
         self.PrevChallengerKeyString = challengerKeyString
         self.HarmonicStateMachine.IsChallenger = False
         self.HarmonicStateMachineChallenger.IsChallenger = True
 
     def setFileName(self,fileName):
         self.fileName = fileName
```

### Comparing `cadence_detector-0.1.0/src/cadence_detector/cadence_detector.py` & `cadence_detector-0.2.0/src/cadence_detector/cadence_detector.py`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.1.0/src/cadence_detector.egg-info/PKG-INFO` & `cadence_detector-0.2.0/src/cadence_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence-detector
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

