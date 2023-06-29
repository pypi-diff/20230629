# Comparing `tmp/yplib-1.9.8.tar.gz` & `tmp/yplib-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.9.8.tar", last modified: Thu Jun 29 02:16:10 2023, max compression
+gzip compressed data, was "dist\yplib-1.9.9.tar", last modified: Thu Jun 29 07:49:25 2023, max compression
```

## Comparing `yplib-1.9.8.tar` & `yplib-1.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:16:10.975786 yplib-1.9.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.9.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-29 02:16:10.975558 yplib-1.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.9.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 02:16:10.976290 yplib-1.9.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-29 02:15:52.000000 yplib-1.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:16:10.972302 yplib-1.9.8/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-1.9.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.9.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.9.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.9.8/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-1.9.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.9.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    26853 2023-06-29 01:15:20.000000 yplib-1.9.8/yplib/index.py
--rw-rw-rw-   0        0        0     4765 2023-06-29 02:15:38.000000 yplib-1.9.8/yplib/mail.py
--rw-rw-rw-   0        0        0     3546 2023-06-28 08:18:28.000000 yplib-1.9.8/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.9.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:16:10.974691 yplib-1.9.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-29 02:16:10.000000 yplib-1.9.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-29 02:16:10.000000 yplib-1.9.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:16:10.000000 yplib-1.9.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 02:16:10.000000 yplib-1.9.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.240543 yplib-1.9.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.9.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-29 07:49:25.240151 yplib-1.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.9.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:49:25.240543 yplib-1.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-29 07:48:32.000000 yplib-1.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.235330 yplib-1.9.9/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-1.9.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.9.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.9.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.9.9/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-1.9.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.9.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-1.9.9/yplib/index.py
+-rw-rw-rw-   0        0        0     4765 2023-06-29 02:15:38.000000 yplib-1.9.9/yplib/mail.py
+-rw-rw-rw-   0        0        0     3546 2023-06-28 08:18:28.000000 yplib-1.9.9/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.9.9/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.239174 yplib-1.9.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.9.8/LICENSE` & `yplib-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/setup.py` & `yplib-1.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.9.8",
+  version="1.9.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.9.8/yplib/__init__.py` & `yplib-1.9.9/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/chart.py` & `yplib-1.9.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/chart_html.py` & `yplib-1.9.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/db.py` & `yplib-1.9.9/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/file.py` & `yplib-1.9.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/http_util.py` & `yplib-1.9.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/index.py` & `yplib-1.9.9/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,54 +295,54 @@
     else:
         s = str(data)
     return s
 
 
 # 根据json的key排序,用于签名
 # 按照 key 排序, 按照 key=value 然后再 & 连接, 如果数据中有 list, 使用 , 连接 list 中的数据, 然后拼接成 str 返回
-# separator : 分隔符 , 默认 &
+# sep : 分隔符 , 默认 &
 # join      : 连接符 , 默认 =
 # join_list : list 数据 连接符 , 默认 ,
-def sort_by_json_key(data_obj, separator='&', join='=', join_list=','):
+def sort_by_json_key(data_obj, sep='&', join='=', join_list=','):
     if isinstance(data_obj, list) or isinstance(data_obj, tuple) or isinstance(data_obj, set):
         return join_list.join(list(map(lambda x: f'{x}', data_obj)))
     if not isinstance(data_obj, dict):
         return str(data_obj)
     data_list = sorted(data_obj.items(), key=lambda x: x[0])
     r_l = []
     for one in data_list:
         value_one = one[1]
         if can_use_json(value_one):
-            s = sort_by_json_key(value_one)
+            s = sort_by_json_key(data_obj=value_one, sep=sep, join=join, join_list=join_list)
         else:
             s = str(value_one)
         r_l.append(f'{one[0]}{join}{s}')
-    return separator.join(r_l)
+    return sep.join(r_l)
 
 
 # data = {}
 # data['merchantId'] = "merchantId"
 # data['currency'] = "IDR"
 # data['accType'] = "payout"
 # data['version'] = "1.0"
