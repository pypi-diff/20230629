# Comparing `tmp/bubble-aide-0.1.4.tar.gz` & `tmp/bubble-aide-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble-aide-0.1.4.tar", last modified: Thu Jun 29 02:58:54 2023, max compression
+gzip compressed data, was "bubble-aide-0.1.5.tar", last modified: Thu Jun 29 08:57:29 2023, max compression
```

## Comparing `bubble-aide-0.1.4.tar` & `bubble-aide-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.978700 bubble-aide-0.1.4/
--rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      707 2023-06-29 02:58:54.978700 bubble-aide-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2419 2023-05-29 01:45:12.000000 bubble-aide-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.947513 bubble-aide-0.1.4/bubble_aide/
--rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.4/bubble_aide/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.963058 bubble-aide-0.1.4/bubble_aide/abc/
--rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.4/bubble_aide/abc/__init__.py
--rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.4/bubble_aide/abc/module.py
--rw-rw-rw-   0        0        0     4886 2023-06-06 06:45:38.000000 bubble-aide-0.1.4/bubble_aide/delegate.py
--rw-rw-rw-   0        0        0    10060 2023-05-31 03:07:23.000000 bubble-aide-0.1.4/bubble_aide/govern.py
--rw-rw-rw-   0        0        0    10025 2023-06-13 03:22:20.000000 bubble-aide-0.1.4/bubble_aide/main.py
--rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.4/bubble_aide/restricting.py
--rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.4/bubble_aide/reward.py
--rw-rw-rw-   0        0        0     1116 2023-05-31 03:07:23.000000 bubble-aide-0.1.4/bubble_aide/slashing.py
--rw-rw-rw-   0        0        0     5813 2023-05-31 03:07:23.000000 bubble-aide-0.1.4/bubble_aide/staking.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.963058 bubble-aide-0.1.4/bubble_aide/statics/
--rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.4/bubble_aide/statics/__init__.py
--rw-rw-rw-   0        0        0    12461 2023-06-13 03:23:44.000000 bubble-aide-0.1.4/bubble_aide/statics/calculator.py
--rw-rw-rw-   0        0        0      915 2023-05-31 03:08:14.000000 bubble-aide-0.1.4/bubble_aide/statics/constant.py
--rw-rw-rw-   0        0        0     3386 2023-06-05 02:48:13.000000 bubble-aide-0.1.4/bubble_aide/statics/contract.py
--rw-rw-rw-   0        0        0     5783 2023-05-25 09:07:03.000000 bubble-aide-0.1.4/bubble_aide/statics/economic.py
--rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.4/bubble_aide/statics/graphqls.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.978700 bubble-aide-0.1.4/bubble_aide/utils/
--rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.4/bubble_aide/utils/__init__.py
--rw-rw-rw-   0        0        0     3377 2023-06-13 03:22:38.000000 bubble-aide-0.1.4/bubble_aide/utils/utils.py
--rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.4/bubble_aide/utils/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:58:54.963058 bubble-aide-0.1.4/bubble_aide.egg-info/
--rw-rw-rw-   0        0        0      707 2023-06-29 02:58:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2023-06-29 02:58:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:58:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 03:23:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      161 2023-06-29 02:58:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 02:58:54.000000 bubble-aide-0.1.4/bubble_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 02:58:54.978700 bubble-aide-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-06-13 03:23:44.000000 bubble-aide-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.794326 bubble-aide-0.1.5/
+-rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-06-29 08:57:29.794326 bubble-aide-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2419 2023-05-29 01:45:12.000000 bubble-aide-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.776737 bubble-aide-0.1.5/bubble_aide/
+-rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.5/bubble_aide/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.783753 bubble-aide-0.1.5/bubble_aide/abc/
+-rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.5/bubble_aide/abc/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.5/bubble_aide/abc/module.py
+-rw-rw-rw-   0        0        0     4886 2023-06-06 06:45:38.000000 bubble-aide-0.1.5/bubble_aide/delegate.py
+-rw-rw-rw-   0        0        0    10060 2023-05-31 03:07:23.000000 bubble-aide-0.1.5/bubble_aide/govern.py
+-rw-rw-rw-   0        0        0    10025 2023-06-13 03:22:20.000000 bubble-aide-0.1.5/bubble_aide/main.py
+-rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.5/bubble_aide/restricting.py
+-rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.5/bubble_aide/reward.py
+-rw-rw-rw-   0        0        0     1116 2023-05-31 03:07:23.000000 bubble-aide-0.1.5/bubble_aide/slashing.py
+-rw-rw-rw-   0        0        0     5813 2023-05-31 03:07:23.000000 bubble-aide-0.1.5/bubble_aide/staking.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.790304 bubble-aide-0.1.5/bubble_aide/statics/
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.5/bubble_aide/statics/__init__.py
+-rw-rw-rw-   0        0        0    12482 2023-06-29 08:53:39.000000 bubble-aide-0.1.5/bubble_aide/statics/calculator.py
+-rw-rw-rw-   0        0        0      915 2023-05-31 03:08:14.000000 bubble-aide-0.1.5/bubble_aide/statics/constant.py
+-rw-rw-rw-   0        0        0     3386 2023-06-05 02:48:13.000000 bubble-aide-0.1.5/bubble_aide/statics/contract.py
+-rw-rw-rw-   0        0        0     5806 2023-06-29 08:56:47.000000 bubble-aide-0.1.5/bubble_aide/statics/economic.py
+-rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.5/bubble_aide/statics/graphqls.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.793304 bubble-aide-0.1.5/bubble_aide/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.5/bubble_aide/utils/__init__.py
+-rw-rw-rw-   0        0        0     3377 2023-06-13 03:22:38.000000 bubble-aide-0.1.5/bubble_aide/utils/utils.py
+-rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.5/bubble_aide/utils/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:57:29.781752 bubble-aide-0.1.5/bubble_aide.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-06-29 08:57:29.000000 bubble-aide-0.1.5/bubble_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2023-06-29 08:57:29.000000 bubble-aide-0.1.5/bubble_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:57:29.000000 bubble-aide-0.1.5/bubble_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 03:23:54.000000 bubble-aide-0.1.5/bubble_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      161 2023-06-29 08:57:29.000000 bubble-aide-0.1.5/bubble_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 08:57:29.000000 bubble-aide-0.1.5/bubble_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:57:29.794326 bubble-aide-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2023-06-29 08:57:19.000000 bubble-aide-0.1.5/setup.py
```

### Comparing `bubble-aide-0.1.4/LICENSE` & `bubble-aide-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/PKG-INFO` & `bubble-aide-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.4
+Version: 0.1.5
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.4/README.md` & `bubble-aide-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/delegate.py` & `bubble-aide-0.1.5/bubble_aide/delegate.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/govern.py` & `bubble-aide-0.1.5/bubble_aide/govern.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/main.py` & `bubble-aide-0.1.5/bubble_aide/main.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/restricting.py` & `bubble-aide-0.1.5/bubble_aide/restricting.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/reward.py` & `bubble-aide-0.1.5/bubble_aide/reward.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/slashing.py` & `bubble-aide-0.1.5/bubble_aide/slashing.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/staking.py` & `bubble-aide-0.1.5/bubble_aide/staking.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/statics/calculator.py` & `bubble-aide-0.1.5/bubble_aide/statics/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, aide: "Aide"):
         self.aide = aide
 
     def get_verifier_count(self):
         """ 获取结算周期的验证人数
         备注：目前链上只能获取当前结算周期的验证人数
         """
