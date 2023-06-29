# Comparing `tmp/jcmutils-1.6.0.tar.gz` & `tmp/jcmutils-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.6.0.tar", last modified: Wed Jun 28 06:12:50 2023, max compression
+gzip compressed data, was "jcmutils-1.6.2.tar", last modified: Thu Jun 29 07:29:06 2023, max compression
```

## Comparing `jcmutils-1.6.0.tar` & `jcmutils-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-28 06:12:50.342671 jcmutils-1.6.0/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.0/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-28 06:12:50.342671 jcmutils-1.6.0/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.0/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-28 06:12:50.342671 jcmutils-1.6.0/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.0/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    15916 2023-06-28 06:11:57.000000 jcmutils-1.6.0/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.0/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.0/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.0/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-28 06:12:50.342671 jcmutils-1.6.0/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-28 06:12:50.000000 jcmutils-1.6.0/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-28 06:12:50.000000 jcmutils-1.6.0/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-28 06:12:50.000000 jcmutils-1.6.0/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-28 06:12:50.000000 jcmutils-1.6.0/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-28 06:12:50.000000 jcmutils-1.6.0/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-28 06:12:50.342671 jcmutils-1.6.0/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-28 06:12:10.000000 jcmutils-1.6.0/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 07:29:06.665431 jcmutils-1.6.2/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.2/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 07:29:06.665431 jcmutils-1.6.2/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.2/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 07:29:06.665431 jcmutils-1.6.2/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.2/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    17869 2023-06-29 07:28:35.000000 jcmutils-1.6.2/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.2/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.2/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.2/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 07:29:06.665431 jcmutils-1.6.2/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 07:29:06.000000 jcmutils-1.6.2/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 07:29:06.000000 jcmutils-1.6.2/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 07:29:06.000000 jcmutils-1.6.2/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 07:29:06.000000 jcmutils-1.6.2/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 07:29:06.000000 jcmutils-1.6.2/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 07:29:06.665431 jcmutils-1.6.2/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 07:27:15.000000 jcmutils-1.6.2/setup.py
```

### Comparing `jcmutils-1.6.0/LICENSE` & `jcmutils-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.0/README.md` & `jcmutils-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.0/jcmutils/dataset_utils.py` & `jcmutils-1.6.2/jcmutils/dataset_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .logger import logger
 import numpy as np
 import os
 import jcmwave
 import cv2
 import yaml
+import random
 
 
 class datagen:
     def __init__(self, jcmp_path, database_path, keys):
         # 初始化成员变量
         self.jcmp_path = jcmp_path
         self.keys = keys
@@ -17,82 +18,33 @@
             abs_resultbag_dir = os.path.join(os.getcwd(), database_path)
         if not os.path.exists(os.path.dirname(database_path)):
             raise Exception("exporting dataset but resultbag dosen't exist")
         self.resultbag = jcmwave.Resultbag(abs_resultbag_dir)
         logger.debug("datagen inited,no error reported")
         logger.debug(
             f"jcmp_path is {jcmp_path},database_path is {abs_resultbag_dir}")
-
-    def export_dataset_one(self, num_of_result, source_density, target_density,target_filename,phi0, vmax, is_light_intense=True, is_symmetry=False):
-        # 路径预处理
-        if not os.path.exists(os.path.dirname(target_filename)):
-            os.makedirs(os.path.dirname(target_filename))
-
-        # 提取无缺陷图像
-        ## 先确定total_result的形状
-        temp_result = self.resultbag.get_result(self.keys[0])
-        field = (temp_result[num_of_result]['field'][0].conj() *
-                 temp_result[num_of_result]['field'][0]).sum(axis=2).real
-        total_results = np.zeros(field.shape)
-        logger.debug(f"total_result shape defined as {total_results.shape}")
-
-        ## 开始逐个提取结果
-        for key in self.keys:
-            result = self.resultbag.get_result(key)
-            field = (result[num_of_result]['field'][0].conj() *
-                     result[num_of_result]['field'][0]).sum(axis=2).real
-            if is_light_intense:
-                field = np.power(field, 2)
-            total_results += field
-            if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
-                field = np.rot90(field, 2)
-                total_results += field
-                logger.debug("key was rotated for symmetry")
         
-        # 合并最终结果
-        vmaxa = np.max(total_results) if vmax is None else vmax
-        afield = (total_results/ vmaxa)*235
-        afield = np.rot90(afield)
-
-        label_name = target_filename + ".txt"
-        with open(label_name,"w") as f:
-            f.write("")
-
-        # 保存超分辨（原图）
-        cv2.imwrite(target_filename + "_origin.jpg",afield)
+        # 随机初始化
+        random.seed()
 
