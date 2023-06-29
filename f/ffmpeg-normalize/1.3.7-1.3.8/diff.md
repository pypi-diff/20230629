# Comparing `tmp/ffmpeg-normalize-1.3.7.tar.gz` & `tmp/ffmpeg-normalize-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpeg-normalize-1.3.7.tar", last modified: Sun Oct 28 16:13:02 2018, max compression
+gzip compressed data, was "dist/ffmpeg-normalize-1.3.8.tar", last modified: Wed Nov 28 09:11:46 2018, max compression
```

## Comparing `ffmpeg-normalize-1.3.7.tar` & `ffmpeg-normalize-1.3.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/
--rw-r--r--   0 werner     (501) staff       (20)    23855 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     1086 2017-02-23 13:37:19.000000 ffmpeg-normalize-1.3.7/LICENSE
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/test/
--rw-r--r--   0 werner     (501) staff       (20)   340678 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.7/test/test.mp4
--rwxr-xr-x   0 werner     (501) staff       (20)     5682 2018-05-05 16:18:34.000000 ffmpeg-normalize-1.3.7/test/test.py
--rw-r--r--   0 werner     (501) staff       (20)       48 2018-04-15 18:38:34.000000 ffmpeg-normalize-1.3.7/test/out.mp4
--rw-r--r--   0 werner     (501) staff       (20)  2894122 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.7/test/test.wav
--rw-r--r--   0 werner     (501) staff       (20)     4176 2018-10-28 16:06:44.000000 ffmpeg-normalize-1.3.7/HISTORY.md
--rw-r--r--   0 werner     (501) staff       (20)      109 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.7/MANIFEST.in
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/
--rw-r--r--   0 werner     (501) staff       (20)     8892 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_streams.py
--rw-r--r--   0 werner     (501) staff       (20)       22 2018-10-28 16:12:21.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_version.py
--rw-r--r--   0 werner     (501) staff       (20)      454 2018-05-07 10:05:58.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_errors.py
--rw-r--r--   0 werner     (501) staff       (20)     6994 2018-08-22 10:10:30.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_ffmpeg_normalize.py
--rw-r--r--   0 werner     (501) staff       (20)    11225 2018-10-28 16:10:57.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_media_file.py
--rw-r--r--   0 werner     (501) staff       (20)      117 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     6001 2018-08-22 10:09:08.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_cmd_utils.py
--rw-r--r--   0 werner     (501) staff       (20)     1866 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/_logger.py
--rw-r--r--   0 werner     (501) staff       (20)    11326 2018-07-09 07:58:42.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    14681 2018-07-09 08:00:19.000000 ffmpeg-normalize-1.3.7/README.md
--rw-r--r--   0 werner     (501) staff       (20)     2200 2018-04-24 15:52:12.000000 ffmpeg-normalize-1.3.7/setup.py
--rw-r--r--   0 werner     (501) staff       (20)      194 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/setup.cfg
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    23855 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)        1 2018-01-23 19:40:59.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)      667 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)       69 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        5 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/requires.txt
--rw-r--r--   0 werner     (501) staff       (20)       17 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2018-10-28 16:13:02.000000 ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/dependency_links.txt
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/
+-rw-r--r--   0 werner     (501) staff       (20)    24020 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2017-02-23 13:37:19.000000 ffmpeg-normalize-1.3.8/LICENSE
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/test/
+-rw-r--r--   0 werner     (501) staff       (20)   340678 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.8/test/test.mp4
+-rwxr-xr-x   0 werner     (501) staff       (20)     5682 2018-05-05 16:18:34.000000 ffmpeg-normalize-1.3.8/test/test.py
+-rw-r--r--   0 werner     (501) staff       (20)       48 2018-04-15 18:38:34.000000 ffmpeg-normalize-1.3.8/test/out.mp4
+-rw-r--r--   0 werner     (501) staff       (20)  2894122 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.8/test/test.wav
+-rw-r--r--   0 werner     (501) staff       (20)     4257 2018-11-28 09:11:11.000000 ffmpeg-normalize-1.3.8/HISTORY.md
+-rw-r--r--   0 werner     (501) staff       (20)      109 2018-01-23 19:40:26.000000 ffmpeg-normalize-1.3.8/MANIFEST.in
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/
+-rw-r--r--   0 werner     (501) staff       (20)     8892 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_streams.py
+-rw-r--r--   0 werner     (501) staff       (20)       22 2018-11-28 09:11:11.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_version.py
+-rw-r--r--   0 werner     (501) staff       (20)      454 2018-05-07 10:05:58.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_errors.py
+-rw-r--r--   0 werner     (501) staff       (20)     6012 2018-11-28 09:11:11.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_ffmpeg_normalize.py
+-rw-r--r--   0 werner     (501) staff       (20)    11225 2018-11-28 08:53:51.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_media_file.py
+-rw-r--r--   0 werner     (501) staff       (20)      117 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     6001 2018-08-22 10:09:08.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_cmd_utils.py
+-rw-r--r--   0 werner     (501) staff       (20)     1866 2018-05-05 16:10:27.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/_logger.py
+-rw-r--r--   0 werner     (501) staff       (20)    12256 2018-11-28 09:11:11.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    14749 2018-11-28 09:11:11.000000 ffmpeg-normalize-1.3.8/README.md
+-rw-r--r--   0 werner     (501) staff       (20)     2200 2018-04-24 15:52:12.000000 ffmpeg-normalize-1.3.8/setup.py
+-rw-r--r--   0 werner     (501) staff       (20)      194 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/setup.cfg
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    24020 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)        1 2018-01-23 19:40:59.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)      667 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)       69 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        5 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       17 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2018-11-28 09:11:46.000000 ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/dependency_links.txt
```

### Comparing `ffmpeg-normalize-1.3.7/PKG-INFO` & `ffmpeg-normalize-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ffmpeg-normalize
-Version: 1.3.7
+Version: 1.3.8
 Summary: Normalize audio via ffmpeg
 Home-page: https://github.com/slhck/ffmpeg-normalize
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Description: # ffmpeg-normalize
         
