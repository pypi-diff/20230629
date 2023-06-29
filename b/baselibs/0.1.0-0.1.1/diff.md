# Comparing `tmp/baselibs-0.1.0.tar.gz` & `tmp/baselibs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baselibs-0.1.0.tar", last modified: Mon Jun 19 02:52:49 2023, max compression
+gzip compressed data, was "dist\baselibs-0.1.1.tar", last modified: Thu Jun 29 03:51:44 2023, max compression
```

## Comparing `baselibs-0.1.0.tar` & `baselibs-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 02:52:49.000000 baselibs-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-19 02:52:49.000000 baselibs-0.1.0/baselibs.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-19 02:52:49.000000 baselibs-0.1.0/baselibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1317 2023-06-19 02:52:49.000000 baselibs-0.1.0/baselibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-19 02:52:49.000000 baselibs-0.1.0/baselibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 02:52:49.000000 baselibs-0.1.0/baselibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29322 2023-06-19 02:52:06.000000 baselibs-0.1.0/baselibs.py
--rw-rw-rw-   0        0        0    35823 2020-04-20 05:16:32.000000 baselibs-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1317 2023-06-19 02:52:49.000000 baselibs-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-06-14 01:22:02.000000 baselibs-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 02:52:49.000000 baselibs-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1518 2023-06-19 02:48:37.000000 baselibs-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 03:51:44.000000 baselibs-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1317 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    30281 2023-06-29 03:45:22.000000 baselibs-0.1.1/baselibs.py
+-rw-rw-rw-   0        0        0    35823 2020-04-20 05:16:32.000000 baselibs-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1317 2023-06-29 03:51:44.000000 baselibs-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-06-14 01:22:02.000000 baselibs-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 03:51:44.000000 baselibs-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-06-29 03:51:29.000000 baselibs-0.1.1/setup.py
```

### Comparing `baselibs-0.1.0/baselibs.egg-info/PKG-INFO` & `baselibs-0.1.1/baselibs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselibs
-Version: 0.1.0
+Version: 0.1.1
 Summary: baselibs
 Home-page: https://github.com/xmxoxo/baselibs
 Author: He xi
 Author-email: xmhexi@qq.com
 License: UNKNOWN
 Project-URL: Blog, https://blog.csdn.net/xmxoxo
 Keywords: baselibs
```

### Comparing `baselibs-0.1.0/baselibs.py` & `baselibs-0.1.1/baselibs.py`

 * *Files 3% similar despite different names*

```diff
@@ -850,16 +850,18 @@
             #print('Processing file:%s ==> %d lines ' % (fname,intLines), end = '')
             print('Processing file:%s ==> %d lines ' % (fname,intLines))
     print('\n%d File(s) ,Total: %d line(s)' % (len(lstF[1]),intTotalLines ) )
     print('merge files to %s' % outfile)
 
 
 def batch_doc2txt (path, outpath=''):
-    ''' 目录(含子目录)下所有文件批量word转txt
-    参数： path:目录；
+    ''' 目录(含子目录)下所有文件批量word（.doc,.docx)转txt
+    参数： 
+    path:目录名；
+    outpath: 输出目录，默认为空表示源目录
     '''
     from win32com import client as wc
     try:
         #lstFile = getFiles(path)
         lstFile = getAllFiles_Generator(path)#, ['doc','docx']
         
         strExt = ''
@@ -905,15 +907,15 @@
     finally:
         wordapp.Quit()
 
 
 def getFieldFromJson (obj, columns, mainname='items', subname=''):
     ''' 从json格式中读取字段'''
 
-    #total = obj['result']['total']
+    # total = obj['result']['total']
     
     result = []
     if mainname:
         lstobj = obj['result'][mainname]
         for x in lstobj:
             dt = []
             for col in columns:
@@ -925,15 +927,15 @@
                 else:
                     if col in x.keys(): 
                         dt.append(x[col])
                     else:
                         dt.append("")
             result.append(dt)
     else:
-        #只有一级的情况
+        # 只有一级的情况
         lstobj = obj['result']
         dt = []
         for col in columns:
             if subname:
                 if col in lstobj[subname].keys(): 
                     dt.append(lstobj[subname][col])
                 else:
@@ -942,11 +944,47 @@
                 if col in lstobj.keys(): 
                     dt.append(lstobj[col])
                 else:
                     dt.append("")
         result.append(dt)
     return result
 
+#-----------------------------------------
+
+def dict_reverse(data:dict, overwrite=0):
+	''' 字典反转，即把key和value对调
+	'''
+	ndict = {}
+	for k,value in data.items():
+		for v in value:
+			if not v in ndict.keys():
+				ndict[v] = k
+			else:
+				if overwrite==1: 
+					# 重复值覆盖方式
+					ndict[v] = k
+				else:
+					# 重复值不覆盖方式
+					pass
+
+	return ndict
+
+def test_dict_reverse():
+	''' 单元测试
+	'''
+	d = {"a":[1,2,3], 'b':[3,5,6,7], 'c':[8,9,10]}
+	print('data:%s'%d)
+	ret = dict_reverse(d)
+	print('overwrite=0, result=%s'%ret)
+	ans = {1: 'a', 2: 'a', 3: 'a', 5: 'b', 6: 'b', 7: 'b', 8: 'c', 9: 'c', 10: 'c'}
+	assert ret == ans
+
+	ret = dict_reverse(d, overwrite=1)
+	print('overwrite=1, result=%s'%ret)
+	ans1 = {1: 'a', 2: 'a', 3: 'b', 5: 'b', 6: 'b', 7: 'b', 8: 'c', 9: 'c', 10: 'c'}
+	assert ret == ans1
+
+
 
 if __name__ == '__main__':
     pass
```

### Comparing `baselibs-0.1.0/LICENSE.txt` & `baselibs-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baselibs-0.1.0/PKG-INFO` & `baselibs-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselibs
-Version: 0.1.0
+Version: 0.1.1
 Summary: baselibs
 Home-page: https://github.com/xmxoxo/baselibs
 Author: He xi
 Author-email: xmhexi@qq.com
 License: UNKNOWN
 Project-URL: Blog, https://blog.csdn.net/xmxoxo
 Keywords: baselibs
```

### Comparing `baselibs-0.1.0/README.md` & `baselibs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `baselibs-0.1.0/setup.py` & `baselibs-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 # 导入静态文件
 file_data = []
 
 setuptools.setup(
     name='baselibs',
-    version='0.1.0',
+    version='0.1.1',
     description='baselibs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='baselibs',
     py_modules=['baselibs'],
     install_requires=[],
     # packages=setuptools.find_packages(),
```

