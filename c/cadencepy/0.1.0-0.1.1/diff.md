# Comparing `tmp/cadencepy-0.1.0.tar.gz` & `tmp/cadencepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadencepy-0.1.0.tar", last modified: Fri Jun  9 07:34:09 2023, max compression
+gzip compressed data, was "cadencepy-0.1.1.tar", last modified: Thu Jun 29 11:48:42 2023, max compression
```

## Comparing `cadencepy-0.1.0.tar` & `cadencepy-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:34:09.099305 cadencepy-0.1.0/
--rw-rw-rw-   0        0        0     1068 2023-06-08 19:07:44.000000 cadencepy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3189 2023-06-09 07:34:09.097293 cadencepy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2661 2023-06-08 19:07:44.000000 cadencepy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 07:34:09.081229 cadencepy-0.1.0/cadencepy.egg-info/
--rw-rw-rw-   0        0        0     3189 2023-06-09 07:34:08.000000 cadencepy-0.1.0/cadencepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-09 07:34:08.000000 cadencepy-0.1.0/cadencepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:34:08.000000 cadencepy-0.1.0/cadencepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 07:34:08.000000 cadencepy-0.1.0/cadencepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 07:34:08.000000 cadencepy-0.1.0/cadencepy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 07:34:09.093241 cadencepy-0.1.0/pycadence/
--rw-rw-rw-   0        0        0        0 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/__init__.py
--rw-rw-rw-   0        0        0      172 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/connect.sh
--rw-rw-rw-   0        0        0       99 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/disconnect.sh
--rw-rw-rw-   0        0        0       87 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/ocean_simulation.sh
--rw-rw-rw-   0        0        0     1610 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/pycadence.py
--rw-rw-rw-   0        0        0      814 2023-06-08 19:07:44.000000 cadencepy-0.1.0/pycadence/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-09 07:34:09.100314 cadencepy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-06-09 07:34:04.000000 cadencepy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:48:42.935703 cadencepy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 11:48:31.000000 cadencepy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-29 11:48:42.935703 cadencepy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-29 11:48:31.000000 cadencepy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:48:42.931703 cadencepy-0.1.1/cadencepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-29 11:48:42.000000 cadencepy-0.1.1/cadencepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 11:48:42.000000 cadencepy-0.1.1/cadencepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:48:42.000000 cadencepy-0.1.1/cadencepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:48:42.000000 cadencepy-0.1.1/cadencepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:48:42.000000 cadencepy-0.1.1/cadencepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:48:42.935703 cadencepy-0.1.1/pycadence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:48:31.000000 cadencepy-0.1.1/pycadence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 11:48:31.000000 cadencepy-0.1.1/pycadence/disconnect.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-29 11:48:31.000000 cadencepy-0.1.1/pycadence/pycadence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-29 11:48:31.000000 cadencepy-0.1.1/pycadence/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:48:42.935703 cadencepy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-29 11:48:31.000000 cadencepy-0.1.1/setup.py
```

### Comparing `cadencepy-0.1.0/LICENSE` & `cadencepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cadencepy-0.1.0/PKG-INFO` & `cadencepy-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-Metadata-Version: 2.1
-Name: cadencepy
-Version: 0.1.0
-Summary: A python SDK for running simulation and reading data from Ocean Cadence
-Home-page: https://github.com/joetho786/PyCadence
-Author: joetho786
-Author-email: thomas.2@iitj.ac.in
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyCadence
- A Python wrapper for running Cadence simulations
-
-## Installation
-1. Ocean Spectre and Python to be installed on the same device
-2. Install PyCadence using pip
-```pip install cadencepy```
-
-## Usage
-1. Make sure to have a template init.ocn file ready
-2. In the ocn file placeholder values must be marked as {{value}} as shown in the sample init.ocn file placed in the sample folder
-3. Create a screen with name ocean_simulation using the following shell command
-```shell
-screen -S ocean_simulation
-```
-4. Install and enable ocean terminal using the following shell commands
-```shell
-ocean
-```
-5. Then detach the screen using ctrl+a+d
-6. Run the following python code to run the simulation
-```python
-import pycadence.pycadence as p
-x = [1,2,3,4,5] # List of values to be substituted in the template
-default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
-p.simulate(x, default,"init.ocn","output.ocn","output.txt")
-```
-7. The result of simulation will be stored output.txt file and the output.ocn file will be the modified template file with the values substituted.
-8. The simulate function also has an argument called read_output which takes a function as an argument. This function will be called after the simulation is complete and the output.txt file is generated. The function should take the output.txt file as an argument and return a dictionary of the values to be substituted in the template file. The following code shows an example of how to use this argument.
-```python
-import pycadence.pycadence as p
-import numpy as np
-
-def read_output(output_log_path):
-    with open(output_log_path, 'r+') as fp:
-        # read an store all lines into list
-        lines = fp.readlines()
-        data=[]
-        for line in lines[2:]:
-            try:
-                temp = line.strip().split(" ")
-                # print(temp)
-                data.append([float(temp[0]),float(temp[-1])])
-            except Exception as e:
-                # print("Error in reading output file")
-                # print(e)
-                pass
-        data = np.array(data)
-    return data
-
-x = [1,2,3,4,5] # List of values to be substituted in the template
-default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
-p.simulate(x, default,"init.ocn","output.ocn","output.txt",read_output)
-```
-9. The above code will read the output.txt file and return a numpy array of the values to be substituted in the template file. The first column of the array will be substituted in the first placeholder and so on. The above code will work for any number of placeholders in the template file.
+Metadata-Version: 2.1
+Name: cadencepy
+Version: 0.1.1
+Summary: A python SDK for running simulation and reading data from Ocean Cadence
+Home-page: https://github.com/joetho786/PyCadence
+Author: joetho786
+Author-email: thomas.2@iitj.ac.in
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyCadence
+ A Python wrapper for running Cadence simulations
+
+## Installation
+1. Ocean Spectre and Python to be installed on the same device
+2. Install PyCadence using pip
+```pip install cadencepy```
+
+## Usage
+1. Make sure to have a template init.ocn file ready
+2. In the ocn file placeholder values must be marked as {{value}} as shown in the sample init.ocn file placed in the sample folder
+3. Create a screen with name ocean_simulation using the following shell command. The screen should be in the directory of the init.ocn file
+```shell
+screen -S ocean_simulation
+```
+4. Install and enable ocean terminal using the following shell commands
+```shell
+ocean
+```
+5. Then detach the screen using ctrl+a+d
+6. Run the following python code to run the simulation
+```python
+from pycadence.pycadence import Connector
+x = [1,2,3,4,5] # List of values to be substituted in the template
+default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
+p=Connector(screen_name="ocean_simulation")
+p.simulate(x, default,"init.ocn","output.ocn","output.txt")
+```
+7. The result of simulation will be stored output.txt file and the output.ocn file will be the modified template file with the values substituted.
+8. The simulate function also has an argument called read_output which takes a function as an argument. This function will be called after the simulation is complete and the output.txt file is generated. The function should take the output.txt file as an argument and return a dictionary of the values to be substituted in the template file. The following code shows an example of how to use this argument.
+```python
+from pycadence.pycadence import Connector
+import numpy as np
+
+def read_output(output_log_path):
+    with open(output_log_path, 'r+') as fp:
+        # read an store all lines into list
+        lines = fp.readlines()
+        data=[]
+        for line in lines[2:]:
+            try:
+                temp = line.strip().split(" ")
+                # print(temp)
+                data.append([float(temp[0]),float(temp[-1])])
+            except Exception as e:
+                # print("Error in reading output file")
+                # print(e)
+                pass
+        data = np.array(data)
+    return data
+
+p=Connector(screen_name="ocean_simulation")
+x = [1,2,3,4,5] # List of values to be substituted in the template
+default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
+p.simulate(x, default,"init.ocn","output.ocn","output.txt",read_output)
+```
+9. The above code will read the output.txt file and return a numpy array of the values to be substituted in the template file. The first column of the array will be substituted in the first placeholder and so on. The above code will work for any number of placeholders in the template file.
```

### Comparing `cadencepy-0.1.0/README.md` & `cadencepy-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 1. Ocean Spectre and Python to be installed on the same device
 2. Install PyCadence using pip
 ```pip install cadencepy```
 
 ## Usage
 1. Make sure to have a template init.ocn file ready
 2. In the ocn file placeholder values must be marked as {{value}} as shown in the sample init.ocn file placed in the sample folder
