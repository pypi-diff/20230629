# Comparing `tmp/urdf2webots-2.0.3.tar.gz` & `tmp/urdf2webots-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urdf2webots-2.0.3.tar", last modified: Mon Nov 14 16:24:22 2022, max compression
+gzip compressed data, was "urdf2webots-2023.1.0.tar", last modified: Thu Jun 29 06:57:12 2023, max compression
```

## Comparing `urdf2webots-2.0.3.tar` & `urdf2webots-2023.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-14 16:24:22.505952 urdf2webots-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8997 2022-11-14 16:24:22.505952 urdf2webots-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-14 16:24:22.505952 urdf2webots-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      805 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-14 16:24:22.505952 urdf2webots-2.0.3/urdf2webots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/gazebo_materials.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16118 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    45999 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/parserURDF.py
--rw-r--r--   0 runner    (1001) docker     (122)    33707 2022-11-14 16:24:10.000000 urdf2webots-2.0.3/urdf2webots/writeRobot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-14 16:24:22.505952 urdf2webots-2.0.3/urdf2webots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8997 2022-11-14 16:24:22.000000 urdf2webots-2.0.3/urdf2webots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      358 2022-11-14 16:24:22.000000 urdf2webots-2.0.3/urdf2webots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-14 16:24:22.000000 urdf2webots-2.0.3/urdf2webots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-14 16:24:22.000000 urdf2webots-2.0.3/urdf2webots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-14 16:24:22.000000 urdf2webots-2.0.3/urdf2webots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:57:12.985193 urdf2webots-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-29 06:57:12.985193 urdf2webots-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:57:12.985193 urdf2webots-2023.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:57:12.985193 urdf2webots-2023.1.0/urdf2webots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/gazebo_materials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46671 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/parserURDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34222 2023-06-29 06:56:58.000000 urdf2webots-2023.1.0/urdf2webots/writeRobot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:57:12.985193 urdf2webots-2023.1.0/urdf2webots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-29 06:57:12.000000 urdf2webots-2023.1.0/urdf2webots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 06:57:12.000000 urdf2webots-2023.1.0/urdf2webots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:57:12.000000 urdf2webots-2023.1.0/urdf2webots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 06:57:12.000000 urdf2webots-2023.1.0/urdf2webots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 06:57:12.000000 urdf2webots-2023.1.0/urdf2webots.egg-info/top_level.txt
```

### Comparing `urdf2webots-2.0.3/LICENSE` & `urdf2webots-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urdf2webots-2.0.3/PKG-INFO` & `urdf2webots-2023.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdf2webots
-Version: 2.0.3
+Version: 2023.1.0
 Summary: A converter between URDF and PROTO files.
 Home-page: https://github.com/cyberbotics/urdf2webots
 Author: Cyberbotics
 Author-email: support@cyberbotics.com
 License: Apache License, Version 2.0
 Description: # urdf2webots
```

### Comparing `urdf2webots-2.0.3/README.md` & `urdf2webots-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `urdf2webots-2.0.3/setup.py` & `urdf2webots-2023.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='urdf2webots',
-    version='2.0.3',
+    version='2023.1.0',
     author='Cyberbotics',
     author_email='support@cyberbotics.com',
     description='A converter between URDF and PROTO files.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cyberbotics/urdf2webots',
     packages=setuptools.find_packages(),
```

### Comparing `urdf2webots-2.0.3/urdf2webots/gazebo_materials.py` & `urdf2webots-2023.1.0/urdf2webots/gazebo_materials.py`

 * *Files identical despite different names*

### Comparing `urdf2webots-2.0.3/urdf2webots/importer.py` & `urdf2webots-2023.1.0/urdf2webots/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 
 """URDF files to Webots PROTO or Robot node converter."""
 
 
 import sys
-
-# Check version of Python
-if sys.version_info < (3,7):
-    sys.exit('urdf2webots requires Python 3.7 or higher.')
-
 import errno
 import argparse
 import os
 import re
 import tempfile
 from xml.dom import minidom
 
 import urdf2webots.parserURDF
 import urdf2webots.writeRobot
 
+# Check version of Python
+if sys.version_info < (3, 7):
+    sys.exit('urdf2webots requires Python 3.7 or higher.')
+
 try:
     import rospkg
 except ImportError:
     pass
 
 try:
     from ament_index_python import PackageNotFoundError
@@ -56,16 +55,16 @@
         if e.errno != errno.EEXIST:
             raise
         else:
             print('Directory "' + directory + '" already exists!')
 
 
 def convertUrdfFile(input=None, output=None, robotName=None, normal=False, boxCollision=False,
-                 toolSlot=None, initTranslation='0 0 0', initRotation='0 0 1 0',
-                 initPos=None, linkToDef=False, jointToDef=False, relativePathPrefix=None, targetVersion='R2022b'):
+                    toolSlot=None, initTranslation='0 0 0', initRotation='0 0 1 0',
+                    initPos=None, linkToDef=False, jointToDef=False, relativePathPrefix=None, targetVersion='R2023b'):
     """Convert a URDF file into a Webots PROTO file or Robot node string."""
     urdfContent = None
     if not input:
         print('''"--input" not specified, a URDF content will be read in the in stdin.\n
             The "</robot>" tag will stop the reading.''')
         urdfContent = ""
         for line in sys.stdin:
