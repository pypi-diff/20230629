# Comparing `tmp/audapa-1.0.6.tar.gz` & `tmp/audapa-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audapa-1.0.6.tar", last modified: Fri Apr 15 13:18:37 2022, max compression
+gzip compressed data, was "audapa-1.0.8.tar", last modified: Sat Apr 16 05:37:15 2022, max compression
```

## Comparing `audapa-1.0.6.tar` & `audapa-1.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-15 13:18:37.897867 audapa-1.0.6/
--rw-rw-r--   0 bc        (1000) bc        (1000)      637 2022-04-15 13:18:37.897867 audapa-1.0.6/PKG-INFO
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-15 13:18:37.893867 audapa-1.0.6/audapa/
--rw-rw-r--   0 bc        (1000) bc        (1000)     2669 2022-03-01 12:07:54.000000 audapa-1.0.6/audapa/arc.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1027 2022-02-21 05:03:18.000000 audapa-1.0.6/audapa/arcbutton.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      503 2022-03-09 04:24:44.000000 audapa-1.0.6/audapa/bar.py
--rw-------   0 bc        (1000) bc        (1000)     1606 2022-03-20 13:17:31.000000 audapa-1.0.6/audapa/blank.py
--rw-------   0 bc        (1000) bc        (1000)      643 2022-04-15 13:17:13.000000 audapa-1.0.6/audapa/build.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      684 2022-03-11 05:54:56.000000 audapa-1.0.6/audapa/delete.py
--rw-------   0 bc        (1000) bc        (1000)     1338 2022-04-03 04:57:41.000000 audapa-1.0.6/audapa/distance.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3573 2022-03-27 08:09:56.000000 audapa-1.0.6/audapa/draw.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3182 2022-04-07 03:29:21.000000 audapa-1.0.6/audapa/drawscroll.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      373 2022-04-11 04:03:05.000000 audapa-1.0.6/audapa/error.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     2253 2022-04-04 06:30:59.000000 audapa-1.0.6/audapa/forms.py
--rw-------   0 bc        (1000) bc        (1000)     1608 2022-04-08 06:22:31.000000 audapa-1.0.6/audapa/goto.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3189 2022-03-06 12:06:46.000000 audapa-1.0.6/audapa/graph.py
--rw-------   0 bc        (1000) bc        (1000)      871 2022-03-12 13:14:20.000000 audapa-1.0.6/audapa/info.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     6341 2022-04-04 17:30:32.000000 audapa-1.0.6/audapa/level.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      186 2022-02-15 10:31:44.000000 audapa-1.0.6/audapa/loop.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      704 2022-04-10 10:18:52.000000 audapa-1.0.6/audapa/main.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1382 2022-03-20 06:56:37.000000 audapa-1.0.6/audapa/move.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     2405 2022-04-02 04:15:43.000000 audapa-1.0.6/audapa/pbox.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3384 2022-04-15 13:17:04.000000 audapa-1.0.6/audapa/play.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3369 2022-04-02 04:16:03.000000 audapa-1.0.6/audapa/point.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3111 2022-04-15 13:09:02.000000 audapa-1.0.6/audapa/points.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1277 2022-03-19 12:32:48.000000 audapa-1.0.6/audapa/r_offset.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1128 2022-02-15 10:31:44.000000 audapa-1.0.6/audapa/record.py
--rw-------   0 bc        (1000) bc        (1000)      279 2022-03-09 06:18:16.000000 audapa-1.0.6/audapa/reload.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1950 2022-04-15 10:25:51.000000 audapa-1.0.6/audapa/save.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1765 2022-04-06 03:59:27.000000 audapa-1.0.6/audapa/seloff.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     4644 2022-04-02 12:25:15.000000 audapa-1.0.6/audapa/sets.py
--rw-------   0 bc        (1000) bc        (1000)     1821 2022-03-26 09:04:37.000000 audapa-1.0.6/audapa/snap.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     3356 2022-04-02 04:55:58.000000 audapa-1.0.6/audapa/spread.py
--rw-------   0 bc        (1000) bc        (1000)     1636 2022-03-25 13:28:00.000000 audapa-1.0.6/audapa/step.py
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-15 13:18:37.897867 audapa-1.0.6/audapa.egg-info/
--rw-rw-r--   0 bc        (1000) bc        (1000)      637 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      691 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/SOURCES.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        1 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/dependency_links.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       45 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/entry_points.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       63 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/requires.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        7 2022-04-15 13:18:37.000000 audapa-1.0.6/audapa.egg-info/top_level.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       38 2022-04-15 13:18:37.897867 audapa-1.0.6/setup.cfg
--rw-rw-r--   0 bc        (1000) bc        (1000)     1054 2022-04-15 13:18:02.000000 audapa-1.0.6/setup.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-16 05:37:15.744140 audapa-1.0.8/
+-rw-rw-r--   0 bc        (1000) bc        (1000)      637 2022-04-16 05:37:15.744140 audapa-1.0.8/PKG-INFO
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-16 05:37:15.740140 audapa-1.0.8/audapa/
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2669 2022-03-01 12:07:54.000000 audapa-1.0.8/audapa/arc.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1027 2022-02-21 05:03:18.000000 audapa-1.0.8/audapa/arcbutton.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      503 2022-03-09 04:24:44.000000 audapa-1.0.8/audapa/bar.py
+-rw-------   0 bc        (1000) bc        (1000)     1606 2022-03-20 13:17:31.000000 audapa-1.0.8/audapa/blank.py
+-rw-------   0 bc        (1000) bc        (1000)      643 2022-04-15 13:20:25.000000 audapa-1.0.8/audapa/build.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      684 2022-03-11 05:54:56.000000 audapa-1.0.8/audapa/delete.py
+-rw-------   0 bc        (1000) bc        (1000)     1338 2022-04-03 04:57:41.000000 audapa-1.0.8/audapa/distance.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3573 2022-03-27 08:09:56.000000 audapa-1.0.8/audapa/draw.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3182 2022-04-07 03:29:21.000000 audapa-1.0.8/audapa/drawscroll.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      373 2022-04-11 04:03:05.000000 audapa-1.0.8/audapa/error.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2253 2022-04-16 05:17:32.000000 audapa-1.0.8/audapa/forms.py
+-rw-------   0 bc        (1000) bc        (1000)     1608 2022-04-08 06:22:31.000000 audapa-1.0.8/audapa/goto.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3189 2022-03-06 12:06:46.000000 audapa-1.0.8/audapa/graph.py
+-rw-------   0 bc        (1000) bc        (1000)      871 2022-03-12 13:14:20.000000 audapa-1.0.8/audapa/info.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     6448 2022-04-16 05:17:32.000000 audapa-1.0.8/audapa/level.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      186 2022-02-15 10:31:44.000000 audapa-1.0.8/audapa/loop.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      704 2022-04-10 10:18:52.000000 audapa-1.0.8/audapa/main.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1382 2022-03-20 06:56:37.000000 audapa-1.0.8/audapa/move.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2405 2022-04-02 04:15:43.000000 audapa-1.0.8/audapa/pbox.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3384 2022-04-15 13:20:25.000000 audapa-1.0.8/audapa/play.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3369 2022-04-02 04:16:03.000000 audapa-1.0.8/audapa/point.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3111 2022-04-15 13:20:25.000000 audapa-1.0.8/audapa/points.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1380 2022-04-16 05:17:32.000000 audapa-1.0.8/audapa/r_offset.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1139 2022-04-16 05:35:23.000000 audapa-1.0.8/audapa/record.py
+-rw-------   0 bc        (1000) bc        (1000)      279 2022-03-09 06:18:16.000000 audapa-1.0.8/audapa/reload.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2014 2022-04-16 05:17:32.000000 audapa-1.0.8/audapa/save.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1765 2022-04-06 03:59:27.000000 audapa-1.0.8/audapa/seloff.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4644 2022-04-02 12:25:15.000000 audapa-1.0.8/audapa/sets.py
+-rw-------   0 bc        (1000) bc        (1000)     1821 2022-03-26 09:04:37.000000 audapa-1.0.8/audapa/snap.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     3356 2022-04-02 04:55:58.000000 audapa-1.0.8/audapa/spread.py
+-rw-------   0 bc        (1000) bc        (1000)     1636 2022-03-25 13:28:00.000000 audapa-1.0.8/audapa/step.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2022-04-16 05:37:15.744140 audapa-1.0.8/audapa.egg-info/
+-rw-rw-r--   0 bc        (1000) bc        (1000)      637 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      691 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/SOURCES.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        1 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/dependency_links.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       45 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/entry_points.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       63 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/requires.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        7 2022-04-16 05:37:15.000000 audapa-1.0.8/audapa.egg-info/top_level.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       38 2022-04-16 05:37:15.748140 audapa-1.0.8/setup.cfg
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1054 2022-04-16 05:37:01.000000 audapa-1.0.8/setup.py
```

### Comparing `audapa-1.0.6/PKG-INFO` & `audapa-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audapa
-Version: 1.0.6
+Version: 1.0.8
 Summary: Audio wave file manipulator
 Home-page: https://github.com/colin-i/audapa
 Author: colin-i
 Author-email: costin.botescu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `audapa-1.0.6/audapa/arc.py` & `audapa-1.0.8/audapa/arc.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/arcbutton.py` & `audapa-1.0.8/audapa/arcbutton.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/blank.py` & `audapa-1.0.8/audapa/blank.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/build.py` & `audapa-1.0.8/audapa/build.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/delete.py` & `audapa-1.0.8/audapa/delete.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/distance.py` & `audapa-1.0.8/audapa/distance.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/draw.py` & `audapa-1.0.8/audapa/draw.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/drawscroll.py` & `audapa-1.0.8/audapa/drawscroll.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/forms.py` & `audapa-1.0.8/audapa/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 	for i in range (0,sz):
 		if points.points[i]._offset_<draw.offset:
 			continue
 		for j in range(i,sz):
 			p=points.points[j]
 			if draw.offset+(w if drawscroll.landscape
 				 else h)<p._offset_:
-				if i>0:
+				if j>0:
 					graph.put(j,p,w,h)
 				return
 			p._put_(w,h,j)
 		return
 
 def toggle(b,a):
 	a=draw.cont
```