@@ -185,19 +185,17 @@
         
         Output Format:
         
         - `-e EXTRA_OUTPUT_OPTIONS, --extra-output-options EXTRA_OUTPUT_OPTIONS`: Extra output options list.
         
             A list of extra ffmpeg command line arguments.
         
-            You can either use a JSON-formatted list, or a simple string of space-
-            separated arguments. If JSON is used, you need to wrap the argument in
-            quotes to prevent shell expansion and to preserve literal quotes
-            inside the string. If a simple string is used, you need to specify the
-            argument with `-e=`.
+            You can either use a JSON-formatted list (i.e., a list of comma-separated, quoted elements within square brackets), or a simple string of space-separated arguments.
+        
+            If JSON is used, you need to wrap the whole argument in quotes to prevent shell expansion and to preserve literal quotes inside the string. If a simple string is used, you need to specify the argument with `-e=`.
         
             Examples: `-e '[ "-vbr", "3" ]'` or `-e="-vbr 3"`
         
         - `-ofmt OUTPUT_FORMAT, --output-format OUTPUT_FORMAT`: Media format to use for output file(s).
         
             See `ffmpeg -formats` for a list.
         
@@ -295,14 +293,18 @@
         CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
         TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
         SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         
         # History
         
+        ## 1.3.7 (2018-11-28)
+        
+        - Clarify extra options and move to main CLI entry point
+        
         ## 1.3.7 (2018-10-28)
         
         - Copy per-stream metadata
         
         ## 1.3.6 (2018-07-09)
         
         - Update README
```

### Comparing `ffmpeg-normalize-1.3.7/LICENSE` & `ffmpeg-normalize-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/test/test.mp4` & `ffmpeg-normalize-1.3.8/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/test/test.py` & `ffmpeg-normalize-1.3.8/test/test.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/test/test.wav` & `ffmpeg-normalize-1.3.8/test/test.wav`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/HISTORY.md` & `ffmpeg-normalize-1.3.8/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 1.3.7 (2018-11-28)
+
+- Clarify extra options and move to main CLI entry point
+
 ## 1.3.7 (2018-10-28)
 
 - Copy per-stream metadata
 
 ## 1.3.6 (2018-07-09)
 
 - Update README
```

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/_streams.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/_streams.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/_ffmpeg_normalize.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/_ffmpeg_normalize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import os
-import json
 from numbers import Number
 from tqdm import tqdm
