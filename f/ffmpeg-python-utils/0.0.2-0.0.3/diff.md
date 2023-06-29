# Comparing `tmp/ffmpeg_python_utils-0.0.2.tar.gz` & `tmp/ffmpeg_python_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_python_utils-0.0.2.tar", last modified: Wed Jun 28 21:58:23 2023, max compression
+gzip compressed data, was "ffmpeg_python_utils-0.0.3.tar", last modified: Thu Jun 29 13:29:24 2023, max compression
```

## Comparing `ffmpeg_python_utils-0.0.2.tar` & `ffmpeg_python_utils-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 21:58:23.833502 ffmpeg_python_utils-0.0.2/
--rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      808 2023-06-28 21:58:23.833502 ffmpeg_python_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1501 2023-06-28 21:05:28.000000 ffmpeg_python_utils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 21:58:23.826502 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/
--rw-rw-rw-   0        0        0     1043 2023-06-28 19:38:55.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/__init__.py
--rw-rw-rw-   0        0        0     1209 2023-06-28 21:45:35.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/config.py
--rw-rw-rw-   0        0        0     4969 2023-06-28 13:56:26.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/inc.py
--rw-rw-rw-   0        0        0    37269 2023-06-28 21:37:28.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/main.py
--rw-rw-rw-   0        0        0     8059 2023-06-28 21:33:03.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/other.py
-drwxrwxrwx   0        0        0        0 2023-06-28 21:58:23.832504 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/
--rw-rw-rw-   0        0        0      808 2023-06-28 21:58:23.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-28 21:58:23.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 21:58:23.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-28 21:58:23.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-28 21:58:23.000000 ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 21:58:23.834502 ffmpeg_python_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-28 21:57:53.000000 ffmpeg_python_utils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:29:24.005845 ffmpeg_python_utils-0.0.3/
+-rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-06-29 13:29:24.005845 ffmpeg_python_utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-06-28 22:10:37.000000 ffmpeg_python_utils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:29:23.997845 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/
+-rw-rw-rw-   0        0        0     1043 2023-06-28 19:38:55.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-06-29 13:01:42.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/config.py
+-rw-rw-rw-   0        0        0     4983 2023-06-29 09:14:35.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/inc.py
+-rw-rw-rw-   0        0        0    37683 2023-06-29 12:27:38.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/main.py
+-rw-rw-rw-   0        0        0     8059 2023-06-28 21:33:03.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/other.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:29:24.004843 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:29:24.006846 ffmpeg_python_utils-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-29 13:28:36.000000 ffmpeg_python_utils-0.0.3/setup.py
```

### Comparing `ffmpeg_python_utils-0.0.2/LICENSE` & `ffmpeg_python_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.2/PKG-INFO` & `ffmpeg_python_utils-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg_python_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.2.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.3.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.2/README.md` & `ffmpeg_python_utils-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Notes
+This library provides functions that create and execute ffmpeg commands using subprocess in Python.
 
 There are good libraries for video editing, such as Moviepy. However, I encountered multiple errors that I could not overcome. 
 
 This library is straightforward but it works. During some activities, I ended up with a bunch of functions that create and start pure ffmpeg scripts with subprocess. So, I decided to publish it here. 
 
-I'm still a novice with ffmpeg and would appreciate some feedback. The project has GPU acceleration set up for Nvidia and AMD, but I don't have an AMD card, so the project needs feedback here. Also, I don't have experience with Linux, so there may be some problems with paths. The project needs feedback here as well.
+There may be some ```issues```. I'm still a novice with ffmpeg and would appreciate some feedback. The project has GPU acceleration set up for Nvidia and AMD, but I don't have an AMD card, so the project needs feedback here. Also, I don't have experience with Linux, so there may be some problems with paths. The project needs feedback here as well.
 
 ## Setting up
 1) First, you need to install it:
 
    ```
    pip install ffmpeg-python-utils
    ```