-3. Create a screen with name ocean_simulation using the following shell command
+3. Create a screen with name ocean_simulation using the following shell command. The screen should be in the directory of the init.ocn file
 ```shell
 screen -S ocean_simulation
 ```
 4. Install and enable ocean terminal using the following shell commands
 ```shell
 ocean
 ```
 5. Then detach the screen using ctrl+a+d
 6. Run the following python code to run the simulation
 ```python
-import pycadence.pycadence as p
+from pycadence.pycadence import Connector
 x = [1,2,3,4,5] # List of values to be substituted in the template
 default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
+p=Connector(screen_name="ocean_simulation")
 p.simulate(x, default,"init.ocn","output.ocn","output.txt")
 ```
 7. The result of simulation will be stored output.txt file and the output.ocn file will be the modified template file with the values substituted.
 8. The simulate function also has an argument called read_output which takes a function as an argument. This function will be called after the simulation is complete and the output.txt file is generated. The function should take the output.txt file as an argument and return a dictionary of the values to be substituted in the template file. The following code shows an example of how to use this argument.
 ```python
-import pycadence.pycadence as p
+from pycadence.pycadence import Connector
 import numpy as np
 
 def read_output(output_log_path):
     with open(output_log_path, 'r+') as fp:
         # read an store all lines into list
         lines = fp.readlines()
         data=[]
@@ -44,12 +45,13 @@
             except Exception as e:
                 # print("Error in reading output file")
                 # print(e)
                 pass
         data = np.array(data)
     return data
 
+p=Connector(screen_name="ocean_simulation")
 x = [1,2,3,4,5] # List of values to be substituted in the template
 default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
 p.simulate(x, default,"init.ocn","output.ocn","output.txt",read_output)
 ```
 9. The above code will read the output.txt file and return a numpy array of the values to be substituted in the template file. The first column of the array will be substituted in the first placeholder and so on. The above code will work for any number of placeholders in the template file.
