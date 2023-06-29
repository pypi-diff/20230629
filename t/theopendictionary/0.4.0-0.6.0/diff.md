# Comparing `tmp/theopendictionary-0.4.0.tar.gz` & `tmp/theopendictionary-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theopendictionary-0.4.0.tar", max compression
+gzip compressed data, was "theopendictionary-0.6.0.tar", max compression
```

## Comparing `theopendictionary-0.4.0.tar` & `theopendictionary-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      422 2023-05-19 21:33:52.150491 theopendictionary-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-01-07 22:51:39.553380 theopendictionary-0.4.0/theopendictionary/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-04 07:15:34.237886 theopendictionary-0.4.0/theopendictionary/odict.py
--rw-r--r--   0        0        0     2405 2023-04-04 07:15:21.644772 theopendictionary-0.4.0/theopendictionary/test_odict.py
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 theopendictionary-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      422 2023-06-29 08:30:21.233423 theopendictionary-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-01-07 22:51:39.553380 theopendictionary-0.6.0/theopendictionary/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-04 07:15:34.237886 theopendictionary-0.6.0/theopendictionary/odict.py
+-rw-r--r--   0        0        0     2527 2023-06-28 20:33:43.169816 theopendictionary-0.6.0/theopendictionary/test_odict.py
+-rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 theopendictionary-0.6.0/PKG-INFO
```

### Comparing `theopendictionary-0.4.0/theopendictionary/odict.py` & `theopendictionary-0.6.0/theopendictionary/odict.py`

 * *Files identical despite different names*

### Comparing `theopendictionary-0.4.0/theopendictionary/test_odict.py` & `theopendictionary-0.6.0/theopendictionary/test_odict.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,44 @@
 
     dict.index()
 
     json = dict.search("run")
 
     expected = '[{"term":"run","etymologies":[{"id":"0","usages":{"n":{"pos":"n","definitions":["Act or instance of running, of moving rapidly using the feet.","Act or instance of hurrying (to or from a place) (not necessarily by foot); dash or errand, trip.","A pleasure trip.","Flight, instance or period of fleeing.","Migration (of fish).","A group of fish that migrate, or ascend a river for the purpose of spawning."]},"v":{"pos":"v","groups":[{"id":"","description":"A number of verb usages","definitions":["(vertebrates) To move swiftly.","(fluids) To flow.","(nautical, of a vessel) To sail before the wind, in distinction from reaching or sailing close-hauled.","(social) To carry out an activity.","To extend or persist, statically or dynamically, through space or time.","(transitive) To execute or carry out a plan, procedure or program."]}]}}}]}]'
 
-    assert len(json) == 1, "there should only be 1 item in the array"
-    assert json[0].get("term") == "run", "json should be %s, received: %s" % (
+    assert len(json) == 2, "there should only be 2 items in the array"
+
+    assert json[0].get("term") == "ran", "json should be %s, received: %s" % (
         expected,
         json,
     )
 
+    assert json[1].get("term") == "run", "json should be %s, received: %s" % (
+        expected,
+        json,
+    )
+
+
 def test_lexicon():
     xml = '<dictionary><entry term="hello"><ety><usage pos="v"><definition>hello world</definition></usage></ety></entry><entry term="world"><ety><usage pos="v"><definition>hello world</definition></usage></ety></entry></dictionary>'
 
     Dictionary.write(xml, "test.odict")
 
     dict = Dictionary("test.odict")
 
     output = dict.lexicon()
 
-    expected = ['hello', 'world']
+    expected = ["hello", "world"]
 
     assert output == expected, "lexicon should be %s, received: %s" % (
         expected,
         output,
     )
 
+
 def test_write_lookup_dictionary():
     xml = '<dictionary><entry term="hello"><ety><usage pos="v"><definition>hello world</definition></usage></ety></entry></dictionary>'
 
     Dictionary.write(xml, "test.odict")
 
     dict = Dictionary("test.odict")
```