-import shlex
-
-try:
-    from json.decoder import JSONDecodeError
-except ImportError:
-    JSONDecodeError = ValueError
 
 from ._cmd_utils import get_ffmpeg_exe, ffmpeg_has_loudnorm
 from ._media_file import MediaFile
 from ._errors import FFmpegNormalizeError
 from ._logger import setup_custom_logger
 
 logger = setup_custom_logger('ffmpeg_normalize')
@@ -106,32 +99,15 @@
         self.sample_rate = int(sample_rate) if sample_rate is not None else None
         self.video_codec = video_codec
         self.video_disable = video_disable
         self.subtitle_disable = subtitle_disable
         self.metadata_disable = metadata_disable
         self.chapters_disable = chapters_disable
 
-        if extra_output_options:
-            try:
-                if isinstance(extra_output_options, str):
-                    if extra_output_options.startswith('['):
-                        try:
-                            self.extra_output_options = [str(s) for s in json.loads(extra_output_options)]
-                        except JSONDecodeError as e:
-                            self.extra_output_options = shlex.split(extra_output_options)
-                    else:
-                        self.extra_output_options = shlex.split(extra_output_options)
-                elif isinstance(extra_output_options, list):
-                    self.extra_output_options = extra_output_options
-            except Exception as e:
-                raise FFmpegNormalizeError(
-                    "Could not parse extra_options: {}".format(e)
-                )
-        else:
-            self.extra_output_options = {}
+        self.extra_output_options = extra_output_options
 
         self.output_format = output_format
         self.dry_run = dry_run
         self.debug = debug
         self.progress = progress
 
         if self.output_format and (self.audio_codec is None or 'pcm' in self.audio_codec) and \
```

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/_media_file.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/_media_file.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/_cmd_utils.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/_cmd_utils.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/_logger.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/_logger.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize/__main__.py` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import argparse
 import textwrap
 import logging
 import os
+import shlex
+import json
+
+try:
+    from json.decoder import JSONDecodeError
+except ImportError:
+    JSONDecodeError = ValueError
 
 from ._version import __version__
 from ._ffmpeg_normalize import FFmpegNormalize, NORMALIZATION_TYPES