### Comparing `audapa-1.0.6/audapa/goto.py` & `audapa-1.0.8/audapa/goto.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/graph.py` & `audapa-1.0.8/audapa/graph.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/info.py` & `audapa-1.0.8/audapa/info.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/level.py` & `audapa-1.0.8/audapa/level.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
 
 def calculate():
 	s=len(points.points)
 	if s>=2:
 		n=0
 		start=points.points[0]._offset_
 		stop=points.points[s-1]._offset_
+		if stop>draw.length: #here and 2 more places (about samples length vs points length)
+			stop=draw.length
 		for i in range(start,stop):
 			n+=abs(draw.samples[i])
 		med=n/(stop-start)
 		#
 		a=get_size()/2
 		b=med-a
 		mid=b/a
```

### Comparing `audapa-1.0.6/audapa/main.py` & `audapa-1.0.8/audapa/main.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/move.py` & `audapa-1.0.8/audapa/move.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/pbox.py` & `audapa-1.0.8/audapa/pbox.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/play.py` & `audapa-1.0.8/audapa/play.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/point.py` & `audapa-1.0.8/audapa/point.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/points.py` & `audapa-1.0.8/audapa/points.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/r_offset.py` & `audapa-1.0.8/audapa/r_offset.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 	cged(a)
 	if sets.turn_page.get_active():
 		drawscroll.edge(a.get_value(),a.get_upper()-a.get_page_size())
 
 def calculate(pos):
 	#pos is is relative to draw
 	pos+=draw.offset