-# # data['b'] = {
-# #     'a': 1,
-# #     'c': 'c',
-# #     'b': 'po',
-# # }
-# # b = [2, 3, 8, 4, "yp"]
-# # data['c'] = b
+# data['b'] = {
+#     'a': 1,
+#     'c': 'c',
+#     'b': 'po',
+# }
+# b = [2, 3, 8, 4, "yp"]
+# data['c'] = b
 # sign = sort_by_json_key(data)
 # print(sign)
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
-# separator : 是否对每一行进行分割,如果存在这个字段,就分割
-# separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# sep : 是否对每一行进行分割,如果存在这个字段,就分割
+# sep_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
 # start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
 # end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
 # end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
 # count :       读取指定的行数
 ################################################
 # 当读取 excel 之类的文件的时候
@@ -351,16 +351,16 @@
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
 # column_date : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 # 返回的数据一定是一个 list
 def to_list(file_name='a.txt',
-            separator=None,
-            separator_all=None,
+            sep=None,
+            sep_all=None,
             start_index=None,
             start_line=None,
             end_index=None,
             end_line=None,
             count=None,
             sheet_index=1,
             column_index=None,
@@ -369,16 +369,16 @@
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         return to_list_from_excel(file_name=file_name,
                                   sheet_index=sheet_index,
                                   column_index=column_index,
                                   column_date=column_date,
                                   column_datetime=column_datetime)
     return to_list_from_txt(file_name=file_name,
-                            separator=separator,
-                            separator_all=separator_all,
+                            sep=sep,
+                            sep_all=sep_all,
                             start_index=start_index,
                             start_line=start_line,
                             end_index=end_index,
                             end_line=end_line,
                             count=count)
 
 
@@ -459,24 +459,24 @@
                             row_data = cell_data
         data_list.append(row_data)
     return data_list
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
-# separator : 是否对每一行进行分割,如果存在这个字段,就分割
-# separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
+# sep : 是否对每一行进行分割,如果存在这个字段,就分割
+# sep_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
 # start_line :  从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
 # end_index :   读取到这个地方结束,从1开始标号 , 不包含这一行
 # end_line :    读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
 # count :       读取指定的行数
 def to_list_from_txt(file_name='a.txt',
-                     separator=None,
-                     separator_all=None,
+                     sep=None,
+                     sep_all=None,
                      start_index=None,
                      start_line=None,
                      end_index=None,
                      end_line=None,
                      count=None):
     if file_is_empty(file_name=file_name):
         return []
@@ -508,43 +508,43 @@
         if end_flag is not None and not end_flag and line.find(end_line) > -1:
             end_flag = True
         if start_flag is not None and not start_flag:
             continue
         elif end_flag is not None and end_flag:
             continue
         c += 1
-        if separator is not None:
-            data_list.append(line.split(str(separator)))
+        if sep is not None:
+            data_list.append(line.split(str(sep)))
         else:
             data_list.append(line)
-    if separator_all is not None:
-        data_list = ''.join(data_list).split(str(separator_all))
+    if sep_all is not None:
+        data_list = ''.join(data_list).split(str(sep_all))
     return data_list
 
 
 # 在 to_list 方法上再嵌套一层,
 # r_str : 返回的数据是否是一个 字符串, ''.join(list)
 # r_json : 返回的数据是否是一个 json 类型的数据
 def to_list_data(file_name='a.txt',
-                 separator=None,
-                 separator_all=None,
+                 sep=None,
+                 sep_all=None,
                  start_index=None,
                  start_line=None,
                  end_index=None,
                  end_line=None,
                  count=None,
                  sheet_index=1,
                  column_index=None,
                  column_date=None,
                  column_datetime=None,
                  r_json=False,
                  r_str=False):
     d = to_list(file_name=file_name,
-                separator=separator,
-                separator_all=separator_all,
+                sep=sep,
+                sep_all=sep_all,
                 start_index=start_index,
                 start_line=start_line,
                 end_index=end_index,
                 end_line=end_line,
                 count=count,
                 sheet_index=sheet_index,
                 column_index=column_index,
```

### Comparing `yplib-1.9.8/yplib/mail.py` & `yplib-1.9.9/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.8/yplib/mail_html.py` & `yplib-1.9.9/yplib/mail_html.py`

 * *Files identical despite different names*