-        # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
-        scale_factor =source_density*1.0/target_density
-        # 缩放电场/光强场到对应的大小
-        scaled_field = cv2.resize(afield, None, fx=scale_factor,# type: ignore
-                                  fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
-
-        # 绘图
-        logger.debug(f"printing max value of results:{np.max(total_results)}")
-        cv2.imwrite(target_filename + ".jpg",scaled_field)
-        logger.info("all target image saved completed!")
-
-
-
-    def export_dataset(self, num_of_result, source_density, target_density,target_filename,phi0,defect_size, vmax,signal_level=0.4,noise_level = 5, is_light_intense=True, is_symmetry=False):
+ 
+    def export_dataset(self, num_of_result,target_density,target_filename,phi0,vmax,signal_level=0.4,noise_level = 5, is_light_intense=True, is_symmetry=False):
         # 路径预处理
         if not os.path.exists(os.path.dirname(target_filename)):
             os.makedirs(os.path.dirname(target_filename))
         yamlpath =os.path.join(os.path.dirname(self.jcmp_path),"properties.yaml")
         
         # 解析YAML，准备必须的数据
         with open(yamlpath) as f:
             data = yaml.load(f,Loader=yaml.FullLoader)
-        # lattice_vector_length = data['latticeVector']['latticeVectorLength']
-        # lattice_angle = data['latticeVector']['latticeAngle']
-        # center_pos = data['centerPos']
-        # shift = data['shift']
+        periodic_x= data['periodicInfo'][0]
+        periodic_y = data['periodicInfo'][1]
+        source_density = data['sourceDensity']
         nodefect_phi0_0 = data['nodefect']['phi0-0']
         nodefect_phi0_90 = data['nodefect']['phi0-90']
-        # origin_size = data['originSize'] 
         
         # 获取模板图像
         if phi0 == 90:
             template_path = nodefect_phi0_90
         else:
             template_path = nodefect_phi0_0
         template_image = cv2.imread(template_path,cv2.IMREAD_GRAYSCALE)
@@ -128,14 +80,35 @@
         
         # 合并最终结果
         vmaxa = np.max(total_results) if vmax is None else vmax
         afield = (total_results/ vmaxa)*235
         afield = np.rot90(afield)
 
         (output_image,(xpos,ypos,width,height)) = self.__process_image(afield,template_image,signal_level)
+        
+        width_lower_border = 0.6*(periodic_x/source_density)/output_image.shape[1]
+        height_lower_border = 0.6*(periodic_y/source_density)/output_image.shape[0]
+        width_lower_warn = 0.9*(periodic_x/source_density)/output_image.shape[1]
+        height_lower_warn = 0.9*(periodic_y/source_density)/output_image.shape[0]
+        width_upper_warn = 1.8*(periodic_x/source_density)/output_image.shape[1]
+        height_upper_warn = 1.8*(periodic_y/source_density)/output_image.shape[0]
+        width_upper_border = 2.1*(periodic_x/source_density)/output_image.shape[1]
+        height_upper_border = 2.1*(periodic_y/source_density)/output_image.shape[0]
+        # 大致检测结果正确性
+        if width <=width_lower_border or height <=height_lower_border :
+            logger.error(f"false mixed image detected,key-{self.keys} was detected too small width or height. the width is {width},height is {height},which is smaller than ({width_lower_border},{height_lower_border}) , try a smaller signal_level")
+            raise Exception("error detected , please read log")
+        if width <= width_lower_warn or height <=height_lower_warn:
+            logger.warning(f"key-{self.keys} mixed image smaller than ({width_lower_warn},{height_lower_warn}) maybe a little bit strage , please check")
+        if width >= width_upper_warn or height >= height_upper_warn:
+            logger.warning(f"key-{self.keys} mixed image lagger than ({width_upper_warn},{height_upper_warn}) maybe a little bit strage , please check")
+        if width >= width_upper_border or height >= height_upper_border:
+            logger.error(f"false mixed image detected,key-{self.keys} was detected too big width or height. the width is {width},height is {height},which is larger than ({width_upper_border},{height_upper_border}), try a larger signal_level")
+            raise Exception("error detected , please read log")
+            
 
         # #####
         # 重要
         # ! 在此行开始，进行数据增广处理
         # ! 增广方式为：
         # ! 微位移方式出图
         # ! 旋转出图
@@ -190,23 +163,25 @@
                 temp_image = scaled_images[i] + gauss
                 temp_image = np.clip(temp_image,0,255)
                 final_images.append(temp_image)
                 final_positions.append(positions[i])
         
         # # 保存
         for i in range(len(final_images)):
+            if random.random() > 0.3:
+                continue
             label_name = target_filename + f"-{i}.txt"
+            file_name = target_filename + f"-{i}.jpg"
+
             with open(label_name,"w") as f:
                 f.write(f"{defect_class} {final_positions[i][0]} {final_positions[i][1]} {final_positions[i][2]} {final_positions[i][3]} ")
+            cv2.imwrite(file_name,final_images[i])
 
         # 绘图
         logger.debug(f"printing max value of results:{np.max(total_results)}")
-        for i in range(len(final_images)):
-            file_name = target_filename + f"-{i}.jpg"
-            cv2.imwrite(file_name,final_images[i])
         logger.info("all target image saved completed!")
         
     def __process_image(self,defect_img,template_img,signal_level,smooth_length=30,extend_length = 15):
         diff_img = defect_img.astype(np.float32) - template_img.astype(np.float32)
         image_shape = template_img.shape
         # diff_img = (diff_img + 125)
         # diff_img = np.clip(diff_img, 0, 255).astype(np.uint8)
@@ -347,8 +322,58 @@
     #     # 缩放电场/光强场到对应的大小
     #     scaled_field = cv2.resize(afield, None, fx=scale_factor,# type: ignore
     #                               fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
 
     #     # 绘图
     #     logger.debug(f"printing max value of results:{np.max(total_results)}")
     #     cv2.imwrite(target_filename,scaled_field)
-    #     logger.info("all target image saved completed!")
+    #     logger.info("all target image saved completed!")
+    #    def export_dataset_one(self, num_of_result, source_density, target_density,target_filename,phi0, vmax, is_light_intense=True, is_symmetry=False):
+    #     # 路径预处理
+    #     if not os.path.exists(os.path.dirname(target_filename)):
+    #         os.makedirs(os.path.dirname(target_filename))
+
+    #     # 提取无缺陷图像
+    #     ## 先确定total_result的形状
+    #     temp_result = self.resultbag.get_result(self.keys[0])
+    #     field = (temp_result[num_of_result]['field'][0].conj() *
+    #              temp_result[num_of_result]['field'][0]).sum(axis=2).real
+    #     total_results = np.zeros(field.shape)
+    #     logger.debug(f"total_result shape defined as {total_results.shape}")
+
+    #     ## 开始逐个提取结果
+    #     for key in self.keys:
+    #         result = self.resultbag.get_result(key)
+    #         field = (result[num_of_result]['field'][0].conj() *
+    #                  result[num_of_result]['field'][0]).sum(axis=2).real
+    #         if is_light_intense:
+    #             field = np.power(field, 2)
+    #         total_results += field
+    #         if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
+    #             field = np.rot90(field, 2)
+    #             total_results += field
+    #             logger.debug("key was rotated for symmetry")
+        
+    #     # 合并最终结果
+    #     vmaxa = np.max(total_results) if vmax is None else vmax
+    #     afield = (total_results/ vmaxa)*235
+    #     afield = np.rot90(afield)
+
+    #     label_name = target_filename + ".txt"
+    #     with open(label_name,"w") as f:
+    #         f.write("")
+
+    #     # 保存超分辨（原图）
+    #     cv2.imwrite(target_filename + "_origin.jpg",afield)
+
+    #     # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
+    #     scale_factor =source_density*1.0/target_density
+    #     # 缩放电场/光强场到对应的大小
+    #     scaled_field = cv2.resize(afield, None, fx=scale_factor,# type: ignore
+    #                               fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
+
+    #     # 绘图
+    #     logger.debug(f"printing max value of results:{np.max(total_results)}")
+    #     cv2.imwrite(target_filename + ".jpg",scaled_field)
+    #     logger.info("all target image saved completed!")
+
+
```

### Comparing `jcmutils-1.6.0/jcmutils/gen_sources.py` & `jcmutils-1.6.2/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.0/jcmutils/logger.py` & `jcmutils-1.6.2/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.0/jcmutils/solver.py` & `jcmutils-1.6.2/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.0/setup.py` & `jcmutils-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.6.0'
+VERSION = '1.6.2'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