+	if pos>draw.length: #here and 2 more places (about samples length vs points length)
+		pos=draw.length
 	st=seloff.start._get_()
 	en=seloff.end._get_()
 	if st==0 and en==0:
 		seloff.start._set_(pos)
 		seloff.end._set_(pos)
 		return
 	n=abs(st-pos)
```

### Comparing `audapa-1.0.6/audapa/record.py` & `audapa-1.0.8/audapa/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 		w=sets.get_data_file(str(int(time()))+".wav")
 		wavefile = wave.open(w,'wb')
 		wavefile.setnchannels(chans)
 		wavefile.setsampwidth(audio.get_sample_size(bits))
 		wavefile.setframerate(rate)
 		#visual
 		b._set_text_(chr(0x23F9))
+		print(w)
 		return
 	stop()
 	b._set_text_(chr(ready))
 def stop():
 	# stop the stream, close it, terminate the pyaudio instantiation
 	stream.stop_stream()
 	stream.close()
```

### Comparing `audapa-1.0.6/audapa/save.py` & `audapa-1.0.8/audapa/save.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def redraw():
 	draw.surf()
 	draw.reset()
 	draw.area.queue_draw()
 
 def set(i,v):
-	try:
+	try: #here and 2 more places (about samples length vs points length)
 		draw.samples[i]=int(v) #there are troubles at write file without int
 	except:
 		pass #this can be ignored
 def apply():
 	s=len(points.points)
 	if s>=2:
 		for i in range(1,s):
```

### Comparing `audapa-1.0.6/audapa/seloff.py` & `audapa-1.0.8/audapa/seloff.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/sets.py` & `audapa-1.0.8/audapa/sets.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/snap.py` & `audapa-1.0.8/audapa/snap.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/spread.py` & `audapa-1.0.8/audapa/spread.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa/step.py` & `audapa-1.0.8/audapa/step.py`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/audapa.egg-info/PKG-INFO` & `audapa-1.0.8/audapa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audapa
-Version: 1.0.6
+Version: 1.0.8
 Summary: Audio wave file manipulator
 Home-page: https://github.com/colin-i/audapa
 Author: colin-i
 Author-email: costin.botescu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `audapa-1.0.6/audapa.egg-info/SOURCES.txt` & `audapa-1.0.8/audapa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audapa-1.0.6/setup.py` & `audapa-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pathlib
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "info.md").read_text()
 
 from setuptools import setup
 setup(name=pkname,
-	version='1.0.6',
+	version='1.0.8',
 	packages=[pkname],
 	#optionals
 	python_requires='>=3.8',
 	install_requires=[
 		"pycairo>=1.20.0","PyGObject>=3.40",
 		"appdirs>=1.4.3",
 		"PyAudio>=0.2.11"],
```