@@ -83,25 +82,24 @@
             urdfContent = file.read()
         if urdfContent is None:
             sys.exit('Could not read the URDF file.')
 
         # Set urdfPath for replacing "package://(.*)" occurences later
         convertUrdfFile.urdfPath = os.path.abspath(input)
 
-    return convertUrdfContent(urdfContent, output, robotName, normal, boxCollision,
-                 toolSlot, initTranslation, initRotation,
-                 initPos, linkToDef, jointToDef, relativePathPrefix, targetVersion)
+    return convertUrdfContent(urdfContent, output, robotName, normal, boxCollision, toolSlot, initTranslation, initRotation,
+                              initPos, linkToDef, jointToDef, relativePathPrefix, targetVersion)
 
 
 convertUrdfFile.urdfPath = None
 
 
 def convertUrdfContent(input, output=None, robotName=None, normal=False, boxCollision=False,
-                 toolSlot=None, initTranslation='0 0 0', initRotation='0 0 1 0',
-                 initPos=None, linkToDef=False, jointToDef=False, relativePathPrefix=None, targetVersion='R2022b'):
+                       toolSlot=None, initTranslation='0 0 0', initRotation='0 0 1 0',
+                       initPos=None, linkToDef=False, jointToDef=False, relativePathPrefix=None, targetVersion='R2023b'):
     """
     Convert a URDF content string into a Webots PROTO file or Robot node string.
     The current working directory will be used for relative paths in your URDF file.
     To use the location of your URDF file for relative paths, please use the convertUrdfFile() function.
     """
     # Retrieve urdfPath if this function has been called from convertUrdfFile()
     # And set urdfDirectory accordingly
@@ -165,25 +163,25 @@
                     try:
                         rospack = rospkg.RosPack()
                         directory = rospack.get_path(packageName)
                     except rospkg.common.ResourceNotFound:
                         sys.stderr.write('Package "%s" not found.\n' % packageName)
                     except NameError:
                         sys.stderr.write('Impossible to find location of "%s" package, installing "rospkg" might help.\n'
-                                        % packageName)
+                                         % packageName)
                 else:
                     try:
                         directory = get_package_share_directory(packageName)
                     except PackageNotFoundError:
                         sys.stderr.write('Package "%s" not found.\n' % packageName)
             else:
                 sys.stderr.write('ROS not sourced, package "%s" will not be found.\n' % packageName)
         if os.path.split(directory)[1]:
             packagePath = os.path.split(directory)[0]
-            input = input.replace('package://'+packageName, packagePath+'/'+packageName)
+            input = input.replace('package://' + packageName, packagePath + '/' + packageName)
         else:
             sys.stderr.write('Can\'t determine package root path.\n')
 
     # Convert the content into Webots robot
     domFile = minidom.parseString(input)
     for child in domFile.childNodes:
         if child.localName == 'robot':
@@ -200,42 +198,44 @@
                     robotName = convertLUtoUN(urdf2webots.parserURDF.getRobotName(child))  # capitalize
                     outputFile = output if output else robotName + '.proto'
 
                 mkdirSafe(outputFile.replace('.proto', '') + '_textures')  # make a dir called 'x_textures'
 
                 protoFile = open(outputFile, 'w')
                 urdf2webots.writeRobot.header(protoFile, urdfPath, robotName)
+                outputDirectory = os.path.dirname(os.path.abspath(outputFile))
             else:
                 tmp_robot_file = tempfile.NamedTemporaryFile(mode="w+", prefix='tempRobotURDFStringWebots')
+                outputDirectory = os.getcwd()
 
             urdf2webots.writeRobot.robotName = robotName
             urdf2webots.parserURDF.robotName = robotName  # pass robotName
 
             robot = child
             linkElementList = []
             jointElementList = []
             for child in robot.childNodes:
                 if child.localName == 'link':
                     linkElementList.append(child)
                 elif child.localName == 'joint':
                     jointElementList.append(child)
                 elif child.localName == 'material':
                     if not child.hasAttribute('name') \
-                        or child.getAttribute('name') not in urdf2webots.parserURDF.Material.namedMaterial:
+                       or child.getAttribute('name') not in urdf2webots.parserURDF.Material.namedMaterial:
                         material = urdf2webots.parserURDF.Material()
                         material.parseFromMaterialNode(child)
 
             linkList = []
             jointList = []
             parentList = []
             childList = []
             rootLink = urdf2webots.parserURDF.Link()
 
             for link in linkElementList:
-                linkList.append(urdf2webots.parserURDF.getLink(link, urdfDirectory))
+                linkList.append(urdf2webots.parserURDF.getLink(link, urdfDirectory, outputDirectory))
             for joint in jointElementList:
                 jointList.append(urdf2webots.parserURDF.getJoint(joint))
 
             for joint in jointList:
                 parentList.append(joint.parent)
                 childList.append(joint.child)
             parentList.sort()
@@ -263,33 +263,34 @@
                     break
 
             for child in robot.childNodes:
                 if child.localName == 'gazebo':
                     urdf2webots.parserURDF.parseGazeboElement(child, rootLink.name, linkList)
 
             sensorList = (urdf2webots.parserURDF.IMU.list +
-                            urdf2webots.parserURDF.P3D.list +
-                            urdf2webots.parserURDF.Camera.list +
-                            urdf2webots.parserURDF.RangeFinder.list +
-                            urdf2webots.parserURDF.Lidar.list)
+                          urdf2webots.parserURDF.P3D.list +
+                          urdf2webots.parserURDF.Camera.list +
+                          urdf2webots.parserURDF.RangeFinder.list +
+                          urdf2webots.parserURDF.Lidar.list)
             print('There are %d links, %d joints and %d sensors' % (len(linkList), len(jointList), len(sensorList)))
 
-            urdf2webots.writeRobot.staticBase = urdf2webots.parserURDF.removeDummyLinksAndStaticBaseFlag(linkList, jointList, sensorList, toolSlot)
+            urdf2webots.writeRobot.staticBase = urdf2webots.parserURDF.removeDummyLinksAndStaticBaseFlag(linkList, jointList,
+                                                                                                         sensorList, toolSlot)
 
             if isProto:
                 urdf2webots.writeRobot.declaration(protoFile, robotName, initTranslation, initRotation)
                 urdf2webots.writeRobot.URDFLink(protoFile, rootLink, 1, parentList, childList, linkList, jointList,
                                                 sensorList, boxCollision=boxCollision, normal=normal, robot=True)
                 protoFile.write('}\n')
                 protoFile.close()
                 return
             else:
-                urdf2webots.writeRobot.URDFLink(tmp_robot_file, rootLink, 0, parentList,
-                            childList, linkList, jointList, sensorList, boxCollision=boxCollision,
-                            normal=normal, robot=True, initTranslation=initTranslation, initRotation=initRotation)
+                urdf2webots.writeRobot.URDFLink(tmp_robot_file, rootLink, 0, parentList, childList, linkList, jointList,
+                                                sensorList, boxCollision=boxCollision, normal=normal, robot=True,
+                                                initTranslation=initTranslation, initRotation=initRotation)
 
                 tmp_robot_file.seek(0)
                 return (tmp_robot_file.read())
     sys.exit('Could not parse the URDF file.\n')
 
 
 if __name__ == '__main__':
@@ -320,15 +321,15 @@
                         'getFromProtoDef(defName) (for PROTO conversion only).')
     parser.add_argument('--joint-to-def', dest='jointToDef', action='store_true', default=False,
                         help='Creates a DEF with the joint name for each joint to be able to access it using '
                         'getFromProtoDef(defName) (for PROTO conversion only).')
     parser.add_argument('--relative-path-prefix', dest='relativePathPrefix', default=None,
                         help='If set and --input not specified, relative paths in your URDF file will be treated relatively '
                         'to it rather than relatively to the current directory from which the script is called.')