-        verifier_list = self.aide.web3.dpos.staking.get_verifier_list()
+        verifier_list = self.aide.web3.dpos.staking.get_verifier_list().call()
         return len(verifier_list)
 
     def get_block_count(self, node_id, start_bn=None, end_bn=None):
         """ 获取节点出块数
         """
         start_bn = start_bn or 0
         end_bn = end_bn or self.aide.bub.block_number
@@ -85,16 +85,16 @@
 
         return start_block, end_block
 
     def get_reward_info(self):
         """ 获取当前结算周期的奖励信息
         """
         # todo: 删除该方法
-        total_staking_reward = self.aide.web3.dpos.staking.get_staking_reward()
-        per_block_reward = self.aide.web3.dpos.staking.get_block_reward()
+        total_staking_reward = self.aide.web3.dpos.staking.get_staking_reward().call()
+        per_block_reward = self.aide.web3.dpos.staking.get_block_reward().call()
         return total_staking_reward, per_block_reward
 
     # def get_node_reward(self, node_id):
     #     """ 即时计算上一个结算周期，节点的总奖励
     #     """
     #     total_staking_reward = self.web3.dpos.staking.get_staking_reward()
     #     verifier_count = self.get_verifier_count()
```

### Comparing `bubble-aide-0.1.4/bubble_aide/statics/constant.py` & `bubble-aide-0.1.5/bubble_aide/statics/constant.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/statics/contract.py` & `bubble-aide-0.1.5/bubble_aide/statics/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/statics/economic.py` & `bubble-aide-0.1.5/bubble_aide/statics/economic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import math
 from typing import Union
 from dataclasses import dataclass
 
 from dacite import from_dict
 
 
 @dataclass
@@ -161,15 +162,15 @@
         return self.increasing_epoch * self.epoch_consensus
 
     @property
     def increasing_epoch(self):
         """ 增发周期结算周期数
         """
         # todo: 修改为实时计算
-        return (self.common.additionalCycleTime * 60) // self.epoch_time
+        return math.ceil((self.common.additionalCycleTime * 60) / self.epoch_time)
 
     @property
     def verifier_count(self):
         """ 最大共识验证人数量
         """
         return self.common.maxConsensusVals
```

### Comparing `bubble-aide-0.1.4/bubble_aide/utils/utils.py` & `bubble-aide-0.1.5/bubble_aide/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide/utils/wrapper.py` & `bubble-aide-0.1.5/bubble_aide/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/bubble_aide.egg-info/PKG-INFO` & `bubble-aide-0.1.5/bubble_aide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.4
+Version: 0.1.5
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.4/bubble_aide.egg-info/SOURCES.txt` & `bubble-aide-0.1.5/bubble_aide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.4/setup.py` & `bubble-aide-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='bubble-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='0.1.4',
+    version='0.1.5',
     description="""bubble aide""",
     # long_description=long_description,
     # long_description_content_type='text/markdown',
     author='Shing',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/bubble-aide',
     include_package_data=True,
```