```

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/__init__.py` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/config.py` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 C_CODEC = 'nvidia'  # nvidia, amd, cpu
 """
-The codec we will use during the project.
+The codec we use.
 """
 # TODO: Find the right settings for AMD.
 C_CODEC_SETTINGS = {
-    'nvidia': '-c:v h264_nvenc -profile:v high -tune hq -rc-lookahead 8 -bf 2 -rc vbr -cq 26 -b:v 0 -maxrate 120M -bufsize 240M',
+    'nvidia': '-c:v h264_nvenc -profile:v high -tune hq -rc-lookahead 8 -bf 2 -rc vbr -cq 10 -b:v 0 -maxrate 120M -bufsize 240M',
     'amd': '-c:v h264_amf',
-    'cpu': '-c:v libx264',
+    'cpu': '-c:v libx264 -crf 15',
 }
 """
 Specific settings for the codec. Nvidia is described here: 
 "https://video.stackexchange.com/questions/29659/is-there-a-way-to-improve-h264-nvenc-output-quality"
+"https://superuser.com/questions/1236275/how-can-i-use-crf-encoding-with-nvenc-in-ffmpeg"
+The default crf for cpu is 23. The higher the crf or cq, the worse the quality, but the smaller the file size.
 """
 
 C_TO_PRINT_PACKAGE_INFO = True
 """Whether to show package info."""
-C_TO_PRINT_EXECUTION_TIME = False
+C_TO_PRINT_EXECUTION_TIME = True
 """Whether to show each function's execution time."""
 
+C_TO_SAVE_LOGS = False
+"""Whether to save ffmpeg logs."""
 C_TO_PRINT_ONLY_FFMPEG_ERRORS = False
 """Whether to print only ffmpeg errors. C_TO_PRINT_ONLY_FFMPEG_ERRORS > C_TO_PRINT_FFMPEG_DEBUG. The code first 
 checks if to print only errors."""
 C_TO_PRINT_FFMPEG_DEBUG = False
 """Whether to show detailed information from ffmpeg."""
-C_TO_SAVE_LOGS = False
-"""Whether to save ffmpeg logs."""
 
 C_TO_RENAME_FILES = False
 """Whether to rename files. It should work with False."""
-C_TO_PRINT_PLOTS = False
+C_TO_PRINT_PLOTS = True
 """Whether to show plots during finding offsets before proceeding."""
```

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/inc.py` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/inc.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     with open(output_path, 'w') as file:
         file.write(string)
     return output_path
 
 def get_codec_meeting_constraints(sizes):
     """
     Function checks if current codec meets specific codec sizes constraint (min 145 for width/height for nvidia).
-    Checks only if size is integer. It takes in account if size is -1.
+    Checks only if size is integer. It proceeds to the next one if size is -1.
     TODO i don't know amd constraints so project needs some update here
     :param sizes: list of pair-sizes or just pair-sizes
     :return: codec to use
     """
     if C_CODEC == 'cpu':
         return C_CODEC
     elif C_CODEC == 'amd':
@@ -121,11 +121,11 @@
                 if isinstance(size, int) and size != -1:
                     if size < 145:
                         use_cpu = True
                         break
         if use_cpu:
             print_info(
                 f'Width or height is less then 145, which is not compatible with nvidia codec. '
-                f'Using libx264 instead.',
+                f'Using cpu (libx264) instead.',
                 'red', C_TO_PRINT_PACKAGE_INFO)
             return 'cpu'
     return C_CODEC
```

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/main.py` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     # Clear tmp file
     if command_file:
         os.remove(command_file)
     # Calculate the time it took. Since ffprobe is lightning fast we do not use it there
     if not is_ffprobe:
         time_diff = datetime.datetime.now() - start_time
         time_diff_seconds = time_diff.total_seconds()
-        print_info(f"Time it took (seconds): {round(time_diff_seconds, 3)}.", 'green', C_TO_PRINT_EXECUTION_TIME)
+        print_info(f"Time it took (seconds): {time_diff_seconds:.2f}.", 'green', C_TO_PRINT_EXECUTION_TIME)
     return res
 
 
 @process
 def add_rectangle_to_video(input_path: str, output_path: str, start_times: list[float], durations: list[float],
                            x_y_coordinates: list[list], sizes: list[list], rect_colors: list[str],
                            opacities: list[float]) -> str:
@@ -445,18 +445,19 @@
           f' -c:a copy "{output_path}"'
     run_command(cmd, filter_str_0 + filter_str_1)
 
     return output_path
 
 
 @process
-def get_concantenated_videos(input_video_paths: list[str], output_path: str, effects: list[str],
-                             transition_durations: list[float]) -> str:
+def get_concantenated_videos(input_video_paths: list[str], output_path: str, effects: list[str] = None,
+                             transition_durations: list[float] = None) -> str:
     """
     Concatenates multiple videos together using ffmpeg.
+    If effects is False-like, then no transition_duration implemented.
 
     Args:
         input_video_paths (list[str]): A list of paths to the input video files.
         output_path (str): The path to the output video file.
         effects (list[str]): A list of transition effects to use between each video. See https://trac.ffmpeg.org/wiki/Xfade for options.
         transition_durations (list[float]): A list of durations for each transition.
 
@@ -470,42 +471,50 @@
     # Get input video durations
     video_durations = []
     sizes = []
     for input_video_path in input_video_paths:
         video_info = get_video_info(input_video_path)
         video_durations.append(video_info['duration'])
         sizes.append([video_info['width'], video_info['height']])
-
-    # Checking for codec
+    # Checking codec
     codec_to_use = get_codec_meeting_constraints(sizes)
 
+
+    # We need this only if effects present
     # Calculate offset time
     offsets = []
-    for i in range(len(video_durations)):
-        offset = video_durations[i] - transition_durations[i]
-        offset += offsets[i - 1] if i > 0 else 0
-        offsets.append(offset)
+    if effects:
+        for i in range(len(video_durations)):
+            offset = video_durations[i] - transition_durations[i]
+            offset += offsets[i - 1] if i > 0 else 0
+            offsets.append(offset)
 
     # Construct input and filter str
     input_str = ''
     filter_vid_str = ''
     filter_aud_str = ''
     for i in range(len(input_video_paths)):
         input_str += f'-i "{input_video_paths[i]}" '
-    for i in range(len(input_video_paths) - 1):
-        filter_vid_str += f'[0]' if i == 0 else f'[vv{i}]'
-        filter_aud_str += f'[0:a]' if i == 0 else f'[afade{i}]'
-        filter_vid_str += f'[{i + 1}:v]xfade=transition={effects[i]}:duration=1:offset={offsets[i]},format=yuv420p[vv{i + 1}];'
-        filter_aud_str += f'[{i + 1}:a]acrossfade=d={transition_durations[i]}[afade{i + 1}];'
+        if not effects:
+            filter_vid_str += f'[{i}:v][{i}:a]'
+    if effects:
+        for i in range(len(input_video_paths) - 1):
+            filter_vid_str += f'[0]' if i == 0 else f'[vv{i}]'
+            filter_aud_str += f'[0:a]' if i == 0 else f'[afade{i}]'
+            filter_vid_str += f'[{i + 1}:v]xfade=transition={effects[i]}:duration=1:offset={offsets[i]},format=yuv420p[vv{i + 1}];'
+            filter_aud_str += f'[{i + 1}:a]acrossfade=d={transition_durations[i]}[afade{i + 1}];'
+
+    filter_vid_str += f'concat=n={len(input_video_paths)}:v=1:a=1[outv]' if not effects else ''
+    map_str = f'-map "[afade{len(input_video_paths) - 1}]" -map "[vv{len(input_video_paths) - 1}]"' if effects else '-map [outv]'
 
     # Run command
     cmd = f'ffmpeg -y {input_str}-movflags +faststart ' \
           f'-filter_complex "{filter_vid_str + filter_aud_str}" ' \
-          f'{C_CODEC_SETTINGS[codec_to_use]} -map "[vv{len(input_video_paths) - 1}]" ' \
-          f'-map "[afade{len(input_video_paths) - 1}]" -fps_mode vfr "{output_path}"'
+          f'{map_str} {C_CODEC_SETTINGS[codec_to_use]} ' \
+          f'-fps_mode vfr "{output_path}"'
     run_command(cmd, filter_vid_str + filter_aud_str)
     return output_path
 
 
 @process
 def get_image_info(input_image_path: str) -> dict:
     """
@@ -596,15 +605,15 @@
     Returns:
         str: The path to the cropped video file.
     """
     codec_to_use = get_codec_meeting_constraints(size)
     filter_str = f"crop={size[0]}:{size[1]}:{x_y_coordinate[0]}:{x_y_coordinate[1]}"
     # Crop the video
     cmd = f'ffmpeg -y -i "{input_video_path}" -movflags use_metadata_tags -movflags +faststart -filter_complex "{filter_str}" ' \
-          f'-crf 17 -preset slow {C_CODEC_SETTINGS[codec_to_use]} -c:a copy "{output_path}" '
+          f' -preset slow {C_CODEC_SETTINGS[codec_to_use]} -c:a copy "{output_path}" '
     run_command(cmd, filter_str)
     return output_path
 
 
 @process
 def get_resized_video(input_video_path: str, output_path: str, size: list) -> str:
     """
```

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils/other.py` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/other.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.2/ffmpeg_python_utils.egg-info/PKG-INFO` & `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg-python-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.2.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.3.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.2/setup.py` & `ffmpeg_python_utils-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '0.0.2'
+version = '0.0.3'
 
 description = 'Python scripts constructing ffmpeg commands and running them by subprocess.'
 
 long_description = ''' Python scripts constructing ffmpeg commands and running them by subprocess.
                     Check documentation: https://lionelcrowl.github.io/ffmpeg-python-utils/
                     '''
```