-    parser.add_argument('--target', dest='targetVersion', default='R2022b',
-                        choices=['R2023a', 'R2022b', 'R2022a', 'R2021b', 'R2021a', 'R2020b', 'R2020a'],
+    parser.add_argument('--target', dest='targetVersion', default='R2023b',
+                        choices=['R2023b', 'R2023a', 'R2022b', 'R2022a', 'R2021b', 'R2021a', 'R2020b', 'R2020a'],
                         help='Sets the Webots version the PROTO will target (will adapt which nodes will be used).')
 
     args = parser.parse_args()
     convertUrdfFile(args.input, args.output, args.robotName, args.normal, args.boxCollision, args.toolSlot,
                     args.initTranslation, args.initRotation, args.initPos, args.linkToDef, args.jointToDef,
                     args.relativePathPrefix, args.targetVersion)
```

### Comparing `urdf2webots-2.0.3/urdf2webots/math_utils.py` & `urdf2webots-2023.1.0/urdf2webots/math_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,20 +141,22 @@
     matrix = matrixFromRotation(rotation)
     v = []
     v.append(vector[0] * matrix[0] + vector[1] * matrix[1] + vector[2] * matrix[2])
     v.append(vector[0] * matrix[3] + vector[1] * matrix[4] + vector[2] * matrix[5])
     v.append(vector[0] * matrix[6] + vector[1] * matrix[7] + vector[2] * matrix[8])
     return v
 
+
 def combineRotations(rotation1, rotation2):
     """Combine two axis-angle rotations."""
     matrix1 = matrixFromRotation(rotation1)
     matrix2 = matrixFromRotation(rotation2)
     matrixRes = multiplyMatrix(matrix1, matrix2)
     return rotationFromMatrix(matrixRes)
 
+
 def combineTranslations(translation1, translation2):
     """Combine two translations."""
     result = []
     for (component1, component2) in zip(translation1, translation2):
         result.append(component1+component2)
     return result
```

### Comparing `urdf2webots-2.0.3/urdf2webots/parserURDF.py` & `urdf2webots-2023.1.0/urdf2webots/parserURDF.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 
 from urdf2webots.gazebo_materials import materials
 from urdf2webots.math_utils import convertRPYtoEulerAxis, rotateVector, combineRotations, combineTranslations
 
 
 # to pass from external
 robotName = ''
-targetVersion = 'R2022b'
+targetVersion = 'R2023b'
+
 
 class Inertia():
     """Define inertia object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.position = [0.0, 0.0, 0.0]
         self.rotation = [0.0, 0.0, 1.0, 0.0]
         self.mass = None
         self.ixx = 1.0
         self.ixy = 0.0
         self.ixz = 0.0
         self.iyy = 1.0
@@ -35,89 +36,89 @@
         self.izz = 1.0
 
 
 class Box():
     """Define box object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.x = 0.0
         self.y = 0.0
         self.z = 0.0
 
 
 class Cylinder():
     """Define cylinder object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.radius = 0.0
         self.height = 0.0
 
 
 class Sphere():
     """Define sphere object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.radius = 0.0
 
 
 class Mesh():
     """Define mesh object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.url = ''
         self.ccw = True
 
 
 class CadShape():
     """Define CadShape object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.url = ''
         self.ccw = True
 
 
 class Geometry():
     """Define geometry object."""
 
     reference = {}
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.box = Box()
         self.cylinder = Cylinder()
         self.sphere = Sphere()
         self.mesh = Mesh()
         self.cadShape = CadShape()
         self.name = None
         self.defName = None
 
 
 class Color():
     """Define color object."""
 
     def __init__(self, red=0.5, green=0.0, blue=0.0, alpha=1.0):
-        """Initializatization."""
+        """Initialization."""
         self.red = red
         self.green = green
         self.blue = blue
         self.alpha = alpha
 
 
 class Material():
     """Define material object."""
 
     namedMaterial = {}
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.emission = Color(0.0, 0.0, 0.0, 1.0)
         self.ambient = Color(0.0, 0.0, 0.0, 0.0)
         self.diffuse = Color(0.5, 0.5, 0.5, 1.0)
         self.specular = Color(0.0, 0.0, 0.0, 1.0)
         self.shininess = None
         self.index_of_refraction = 1.0
         self.texture = ""
@@ -141,90 +142,90 @@
                 assert False
 
 
 class Visual():
     """Define visual object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.position = [0.0, 0.0, 0.0]
         self.rotation = [0.0, 0.0, 1.0, 0.0]
         self.scale = [1.0, 1.0, 1.0]
         self.geometry = Geometry()
         self.material = Material()
 
 
 class Collision():
     """Define collision object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.position = [0.0, 0.0, 0.0]
         self.rotation = [0.0, 0.0, 1.0, 0.0]
         self.scale = [1.0, 1.0, 1.0]
         self.geometry = Geometry()
 
 
 class Calibration():
     """Define calibration object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.limit = 0.0
         self.rising = True
 
 
 class Dynamics():
     """Define dynamics object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.damping = 0.0
         self.friction = 0.0
 
 
 class Limit():
     """Define joint limit object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.lower = 0.0
         self.upper = 0.0
         self.effort = 10000  # if not specified in the URDF, there is no limit
         self.velocity = 0.0
 
 
 class Safety():
     """Define joint safety object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.lower = 0.0
         self.upper = 0.0
         self.kPosition = 0.0
         self.kVelocity = 0.0
 
 
 class Link():
     """Define link object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'default'
         self.inertia = Inertia()
         self.visual = []
         self.collision = []
         self.forceSensor = False
 
 
 class Joint():
     """Define joint object."""
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'default'
         self.type = 'default'
         self.position = [0.0, 0.0, 0.0]
         self.rotation = [0.0, 0.0, 1.0, 0.0]
         self.parent = 'default'
         self.child = 'default'
         self.axis = []
@@ -236,28 +237,28 @@
 
 class IMU():
     """Define an IMU sensor."""
 
     list = []
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'imu'
         self.gaussianNoise = 0
         self.parentLink = None
 
     def export(self, file, indentationLevel):
         """Export this IMU."""
         indent = '  '
 
         # export InertialUnit
         file.write(indentationLevel * indent + 'InertialUnit {\n')
         file.write(indentationLevel * indent + '  name "%s inertial"\n' % self.name)
         if self.gaussianNoise > 0:
-            file.write(indentationLevel * indent + '  noise %lf\n' % (self.gaussianNoise / (math.pi/2)))
+            file.write(indentationLevel * indent + '  noise %lf\n' % (self.gaussianNoise / (math.pi / 2)))
         file.write(indentationLevel * indent + '}\n')
 
         # export Accelerometer
         file.write(indentationLevel * indent + 'Accelerometer {\n')
         file.write(indentationLevel * indent + '  name "%s accelerometer"\n' % self.name)
         if self.gaussianNoise > 0:
             file.write(indentationLevel * indent + '  lookupTable [-100 -100 %lf, 100 100 %lf]\n' %
@@ -283,15 +284,15 @@
 
 class P3D():
     """Define P3D (ground truth pose)."""
 
     list = []
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'p3d'
         self.gaussianNoise = 0
         self.noiseCorrelation = 0
         self.speedNoise = 0
         self.parentLink = None
 
     def export(self, file, indentationLevel):
@@ -307,15 +308,15 @@
             file.write(indentationLevel * indent + '  speedNoise %lf\n' % self.speedNoise)
         file.write(indentationLevel * indent + '}\n')
 
         # export InertialUnit
         file.write(indentationLevel * indent + 'InertialUnit {\n')
         file.write(indentationLevel * indent + '  name "%s inertial"\n' % self.name)
         if self.gaussianNoise > 0:
-            file.write(indentationLevel * indent + '  noise %lf\n' % (self.gaussianNoise / (math.pi/2)))
+            file.write(indentationLevel * indent + '  noise %lf\n' % (self.gaussianNoise / (math.pi / 2)))
         file.write(indentationLevel * indent + '}\n')
 
         # export Gyro
         file.write(indentationLevel * indent + 'Gyro {\n')
         file.write(indentationLevel * indent + '  name "%s gyro"\n' % self.name)
         if self.gaussianNoise > 0:
             file.write(indentationLevel * indent + '  lookupTable [-100 -100 %lf, 100 100 %lf]\n' %
@@ -325,15 +326,15 @@
 
 class Camera():
     """Define a camera sensor."""
 
     list = []
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'camera'
         self.fov = None
         self.width = None
         self.height = None
         self.noise = None
         self.isImager = True
 
@@ -397,15 +398,15 @@
 
 class Lidar():
     """Define a lidar sensor."""
 
     list = []
 
     def __init__(self):
-        """Initializatization."""
+        """Initialization."""
         self.name = 'lidar'
         self.fov = None
         self.verticalFieldOfView = None
         self.horizontalResolution = None
         self.numberOfLayers = 1
         self.minRange = None
         self.maxRange = None
@@ -510,15 +511,15 @@
         inertia.ixz = float(matrixNode.getAttribute('ixz'))
         inertia.iyy = float(matrixNode.getAttribute('iyy'))
         inertia.iyz = float(matrixNode.getAttribute('iyz'))
         inertia.izz = float(matrixNode.getAttribute('izz'))
     return inertia
 
 
-def getVisual(link, node, path):
+def getVisual(link, node, path, outputDirectory):
     """Parse visual data of a link."""
     for index in range(0, len(node.getElementsByTagName('visual'))):
         visual = Visual()
         visualElement = node.getElementsByTagName('visual')[index]
         if hasElement(visualElement, 'origin'):
             if visualElement.getElementsByTagName('origin')[0].getAttribute('xyz'):
                 visual.position = getPosition(visualElement)
@@ -590,15 +591,16 @@
             link.visual.append(visual)
         elif hasElement(geometryElement, 'sphere'):
             visual.geometry.sphere.radius = float(geometryElement.getElementsByTagName('sphere')[0].getAttribute('radius'))
             link.visual.append(visual)
         elif hasElement(geometryElement, 'mesh'):
             meshfile = geometryElement.getElementsByTagName('mesh')[0].getAttribute('filename')
             if not os.path.isabs(meshfile):
-                meshfile = os.path.normpath(os.path.join(path, meshfile))
+                # Use the path relative to the output file
+                meshfile = os.path.normpath(os.path.relpath(os.path.join(path, meshfile), outputDirectory))
             # hack for gazebo mesh database
             if meshfile.count('package'):
                 idx0 = meshfile.find('package://')
                 meshfile = meshfile[idx0 + len('package://'):]
             if geometryElement.getElementsByTagName('mesh')[0].getAttribute('scale'):
                 meshScale = geometryElement.getElementsByTagName('mesh')[0].getAttribute('scale').split()
                 visual.scale[0] = float(meshScale[0])
@@ -629,15 +631,15 @@
                     visual.geometry.name = name
                     Geometry.reference[name] = visual.geometry
                 link.visual.append(visual)
             else:
                 print('Unsupported format: \"' + extension + '\"')
 
 
-def getCollision(link, node, path):
+def getCollision(link, node, path, outputDirectory):
     """Parse collision of a link."""
     for index in range(0, len(node.getElementsByTagName('collision'))):
         collision = Collision()
         collisionElement = node.getElementsByTagName('collision')[index]
         if hasElement(collisionElement, 'origin'):
             if collisionElement.getElementsByTagName('origin')[0].getAttribute('xyz'):
                 collision.position = getPosition(collisionElement)
@@ -658,22 +660,28 @@
             collision.geometry.cylinder.radius = float(element.getAttribute('radius'))
             collision.geometry.cylinder.height = float(element.getAttribute('length'))
             link.collision.append(collision)
         elif hasElement(geometryElement, 'sphere'):
             collision.geometry.sphere.radius = float(geometryElement.getElementsByTagName('sphere')[0].getAttribute('radius'))
             link.collision.append(collision)
         elif hasElement(geometryElement, 'mesh'):
-            meshfile = os.path.normpath(os.path.join(path,
-                                                     geometryElement.getElementsByTagName('mesh')[0].getAttribute('filename')))
+            meshfile = geometryElement.getElementsByTagName('mesh')[0].getAttribute('filename')
+            if not os.path.isabs(meshfile):
+                # Use the path relative to the output file
+                meshfile = os.path.normpath(os.path.relpath(os.path.join(path, meshfile), outputDirectory))
             extension = os.path.splitext(meshfile)[1].lower()
             if geometryElement.getElementsByTagName('mesh')[0].getAttribute('scale'):
                 meshScale = geometryElement.getElementsByTagName('mesh')[0].getAttribute('scale').split()
                 collision.scale[0] = float(meshScale[0])
                 collision.scale[1] = float(meshScale[1])
                 collision.scale[2] = float(meshScale[2])
+                if (targetVersion >= 'R2023b' and collision.scale[0] != 1.0 and collision.scale[1] != 1.0
+                        and collision.scale[2] != 1.0):
+                    print('\033[1;33mWarning: BoundingObjects (collisions tags) cannot be scaled in version R2023b!'
+                          ' Please create a separate model.\033[0m')
                 if collision.scale[0] * collision.scale[1] * collision.scale[2] < 0.0:
                     if extension in ['.dae', '.obj', '.stl']:
                         collision.geometry.mesh.ccw = False
             # hack for gazebo mesh database
             if meshfile.count('package'):
                 idx0 = meshfile.find('package://')
                 meshfile = meshfile[idx0 + len('package://'):]
@@ -751,24 +759,24 @@
         safety.upper = float(node.getElementsByTagName('safety_controller')[0].getAttribute('soft_upper_limit'))
     if node.getElementsByTagName('safety_controller')[0].getAttribute('k_position'):
         safety.kPosition = float(node.getElementsByTagName('safety_controller')[0].getAttribute('k_position'))
     safety.kVelocity = float(node.getElementsByTagName('safety_controller')[0].getAttribute('k_velocity'))
     return safety
 
 
-def getLink(node, path):
+def getLink(node, path, outputDirectory):
     """Parse a link."""
     link = Link()
     link.name = node.getAttribute('name')
     if hasElement(node, 'inertial'):
         link.inertia = getInertia(node)
     if hasElement(node, 'visual'):
-        getVisual(link, node, path)
+        getVisual(link, node, path, outputDirectory)
     if hasElement(node, 'collision'):
-        getCollision(link, node, path)
+        getCollision(link, node, path, outputDirectory)
     if not any([hasElement(node, 'inertial'), hasElement(node, 'visual'), hasElement(node, 'collision')]):
         link.inertia.mass = None
     return link
 
 
 def getJoint(node):
     """Parse a joint."""
@@ -798,14 +806,15 @@
 def isRootLink(link, childList):
     """Check if a link is root link."""
     for child in childList:
         if link == child:
             return False
     return True
 
+
 def removeDummyLinksAndStaticBaseFlag(linkList, jointList, sensorList, toolSlot):
     """Remove the dummy links (links without masses) and return true in case a dummy link should
     set the base of the robot as static. """
     staticBase = False
     linkIndex = 0
     childList = []
     for joint in jointList:
@@ -840,29 +849,31 @@
                     childJointIndex = index
                 elif joint.child == link.name:
                     parentJointIndex = index
 
             if parentJointIndex is not None:
                 if childJointIndex is not None:
                     jointList[parentJointIndex].child = jointList[childJointIndex].child
-                    jointList[parentJointIndex].position = combineTranslations(jointList[parentJointIndex].position, rotateVector(
-                        jointList[childJointIndex].position, jointList[parentJointIndex].rotation))
+                    jointList[parentJointIndex].position = combineTranslations(
+                        jointList[parentJointIndex].position,
+                        rotateVector(jointList[childJointIndex].position, jointList[parentJointIndex].rotation)
+                    )
                     jointList[parentJointIndex].rotation = combineRotations(
                         jointList[childJointIndex].rotation, jointList[parentJointIndex].rotation)
                     jointList[parentJointIndex].name = jointList[parentJointIndex].parent + \
                         "-" + jointList[parentJointIndex].child
                     jointList.remove(jointList[childJointIndex])
                 else:
                     # Special case for dummy non-root links used to fix the base of the robot
                     parentLink = jointList[parentJointIndex].parent
                     if isRootLink(parentLink, childList):
                         # Ensure the parent link does not have physics, if it does, it should be kept as-is
                         # since some sensors require the parent to have physics
-                        for l in linkList:
-                            if l.name == parentLink and l.inertia.mass is None:
+                        for item in linkList:
+                            if item.name == parentLink and item.inertia.mass is None:
                                 staticBase = True
 
                     jointList.remove(jointList[parentJointIndex])
 
             # This link can be removed
             linkList.remove(link)
 
@@ -954,19 +965,20 @@
                 if hasElement(rangeElement, 'resolution'):
                     rangefinder.resolution = float(rangeElement.getElementsByTagName('resolution')[0].firstChild.nodeValue)
             if hasElement(sensorElement, 'noise'):
                 noiseElement = sensorElement.getElementsByTagName('noise')[0]
                 if hasElement(noiseElement, 'stddev'):
                     rangefinder.noise = float(noiseElement.getElementsByTagName('stddev')[0].firstChild.nodeValue)
                     if rangefinder.maxRange:
-                            rangefinder.noise /= rangefinder.maxRange
+                        rangefinder.noise /= rangefinder.maxRange
             # minRange and near default values are 0.01 in Webots; ensure constraint near <= minRange
             if rangefinder.near and rangefinder.minRange and rangefinder.near > rangefinder.minRange:
                 rangefinder.minRange = rangefinder.near
-                print('The "minRange" value cannot be strictly inferior to the "near" value for a rangefinder, "minRange" has been set to the value of "near".')
+                print('The "minRange" value cannot be strictly inferior to the "near" value for a rangefinder, "minRange" has '
+                      'been set to the value of "near".')
             elif not rangefinder.near and rangefinder.minRange < 0.01:
                 rangefinder.near = rangefinder.minRange
             elif not rangefinder.minRange and rangefinder.near > 0.01:
                 rangefinder.minRange = rangefinder.near
             RangeFinder.list.append(rangefinder)
         elif sensorElement.getAttribute('type') == 'ray' or sensorElement.getAttribute('type') == 'gpu_ray':
             lidar = Lidar()
@@ -1011,13 +1023,14 @@
                     if hasElement(noiseElement, 'stddev'):
                         lidar.noise = float(noiseElement.getElementsByTagName('stddev')[0].firstChild.nodeValue)
                         if lidar.maxRange:
                             lidar.noise /= lidar.maxRange
                 # minRange and near default values are 0.01 in Webots; ensure constraint near <= minRange
                 if lidar.near and lidar.minRange and lidar.near > lidar.minRange:
                     lidar.minRange = lidar.near
-                    print('The "minRange" value cannot be strictly inferior to the "near" value for a lidar, "minRange" has been set to the value of "near".')
+                    print('The "minRange" value cannot be strictly inferior to the "near" value for a lidar, "minRange" has '
+                          'been set to the value of "near".')
                 elif not lidar.near and lidar.minRange < 0.01:
                     lidar.near = lidar.minRange
                 elif not lidar.minRange and lidar.near > 0.01:
                     lidar.minRange = lidar.near
             Lidar.list.append(lidar)
```

### Comparing `urdf2webots-2.0.3/urdf2webots/writeRobot.py` & `urdf2webots-2023.1.0/urdf2webots/writeRobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 toolSlot = None
 staticBase = False
 robotName = ''
 initPos = None
 linkToDef = False
 jointToDef = False
 indexSolid = 0
-targetVersion = 'R2022b'
+targetVersion = 'R2023b'
 
 
 class RGB():
     """RGB color object."""
 
     def __init__(self):
         """Initialization."""
         self.red = 0.5
         self.green = 0.5
         self.blue = 0.5
 
     def __eq__(self, other):
         """To compare a RGB color with a float list."""
         if type(other) == list:
-            return ((self.red, self.green, self.blue) == (other[0], other[1],  other[2]))
-        return ((self.red, self.green, self.blue) == (other.red, other.green,  other.blue))
+            return ((self.red, self.green, self.blue) == (other[0], other[1], other[2]))
+        return ((self.red, self.green, self.blue) == (other.red, other.green, other.blue))
 
 
 # ref: https://marcodiiga.github.io/rgba-to-rgb-conversion
 def RGBA2RGB(RGBA_color, RGB_background=RGB()):
     """Convert RGBA to RGB expression."""
     alpha = RGBA_color.alpha
 
@@ -141,15 +141,18 @@
         # 2: export Sensors
         for sensor in sensorList:
             if sensor.parentLink == link.name:
                 if not haveChild:
                     haveChild = True
                     robotFile.write((level + 1) * indent + 'children [\n')
                 if hasattr(sensor, 'isImager') and sensor.isImager:
-                    robotFile.write((level + 2) * indent + 'Transform {\n')
+                    if (targetVersion >= 'R2023b'):
+                        robotFile.write((level + 2) * indent + 'Pose {\n')
+                    else:
+                        robotFile.write((level + 2) * indent + 'Transform {\n')
                     robotFile.write((level + 3) * indent + 'translation 0 0 0\n')
                     robotFile.write((level + 3) * indent + 'rotation 0.577350 -0.577350 0.577350 2.094395\n')
                     robotFile.write((level + 3) * indent + 'children [\n')
                     sensor.export(robotFile, level + 4)
                     robotFile.write((level + 3) * indent + ']\n')
                     robotFile.write((level + 2) * indent + '}\n')
                 else:
@@ -256,26 +259,30 @@
     if hasGroup:
         robotFile.write('Group {\n')
         robotFile.write((level + 1) * indent + 'children [\n')
         boundingLevel = level + 2
 
     for boundingObject in link.collision:
         initialIndent = boundingLevel * indent if hasGroup else ''
-        if not boxCollision and (boundingObject.position != [0.0, 0.0, 0.0] or boundingObject.rotation[3] != 0.0 or boundingObject.scale != [1.0, 1.0, 1.0]):
-            robotFile.write(initialIndent + 'Transform {\n')
+        if not boxCollision and (boundingObject.position != [0.0, 0.0, 0.0] or boundingObject.rotation[3] != 0.0
+                                 or (targetVersion < 'R2023b' and boundingObject.scale != [1.0, 1.0, 1.0])):
+            if (targetVersion >= 'R2023b'):
+                robotFile.write(initialIndent + 'Pose {\n')
+            else:
+                robotFile.write(initialIndent + 'Transform {\n')
             if boundingObject.position != [0.0, 0.0, 0.0]:
                 robotFile.write((boundingLevel + 1) * indent + 'translation %lf %lf %lf\n' % (boundingObject.position[0],
                                                                                               boundingObject.position[1],
                                                                                               boundingObject.position[2]))
             if boundingObject.rotation[3] != 0.0:
                 robotFile.write((boundingLevel + 1) * indent + 'rotation %lf %lf %lf %lf\n' % (boundingObject.rotation[0],
                                                                                                boundingObject.rotation[1],
                                                                                                boundingObject.rotation[2],
                                                                                                boundingObject.rotation[3]))
-            if boundingObject.scale != [1.0, 1.0, 1.0]:
+            if boundingObject.scale != [1.0, 1.0, 1.0] and targetVersion < 'R2023b':
                 robotFile.write((boundingLevel + 1) * indent + 'scale %lf %lf %lf\n' % (boundingObject.scale[0],
                                                                                         boundingObject.scale[1],
                                                                                         boundingObject.scale[2]))
             robotFile.write((boundingLevel + 1) * indent + 'children [\n')
             boundingLevel = boundingLevel + 2
             hasGroup = True
             initialIndent = boundingLevel * indent
@@ -445,15 +452,18 @@
     """Write a Shape."""
     indent = '  '
     shapeLevel = level
     transform = False
 
     for visualNode in link.visual:
         if visualNode.position != [0.0, 0.0, 0.0] or visualNode.rotation[3] != 0.0 or visualNode.scale != [1.0, 1.0, 1.0]:
-            robotFile.write(shapeLevel * indent + 'Transform {\n')
+            if (visualNode.scale != [1.0, 1.0, 1.0]):
+                robotFile.write(shapeLevel * indent + 'Transform {\n')
+            else:
+                robotFile.write(shapeLevel * indent + 'Pose {\n')
             if visualNode.position != [0.0, 0.0, 0.0]:
                 robotFile.write((shapeLevel + 1) * indent + 'translation %lf %lf %lf\n' % (visualNode.position[0],
                                                                                            visualNode.position[1],
                                                                                            visualNode.position[2]))
             if visualNode.rotation[3] != 0.0:
                 robotFile.write((shapeLevel + 1) * indent + 'rotation %lf %lf %lf %lf\n' % (visualNode.rotation[0],
                                                                                             visualNode.rotation[1],
@@ -579,15 +589,15 @@
     robotFile.write((level + 1) * indent + 'endPoint')
     found_link = False
     for childLink in linkList:
         if childLink.name == joint.child:
             URDFLink(robotFile, childLink, level + 1, parentList, childList,
                      linkList, jointList, sensorList, endpointPosition, endpointRotation,
                      boxCollision, normal, endpoint=True)
-            assert(not found_link)
+            assert not found_link
             found_link = True
     # case that non-existing link cited, set dummy flag
     if not found_link and joint.child:
         URDFLink(robotFile, joint.child, level + 1, parentList, childList,
                  linkList, jointList, sensorList, endpointPosition, endpointRotation,
                  boxCollision, normal, dummy=True)
         print('warning: link ' + joint.child + ' is dummy!')
```

### Comparing `urdf2webots-2.0.3/urdf2webots.egg-info/PKG-INFO` & `urdf2webots-2023.1.0/urdf2webots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdf2webots
-Version: 2.0.3
+Version: 2023.1.0
 Summary: A converter between URDF and PROTO files.
 Home-page: https://github.com/cyberbotics/urdf2webots
 Author: Cyberbotics
 Author-email: support@cyberbotics.com
 License: Apache License, Version 2.0
 Description: # urdf2webots
```