```

### Comparing `cadencepy-0.1.0/cadencepy.egg-info/PKG-INFO` & `cadencepy-0.1.1/cadencepy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-Metadata-Version: 2.1
-Name: cadencepy
-Version: 0.1.0
-Summary: A python SDK for running simulation and reading data from Ocean Cadence
-Home-page: https://github.com/joetho786/PyCadence
-Author: joetho786
-Author-email: thomas.2@iitj.ac.in
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyCadence
- A Python wrapper for running Cadence simulations
-
-## Installation
-1. Ocean Spectre and Python to be installed on the same device
-2. Install PyCadence using pip
-```pip install cadencepy```
-
-## Usage
-1. Make sure to have a template init.ocn file ready
-2. In the ocn file placeholder values must be marked as {{value}} as shown in the sample init.ocn file placed in the sample folder
-3. Create a screen with name ocean_simulation using the following shell command
-```shell
-screen -S ocean_simulation
-```
-4. Install and enable ocean terminal using the following shell commands
-```shell
-ocean
-```
-5. Then detach the screen using ctrl+a+d
-6. Run the following python code to run the simulation
-```python
-import pycadence.pycadence as p
-x = [1,2,3,4,5] # List of values to be substituted in the template
-default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
-p.simulate(x, default,"init.ocn","output.ocn","output.txt")
-```
-7. The result of simulation will be stored output.txt file and the output.ocn file will be the modified template file with the values substituted.
-8. The simulate function also has an argument called read_output which takes a function as an argument. This function will be called after the simulation is complete and the output.txt file is generated. The function should take the output.txt file as an argument and return a dictionary of the values to be substituted in the template file. The following code shows an example of how to use this argument.
-```python
-import pycadence.pycadence as p
-import numpy as np
-
-def read_output(output_log_path):
-    with open(output_log_path, 'r+') as fp:
-        # read an store all lines into list
-        lines = fp.readlines()
-        data=[]
-        for line in lines[2:]:
-            try:
-                temp = line.strip().split(" ")
-                # print(temp)
-                data.append([float(temp[0]),float(temp[-1])])
-            except Exception as e:
-                # print("Error in reading output file")
-                # print(e)
-                pass
-        data = np.array(data)
-    return data
-
-x = [1,2,3,4,5] # List of values to be substituted in the template
-default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
-p.simulate(x, default,"init.ocn","output.ocn","output.txt",read_output)
-```
-9. The above code will read the output.txt file and return a numpy array of the values to be substituted in the template file. The first column of the array will be substituted in the first placeholder and so on. The above code will work for any number of placeholders in the template file.
+Metadata-Version: 2.1
+Name: cadencepy
+Version: 0.1.1
+Summary: A python SDK for running simulation and reading data from Ocean Cadence
+Home-page: https://github.com/joetho786/PyCadence
+Author: joetho786
+Author-email: thomas.2@iitj.ac.in
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyCadence
+ A Python wrapper for running Cadence simulations
+
+## Installation
+1. Ocean Spectre and Python to be installed on the same device
+2. Install PyCadence using pip
+```pip install cadencepy```
+
+## Usage
+1. Make sure to have a template init.ocn file ready
+2. In the ocn file placeholder values must be marked as {{value}} as shown in the sample init.ocn file placed in the sample folder
+3. Create a screen with name ocean_simulation using the following shell command. The screen should be in the directory of the init.ocn file
+```shell
+screen -S ocean_simulation
+```
+4. Install and enable ocean terminal using the following shell commands
+```shell
+ocean
+```
+5. Then detach the screen using ctrl+a+d
+6. Run the following python code to run the simulation
+```python
+from pycadence.pycadence import Connector
+x = [1,2,3,4,5] # List of values to be substituted in the template
+default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
+p=Connector(screen_name="ocean_simulation")
+p.simulate(x, default,"init.ocn","output.ocn","output.txt")
+```
+7. The result of simulation will be stored output.txt file and the output.ocn file will be the modified template file with the values substituted.
+8. The simulate function also has an argument called read_output which takes a function as an argument. This function will be called after the simulation is complete and the output.txt file is generated. The function should take the output.txt file as an argument and return a dictionary of the values to be substituted in the template file. The following code shows an example of how to use this argument.
+```python
+from pycadence.pycadence import Connector
+import numpy as np
+
+def read_output(output_log_path):
+    with open(output_log_path, 'r+') as fp:
+        # read an store all lines into list
+        lines = fp.readlines()
+        data=[]
+        for line in lines[2:]:
+            try:
+                temp = line.strip().split(" ")
+                # print(temp)
+                data.append([float(temp[0]),float(temp[-1])])
+            except Exception as e:
+                # print("Error in reading output file")
+                # print(e)
+                pass
+        data = np.array(data)
+    return data
+
+p=Connector(screen_name="ocean_simulation")
+x = [1,2,3,4,5] # List of values to be substituted in the template
+default = [1,2,3,4,5] # List of default values to be substituted in the template in case of error
+p.simulate(x, default,"init.ocn","output.ocn","output.txt",read_output)
+```
+9. The above code will read the output.txt file and return a numpy array of the values to be substituted in the template file. The first column of the array will be substituted in the first placeholder and so on. The above code will work for any number of placeholders in the template file.
```

### Comparing `cadencepy-0.1.0/pycadence/utils.py` & `cadencepy-0.1.1/pycadence/utils.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.1.0/setup.py` & `cadencepy-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readall(path):
     with open(path) as fp:
         return fp.read()
 
 setup(
     name="cadencepy",
-    version="0.1.0",
+    version="0.1.1",
     author="joetho786",
     author_email="thomas.2@iitj.ac.in",
     description="A python SDK for running simulation and reading data from Ocean Cadence",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/joetho786/PyCadence",
     packages=find_packages(),
```