+from ._errors import FFmpegNormalizeError
 from ._logger import setup_custom_logger
 logger = setup_custom_logger('ffmpeg_normalize')
 
 def create_parser():
     parser = argparse.ArgumentParser(
         prog="ffmpeg-normalize",
         description=textwrap.dedent("""\
@@ -257,19 +265,22 @@
         '-e', '--extra-output-options',
         type=str,
         help=textwrap.dedent("""\
         Extra output options list.
 
         A list of extra ffmpeg command line arguments.
 
-        You can either use a JSON-formatted list, or a simple string of space-
-        separated arguments. If JSON is used, you need to wrap the argument in
-        quotes to prevent shell expansion and to preserve literal quotes
-        inside the string. If a simple string is used, you need to specify the
-        argument with `-e=`.
+        You can either use a JSON-formatted list (i.e., a list of
+        comma-separated, quoted elements within square brackets), or a simple
+        string of space-separated arguments.
+
+        If JSON is used, you need to wrap the whole argument in quotes to
+        prevent shell expansion and to preserve literal quotes inside the
+        string. If a simple string is used, you need to specify the argument
+        with `-e=`.
 
         Examples: `-e '[ "-vbr", "3" ]'` or `-e="-vbr 3"`
         """)
     )
     group_format.add_argument(
         '-ofmt', '--output-format',
         type=str,
@@ -298,14 +309,30 @@
     cli_args = create_parser().parse_args()
 
     if cli_args.debug:
         logger.setLevel(logging.DEBUG)
     elif cli_args.verbose:
         logger.setLevel(logging.INFO)
 
+    # parse extra options
+    extra_output_options = []
+    if cli_args.extra_output_options:
+        try:
+            if cli_args.extra_output_options.startswith('['):
+                try:
+                    extra_output_options = [str(s) for s in json.loads(cli_args.extra_output_options)]
+                except JSONDecodeError as e:
+                    extra_output_options = shlex.split(cli_args.extra_output_options)
+            else:
+                extra_output_options = shlex.split(cli_args.extra_output_options)
+        except Exception as e:
+            raise FFmpegNormalizeError(
+                "Could not parse extra_options: {}".format(e)
+            )
+
     ffmpeg_normalize = FFmpegNormalize(
         normalization_type=cli_args.normalization_type,
         target_level=cli_args.target_level,
         print_stats=cli_args.print_stats,
         loudness_range_target=cli_args.loudness_range_target,
         # threshold=cli_args.threshold,
         true_peak=cli_args.true_peak,
@@ -315,15 +342,15 @@
         audio_bitrate=cli_args.audio_bitrate,
         sample_rate=cli_args.sample_rate,
         video_codec=cli_args.video_codec,
         video_disable=cli_args.video_disable,
         subtitle_disable=cli_args.subtitle_disable,
         metadata_disable=cli_args.metadata_disable,
         chapters_disable=cli_args.chapters_disable,
-        extra_output_options=cli_args.extra_output_options,
+        extra_output_options=extra_output_options,
         output_format=cli_args.output_format,
         dry_run=cli_args.dry_run,
         progress=cli_args.progress,
     )
 
     for index, input_file in enumerate(cli_args.input):
         if cli_args.output is not None and index < len(cli_args.output):
```

### Comparing `ffmpeg-normalize-1.3.7/README.md` & `ffmpeg-normalize-1.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -177,19 +177,17 @@
 
 Output Format:
 
 - `-e EXTRA_OUTPUT_OPTIONS, --extra-output-options EXTRA_OUTPUT_OPTIONS`: Extra output options list.
 
     A list of extra ffmpeg command line arguments.
 
-    You can either use a JSON-formatted list, or a simple string of space-
-    separated arguments. If JSON is used, you need to wrap the argument in
-    quotes to prevent shell expansion and to preserve literal quotes
-    inside the string. If a simple string is used, you need to specify the
-    argument with `-e=`.
+    You can either use a JSON-formatted list (i.e., a list of comma-separated, quoted elements within square brackets), or a simple string of space-separated arguments.
+
+    If JSON is used, you need to wrap the whole argument in quotes to prevent shell expansion and to preserve literal quotes inside the string. If a simple string is used, you need to specify the argument with `-e=`.
 
     Examples: `-e '[ "-vbr", "3" ]'` or `-e="-vbr 3"`
 
 - `-ofmt OUTPUT_FORMAT, --output-format OUTPUT_FORMAT`: Media format to use for output file(s).
 
     See `ffmpeg -formats` for a list.
```

### Comparing `ffmpeg-normalize-1.3.7/setup.py` & `ffmpeg-normalize-1.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/PKG-INFO` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ffmpeg-normalize
-Version: 1.3.7
+Version: 1.3.8
 Summary: Normalize audio via ffmpeg
 Home-page: https://github.com/slhck/ffmpeg-normalize
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Description: # ffmpeg-normalize
         
@@ -185,19 +185,17 @@
         
         Output Format:
         
         - `-e EXTRA_OUTPUT_OPTIONS, --extra-output-options EXTRA_OUTPUT_OPTIONS`: Extra output options list.
         
             A list of extra ffmpeg command line arguments.
         
-            You can either use a JSON-formatted list, or a simple string of space-
-            separated arguments. If JSON is used, you need to wrap the argument in
-            quotes to prevent shell expansion and to preserve literal quotes
-            inside the string. If a simple string is used, you need to specify the
-            argument with `-e=`.
+            You can either use a JSON-formatted list (i.e., a list of comma-separated, quoted elements within square brackets), or a simple string of space-separated arguments.
+        
+            If JSON is used, you need to wrap the whole argument in quotes to prevent shell expansion and to preserve literal quotes inside the string. If a simple string is used, you need to specify the argument with `-e=`.
         
             Examples: `-e '[ "-vbr", "3" ]'` or `-e="-vbr 3"`
         
         - `-ofmt OUTPUT_FORMAT, --output-format OUTPUT_FORMAT`: Media format to use for output file(s).
         
             See `ffmpeg -formats` for a list.
         
@@ -295,14 +293,18 @@
         CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
         TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
         SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         
         # History
         
+        ## 1.3.7 (2018-11-28)
+        
+        - Clarify extra options and move to main CLI entry point
+        
         ## 1.3.7 (2018-10-28)
         
         - Copy per-stream metadata
         
         ## 1.3.6 (2018-07-09)
         
         - Update README
```

### Comparing `ffmpeg-normalize-1.3.7/ffmpeg_normalize.egg-info/SOURCES.txt` & `ffmpeg-normalize-1.3.8/ffmpeg_normalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

